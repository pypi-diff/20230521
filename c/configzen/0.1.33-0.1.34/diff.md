# Comparing `tmp/configzen-0.1.33.tar.gz` & `tmp/configzen-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.33.tar", max compression
+gzip compressed data, was "configzen-0.1.34.tar", max compression
```

## Comparing `configzen-0.1.33.tar` & `configzen-0.1.34.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.33/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.33/configzen/__main__.py
--rw-r--r--   0        0        0    56484 2023-05-21 16:34:20.655362 configzen-0.1.33/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.33/configzen/errors.py
--rw-r--r--   0        0        0    20369 2023-05-21 16:37:17.254969 configzen-0.1.33/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.33/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.33/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.33/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-21 16:39:02.994137 configzen-0.1.33/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.33/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.33/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.34/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.34/configzen/__main__.py
+-rw-r--r--   0        0        0    56484 2023-05-21 16:34:20.655362 configzen-0.1.34/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.34/configzen/errors.py
+-rw-r--r--   0        0        0    20374 2023-05-21 16:41:09.970722 configzen-0.1.34/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.34/configzen/py.typed
+-rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.34/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.34/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-21 16:41:56.770760 configzen-0.1.34/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.34/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.34/PKG-INFO
```

### Comparing `configzen-0.1.33/configzen/__main__.py` & `configzen-0.1.34/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.33/configzen/config.py` & `configzen-0.1.34/configzen/config.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.33/configzen/errors.py` & `configzen-0.1.34/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.33/configzen/processor.py` & `configzen-0.1.34/configzen/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -685,15 +685,15 @@
             state |= {substitution_directive: resource} | {
                 key: state.pop(key) for key in set(state)
             }
 
         state |= overrides
         extras: dict[str, Any] = {
             key: state.pop(key)
-            for key in state
+            for key in set(state)
             if key not in key_order
         }
 
         # Preserve the order of keys in the original configuration.
         for key in filter(state.__contains__, key_order):
             state[key] = state.pop(key)
```

### Comparing `configzen-0.1.33/configzen/typedefs.py` & `configzen-0.1.34/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.33/LICENSE` & `configzen-0.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.33/pyproject.toml` & `configzen-0.1.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.33"
+version = "0.1.34"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.33/README.md` & `configzen-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.33/PKG-INFO` & `configzen-0.1.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.33
+Version: 0.1.34
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

