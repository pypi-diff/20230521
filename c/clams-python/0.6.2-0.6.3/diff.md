# Comparing `tmp/clams-python-0.6.2.tar.gz` & `tmp/clams-python-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-0.6.2.tar", last modified: Fri May 19 20:53:50 2023, max compression
+gzip compressed data, was "clams-python-0.6.3.tar", last modified: Sun May 21 00:24:36 2023, max compression
```

## Comparing `clams-python-0.6.2.tar` & `clams-python-0.6.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.372418 clams-python-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-19 20:53:25.000000 clams-python-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 20:53:25.000000 clams-python-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-19 20:53:50.372418 clams-python-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-19 20:53:25.000000 clams-python-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 20:53:25.000000 clams-python-0.6.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    16524 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.364417 clams-python-0.6.2/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/CLAMS-generic-readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/develop/templates/github/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/github/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/develop/templates/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/github/workflows/issue-apps-project.yml
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/github/workflows/issue-assign.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/github/workflows/issue-close.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/github/workflows/publish.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 20:53:25.000000 clams-python-0.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:53:50.372418 clams-python-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-19 20:53:25.000000 clams-python-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.372418 clams-python-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-05-19 20:53:25.000000 clams-python-0.6.2/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-19 20:53:25.000000 clams-python-0.6.2/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.184832 clams-python-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-21 00:24:01.000000 clams-python-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-21 00:24:01.000000 clams-python-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-21 00:24:36.184832 clams-python-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-21 00:24:01.000000 clams-python-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 00:24:02.000000 clams-python-0.6.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.176832 clams-python-0.6.3/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.176832 clams-python-0.6.3/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.176832 clams-python-0.6.3/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.176832 clams-python-0.6.3/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.176832 clams-python-0.6.3/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/CLAMS-generic-readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/develop/templates/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/github/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/develop/templates/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/github/workflows/issue-apps-project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/github/workflows/issue-assign.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/github/workflows/issue-close.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/github/workflows/publish.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.184832 clams-python-0.6.3/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-21 00:24:01.000000 clams-python-0.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:24:36.184832 clams-python-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-21 00:24:01.000000 clams-python-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.184832 clams-python-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-05-21 00:24:01.000000 clams-python-0.6.3/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-21 00:24:01.000000 clams-python-0.6.3/tests/test_clamscli.py
```

### Comparing `clams-python-0.6.2/LICENSE` & `clams-python-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/PKG-INFO` & `clams-python-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 0.6.2
+Version: 0.6.3
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-0.6.2/README.md` & `clams-python-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/__init__.py` & `clams-python-0.6.3/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/app/__init__.py` & `clams-python-0.6.3/clams/app/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/appmetadata/__init__.py` & `clams-python-0.6.3/clams/appmetadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 app_version_envvar_key = 'CLAMS_APP_VERSION'
 # type aliases to use in app metadata and runtime parameter processing 
 primitives = Union[int, float, bool, str]
 # these names are taken from the JSON schema data types
 param_value_types = Literal['integer', 'number', 'string', 'boolean']
 
 param_value_types_values = param_value_types.__args__  # pytype: disable=attribute-error
-app_directory_baseurl = "https://apps.clams.ai"
+app_directory_baseurl = "http://apps.clams.ai"
 
 
 def get_clams_pyver():
     # real hack to avoid import clams as a package in gh-action workflow
     try:
         import clams
         return clams.__version__
```

### Comparing `clams-python-0.6.2/clams/develop/__init__.py` & `clams-python-0.6.3/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/develop/templates/app/.gitignore` & `clams-python-0.6.3/clams/develop/templates/app/.gitignore`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/develop/templates/app/CLAMS-generic-readme.md` & `clams-python-0.6.3/clams/develop/templates/app/CLAMS-generic-readme.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/develop/templates/app/Containerfile` & `clams-python-0.6.3/clams/develop/templates/app/Containerfile`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/develop/templates/app/README.md` & `clams-python-0.6.3/clams/develop/templates/app/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/develop/templates/app/app.py` & `clams-python-0.6.3/clams/develop/templates/app/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     def __init__(self):
         super().__init__()
 
     def _appmetadata(self):
         # see https://sdk.clams.ai/autodoc/clams.app.html#clams.app.ClamsApp._load_appmetadata
         # Also check out ``metadata.py`` in this directory. 
