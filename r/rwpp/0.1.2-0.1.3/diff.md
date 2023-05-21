# Comparing `tmp/rwpp-0.1.2.tar.gz` & `tmp/rwpp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwpp-0.1.2.tar", max compression
+gzip compressed data, was "rwpp-0.1.3.tar", max compression
```

## Comparing `rwpp-0.1.2.tar` & `rwpp-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1036 2023-05-04 15:24:54.106930 rwpp-0.1.2/LICENSE
--rwxr-xr-x   0        0        0     4091 2023-05-04 15:24:54.106930 rwpp-0.1.2/README.md
--rwxr-xr-x   0        0        0      458 2023-05-10 05:38:14.705489 rwpp-0.1.2/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-05-04 15:24:54.110263 rwpp-0.1.2/rwpp/__init__.py
--rwxr-xr-x   0        0        0     3256 2023-05-10 04:57:26.244100 rwpp-0.1.2/rwpp/main.py
--rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 rwpp-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1036 2023-05-18 09:28:32.742220 rwpp-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4091 2023-05-18 09:28:32.742220 rwpp-0.1.3/README.md
+-rw-r--r--   0        0        0      458 2023-05-21 16:59:52.154120 rwpp-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 09:28:32.746220 rwpp-0.1.3/rwpp/__init__.py
+-rw-r--r--   0        0        0     3310 2023-05-21 16:51:47.997274 rwpp-0.1.3/rwpp/main.py
+-rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 rwpp-0.1.3/PKG-INFO
```

### Comparing `rwpp-0.1.2/LICENSE` & `rwpp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rwpp-0.1.2/README.md` & `rwpp-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rwpp-0.1.2/rwpp/main.py` & `rwpp-0.1.3/rwpp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 app = typer.Typer()
 
 
 #  Main download function
 # @app.command()
 def download(subreddit, limit, download_path, time=None, sort_by=None):
     # Check for download path
+    download_path = os.path.expanduser(download_path)
     if not os.path.isdir(f"{download_path}/{subreddit}"):
         os.makedirs(f"{download_path}/{subreddit}")
 
     downloaded_images = os.listdir(f"{download_path}/{subreddit}")
 
     accepted_formats = [".jpg", ".jpeg", ".png"]
```

### Comparing `rwpp-0.1.2/PKG-INFO` & `rwpp-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwpp
-Version: 0.1.2
+Version: 0.1.3
 Summary: Reddit Wallpaper Puller, a simple CLI to pull wallpapers from Reddit.
 Author: Ducky
 Author-email: duckbox007@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

