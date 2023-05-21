# Comparing `tmp/fling_cli-0.1.5.tar.gz` & `tmp/fling_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_cli-0.1.5.tar", max compression
+gzip compressed data, was "fling_cli-0.1.6.tar", max compression
```

## Comparing `fling_cli-0.1.5.tar` & `fling_cli-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2163 2023-04-05 23:25:42.977524 fling_cli-0.1.5/README.md
--rw-r--r--   0        0        0      647 2023-05-17 22:43:54.774155 fling_cli-0.1.5/fling_cli/__init__.py
--rw-r--r--   0        0        0     2190 2023-05-17 22:30:05.611005 fling_cli-0.1.5/fling_cli/auth.py
--rw-r--r--   0        0        0        0 2023-04-04 19:06:55.600802 fling_cli-0.1.5/fling_cli/bin/__init__.py
--rw-r--r--   0        0        0     6306 2023-05-13 22:09:25.053951 fling_cli-0.1.5/fling_cli/bin/fling.py
--rw-r--r--   0        0        0     1492 2023-05-13 23:40:28.872299 fling_cli-0.1.5/fling_cli/certbot_fling_plugin.py
--rw-r--r--   0        0        0     3834 2023-04-08 02:13:26.640377 fling_cli-0.1.5/fling_cli/logo-hc.txt
--rw-r--r--   0        0        0      990 2023-05-17 22:43:43.996942 fling_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 fling_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2163 2023-04-05 23:25:42.977524 fling_cli-0.1.6/README.md
+-rw-r--r--   0        0        0      647 2023-05-21 21:48:46.490496 fling_cli-0.1.6/fling_cli/__init__.py
+-rw-r--r--   0        0        0     2286 2023-05-21 21:47:47.016971 fling_cli-0.1.6/fling_cli/auth.py
+-rw-r--r--   0        0        0        0 2023-04-04 19:06:55.600802 fling_cli-0.1.6/fling_cli/bin/__init__.py
+-rw-r--r--   0        0        0     6306 2023-05-13 22:09:25.053951 fling_cli-0.1.6/fling_cli/bin/fling.py
+-rw-r--r--   0        0        0     1492 2023-05-13 23:40:28.872299 fling_cli-0.1.6/fling_cli/certbot_fling_plugin.py
+-rw-r--r--   0        0        0     3834 2023-04-08 02:13:26.640377 fling_cli-0.1.6/fling_cli/logo-hc.txt
+-rw-r--r--   0        0        0      990 2023-05-21 21:48:40.064803 fling_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 fling_cli-0.1.6/PKG-INFO
```

### Comparing `fling_cli-0.1.5/README.md` & `fling_cli-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.5/fling_cli/__init__.py` & `fling_cli-0.1.6/fling_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 
 import keyring
 from click.exceptions import UsageError
 from fling_core import settings
 from fling_client.client import Client
```

### Comparing `fling_cli-0.1.5/fling_cli/auth.py` & `fling_cli-0.1.6/fling_cli/auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import keyring
 import uvicorn
 from fastapi import BackgroundTasks, FastAPI
 from fastapi.responses import HTMLResponse
 from starlette.responses import RedirectResponse
 from fling_core import settings
+import pathlib
 
 
 stored_state = None
 
 
 def make_app():
     app = FastAPI()
@@ -30,16 +31,16 @@
     @app.get("/callback")
     async def callback(state: str, token: str, username: str):
         # Die after this request finishes, no matter what
 
         if state != stored_state:
             raise Exception("State doesn't match, bad!")
         print(f"Saving token for `{username}` to keyring.")
-        os.makedirs("~/.flingdev", exist_ok=True)
-        with open("flinguser.txt", "w") as userfile:
+        os.makedirs(pathlib.Path(pathlib.Path.home(), ".flingdev"), exist_ok=True)
+        with open(pathlib.Path(pathlib.Path.home(), ".flingdev", "flinguser.txt"), "w") as userfile:
             userfile.write(username)
         keyring.set_password("fling-github-token", username, token)
         # default_password = keyring.get_password("fling-github-token", "system-default")
         # if not default_password:
         #     print(f"No default account, Saving token for `{username}` as default.")
         keyring.set_password("fling-github-token", "system-default", token)
         return RedirectResponse('http://localhost:5817', status_code=302)
```

### Comparing `fling_cli-0.1.5/fling_cli/bin/fling.py` & `fling_cli-0.1.6/fling_cli/bin/fling.py`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.5/fling_cli/certbot_fling_plugin.py` & `fling_cli-0.1.6/fling_cli/certbot_fling_plugin.py`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.5/fling_cli/logo-hc.txt` & `fling_cli-0.1.6/fling_cli/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.5/pyproject.toml` & `fling_cli-0.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fling-cli"
-version = "0.1.5"
+version = "0.1.6"
 description = "Side Project Management from the command line"
 authors = ["Joshua McKenty <jmckenty@gmail.com>", "Anouk Ruhaak <anoukruhaak@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fling_cli"}]
 
 [tool.poetry.dependencies]
 click = "*"
```

### Comparing `fling_cli-0.1.5/PKG-INFO` & `fling_cli-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: Side Project Management from the command line
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

