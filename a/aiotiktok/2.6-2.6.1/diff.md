# Comparing `tmp/aiotiktok-2.6.tar.gz` & `tmp/aiotiktok-2.6.1.tar.gz`

## Comparing `aiotiktok-2.6.tar` & `aiotiktok-2.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/__init__.py
--rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/client.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/constants.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/exceptions.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/extractors.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 aiotiktok-2.6/aiotiktok/types.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiotiktok-2.6/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.6/LICENSE
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 aiotiktok-2.6/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 aiotiktok-2.6/pyproject.toml
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 aiotiktok-2.6/PKG-INFO
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/__init__.py
+-rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/client.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/constants.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/exceptions.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/extractors.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/types.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/LICENSE
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/PKG-INFO
```

### Comparing `aiotiktok-2.6/aiotiktok/client.py` & `aiotiktok-2.6.1/aiotiktok/client.py`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6/aiotiktok/constants.py` & `aiotiktok-2.6.1/aiotiktok/constants.py`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6/aiotiktok/extractors.py` & `aiotiktok-2.6.1/aiotiktok/extractors.py`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6/aiotiktok/types.py` & `aiotiktok-2.6.1/aiotiktok/types.py`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6/.gitignore` & `aiotiktok-2.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6/LICENSE` & `aiotiktok-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6/README.md` & `aiotiktok-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6/pyproject.toml` & `aiotiktok-2.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     { name = "sheldy" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "aiohttp",
-    "pydantic",
+    "httpx",
+    "msgspec",
 ]
 
 [project.urls]
 Homepage = "https://github.com/sheldygg/aiotiktok"
 
 [tool.hatch.version]
 path = "aiotiktok/__init__.py"
```

### Comparing `aiotiktok-2.6/PKG-INFO` & `aiotiktok-2.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: aiotiktok
-Version: 2.6
+Version: 2.6.1
 Summary: Tool for parse tiktok data
 Project-URL: Homepage, https://github.com/sheldygg/aiotiktok
 Author: sheldy
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: aiohttp
-Requires-Dist: pydantic
+Requires-Dist: httpx
+Requires-Dist: msgspec
 Description-Content-Type: text/markdown
 
 # aiotiktok
 
 [![PyPi Package Version](https://img.shields.io/pypi/v/aiotiktok?color=blue)](https://pypi.org/project/aiotiktok/)
 [![Downloads](https://img.shields.io/pypi/dm/aiotiktok?color=blue)](https://pypi.org/project/aiotiktok/)
```

