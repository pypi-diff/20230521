# Comparing `tmp/autoklik-0.1.1.tar.gz` & `tmp/autoklik-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoklik-0.1.1.tar", max compression
+gzip compressed data, was "autoklik-0.2.0.tar", max compression
```

## Comparing `autoklik-0.1.1.tar` & `autoklik-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2021-07-12 21:08:18.447295 autoklik-0.1.1/LICENSE
--rw-r--r--   0        0        0      114 2021-07-12 21:08:18.447295 autoklik-0.1.1/README.md
--rw-r--r--   0        0        0     5328 2021-07-12 21:08:18.447295 autoklik-0.1.1/autoklik/__init__.py
--rw-r--r--   0        0        0       22 2021-07-12 21:08:18.447295 autoklik-0.1.1/autoklik/__version__.py
--rw-r--r--   0        0        0      526 2021-07-12 21:08:18.447295 autoklik-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      796 2021-07-12 21:08:25.962436 autoklik-0.1.1/setup.py
--rw-r--r--   0        0        0      599 2021-07-12 21:08:25.962763 autoklik-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-07-09 18:44:15.520792 autoklik-0.2.0/LICENSE
+-rw-r--r--   0        0        0      114 2021-08-14 10:20:37.364992 autoklik-0.2.0/README.md
+-rw-r--r--   0        0        0       75 2023-05-21 18:24:16.324559 autoklik-0.2.0/autoklik/__init__.py
+-rw-r--r--   0        0        0       39 2021-08-14 10:33:38.854925 autoklik-0.2.0/autoklik/__main__.py
+-rw-r--r--   0        0        0     7117 2023-05-10 22:04:19.189872 autoklik-0.2.0/autoklik/main.py
+-rw-r--r--   0        0        0      549 2023-05-21 18:24:38.444759 autoklik-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 autoklik-0.2.0/PKG-INFO
```

### Comparing `autoklik-0.1.1/LICENSE` & `autoklik-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoklik-0.1.1/autoklik/__init__.py` & `autoklik-0.2.0/autoklik/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """
 
 import argparse
 import logging
 import subprocess
 import time
 
-
 CLICK_NAMES = {"1": "left click", "2": "middle click", "3": "right click"}
 
 
 def setup_arguments():
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument(
         "-t",
@@ -42,14 +41,21 @@
     )
     parser.add_argument(
         "-f",
         "--ignore-when-focused",
         action="store_true",
         help="Don't send clicks to the select window when that window is focused.",
     )
+    parser.add_argument(
+        "-a",
+        "--alternate",
+        choices=["1", "2", "3"],
+        nargs=2,
+        help="Alternate between two different types of clicks",
+    )
     return parser
 
 
 def main():
     logging.basicConfig(format="%(asctime)s - %(message)s", level=logging.WARNING)
     parser = setup_arguments()
     args = parser.parse_args()
@@ -66,17 +72,31 @@
         window = {
             "window_id": window_id,
             "window_name": get_window_name_from_id(window_id),
         }
     else:
         window = select_window()
 
-    click = {"click_id": args.type, "click_name": CLICK_NAMES[args.type]}
+    if args.alternate is None:
+        click = {"click_id": args.type, "click_name": CLICK_NAMES[args.type]}
+
+        do_click(window, click, args.interval, args.ignore_when_focused)
+    else:
+        clicks = [
+            {
+                "click_id": args.alternate[0],
+                "click_name": CLICK_NAMES[args.alternate[0]],
+            },
+            {
+                "click_id": args.alternate[1],
+                "click_name": CLICK_NAMES[args.alternate[1]],
+            },
+        ]
 
-    do_click(window, click, args.interval, args.ignore_when_focused)
+        do_clicks(window, clicks, args.interval, args.ignore_when_focused)
 
 
 def select_window():
     print("Please select a window")
     window_id = (
         subprocess.run(["xdotool", "selectwindow"], capture_output=True)
         .stdout.strip()
@@ -164,22 +184,55 @@
                 logging.info("click skipped")
                 continue
 
         send_click(window, click)
         next_time += (time.time() - next_time) // interval * interval + interval
 
 
+def do_clicks(window, clicks, interval, ignore_when_focused):
+    print(
+        f"Sending {clicks[0]['click_name']}s and {clicks[1]['click_name']}s to {window['window_name']}, alternating between them every {interval}ms."
+    )
+
+    interval = interval / 1000
+    next_time = time.time() + interval
+    current_click = 0
+
+    while True:
+        time.sleep(max(0, next_time - time.time()))
+
+        if ignore_when_focused:
+            active_window = (
+                subprocess.run(["xdotool", "getactivewindow"], capture_output=True)
+                .stdout.strip()
+                .decode("UTF-8")
+            )
+
+            logging.debug(f"active window id: {active_window}")
+            logging.debug(f"sending clicks to window id: {window['window_id']}")
+
+            if active_window == window["window_id"]:
+                next_time += (time.time() - next_time) // interval * interval + interval
+                logging.info("click skipped")
+                continue
+
+        send_click(window, clicks[current_click])
+
+        if current_click == 0:
+            current_click = 1
+        else:
+            current_click = 0
+
+        next_time += (time.time() - next_time) // interval * interval + interval
+
+
 def send_click(window, click):
     # Send mouse down and up separately to prevent wrong mouse inputs from being
     # sent when those inputs are press on the actual mouse at the same time a click
     # event is sent
     subprocess.run(
         ["xdotool", "mousedown", "--window", window["window_id"], click["click_id"]]
     )
     subprocess.run(
         ["xdotool", "mouseup", "--window", window["window_id"], click["click_id"]]
     )
     logging.info(f"{click['click_name']} sent")
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `autoklik-0.1.1/pyproject.toml` & `autoklik-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "autoklik"
-version = "0.1.1"
+version = "0.2.0"
 description = "Auto clicker built around xdotool."
 authors = ["Magnus Walbeck <mw@mwalbeck.org>"]
 readme = "README.md"
 repository = "https://git.walbeck.it/mwalbeck/autoklik"
 packages = [{ include = "autoklik" }]
 
 [tool.poetry.scripts]
-autoklik = "autoklik.__init__:main"
+autoklik = "autoklik.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^3.9.2"
 black = "^21.6b0"
+flake8-bugbear = "^21.4.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autoklik-0.1.1/PKG-INFO` & `autoklik-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: autoklik
-Version: 0.1.1
+Version: 0.2.0
 Summary: Auto clicker built around xdotool.
 Home-page: https://git.walbeck.it/mwalbeck/autoklik
 Author: Magnus Walbeck
 Author-email: mw@mwalbeck.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://git.walbeck.it/mwalbeck/autoklik
 Description-Content-Type: text/markdown
 
 # Autoklik
 
 An auto clicker built around xdotool.
```

