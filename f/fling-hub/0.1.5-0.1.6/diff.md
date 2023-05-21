# Comparing `tmp/fling_hub-0.1.5.tar.gz` & `tmp/fling_hub-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_hub-0.1.5.tar", max compression
+gzip compressed data, was "fling_hub-0.1.6.tar", max compression
```

## Comparing `fling_hub-0.1.5.tar` & `fling_hub-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       57 2023-05-14 06:13:51.220760 fling_hub-0.1.5/README.md
--rw-r--r--   0        0        0        5 2023-05-21 18:38:24.782214 fling_hub-0.1.5/VERSION
--rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 fling_hub-0.1.5/build.py
--rw-r--r--   0        0        0       22 2023-05-21 18:38:29.530314 fling_hub-0.1.5/fling_hub/__init__.py
--rw-r--r--   0        0        0     2158 2023-05-19 22:01:24.121786 fling_hub-0.1.5/fling_hub/flingroute.py
--rw-r--r--   0        0        0      903 2023-05-20 00:05:15.055873 fling_hub-0.1.5/fling_hub/hub.plist.template
--rwxr-xr-x   0        0        0  8301312 2023-05-20 20:12:28.547737 fling_hub-0.1.5/fling_hub/loophost
--rw-r--r--   0        0        0      814 2023-05-20 01:14:11.424956 fling_hub-0.1.5/fling_hub/loophost.plist.template
--rw-r--r--   0        0        0     3920 2023-05-20 20:22:55.829947 fling_hub-0.1.5/fling_hub/postinstall.py
--rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 fling_hub-0.1.5/fling_hub/static/fling-logo-dark.png
--rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 fling_hub-0.1.5/fling_hub/static/fling-logo-light.png
--rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 fling_hub-0.1.5/fling_hub/static/logo-hc.txt
--rw-r--r--   0        0        0     1208 2023-05-16 18:15:32.432199 fling_hub-0.1.5/fling_hub/templates/admin.html
--rw-r--r--   0        0        0     2175 2023-05-16 18:10:10.679092 fling_hub-0.1.5/fling_hub/templates/local.html
--rw-r--r--   0        0        0     1081 2023-05-18 00:14:10.759502 fling_hub-0.1.5/fling_hub/templates/partials/apptable.html
--rw-r--r--   0        0        0      282 2023-05-16 18:40:57.186236 fling_hub-0.1.5/fling_hub/templates/partials/upgrade.html
--rw-r--r--   0        0        0     1099 2023-05-21 18:38:19.520576 fling_hub-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 fling_hub-0.1.5/setup.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 fling_hub-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-05-14 06:13:51.220760 fling_hub-0.1.6/README.md
+-rw-r--r--   0        0        0        5 2023-05-21 21:20:45.888014 fling_hub-0.1.6/VERSION
+-rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 fling_hub-0.1.6/build.py
+-rw-r--r--   0        0        0       22 2023-05-21 21:20:43.379682 fling_hub-0.1.6/fling_hub/__init__.py
+-rw-r--r--   0        0        0     2158 2023-05-19 22:01:24.121786 fling_hub-0.1.6/fling_hub/flingroute.py
+-rw-r--r--   0        0        0      903 2023-05-20 00:05:15.055873 fling_hub-0.1.6/fling_hub/hub.plist.template
+-rwxr-xr-x   0        0        0  8301312 2023-05-20 20:12:28.547737 fling_hub-0.1.6/fling_hub/loophost
+-rw-r--r--   0        0        0      814 2023-05-20 01:14:11.424956 fling_hub-0.1.6/fling_hub/loophost.plist.template
+-rw-r--r--   0        0        0     3994 2023-05-21 21:11:27.044451 fling_hub-0.1.6/fling_hub/postinstall.py
+-rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 fling_hub-0.1.6/fling_hub/static/fling-logo-dark.png
+-rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 fling_hub-0.1.6/fling_hub/static/fling-logo-light.png
+-rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 fling_hub-0.1.6/fling_hub/static/logo-hc.txt
+-rw-r--r--   0        0        0     1211 2023-05-21 21:11:46.157275 fling_hub-0.1.6/fling_hub/templates/admin.html
+-rw-r--r--   0        0        0     2178 2023-05-21 21:11:54.645785 fling_hub-0.1.6/fling_hub/templates/local.html
+-rw-r--r--   0        0        0     1081 2023-05-18 00:14:10.759502 fling_hub-0.1.6/fling_hub/templates/partials/apptable.html
+-rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 fling_hub-0.1.6/fling_hub/templates/partials/upgrade.html
+-rw-r--r--   0        0        0     1099 2023-05-21 21:20:53.660432 fling_hub-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 fling_hub-0.1.6/setup.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 fling_hub-0.1.6/PKG-INFO
```

### Comparing `fling_hub-0.1.5/build.py` & `fling_hub-0.1.6/build.py`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.5/fling_hub/flingroute.py` & `fling_hub-0.1.6/fling_hub/flingroute.py`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.5/fling_hub/hub.plist.template` & `fling_hub-0.1.6/fling_hub/hub.plist.template`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.5/fling_hub/loophost` & `fling_hub-0.1.6/fling_hub/loophost`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.5/fling_hub/loophost.plist.template` & `fling_hub-0.1.6/fling_hub/loophost.plist.template`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.5/fling_hub/postinstall.py` & `fling_hub-0.1.6/fling_hub/postinstall.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import subprocess
 from subprocess import run, call, Popen
 from fling_cli.auth import gh_authenticate
 import shutil
 from string import Template
 
 
+LOOPHOST_DOMAIN = "loophost.dev"
 TARGET_DIR = pathlib.Path(pathlib.Path.home(), ".flingdev")
 PYEX = sys.executable
 HUBDIR = os.path.dirname(os.path.realpath(fling_hub.__file__))
 USERNAME = None
 if os.path.exists(pathlib.Path(TARGET_DIR, "flinguser.txt")):
     with open(pathlib.Path(TARGET_DIR, "flinguser.txt"), "r") as userfile:
         USERNAME = userfile.read()
@@ -29,15 +30,15 @@
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         stdin=subprocess.PIPE,
         cwd=TARGET_DIR,
     )
     print("All finished.")
-    run(f"open 'https://{USERNAME}.fling.dev'")
+    run(f"open 'https://{USERNAME}.{LOOPHOST_DOMAIN}'")
     sys.exit()
 
 
 def post_install_one():
     print("Installing LoopHost...")
     os.makedirs(pathlib.Path(TARGET_DIR, "certs"), exist_ok=True)
     os.chdir(TARGET_DIR)
@@ -69,18 +70,18 @@
                 "certonly",
                 "--config-dir ./",
                 "--work-dir ./",
                 "--logs-dir ./",
                 "--non-interactive",
                 "--expand",
                 "--agree-tos",
-                "-m webmaster@fling.dev",
+                f"-m webmaster@{LOOPHOST_DOMAIN}",
                 "--authenticator=fling_authenticator",
-                f'-d "*.{USERNAME}.fling.dev"',
-                f'-d "{USERNAME}.fling.dev"',
+                f'-d "*.{USERNAME}.{LOOPHOST_DOMAIN}"',
+                f'-d "{USERNAME}.{LOOPHOST_DOMAIN}"',
                 "--fling_authenticator-propagation-seconds=15",
             ]
         ),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         stdin=subprocess.PIPE,
         cwd=TARGET_DIR,
@@ -89,15 +90,15 @@
     )
 
 
 def setup_launchd_scripts():
     global USERNAME, TARGET_DIR, HUBDIR, PYEX
     if not os.path.exists(pathlib.Path(TARGET_DIR, "loophost.json")):
         with open(pathlib.Path(TARGET_DIR, "loophost.json"), "w") as datafile:
-            data = {"apps": {}, "fqdn": f"{USERNAME}.fling.dev"}
+            data = {"apps": {}, "fqdn": f"{USERNAME}.{LOOPHOST_DOMAIN}"}
             datafile.write(json.dumps(data))
     shutil.copy2(pathlib.Path(HUBDIR, "loophost.plist.template"), TARGET_DIR)
     shutil.copy2(pathlib.Path(HUBDIR, "hub.plist.template"), TARGET_DIR)
 
     d = {"CWD": TARGET_DIR, "USERNAME": USERNAME, "PYEX": PYEX, "HUBDIR": HUBDIR}
 
     templates = [
```

