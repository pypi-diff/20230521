# Comparing `tmp/cluedin-2.1.0.tar.gz` & `tmp/cluedin-2.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluedin-2.1.0.tar", max compression
+gzip compressed data, was "cluedin-2.1.0rc1.tar", max compression
```

## Comparing `cluedin-2.1.0.tar` & `cluedin-2.1.0rc1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1093 2023-05-01 19:58:59.989579 cluedin-2.1.0/LICENSE
--rw-r--r--   0        0        0     6887 2023-05-21 13:07:36.800967 cluedin-2.1.0/cluedin/README.md
--rw-r--r--   0        0        0      214 2023-05-21 12:33:01.908448 cluedin-2.1.0/cluedin/__init__.py
--rw-r--r--   0        0        0     9727 2023-05-20 19:26:50.338507 cluedin-2.1.0/cluedin/account.py
--rw-r--r--   0        0        0     5735 2023-05-14 19:14:24.796902 cluedin-2.1.0/cluedin/context.py
--rw-r--r--   0        0        0     1450 2023-05-21 13:07:14.463017 cluedin-2.1.0/cluedin/entity.py
--rw-r--r--   0        0        0      119 2023-05-14 19:14:24.797006 cluedin-2.1.0/cluedin/env.py
--rw-r--r--   0        0        0     2061 2023-05-14 19:14:24.797108 cluedin-2.1.0/cluedin/gql.py
--rw-r--r--   0        0        0      492 2023-05-14 19:14:24.797191 cluedin-2.1.0/cluedin/jwt.py
--rw-r--r--   0        0        0     3853 2023-05-14 19:14:24.797279 cluedin-2.1.0/cluedin/public.py
--rw-r--r--   0        0        0      669 2023-05-20 19:54:13.830640 cluedin-2.1.0/cluedin/vocab.py
--rw-r--r--   0        0        0      570 2023-05-21 14:32:06.881096 cluedin-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7585 1970-01-01 00:00:00.000000 cluedin-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-01 19:58:59.989579 cluedin-2.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     6887 2023-05-21 13:07:36.800967 cluedin-2.1.0rc1/cluedin/README.md
+-rw-r--r--   0        0        0      214 2023-05-21 12:33:01.908448 cluedin-2.1.0rc1/cluedin/__init__.py
+-rw-r--r--   0        0        0     9727 2023-05-20 19:26:50.338507 cluedin-2.1.0rc1/cluedin/account.py
+-rw-r--r--   0        0        0     5735 2023-05-14 19:14:24.796902 cluedin-2.1.0rc1/cluedin/context.py
+-rw-r--r--   0        0        0     1450 2023-05-21 13:07:14.463017 cluedin-2.1.0rc1/cluedin/entity.py
+-rw-r--r--   0        0        0      119 2023-05-14 19:14:24.797006 cluedin-2.1.0rc1/cluedin/env.py
+-rw-r--r--   0        0        0     2061 2023-05-14 19:14:24.797108 cluedin-2.1.0rc1/cluedin/gql.py
+-rw-r--r--   0        0        0      492 2023-05-14 19:14:24.797191 cluedin-2.1.0rc1/cluedin/jwt.py
+-rw-r--r--   0        0        0     3853 2023-05-14 19:14:24.797279 cluedin-2.1.0rc1/cluedin/public.py
+-rw-r--r--   0        0        0      669 2023-05-20 19:54:13.830640 cluedin-2.1.0rc1/cluedin/vocab.py
+-rw-r--r--   0        0        0      573 2023-05-21 14:27:36.205692 cluedin-2.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7588 1970-01-01 00:00:00.000000 cluedin-2.1.0rc1/PKG-INFO
```

### Comparing `cluedin-2.1.0/LICENSE` & `cluedin-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0/cluedin/README.md` & `cluedin-2.1.0rc1/cluedin/README.md`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0/cluedin/account.py` & `cluedin-2.1.0rc1/cluedin/account.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0/cluedin/context.py` & `cluedin-2.1.0rc1/cluedin/context.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0/cluedin/entity.py` & `cluedin-2.1.0rc1/cluedin/entity.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0/cluedin/gql.py` & `cluedin-2.1.0rc1/cluedin/gql.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0/cluedin/public.py` & `cluedin-2.1.0rc1/cluedin/public.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0/cluedin/vocab.py` & `cluedin-2.1.0rc1/cluedin/vocab.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.1.0/pyproject.toml` & `cluedin-2.1.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cluedin"
-version = "2.1.0"
+version = "2.1.0rc1"
 description = "A Python client for CluedIn API."
 authors = ["Roman Klimenko <romaklimenko@gmail.com>"]
 readme = "cluedin/README.md"
 license = "MIT"
 keywords = ["cluedin", "mdm", "master data management"]
 maintainers = ["Roman Klimenko <romaklimenko@gmail.com>"]
 homepage = "https://github.com/romaklimenko/cluedin"
```

### Comparing `cluedin-2.1.0/PKG-INFO` & `cluedin-2.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluedin
-Version: 2.1.0
+Version: 2.1.0rc1
 Summary: A Python client for CluedIn API.
 Home-page: https://github.com/romaklimenko/cluedin
 License: MIT
 Keywords: cluedin,mdm,master data management
 Author: Roman Klimenko
 Author-email: romaklimenko@gmail.com
 Maintainer: Roman Klimenko
```

