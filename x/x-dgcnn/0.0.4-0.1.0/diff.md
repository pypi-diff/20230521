# Comparing `tmp/x-dgcnn-0.0.4.tar.gz` & `tmp/x-dgcnn-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-dgcnn-0.0.4.tar", last modified: Sun May 21 18:40:27 2023, max compression
+gzip compressed data, was "x-dgcnn-0.1.0.tar", last modified: Sun May 21 18:46:26 2023, max compression
```

## Comparing `x-dgcnn-0.0.4.tar` & `x-dgcnn-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:40:27.052287 x-dgcnn-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-21 18:40:16.000000 x-dgcnn-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-21 18:40:27.052287 x-dgcnn-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-21 18:40:16.000000 x-dgcnn-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:40:27.052287 x-dgcnn-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-21 18:40:16.000000 x-dgcnn-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:40:27.052287 x-dgcnn-0.0.4/x_dgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-21 18:40:16.000000 x-dgcnn-0.0.4/x_dgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-05-21 18:40:16.000000 x-dgcnn-0.0.4/x_dgcnn/dgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-21 18:40:16.000000 x-dgcnn-0.0.4/x_dgcnn/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:40:27.052287 x-dgcnn-0.0.4/x_dgcnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-21 18:40:27.000000 x-dgcnn-0.0.4/x_dgcnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-21 18:40:27.000000 x-dgcnn-0.0.4/x_dgcnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:40:27.000000 x-dgcnn-0.0.4/x_dgcnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 18:40:27.000000 x-dgcnn-0.0.4/x_dgcnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 18:40:27.000000 x-dgcnn-0.0.4/x_dgcnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:46:26.846300 x-dgcnn-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-21 18:46:16.000000 x-dgcnn-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-21 18:46:26.846300 x-dgcnn-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-21 18:46:16.000000 x-dgcnn-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:46:26.846300 x-dgcnn-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-21 18:46:16.000000 x-dgcnn-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:46:26.846300 x-dgcnn-0.1.0/x_dgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-21 18:46:16.000000 x-dgcnn-0.1.0/x_dgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-05-21 18:46:16.000000 x-dgcnn-0.1.0/x_dgcnn/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-21 18:46:16.000000 x-dgcnn-0.1.0/x_dgcnn/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:46:26.846300 x-dgcnn-0.1.0/x_dgcnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-21 18:46:26.000000 x-dgcnn-0.1.0/x_dgcnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-21 18:46:26.000000 x-dgcnn-0.1.0/x_dgcnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:46:26.000000 x-dgcnn-0.1.0/x_dgcnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 18:46:26.000000 x-dgcnn-0.1.0/x_dgcnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 18:46:26.000000 x-dgcnn-0.1.0/x_dgcnn.egg-info/top_level.txt
```

### Comparing `x-dgcnn-0.0.4/LICENSE` & `x-dgcnn-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.0.4/PKG-INFO` & `x-dgcnn-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.0.4
+Version: 0.1.0
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `x-dgcnn-0.0.4/README.md` & `x-dgcnn-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.0.4/setup.py` & `x-dgcnn-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='x-dgcnn',
     packages=find_packages(),
-    version='0.0.4',
+    version='0.1.0',
     license='MIT',
     description='X-DGCNN - Pytorch',
     author='Kaidi Shen',
     url='https://github.com/kentechx/x-dgcnn',
     long_description_content_type='text/markdown',
     keywords=[
         '3D segmentation',
```

### Comparing `x-dgcnn-0.0.4/x_dgcnn/dgcnn.py` & `x-dgcnn-0.1.0/x_dgcnn/dgcnn.py`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.0.4/x_dgcnn/route.py` & `x-dgcnn-0.1.0/x_dgcnn/route.py`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.0.4/x_dgcnn.egg-info/PKG-INFO` & `x-dgcnn-0.1.0/x_dgcnn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.0.4
+Version: 0.1.0
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

