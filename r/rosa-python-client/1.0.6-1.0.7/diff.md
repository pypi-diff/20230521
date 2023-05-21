# Comparing `tmp/rosa_python_client-1.0.6.tar.gz` & `tmp/rosa_python_client-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosa_python_client-1.0.6.tar", max compression
+gzip compressed data, was "rosa_python_client-1.0.7.tar", max compression
```

## Comparing `rosa_python_client-1.0.6.tar` & `rosa_python_client-1.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      511 2023-05-18 17:04:08.629169 rosa_python_client-1.0.6/README.md
--rw-r--r--   0        0        0      353 2023-05-18 17:04:08.629169 rosa_python_client-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-18 17:04:08.629169 rosa_python_client-1.0.6/rosa/__init__.py
--rw-r--r--   0        0        0     5360 2023-05-18 17:04:08.629169 rosa_python_client-1.0.6/rosa/cli.py
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rosa_python_client-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      511 2023-05-21 12:42:53.461794 rosa_python_client-1.0.7/README.md
+-rw-r--r--   0        0        0      353 2023-05-21 12:42:53.462794 rosa_python_client-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-21 12:42:53.462794 rosa_python_client-1.0.7/rosa/__init__.py
+-rw-r--r--   0        0        0     5360 2023-05-21 12:42:53.462794 rosa_python_client-1.0.7/rosa/cli.py
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rosa_python_client-1.0.7/PKG-INFO
```

### Comparing `rosa_python_client-1.0.6/rosa/cli.py` & `rosa_python_client-1.0.7/rosa/cli.py`

 * *Files identical despite different names*

### Comparing `rosa_python_client-1.0.6/PKG-INFO` & `rosa_python_client-1.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosa-python-client
-Version: 1.0.6
+Version: 1.0.7
 Summary: Wrapper for rosa cli
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

