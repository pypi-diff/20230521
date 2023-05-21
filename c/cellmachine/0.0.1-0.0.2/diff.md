# Comparing `tmp/cellmachine-0.0.1.tar.gz` & `tmp/cellmachine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmachine-0.0.1.tar", last modified: Tue Jun 21 02:23:52 2022, max compression
+gzip compressed data, was "cellmachine-0.0.2.tar", last modified: Tue Jun 21 14:45:19 2022, max compression
```

## Comparing `cellmachine-0.0.1.tar` & `cellmachine-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 02:23:52.214356 cellmachine-0.0.1/
--rw-r--r--   0 189741     (502) staff       (20)    35149 2022-06-21 01:57:50.000000 cellmachine-0.0.1/LICENSE
--rw-r--r--   0 189741     (502) staff       (20)      633 2022-06-21 02:23:52.214239 cellmachine-0.0.1/PKG-INFO
--rw-r--r--   0 189741     (502) staff       (20)       70 2022-06-21 01:57:50.000000 cellmachine-0.0.1/README.md
--rw-r--r--   0 189741     (502) staff       (20)      636 2022-06-21 02:23:44.000000 cellmachine-0.0.1/pyproject.toml
--rw-r--r--   0 189741     (502) staff       (20)       38 2022-06-21 02:23:52.214390 cellmachine-0.0.1/setup.cfg
-drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 02:23:52.213263 cellmachine-0.0.1/src/
-drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 02:23:52.213721 cellmachine-0.0.1/src/cellmachine/
--rw-r--r--   0 189741     (502) staff       (20)        0 2022-06-21 02:20:07.000000 cellmachine-0.0.1/src/cellmachine/__init__.py
-drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 02:23:52.214081 cellmachine-0.0.1/src/cellmachine.egg-info/
--rw-r--r--   0 189741     (502) staff       (20)      633 2022-06-21 02:23:51.000000 cellmachine-0.0.1/src/cellmachine.egg-info/PKG-INFO
--rw-r--r--   0 189741     (502) staff       (20)      216 2022-06-21 02:23:52.000000 cellmachine-0.0.1/src/cellmachine.egg-info/SOURCES.txt
--rw-r--r--   0 189741     (502) staff       (20)        1 2022-06-21 02:23:51.000000 cellmachine-0.0.1/src/cellmachine.egg-info/dependency_links.txt
--rw-r--r--   0 189741     (502) staff       (20)       12 2022-06-21 02:23:52.000000 cellmachine-0.0.1/src/cellmachine.egg-info/top_level.txt
+drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 14:45:19.859187 cellmachine-0.0.2/
+-rw-r--r--   0 189741     (502) staff       (20)    35149 2022-06-21 01:57:50.000000 cellmachine-0.0.2/LICENSE
+-rw-r--r--   0 189741     (502) staff       (20)     6179 2022-06-21 14:45:19.859042 cellmachine-0.0.2/PKG-INFO
+-rw-r--r--   0 189741     (502) staff       (20)     5615 2022-06-21 14:43:54.000000 cellmachine-0.0.2/README.md
+-rw-r--r--   0 189741     (502) staff       (20)      636 2022-06-21 14:44:20.000000 cellmachine-0.0.2/pyproject.toml
+-rw-r--r--   0 189741     (502) staff       (20)       38 2022-06-21 14:45:19.859223 cellmachine-0.0.2/setup.cfg
+drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 14:45:19.857244 cellmachine-0.0.2/src/
+drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 14:45:19.858196 cellmachine-0.0.2/src/cellmachine/
+-rw-r--r--   0 189741     (502) staff       (20)     3880 2022-06-21 14:43:56.000000 cellmachine-0.0.2/src/cellmachine/__init__.py
+drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 14:45:19.858853 cellmachine-0.0.2/src/cellmachine.egg-info/
+-rw-r--r--   0 189741     (502) staff       (20)     6179 2022-06-21 14:45:19.000000 cellmachine-0.0.2/src/cellmachine.egg-info/PKG-INFO
+-rw-r--r--   0 189741     (502) staff       (20)      216 2022-06-21 14:45:19.000000 cellmachine-0.0.2/src/cellmachine.egg-info/SOURCES.txt
+-rw-r--r--   0 189741     (502) staff       (20)        1 2022-06-21 14:45:19.000000 cellmachine-0.0.2/src/cellmachine.egg-info/dependency_links.txt
+-rw-r--r--   0 189741     (502) staff       (20)       12 2022-06-21 14:45:19.000000 cellmachine-0.0.2/src/cellmachine.egg-info/top_level.txt
```

### Comparing `cellmachine-0.0.1/LICENSE` & `cellmachine-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmachine-0.0.1/PKG-INFO` & `cellmachine-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-Metadata-Version: 2.1
-Name: cellmachine
-Version: 0.0.1
-Summary: A python library to help with cell machine development
-Author-email: kegnh <william@kegnh.com>
-Project-URL: Homepage, https://github.com/itskegnh/cellmachine
-Project-URL: Bug Tracker, https://github.com/itskegnh/cellmachine/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
-# cellmachine
-A python library to help with cell machine development.
+[project]
+name = "cellmachine"
+version = "0.0.2"
+authors = [
+  { name="kegnh", email="william@kegnh.com" },
+]
+description = "A python library to help with cell machine development"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/itskegnh/cellmachine"
+"Bug Tracker" = "https://github.com/itskegnh/cellmachine/issues"
```

