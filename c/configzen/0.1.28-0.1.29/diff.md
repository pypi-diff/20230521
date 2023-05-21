# Comparing `tmp/configzen-0.1.28.tar.gz` & `tmp/configzen-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.28.tar", max compression
+gzip compressed data, was "configzen-0.1.29.tar", max compression
```

## Comparing `configzen-0.1.28.tar` & `configzen-0.1.29.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.28/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.28/configzen/__main__.py
--rw-r--r--   0        0        0    55495 2023-05-21 04:44:38.904137 configzen-0.1.28/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.28/configzen/errors.py
--rw-r--r--   0        0        0    19854 2023-05-21 04:35:55.247433 configzen-0.1.28/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.28/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.28/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.28/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-21 04:45:33.672600 configzen-0.1.28/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.28/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.28/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.29/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.29/configzen/__main__.py
+-rw-r--r--   0        0        0    55527 2023-05-21 05:27:05.631245 configzen-0.1.29/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.29/configzen/errors.py
+-rw-r--r--   0        0        0    19854 2023-05-21 04:35:55.247433 configzen-0.1.29/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.29/configzen/py.typed
+-rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.29/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.29/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-21 05:30:21.377497 configzen-0.1.29/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.29/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.29/PKG-INFO
```

### Comparing `configzen-0.1.28/configzen/__main__.py` & `configzen-0.1.29/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.28/configzen/config.py` & `configzen-0.1.29/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1689,15 +1689,15 @@
         ):
             context.enter(name).bind_to(value)
         return value
 
     def __deepcopy__(
         self: ConfigModelT, memodict: dict[Any, Any] | None = None
     ) -> ConfigModelT:
-        return self.parse_obj(export(self))
+        return type(self)(**copy.deepcopy(dict(self._iter(to_dict=False))))
 
     def __getattribute__(self, attr: str) -> Any:
         value = super().__getattribute__(attr)
         if isinstance(value, ConfigModel):
             return self._ensure_settings_with_context(attr, value)
         return value
```

### Comparing `configzen-0.1.28/configzen/errors.py` & `configzen-0.1.29/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.28/configzen/processor.py` & `configzen-0.1.29/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.28/configzen/typedefs.py` & `configzen-0.1.29/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.28/LICENSE` & `configzen-0.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.28/pyproject.toml` & `configzen-0.1.29/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.28"
+version = "0.1.29"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.28/README.md` & `configzen-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.28/PKG-INFO` & `configzen-0.1.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.28
+Version: 0.1.29
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

