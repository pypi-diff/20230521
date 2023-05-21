# Comparing `tmp/mixdiff-1.1.3.tar.gz` & `tmp/mixdiff-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixdiff-1.1.3.tar", last modified: Sat May 20 18:43:36 2023, max compression
+gzip compressed data, was "mixdiff-1.1.4.tar", last modified: Sun May 21 12:06:09 2023, max compression
```

## Comparing `mixdiff-1.1.3.tar` & `mixdiff-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:36.010338 mixdiff-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-20 18:43:25.000000 mixdiff-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-05-20 18:43:36.010338 mixdiff-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-05-20 18:43:25.000000 mixdiff-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:36.010338 mixdiff-1.1.3/mixdiff/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-20 18:43:25.000000 mixdiff-1.1.3/mixdiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20181 2023-05-20 18:43:25.000000 mixdiff-1.1.3/mixdiff/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-20 18:43:25.000000 mixdiff-1.1.3/mixdiff/extrasmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-20 18:43:25.000000 mixdiff-1.1.3/mixdiff/imgtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-05-20 18:43:25.000000 mixdiff-1.1.3/mixdiff/tiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:36.010338 mixdiff-1.1.3/mixdiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-05-20 18:43:35.000000 mixdiff-1.1.3/mixdiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-20 18:43:36.000000 mixdiff-1.1.3/mixdiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:43:35.000000 mixdiff-1.1.3/mixdiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-20 18:43:35.000000 mixdiff-1.1.3/mixdiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 18:43:35.000000 mixdiff-1.1.3/mixdiff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 18:43:36.010338 mixdiff-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-20 18:43:25.000000 mixdiff-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:06:09.149546 mixdiff-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-21 12:05:51.000000 mixdiff-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-05-21 12:06:09.145546 mixdiff-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-05-21 12:05:51.000000 mixdiff-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:06:09.145546 mixdiff-1.1.4/mixdiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-21 12:05:51.000000 mixdiff-1.1.4/mixdiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20181 2023-05-21 12:05:51.000000 mixdiff-1.1.4/mixdiff/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-21 12:05:51.000000 mixdiff-1.1.4/mixdiff/extrasmixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-21 12:05:51.000000 mixdiff-1.1.4/mixdiff/imgtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-05-21 12:05:51.000000 mixdiff-1.1.4/mixdiff/tiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:06:09.145546 mixdiff-1.1.4/mixdiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-05-21 12:06:09.000000 mixdiff-1.1.4/mixdiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 12:06:09.000000 mixdiff-1.1.4/mixdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:06:09.000000 mixdiff-1.1.4/mixdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-21 12:06:09.000000 mixdiff-1.1.4/mixdiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 12:06:09.000000 mixdiff-1.1.4/mixdiff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 12:06:09.149546 mixdiff-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-21 12:05:51.000000 mixdiff-1.1.4/setup.py
```

### Comparing `mixdiff-1.1.3/LICENSE` & `mixdiff-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mixdiff-1.1.3/PKG-INFO` & `mixdiff-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixdiff
-Version: 1.1.3
+Version: 1.1.4
 Summary: Mixture of Diffusers for scene composition and high resolution image generation .
 Home-page: https://github.com/albarji/mixture-of-diffusers
 Author: Alvaro Barbero
 License: MIT
 Keywords: artificial-intelligence,deep-learning,diffusion-models
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

### Comparing `mixdiff-1.1.3/README.md` & `mixdiff-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mixdiff-1.1.3/mixdiff/canvas.py` & `mixdiff-1.1.4/mixdiff/canvas.py`

 * *Files identical despite different names*

### Comparing `mixdiff-1.1.3/mixdiff/extrasmixin.py` & `mixdiff-1.1.4/mixdiff/extrasmixin.py`

 * *Files identical despite different names*

### Comparing `mixdiff-1.1.3/mixdiff/imgtools.py` & `mixdiff-1.1.4/mixdiff/imgtools.py`

 * *Files identical despite different names*

### Comparing `mixdiff-1.1.3/mixdiff/tiling.py` & `mixdiff-1.1.4/mixdiff/tiling.py`

 * *Files identical despite different names*

### Comparing `mixdiff-1.1.3/mixdiff.egg-info/PKG-INFO` & `mixdiff-1.1.4/mixdiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixdiff
-Version: 1.1.3
+Version: 1.1.4
 Summary: Mixture of Diffusers for scene composition and high resolution image generation .
 Home-page: https://github.com/albarji/mixture-of-diffusers
 Author: Alvaro Barbero
 License: MIT
 Keywords: artificial-intelligence,deep-learning,diffusion-models
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

### Comparing `mixdiff-1.1.3/setup.py` & `mixdiff-1.1.4/setup.py`

 * *Files identical despite different names*

