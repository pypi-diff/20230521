# Comparing `tmp/ResponsePrediction-0.0.4.tar.gz` & `tmp/ResponsePrediction-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ResponsePrediction-0.0.4.tar", last modified: Tue May  2 11:54:25 2023, max compression
+gzip compressed data, was "ResponsePrediction-0.0.5.tar", last modified: Sun May 21 11:59:07 2023, max compression
```

## Comparing `ResponsePrediction-0.0.4.tar` & `ResponsePrediction-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41009 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/src/ResponsePrediction/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-02 11:54:19.000000 ResponsePrediction-0.0.4/src/ResponsePrediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/src/ResponsePrediction/_deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/src/ResponsePrediction/_stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-02 11:54:14.000000 ResponsePrediction-0.0.4/src/ResponsePrediction/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:54:25.844715 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41009 2023-05-02 11:54:25.000000 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-02 11:54:25.000000 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:54:25.000000 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 11:54:25.000000 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 11:54:25.000000 ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:59:07.565404 ResponsePrediction-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 11:58:48.000000 ResponsePrediction-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41009 2023-05-21 11:59:07.565404 ResponsePrediction-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 11:58:48.000000 ResponsePrediction-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-21 11:58:48.000000 ResponsePrediction-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 11:59:07.565404 ResponsePrediction-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:59:07.561404 ResponsePrediction-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:59:07.561404 ResponsePrediction-0.0.5/src/ResponsePrediction/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 11:58:58.000000 ResponsePrediction-0.0.5/src/ResponsePrediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-05-21 11:58:48.000000 ResponsePrediction-0.0.5/src/ResponsePrediction/_deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-21 11:58:48.000000 ResponsePrediction-0.0.5/src/ResponsePrediction/_stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-21 11:58:48.000000 ResponsePrediction-0.0.5/src/ResponsePrediction/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:59:07.565404 ResponsePrediction-0.0.5/src/ResponsePrediction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41009 2023-05-21 11:59:07.000000 ResponsePrediction-0.0.5/src/ResponsePrediction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-21 11:59:07.000000 ResponsePrediction-0.0.5/src/ResponsePrediction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:59:07.000000 ResponsePrediction-0.0.5/src/ResponsePrediction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 11:59:07.000000 ResponsePrediction-0.0.5/src/ResponsePrediction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 11:59:07.000000 ResponsePrediction-0.0.5/src/ResponsePrediction.egg-info/top_level.txt
```

### Comparing `ResponsePrediction-0.0.4/LICENSE` & `ResponsePrediction-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ResponsePrediction-0.0.4/PKG-INFO` & `ResponsePrediction-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResponsePrediction
-Version: 0.0.4
+Version: 0.0.5
 Summary: Vessel wave-induced response prediction
 Author-email: Jan-Erik Hygen <j-e.hygen@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ResponsePrediction-0.0.4/pyproject.toml` & `ResponsePrediction-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ResponsePrediction-0.0.4/src/ResponsePrediction/_stochastic.py` & `ResponsePrediction-0.0.5/src/ResponsePrediction/_stochastic.py`

 * *Files identical despite different names*

### Comparing `ResponsePrediction-0.0.4/src/ResponsePrediction/_tools.py` & `ResponsePrediction-0.0.5/src/ResponsePrediction/_tools.py`

 * *Files identical despite different names*

### Comparing `ResponsePrediction-0.0.4/src/ResponsePrediction.egg-info/PKG-INFO` & `ResponsePrediction-0.0.5/src/ResponsePrediction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResponsePrediction
-Version: 0.0.4
+Version: 0.0.5
 Summary: Vessel wave-induced response prediction
 Author-email: Jan-Erik Hygen <j-e.hygen@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

