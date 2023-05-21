# Comparing `tmp/pebbles_bot-0.3.1.tar.gz` & `tmp/pebbles_bot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pebbles_bot-0.3.1.tar", last modified: Wed Apr 19 19:39:48 2023, max compression
+gzip compressed data, was "pebbles_bot-0.3.2.tar", last modified: Sun May 21 19:50:47 2023, max compression
```

## Comparing `pebbles_bot-0.3.1.tar` & `pebbles_bot-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:48.717073 pebbles_bot-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-19 19:39:48.717073 pebbles_bot-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:48.717073 pebbles_bot-0.3.1/pebbles_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/pebbles_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/pebbles_bot/pb_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/pebbles_bot/pb_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/pebbles_bot/pebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:48.717073 pebbles_bot-0.3.1/pebbles_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-19 19:39:48.717073 pebbles_bot-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:50:47.818683 pebbles_bot-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-21 19:50:47.818683 pebbles_bot-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:50:47.814683 pebbles_bot-0.3.2/pebbles_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/pebbles_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/pebbles_bot/pb_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/pebbles_bot/pb_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/pebbles_bot/pebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:50:47.814683 pebbles_bot-0.3.2/pebbles_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-21 19:50:47.818683 pebbles_bot-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/setup.py
```

### Comparing `pebbles_bot-0.3.1/LICENSE` & `pebbles_bot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pebbles_bot-0.3.1/PKG-INFO` & `pebbles_bot-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pebbles_bot
-Version: 0.3.1
+Version: 0.3.2
 Summary: Telegram bot that runs Linux shell commands
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pebbles_bot-0.3.1/README.md` & `pebbles_bot-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pebbles_bot-0.3.1/pebbles_bot/pb_main.py` & `pebbles_bot-0.3.2/pebbles_bot/pb_main.py`

 * *Files identical despite different names*

### Comparing `pebbles_bot-0.3.1/pebbles_bot/pb_tools.py` & `pebbles_bot-0.3.2/pebbles_bot/pb_tools.py`

 * *Files identical despite different names*

### Comparing `pebbles_bot-0.3.1/pebbles_bot/pebot.py` & `pebbles_bot-0.3.2/pebbles_bot/pebot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sys
 import yaml
+import argparse
 from pathlib import Path
 from .pb_main import Pebbles
 
 
 def config_reader():
     """
     Reads the config file and returns a dictionary
@@ -22,36 +23,39 @@
             return None
     else:
         print(f"Config file {config} not found")
         return None
 
 
 def main():
+    parser = argparse.ArgumentParser(description="Run Pebbles.")
+    parser.add_argument('--notify', action='store_true', help='Notification message to send')
+    args = parser.parse_args()
+
     api_key = os.environ.get("PEBBLES_API_KEY")
     whitelist_ids = os.environ.get("PEBBLES_USER_WHITELIST")
 
     if not api_key:
         print("Pebbles API key not found")
         sys.exit(0)
 
     if not whitelist_ids:
         print("Pebbles user whitelist not found")
         sys.exit(0)
 
-    notify = "--notify" in sys.argv
-    if notify:
-        sys.argv.remove("--notify")
-        notify = sys.stdin.read()
-
     pebbles_config = config_reader()
     if pebbles_config:
         whitelist_ids = pebbles_config["whitelist_ids"]
 
+    notify = sys.stdin.read() if args.notify else None
+
     Pebbles(
         api_key=api_key,
         whitelist=whitelist_ids.split(","),
         notify=notify,
     )
 
 
 if __name__ == "__main__":
     main()
+
+
```

### Comparing `pebbles_bot-0.3.1/pebbles_bot.egg-info/PKG-INFO` & `pebbles_bot-0.3.2/pebbles_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pebbles-bot
-Version: 0.3.1
+Version: 0.3.2
 Summary: Telegram bot that runs Linux shell commands
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pebbles_bot-0.3.1/setup.cfg` & `pebbles_bot-0.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pebbles_bot
-version = 0.3.1
+version = 0.3.2
 description = Telegram bot that runs Linux shell commands
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lab-Brat
 author_email = labbrat_social@pm.me
 url = https://github.com/Lab-Brat/pyLookout
 license = MIT
```

