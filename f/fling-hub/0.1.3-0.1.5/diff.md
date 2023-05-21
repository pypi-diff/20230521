# Comparing `tmp/fling_hub-0.1.3.tar.gz` & `tmp/fling_hub-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_hub-0.1.3.tar", max compression
+gzip compressed data, was "fling_hub-0.1.5.tar", max compression
```

## Comparing `fling_hub-0.1.3.tar` & `fling_hub-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       57 2023-05-14 06:13:51.220760 fling_hub-0.1.3/README.md
--rw-r--r--   0        0        0        5 2023-05-20 07:36:20.449774 fling_hub-0.1.3/VERSION
--rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 fling_hub-0.1.3/build.py
--rw-r--r--   0        0        0       22 2023-05-20 07:36:26.820788 fling_hub-0.1.3/fling_hub/__init__.py
--rw-r--r--   0        0        0     2158 2023-05-19 22:01:24.121786 fling_hub-0.1.3/fling_hub/flingroute.py
--rw-r--r--   0        0        0      903 2023-05-20 00:05:15.055873 fling_hub-0.1.3/fling_hub/hub.plist.template
--rwxr-xr-x   0        0        0  8080834 2023-05-20 06:52:18.018000 fling_hub-0.1.3/fling_hub/loophost
--rw-r--r--   0        0        0      814 2023-05-20 01:14:11.424956 fling_hub-0.1.3/fling_hub/loophost.plist.template
--rw-r--r--   0        0        0     3680 2023-05-20 07:15:55.241334 fling_hub-0.1.3/fling_hub/postinstall.py
--rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 fling_hub-0.1.3/fling_hub/static/fling-logo-dark.png
--rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 fling_hub-0.1.3/fling_hub/static/fling-logo-light.png
--rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 fling_hub-0.1.3/fling_hub/static/logo-hc.txt
--rw-r--r--   0        0        0     1208 2023-05-16 18:15:32.432199 fling_hub-0.1.3/fling_hub/templates/admin.html
--rw-r--r--   0        0        0     2175 2023-05-16 18:10:10.679092 fling_hub-0.1.3/fling_hub/templates/local.html
--rw-r--r--   0        0        0     1081 2023-05-18 00:14:10.759502 fling_hub-0.1.3/fling_hub/templates/partials/apptable.html
--rw-r--r--   0        0        0      282 2023-05-16 18:40:57.186236 fling_hub-0.1.3/fling_hub/templates/partials/upgrade.html
--rw-r--r--   0        0        0     1088 2023-05-20 07:35:50.007718 fling_hub-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 fling_hub-0.1.3/setup.py
--rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 fling_hub-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-05-14 06:13:51.220760 fling_hub-0.1.5/README.md
+-rw-r--r--   0        0        0        5 2023-05-21 18:38:24.782214 fling_hub-0.1.5/VERSION
+-rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 fling_hub-0.1.5/build.py
+-rw-r--r--   0        0        0       22 2023-05-21 18:38:29.530314 fling_hub-0.1.5/fling_hub/__init__.py
+-rw-r--r--   0        0        0     2158 2023-05-19 22:01:24.121786 fling_hub-0.1.5/fling_hub/flingroute.py
+-rw-r--r--   0        0        0      903 2023-05-20 00:05:15.055873 fling_hub-0.1.5/fling_hub/hub.plist.template
+-rwxr-xr-x   0        0        0  8301312 2023-05-20 20:12:28.547737 fling_hub-0.1.5/fling_hub/loophost
+-rw-r--r--   0        0        0      814 2023-05-20 01:14:11.424956 fling_hub-0.1.5/fling_hub/loophost.plist.template
+-rw-r--r--   0        0        0     3920 2023-05-20 20:22:55.829947 fling_hub-0.1.5/fling_hub/postinstall.py
+-rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 fling_hub-0.1.5/fling_hub/static/fling-logo-dark.png
+-rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 fling_hub-0.1.5/fling_hub/static/fling-logo-light.png
+-rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 fling_hub-0.1.5/fling_hub/static/logo-hc.txt
+-rw-r--r--   0        0        0     1208 2023-05-16 18:15:32.432199 fling_hub-0.1.5/fling_hub/templates/admin.html
+-rw-r--r--   0        0        0     2175 2023-05-16 18:10:10.679092 fling_hub-0.1.5/fling_hub/templates/local.html
+-rw-r--r--   0        0        0     1081 2023-05-18 00:14:10.759502 fling_hub-0.1.5/fling_hub/templates/partials/apptable.html
+-rw-r--r--   0        0        0      282 2023-05-16 18:40:57.186236 fling_hub-0.1.5/fling_hub/templates/partials/upgrade.html
+-rw-r--r--   0        0        0     1099 2023-05-21 18:38:19.520576 fling_hub-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 fling_hub-0.1.5/setup.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 fling_hub-0.1.5/PKG-INFO
```

### Comparing `fling_hub-0.1.3/build.py` & `fling_hub-0.1.5/build.py`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.3/fling_hub/flingroute.py` & `fling_hub-0.1.5/fling_hub/flingroute.py`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.3/fling_hub/hub.plist.template` & `fling_hub-0.1.5/fling_hub/hub.plist.template`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.3/fling_hub/loophost.plist.template` & `fling_hub-0.1.5/fling_hub/loophost.plist.template`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.3/fling_hub/postinstall.py` & `fling_hub-0.1.5/fling_hub/postinstall.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,29 +10,34 @@
 from string import Template
 
 
 TARGET_DIR = pathlib.Path(pathlib.Path.home(), ".flingdev")
 PYEX = sys.executable
 HUBDIR = os.path.dirname(os.path.realpath(fling_hub.__file__))
 USERNAME = None
