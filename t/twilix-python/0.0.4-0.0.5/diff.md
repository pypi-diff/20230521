# Comparing `tmp/twilix-python-0.0.4.tar.gz` & `tmp/twilix-python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilix-python-0.0.4.tar", last modified: Sun May 21 12:28:17 2023, max compression
+gzip compressed data, was "twilix-python-0.0.5.tar", last modified: Sun May 21 12:30:52 2023, max compression
```

## Comparing `twilix-python-0.0.4.tar` & `twilix-python-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:28:17.275436 twilix-python-0.0.4/
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-05-20 02:14:08.000000 twilix-python-0.0.4/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-21 12:28:17.275286 twilix-python-0.0.4/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      133 2023-05-20 15:30:27.000000 twilix-python-0.0.4/README.md
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-05-21 12:28:17.275485 twilix-python-0.0.4/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      377 2023-05-21 11:54:37.000000 twilix-python-0.0.4/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:28:17.273874 twilix-python-0.0.4/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      575 2023-05-21 12:28:10.000000 twilix-python-0.0.4/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      360 2023-05-20 15:30:28.000000 twilix-python-0.0.4/tests/test_semantic_search.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:28:17.274261 twilix-python-0.0.4/twilix/
--rw-r--r--   0 jackywong   (501) staff       (20)     3149 2023-05-21 12:28:08.000000 twilix-python-0.0.4/twilix/__init__.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:28:17.275089 twilix-python-0.0.4/twilix_python.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-21 12:28:17.000000 twilix-python-0.0.4/twilix_python.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      278 2023-05-21 12:28:17.000000 twilix-python-0.0.4/twilix_python.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-05-21 12:28:17.000000 twilix-python-0.0.4/twilix_python.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-05-21 12:28:17.000000 twilix-python-0.0.4/twilix_python.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        7 2023-05-21 12:28:17.000000 twilix-python-0.0.4/twilix_python.egg-info/top_level.txt
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:30:52.168648 twilix-python-0.0.5/
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-05-20 02:14:08.000000 twilix-python-0.0.5/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-21 12:30:52.168482 twilix-python-0.0.5/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      133 2023-05-21 12:30:44.000000 twilix-python-0.0.5/README.md
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-05-21 12:30:52.168697 twilix-python-0.0.5/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      377 2023-05-21 12:30:48.000000 twilix-python-0.0.5/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:30:52.166689 twilix-python-0.0.5/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      575 2023-05-21 12:28:10.000000 twilix-python-0.0.5/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      360 2023-05-20 15:30:28.000000 twilix-python-0.0.5/tests/test_semantic_search.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:30:52.167091 twilix-python-0.0.5/twilix/
+-rw-r--r--   0 jackywong   (501) staff       (20)     3149 2023-05-21 12:28:08.000000 twilix-python-0.0.5/twilix/__init__.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:30:52.168140 twilix-python-0.0.5/twilix_python.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-21 12:30:52.000000 twilix-python-0.0.5/twilix_python.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      278 2023-05-21 12:30:52.000000 twilix-python-0.0.5/twilix_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-05-21 12:30:52.000000 twilix-python-0.0.5/twilix_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-05-21 12:30:52.000000 twilix-python-0.0.5/twilix_python.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        7 2023-05-21 12:30:52.000000 twilix-python-0.0.5/twilix_python.egg-info/top_level.txt
```

### Comparing `twilix-python-0.0.4/LICENSE` & `twilix-python-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twilix-python-0.0.4/tests/test_crud.py` & `twilix-python-0.0.5/tests/test_crud.py`

 * *Files identical despite different names*

### Comparing `twilix-python-0.0.4/twilix/__init__.py` & `twilix-python-0.0.5/twilix/__init__.py`

 * *Files identical despite different names*

