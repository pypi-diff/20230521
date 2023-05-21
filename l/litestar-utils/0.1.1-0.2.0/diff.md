# Comparing `tmp/litestar_utils-0.1.1.tar.gz` & `tmp/litestar_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar_utils-0.1.1.tar", max compression
+gzip compressed data, was "litestar_utils-0.2.0.tar", max compression
```

## Comparing `litestar_utils-0.1.1.tar` & `litestar_utils-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1096 2023-05-04 13:26:52.978226 litestar_utils-0.1.1/LICENSE
--rw-r--r--   0        0        0      226 2023-05-04 09:02:18.816868 litestar_utils-0.1.1/litestar_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 12:13:26.826006 litestar_utils-0.1.1/litestar_utils/tasks.py
--rw-r--r--   0        0        0     1916 2023-05-04 14:08:56.030016 litestar_utils-0.1.1/litestar_utils/timing.py
--rw-r--r--   0        0        0      562 2023-05-04 14:28:54.295847 litestar_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1194 2023-05-04 14:25:22.540119 litestar_utils-0.1.1/README.md
--rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 litestar_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-04 13:26:52.978226 litestar_utils-0.2.0/LICENSE
+-rw-r--r--   0        0        0      312 2023-05-21 09:17:20.959053 litestar_utils-0.2.0/litestar_utils/__init__.py
+-rw-r--r--   0        0        0     1118 2023-05-21 09:17:20.959053 litestar_utils-0.2.0/litestar_utils/text.py
+-rw-r--r--   0        0        0     1916 2023-05-04 16:04:09.230309 litestar_utils-0.2.0/litestar_utils/timing.py
+-rw-r--r--   0        0        0      562 2023-05-21 09:17:20.959053 litestar_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2629 2023-05-21 09:17:20.959053 litestar_utils-0.2.0/README.md
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 litestar_utils-0.2.0/PKG-INFO
```

### Comparing `litestar_utils-0.1.1/LICENSE` & `litestar_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar_utils-0.1.1/litestar_utils/timing.py` & `litestar_utils-0.2.0/litestar_utils/timing.py`

 * *Files identical despite different names*

### Comparing `litestar_utils-0.1.1/pyproject.toml` & `litestar_utils-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litestar-utils"
-version = "0.1.1"
+version = "0.2.0"
 description = "Utilities for the Litestar framework."
 authors = ["Alessandro Ferrini <alessandro.ferrini@apptecsrl.com>"]
 readme = "README.md"
 packages = [{include = "litestar_utils"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

