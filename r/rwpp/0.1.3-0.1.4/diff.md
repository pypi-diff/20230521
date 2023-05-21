# Comparing `tmp/rwpp-0.1.3.tar.gz` & `tmp/rwpp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwpp-0.1.3.tar", max compression
+gzip compressed data, was "rwpp-0.1.4.tar", max compression
```

## Comparing `rwpp-0.1.3.tar` & `rwpp-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1036 2023-05-18 09:28:32.742220 rwpp-0.1.3/LICENSE
--rw-r--r--   0        0        0     4091 2023-05-18 09:28:32.742220 rwpp-0.1.3/README.md
--rw-r--r--   0        0        0      458 2023-05-21 16:59:52.154120 rwpp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-18 09:28:32.746220 rwpp-0.1.3/rwpp/__init__.py
--rw-r--r--   0        0        0     3310 2023-05-21 16:51:47.997274 rwpp-0.1.3/rwpp/main.py
--rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 rwpp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1036 2023-05-18 09:28:32.742220 rwpp-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4481 2023-05-21 17:03:01.838556 rwpp-0.1.4/README.md
+-rw-r--r--   0        0        0      458 2023-05-21 17:05:02.738834 rwpp-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 09:28:32.746220 rwpp-0.1.4/rwpp/__init__.py
+-rw-r--r--   0        0        0     3312 2023-05-21 17:03:48.530664 rwpp-0.1.4/rwpp/main.py
+-rw-r--r--   0        0        0     5101 1970-01-01 00:00:00.000000 rwpp-0.1.4/PKG-INFO
```

### Comparing `rwpp-0.1.3/LICENSE` & `rwpp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rwpp-0.1.3/README.md` & `rwpp-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -60,14 +60,29 @@
 ```
 
 
 ### Publishing
 
 Publishing the project to Pypi or Test Pypi is now done using Poetry. After you have made all the necessary commits, tested everything to ensure it runs as expected and setup your Pypi tokens in Poetry ([read more here](https://stackoverflow.com/questions/68882603/using-python-poetry-to-publish-to-test-pypi-org)), the process is as follows below.
 
+First add your pypi API token using `poetry config`.
+
+```bash
+poetry config pypi-token.pypi <token>
+```
+
+For uploading to Test Pypi first add the repository to your config and then your token.
+
+```bash
+poetry config repositories.test-pypi https://test.pypi.org/legacy/
+poetry config pypi-token.test-pypi <token>
+```
+
+Each time you need to publish the project you can use `poetry publish`.
+
 ```bash
 # Bump version
 poetry version patch
 
 # Publish
 poetry publish
 # poetry publish -r test-pypi
```

### Comparing `rwpp-0.1.3/rwpp/main.py` & `rwpp-0.1.4/rwpp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     ),
     limit: int = typer.Option(
         10,
         help="The amount of posts to pull from subreddit(s)",
         prompt="How many images would you like to download? ",
     ),
     download_path: str = typer.Option(
-        "./downloads",
+        "~/.wallpapers",
         help="The path where you would like to save images",
         prompt="Where would you like to save the images? ",
     ),
     sort_by: str = typer.Option(
         "hot",
         help="The sort order to pull images by",
         prompt="Sort order for images?: [hot, new, top, rising] ",
```

### Comparing `rwpp-0.1.3/PKG-INFO` & `rwpp-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwpp
-Version: 0.1.3
+Version: 0.1.4
 Summary: Reddit Wallpaper Puller, a simple CLI to pull wallpapers from Reddit.
 Author: Ducky
 Author-email: duckbox007@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -77,14 +77,29 @@
 ```
 
 
 ### Publishing
 
 Publishing the project to Pypi or Test Pypi is now done using Poetry. After you have made all the necessary commits, tested everything to ensure it runs as expected and setup your Pypi tokens in Poetry ([read more here](https://stackoverflow.com/questions/68882603/using-python-poetry-to-publish-to-test-pypi-org)), the process is as follows below.
 
+First add your pypi API token using `poetry config`.
+
+```bash
+poetry config pypi-token.pypi <token>
+```
+
+For uploading to Test Pypi first add the repository to your config and then your token.
+
+```bash
+poetry config repositories.test-pypi https://test.pypi.org/legacy/
+poetry config pypi-token.test-pypi <token>
+```
+
+Each time you need to publish the project you can use `poetry publish`.
+
 ```bash
 # Bump version
 poetry version patch
 
 # Publish
 poetry publish
 # poetry publish -r test-pypi
```