### Comparing `fling_hub-0.1.5/fling_hub/static/fling-logo-dark.png` & `fling_hub-0.1.6/fling_hub/static/fling-logo-dark.png`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.5/fling_hub/static/fling-logo-light.png` & `fling_hub-0.1.6/fling_hub/static/fling-logo-light.png`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.5/fling_hub/static/logo-hc.txt` & `fling_hub-0.1.6/fling_hub/static/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.5/fling_hub/templates/admin.html` & `fling_hub-0.1.6/fling_hub/templates/admin.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends "start/base.html" %}
-{% block title %}fling.dev: Local software development with Loophosting{% endblock %}
+{% block title %}Loophost.dev: Local software development with Loophosting{% endblock %}
 {% block head %}
 {{ super() }}
 <style>
 
 body {
     font-family: monospace;
     background-color: black;
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_srl3f_e9_/tmprynsim5j_TarContainer/0/12.html", line 51, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_srl3f_e9_/tmprynsim5j_TarContainer/0/12.html", line 51, column 0: CDATA terminal not found*

```diff
@@ -1,2 +1,2 @@
-{% extends "start/base.html" %} {% block title %}fling.dev: Local software
+{% extends "start/base.html" %} {% block title %}Loophost.dev: Local software
 development with Loophosting{% endblock %} {% block head %} {{ super() }}
```

### Comparing `fling_hub-0.1.5/fling_hub/templates/local.html` & `fling_hub-0.1.6/fling_hub/templates/local.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "start/base.html" %} {% block title %}fling.dev: Local software development with Loophosting{%
+{% extends "start/base.html" %} {% block title %}Loophost.dev: Local software development with Loophosting{%
 endblock %} {% block head %} {{ super() }}
 <style>
   body {
     font-family: monospace;
     background-color: black;
     color: green;
   }
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "start/base.html" %} {% block title %}fling.dev: Local software
+{% extends "start/base.html" %} {% block title %}Loophost.dev: Local software
 development with Loophosting{% endblock %} {% block head %} {{ super() }}
  {% endblock %} {% block body %}
 {% block content %} {{ super() }}
 [/static/fling-logo-dark.png]
 **** Configuration for "{{project}}" ****
 {% if project not in apps %} We don't know where this app is running yet.
```

### Comparing `fling_hub-0.1.5/fling_hub/templates/partials/apptable.html` & `fling_hub-0.1.6/fling_hub/templates/partials/apptable.html`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.5/pyproject.toml` & `fling_hub-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "poetry>=0.12", "setuptools", "wheel", "setuptools-cpp", "setuptools-golang"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fling-hub"
-version = "0.1.5"
+version = "0.1.6"
 description = "Loophost: for a better local dev"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
     "Anouk Ruhaak <anoukruhaak@gmail.com>",
 ]
 readme = "README.md"
 include = [{ path = "VERSION" },
```

### Comparing `fling_hub-0.1.5/PKG-INFO` & `fling_hub-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-hub
-Version: 0.1.5
+Version: 0.1.6
 Summary: Loophost: for a better local dev
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