+        # When using the ``metadata.py`` leave this do-nothing "pass" method here. 
         pass
 
     def _annotate(self, mmif: Union[str, dict, Mmif], **parameters) -> Mmif:
         # see https://sdk.clams.ai/autodoc/clams.app.html#clams.app.ClamsApp._annotate
         raise NotImplementedError
```

### Comparing `clams-python-0.6.2/clams/develop/templates/app/metadata.py` & `clams-python-0.6.3/clams/develop/templates/app/metadata.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/develop/templates/github/README.md` & `clams-python-0.6.3/clams/develop/templates/github/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/develop/templates/github/workflows/publish.yml` & `clams-python-0.6.3/clams/develop/templates/github/workflows/publish.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: "App Publisher: image>ghcr, metadata>appdir"
+name: "📦 Publish image>ghcr, metadata>appdir"
 
 on:
   workflow_dispatch:
     inputs:
       tag:
         required: true
         type: string
@@ -10,41 +10,41 @@
   push:
     tags:
       - '*'
 
 jobs:
   set-version:
     runs-on: ubuntu-latest
-    name: 📌 Set VERSION value
+    name: "🏷 Set version value"
     outputs:
       version: ${{ steps.output_version.outputs.version }}
     steps:
-      - name: set VERSION value from dispatch inputs
+      - name: "📌 Set VERSION value from dispatch inputs"
         id: get_version_dispatch
         if: ${{ github.event_name == 'workflow_dispatch' }}
         run: echo "VERSION=${{ github.event.inputs.tag }}" >> $GITHUB_ENV
-      - name: set VERSION value from pushed tag
+      - name: "📌 Set VERSION value from pushed tag"
         id: get_version_tag
         if: ${{ github.event_name == 'push' }}
         run: echo "VERSION=$(echo "${{ github.ref }}" | cut -d/ -f3)" >> $GITHUB_ENV
-      - name: output result into an env-var
+      - name: "🏷 Record VERSION for follow-up jobs"
         id: output_version
         run: |
           echo "version=${{ env.VERSION }}" >> $GITHUB_OUTPUT
   publish-image:
     needs: ['set-version']
-    name: 🐳 Build and deploy to a container repository
+    name: "🤙 Call app container workflow"
     uses: clamsproject/.github/.github/workflows/app-container.yml@main
     secrets: inherit
     with:
       version: ${{ needs.set-version.outputs.version }}
       arm64: false
   register-appdir:
     needs: ['set-version', 'publish-image']
-    name: 📝 Register to CLASM app directory
+    name: "🤙 Call app registration workflow"
     uses: clamsproject/apps/.github/workflows/register.yml@main
     secrets: inherit
     with:
       repo: ${{ github.repository }}
       tag: ${{ needs.set-version.outputs.version }}
       container: 'ghcr.io/${{ github.repository }}:${{ needs.set-version.outputs.version }}'
```

### Comparing `clams-python-0.6.2/clams/restify/__init__.py` & `clams-python-0.6.3/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams/source/__init__.py` & `clams-python-0.6.3/clams/source/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/clams_python.egg-info/PKG-INFO` & `clams-python-0.6.3/clams_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 0.6.2
+Version: 0.6.3
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-0.6.2/clams_python.egg-info/SOURCES.txt` & `clams-python-0.6.3/clams_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/setup.py` & `clams-python-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/tests/test_clamsapp.py` & `clams-python-0.6.3/tests/test_clamsapp.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.2/tests/test_clamscli.py` & `clams-python-0.6.3/tests/test_clamscli.py`

 * *Files identical despite different names*