+if os.path.exists(pathlib.Path(TARGET_DIR, "flinguser.txt")):
+    with open(pathlib.Path(TARGET_DIR, "flinguser.txt"), "r") as userfile:
+        USERNAME = userfile.read()
 
 
 def restart_as_sudo():
+    global USERNAME
     print(
         "Switching to root user to install web services (you will be prompted for your password)"
     )
     run(
         "sudo python3 -m fling_hub.postinstall",
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         stdin=subprocess.PIPE,
         cwd=TARGET_DIR,
     )
     print("All finished.")
+    run(f"open 'https://{USERNAME}.fling.dev'")
     sys.exit()
 
 
 def post_install_one():
     print("Installing LoopHost...")
     os.makedirs(pathlib.Path(TARGET_DIR, "certs"), exist_ok=True)
     os.chdir(TARGET_DIR)
```

### Comparing `fling_hub-0.1.3/fling_hub/static/fling-logo-dark.png` & `fling_hub-0.1.5/fling_hub/static/fling-logo-dark.png`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.3/fling_hub/static/fling-logo-light.png` & `fling_hub-0.1.5/fling_hub/static/fling-logo-light.png`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.3/fling_hub/static/logo-hc.txt` & `fling_hub-0.1.5/fling_hub/static/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.3/fling_hub/templates/admin.html` & `fling_hub-0.1.5/fling_hub/templates/admin.html`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.3/fling_hub/templates/local.html` & `fling_hub-0.1.5/fling_hub/templates/local.html`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.3/fling_hub/templates/partials/apptable.html` & `fling_hub-0.1.5/fling_hub/templates/partials/apptable.html`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.3/pyproject.toml` & `fling_hub-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 [build-system]
 requires = ["poetry-core", "poetry>=0.12", "setuptools", "wheel", "setuptools-cpp", "setuptools-golang"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fling-hub"
-version = "0.1.3"
-description = "Loophost for a better local dev"
+version = "0.1.5"
+description = "Loophost: for a better local dev"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
     "Anouk Ruhaak <anoukruhaak@gmail.com>",
 ]
 readme = "README.md"
 include = [{ path = "VERSION" }, 
             { path = "README.md" }, 
             { path = "setup.py" }, 
             { path = "build.py" }, 
             { path = "fling_hub/templates" }, 
-            { path = "fling_hub/loophost/*"}, 
+            { path = "fling_hub/loophost"}, 
             { path = "fling_hub/*.plist.template"}] 
 packages = [
     { include = "fling_hub" },
 ]
 build = "build.py"
 
 [tool.poetry.urls]
 homepage = "https://fling.dev"
 documentation = "https://readthedocs.org/fling-hub"
 repository = "https://github.com/delving-co/fling-hub.git"
 
-# [tool.poetry.group.dev.dependencies]
-# black = "^23.3.0"
-# setuptools = "*"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+setuptools = "*"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fling-start = "*"
 fling-cli = "0.1.5"
 certbot = "*"
 flask = "*"
+lastversion = "*"
```

### Comparing `fling_hub-0.1.3/PKG-INFO` & `fling_hub-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: fling-hub
-Version: 0.1.3
-Summary: Loophost for a better local dev
+Version: 0.1.5
+Summary: Loophost: for a better local dev
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certbot
 Requires-Dist: flask
 Requires-Dist: fling-cli (==0.1.5)
 Requires-Dist: fling-start
+Requires-Dist: lastversion
 Project-URL: documentation, https://readthedocs.org/fling-hub
 Project-URL: homepage, https://fling.dev
 Project-URL: repository, https://github.com/delving-co/fling-hub.git
 Description-Content-Type: text/markdown
 
 # Fling-Hub
 ### The loophost experience you always wanted
```

