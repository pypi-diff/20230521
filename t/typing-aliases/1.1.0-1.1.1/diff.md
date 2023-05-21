# Comparing `tmp/typing_aliases-1.1.0.tar.gz` & `tmp/typing_aliases-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_aliases-1.1.0.tar", max compression
+gzip compressed data, was "typing_aliases-1.1.1.tar", max compression
```

## Comparing `typing_aliases-1.1.0.tar` & `typing_aliases-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1092 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/LICENSE
--rw-r--r--   0        0        0     2809 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/README.md
--rw-r--r--   0        0        0     2657 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4600 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/typing_aliases/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/typing_aliases/py.typed
--rw-r--r--   0        0        0    16879 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/typing_aliases/typing.py
--rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 typing_aliases-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-21 10:57:14.774041 typing_aliases-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2809 2023-05-21 10:57:14.774041 typing_aliases-1.1.1/README.md
+-rw-r--r--   0        0        0     2657 2023-05-21 10:57:14.778041 typing_aliases-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4600 2023-05-21 10:57:14.778041 typing_aliases-1.1.1/typing_aliases/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:57:14.778041 typing_aliases-1.1.1/typing_aliases/py.typed
+-rw-r--r--   0        0        0    16854 2023-05-21 10:57:14.778041 typing_aliases-1.1.1/typing_aliases/typing.py
+-rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 typing_aliases-1.1.1/PKG-INFO
```

### Comparing `typing_aliases-1.1.0/LICENSE` & `typing_aliases-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typing_aliases-1.1.0/README.md` & `typing_aliases-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 $ poetry add typing-aliases
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-typing-aliases = "^1.1.0"
+typing-aliases = "^1.1.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.typing-aliases]
 git = "https://github.com/nekitdev/typing-aliases.git"
```

### Comparing `typing_aliases-1.1.0/pyproject.toml` & `typing_aliases-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typing-aliases"
-version = "1.1.0"
+version = "1.1.1"
 description = "Various type aliases."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/typing-aliases"
@@ -102,15 +102,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "typing-aliases"
-version = "1.1.0"
+version = "1.1.1"
 url = "https://github.com/nekitdev/typing-aliases"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `typing_aliases-1.1.0/typing_aliases/__init__.py` & `typing_aliases-1.1.1/typing_aliases/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Various type aliases."
 __url__ = "https://github.com/nekitdev/typing-aliases"
 
 __title__ = "typing_aliases"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 from typing_aliases.typing import (
     AnyAsyncCallable,
     AnyAsyncContextManager,
     AnyCallable,
     AnyContextManager,
     AnyError,
```

### Comparing `typing_aliases-1.1.0/typing_aliases/typing.py` & `typing_aliases-1.1.1/typing_aliases/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
 """Represents async selectors."""
 AnySelectors = AnyIterable[bool]
 """Represents any selectors, async or not."""
 
 # recursive iterables
 
 RecursiveIterable = Union[T, Iterable["RecursiveIterable[T]"]]
-"""Represents recursive iterables, up to 8 levels in depth."""
+"""Represents recursive iterables."""
 
 RecursiveAsyncIterable = Union[T, AsyncIterable["RecursiveAsyncIterable[T]"]]
 """Represents recursive async iterables."""
 
 RecursiveAnyIterable = Union[T, AnyIterable["RecursiveAnyIterable[T]"]]
 """Represents recursive iterables, async or not."""
```

### Comparing `typing_aliases-1.1.0/PKG-INFO` & `typing_aliases-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing-aliases
-Version: 1.1.0
+Version: 1.1.1
 Summary: Various type aliases.
 Home-page: https://github.com/nekitdev/typing-aliases
 License: MIT
 Keywords: python,typing,alias
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -67,15 +67,15 @@
 $ poetry add typing-aliases
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-typing-aliases = "^1.1.0"
+typing-aliases = "^1.1.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.typing-aliases]
 git = "https://github.com/nekitdev/typing-aliases.git"
```

