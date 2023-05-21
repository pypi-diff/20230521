# Comparing `tmp/cdklabs.appsync-utils-0.0.94.tar.gz` & `tmp/cdklabs.appsync-utils-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.appsync-utils-0.0.94.tar", last modified: Sat May 20 00:18:36 2023, max compression
+gzip compressed data, was "cdklabs.appsync-utils-0.0.95.tar", last modified: Sun May 21 00:17:13 2023, max compression
```

## Comparing `cdklabs.appsync-utils-0.0.94.tar` & `cdklabs.appsync-utils-0.0.95.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:18:36.575554 cdklabs.appsync-utils-0.0.94/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-20 00:18:19.000000 cdklabs.appsync-utils-0.0.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 00:18:19.000000 cdklabs.appsync-utils-0.0.94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-20 00:18:19.000000 cdklabs.appsync-utils-0.0.94/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-20 00:18:36.575554 cdklabs.appsync-utils-0.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-20 00:18:19.000000 cdklabs.appsync-utils-0.0.94/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-20 00:18:19.000000 cdklabs.appsync-utils-0.0.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:18:36.575554 cdklabs.appsync-utils-0.0.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-20 00:18:19.000000 cdklabs.appsync-utils-0.0.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:18:36.575554 cdklabs.appsync-utils-0.0.94/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:18:36.575554 cdklabs.appsync-utils-0.0.94/src/awscdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:18:36.575554 cdklabs.appsync-utils-0.0.94/src/awscdk/appsync_utils/
--rw-r--r--   0 runner    (1001) docker     (123)   134850 2023-05-20 00:18:19.000000 cdklabs.appsync-utils-0.0.94/src/awscdk/appsync_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:18:36.575554 cdklabs.appsync-utils-0.0.94/src/awscdk/appsync_utils/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-20 00:18:19.000000 cdklabs.appsync-utils-0.0.94/src/awscdk/appsync_utils/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82444 2023-05-20 00:18:19.000000 cdklabs.appsync-utils-0.0.94/src/awscdk/appsync_utils/_jsii/awscdk-appsync-utils@0.0.94.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:18:19.000000 cdklabs.appsync-utils-0.0.94/src/awscdk/appsync_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:18:36.575554 cdklabs.appsync-utils-0.0.94/src/cdklabs.appsync_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-20 00:18:36.000000 cdklabs.appsync-utils-0.0.94/src/cdklabs.appsync_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-20 00:18:36.000000 cdklabs.appsync-utils-0.0.94/src/cdklabs.appsync_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:18:36.000000 cdklabs.appsync-utils-0.0.94/src/cdklabs.appsync_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-20 00:18:36.000000 cdklabs.appsync-utils-0.0.94/src/cdklabs.appsync_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-20 00:18:36.000000 cdklabs.appsync-utils-0.0.94/src/cdklabs.appsync_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:17:13.064668 cdklabs.appsync-utils-0.0.95/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-21 00:16:59.000000 cdklabs.appsync-utils-0.0.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 00:16:59.000000 cdklabs.appsync-utils-0.0.95/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-21 00:16:59.000000 cdklabs.appsync-utils-0.0.95/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-21 00:17:13.064668 cdklabs.appsync-utils-0.0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-21 00:16:59.000000 cdklabs.appsync-utils-0.0.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-21 00:16:59.000000 cdklabs.appsync-utils-0.0.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:17:13.064668 cdklabs.appsync-utils-0.0.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-21 00:16:59.000000 cdklabs.appsync-utils-0.0.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:17:13.064668 cdklabs.appsync-utils-0.0.95/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:17:13.064668 cdklabs.appsync-utils-0.0.95/src/awscdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:17:13.064668 cdklabs.appsync-utils-0.0.95/src/awscdk/appsync_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   134850 2023-05-21 00:16:59.000000 cdklabs.appsync-utils-0.0.95/src/awscdk/appsync_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:17:13.064668 cdklabs.appsync-utils-0.0.95/src/awscdk/appsync_utils/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-21 00:16:59.000000 cdklabs.appsync-utils-0.0.95/src/awscdk/appsync_utils/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82441 2023-05-21 00:16:59.000000 cdklabs.appsync-utils-0.0.95/src/awscdk/appsync_utils/_jsii/awscdk-appsync-utils@0.0.95.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:16:59.000000 cdklabs.appsync-utils-0.0.95/src/awscdk/appsync_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:17:13.064668 cdklabs.appsync-utils-0.0.95/src/cdklabs.appsync_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-21 00:17:13.000000 cdklabs.appsync-utils-0.0.95/src/cdklabs.appsync_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-21 00:17:13.000000 cdklabs.appsync-utils-0.0.95/src/cdklabs.appsync_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:17:13.000000 cdklabs.appsync-utils-0.0.95/src/cdklabs.appsync_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-21 00:17:13.000000 cdklabs.appsync-utils-0.0.95/src/cdklabs.appsync_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 00:17:13.000000 cdklabs.appsync-utils-0.0.95/src/cdklabs.appsync_utils.egg-info/top_level.txt
```

### Comparing `cdklabs.appsync-utils-0.0.94/LICENSE` & `cdklabs.appsync-utils-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.94/PKG-INFO` & `cdklabs.appsync-utils-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.appsync-utils
-Version: 0.0.94
+Version: 0.0.95
 Summary: Utilities for creating appsync apis using aws-cdk
 Home-page: https://github.com/cdklabs/awscdk-appsync-utils.git
 Author: Mitchell Valine<mitchellvaline@yahoo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/awscdk-appsync-utils.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.appsync-utils-0.0.94/README.md` & `cdklabs.appsync-utils-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.94/setup.py` & `cdklabs.appsync-utils-0.0.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.appsync-utils",
-    "version": "0.0.94",
+    "version": "0.0.95",
     "description": "Utilities for creating appsync apis using aws-cdk",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/awscdk-appsync-utils.git",
     "long_description_content_type": "text/markdown",
     "author": "Mitchell Valine<mitchellvaline@yahoo.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "awscdk.appsync_utils",
         "awscdk.appsync_utils._jsii"
     ],
     "package_data": {
         "awscdk.appsync_utils._jsii": [
-            "awscdk-appsync-utils@0.0.94.jsii.tgz"
+            "awscdk-appsync-utils@0.0.95.jsii.tgz"
         ],
         "awscdk.appsync_utils": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdklabs.appsync-utils-0.0.94/src/awscdk/appsync_utils/__init__.py` & `cdklabs.appsync-utils-0.0.95/src/awscdk/appsync_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.94/src/cdklabs.appsync_utils.egg-info/PKG-INFO` & `cdklabs.appsync-utils-0.0.95/src/cdklabs.appsync_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.appsync-utils
-Version: 0.0.94
+Version: 0.0.95
 Summary: Utilities for creating appsync apis using aws-cdk
 Home-page: https://github.com/cdklabs/awscdk-appsync-utils.git
 Author: Mitchell Valine<mitchellvaline@yahoo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/awscdk-appsync-utils.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

