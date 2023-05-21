# Comparing `tmp/configzen-0.1.34.tar.gz` & `tmp/configzen-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.34.tar", max compression
+gzip compressed data, was "configzen-0.1.35.tar", max compression
```

## Comparing `configzen-0.1.34.tar` & `configzen-0.1.35.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.34/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.34/configzen/__main__.py
--rw-r--r--   0        0        0    56484 2023-05-21 16:34:20.655362 configzen-0.1.34/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.34/configzen/errors.py
--rw-r--r--   0        0        0    20374 2023-05-21 16:41:09.970722 configzen-0.1.34/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.34/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.34/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.34/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-21 16:41:56.770760 configzen-0.1.34/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.34/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.34/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.35/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.35/configzen/__main__.py
+-rw-r--r--   0        0        0    56484 2023-05-21 16:34:20.655362 configzen-0.1.35/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.35/configzen/errors.py
+-rw-r--r--   0        0        0    20443 2023-05-21 16:48:48.942144 configzen-0.1.35/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.35/configzen/py.typed
+-rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.35/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.35/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-21 16:49:17.892476 configzen-0.1.35/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.35/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.35/PKG-INFO
```

### Comparing `configzen-0.1.34/configzen/__main__.py` & `configzen-0.1.35/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.34/configzen/config.py` & `configzen-0.1.35/configzen/config.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.34/configzen/errors.py` & `configzen-0.1.35/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.34/configzen/processor.py` & `configzen-0.1.35/configzen/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -672,29 +672,31 @@
             elif counterpart_value != value:
                 overrides[key] = counterpart_value
                 del substituted_values[key]
 
         for value in state.values():
             cls.export(value, metadata=None)
 
+        # TODO: Optimize. We iterate over the same about 3-4 times.
+
+        state |= overrides
+        extras: dict[str, Any] = {
+            key: state.pop(key)
+            for key in set(state)
+            if key not in key_order
+        }
+
         if substituted_values:
             substitution_directive = cls.directive(Directives.EXTEND)
             resource = context.loader.resource
             if route:
                 resource = cls.route_separator.join((str(resource), route))
             # Put the substitution directive at the beginning of the state in-place.
             state |= {substitution_directive: resource} | {
                 key: state.pop(key) for key in set(state)
             }
 
-        state |= overrides
-        extras: dict[str, Any] = {
-            key: state.pop(key)
-            for key in set(state)
-            if key not in key_order
-        }
-
         # Preserve the order of keys in the original configuration.
         for key in filter(state.__contains__, key_order):
             state[key] = state.pop(key)
 
         state |= extras
```

### Comparing `configzen-0.1.34/configzen/typedefs.py` & `configzen-0.1.35/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.34/LICENSE` & `configzen-0.1.35/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.34/pyproject.toml` & `configzen-0.1.35/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.34"
+version = "0.1.35"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.34/README.md` & `configzen-0.1.35/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.34/PKG-INFO` & `configzen-0.1.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.34
+Version: 0.1.35
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

