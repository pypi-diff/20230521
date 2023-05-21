# Comparing `tmp/spiderYa-0.1.3.tar.gz` & `tmp/spiderYa-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiderYa-0.1.3.tar", last modified: Sun May 21 16:11:36 2023, max compression
+gzip compressed data, was "spiderYa-0.1.4.tar", last modified: Sun May 21 16:15:00 2023, max compression
```

## Comparing `spiderYa-0.1.3.tar` & `spiderYa-0.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:11:36.793174 spiderYa-0.1.3/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1068 2023-05-21 14:40:37.000000 spiderYa-0.1.3/LICENSE
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 16:11:36.793174 spiderYa-0.1.3/PKG-INFO
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      170 2023-05-21 14:40:37.000000 spiderYa-0.1.3/README.md
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       78 2023-05-21 16:11:36.809174 spiderYa-0.1.3/setup.cfg
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1636 2023-05-21 16:11:25.000000 spiderYa-0.1.3/setup.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:11:36.525179 spiderYa-0.1.3/spider/
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:11:36.665176 spiderYa-0.1.3/spider/R_script/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/R_script/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      480 2023-05-21 14:40:41.000000 spiderYa-0.1.3/spider/R_script/run_SPARKX.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      765 2023-05-21 14:40:40.000000 spiderYa-0.1.3/spider/R_script/run_nnSVG.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2815 2023-05-21 14:40:41.000000 spiderYa-0.1.3/spider/R_script/run_spatalk.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6149 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/SPIDER.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:11:36.665176 spiderYa-0.1.3/spider/SpatialDE/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      802 2023-05-21 14:40:41.000000 spiderYa-0.1.3/spider/SpatialDE/__init__.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:11:36.793174 spiderYa-0.1.3/spider/SpatialDE/_internal/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1156 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/distance_cache.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11731 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/gpflow_helpers.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3326 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/kernels.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11116 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/models.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1150 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/optimizer.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9297 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/score_test.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     5569 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/sm_kernel.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11625 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/svca.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1762 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/tf_dataset.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3700 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/util.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2067 2023-05-21 14:40:45.000000 spiderYa-0.1.3/spider/SpatialDE/_internal/util_mixture.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    14715 2023-05-21 14:40:41.000000 spiderYa-0.1.3/spider/SpatialDE/aeh.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8305 2023-05-21 14:40:41.000000 spiderYa-0.1.3/spider/SpatialDE/de_test.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    16006 2023-05-21 14:40:41.000000 spiderYa-0.1.3/spider/SpatialDE/dp_hmrf.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13415 2023-05-21 14:40:41.000000 spiderYa-0.1.3/spider/SpatialDE/gaussian_process.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3323 2023-05-21 14:40:41.000000 spiderYa-0.1.3/spider/SpatialDE/io.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6818 2023-05-21 14:40:41.000000 spiderYa-0.1.3/spider/SpatialDE/svca.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       43 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2958 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/clustering.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9892 2023-05-21 14:40:37.000000 spiderYa-0.1.3/spider/enrichment.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:11:36.793174 spiderYa-0.1.3/spider/lrdb/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/lrdb/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8280 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/preprocess.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    26596 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/svi.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      996 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/trajectory.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2689 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/util.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       21 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/version.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    15772 2023-05-21 14:40:38.000000 spiderYa-0.1.3/spider/visualization.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:11:36.793174 spiderYa-0.1.3/spiderYa.egg-info/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 16:11:36.000000 spiderYa-0.1.3/spiderYa.egg-info/PKG-INFO
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1198 2023-05-21 16:11:36.000000 spiderYa-0.1.3/spiderYa.egg-info/SOURCES.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 16:11:36.000000 spiderYa-0.1.3/spiderYa.egg-info/dependency_links.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      308 2023-05-21 16:11:36.000000 spiderYa-0.1.3/spiderYa.egg-info/requires.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        7 2023-05-21 16:11:36.000000 spiderYa-0.1.3/spiderYa.egg-info/top_level.txt
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:15:00.461361 spiderYa-0.1.4/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1068 2023-05-21 14:40:37.000000 spiderYa-0.1.4/LICENSE
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 16:15:00.461361 spiderYa-0.1.4/PKG-INFO
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      170 2023-05-21 14:40:37.000000 spiderYa-0.1.4/README.md
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       78 2023-05-21 16:15:00.553359 spiderYa-0.1.4/setup.cfg
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1638 2023-05-21 16:14:42.000000 spiderYa-0.1.4/setup.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:15:00.217365 spiderYa-0.1.4/spider/
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:15:00.345363 spiderYa-0.1.4/spider/R_script/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/R_script/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      480 2023-05-21 14:40:41.000000 spiderYa-0.1.4/spider/R_script/run_SPARKX.R
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      765 2023-05-21 14:40:40.000000 spiderYa-0.1.4/spider/R_script/run_nnSVG.R
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2815 2023-05-21 14:40:41.000000 spiderYa-0.1.4/spider/R_script/run_spatalk.R
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6149 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/SPIDER.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:15:00.345363 spiderYa-0.1.4/spider/SpatialDE/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      802 2023-05-21 14:40:41.000000 spiderYa-0.1.4/spider/SpatialDE/__init__.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:15:00.461361 spiderYa-0.1.4/spider/SpatialDE/_internal/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1156 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/distance_cache.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11731 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/gpflow_helpers.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3326 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/kernels.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11116 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/models.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1150 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/optimizer.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9297 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/score_test.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     5569 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/sm_kernel.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11625 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/svca.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1762 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/tf_dataset.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3700 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/util.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2067 2023-05-21 14:40:45.000000 spiderYa-0.1.4/spider/SpatialDE/_internal/util_mixture.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    14715 2023-05-21 14:40:41.000000 spiderYa-0.1.4/spider/SpatialDE/aeh.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8305 2023-05-21 14:40:41.000000 spiderYa-0.1.4/spider/SpatialDE/de_test.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    16006 2023-05-21 14:40:41.000000 spiderYa-0.1.4/spider/SpatialDE/dp_hmrf.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13415 2023-05-21 14:40:41.000000 spiderYa-0.1.4/spider/SpatialDE/gaussian_process.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3323 2023-05-21 14:40:41.000000 spiderYa-0.1.4/spider/SpatialDE/io.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6818 2023-05-21 14:40:41.000000 spiderYa-0.1.4/spider/SpatialDE/svca.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       43 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2958 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/clustering.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9892 2023-05-21 14:40:37.000000 spiderYa-0.1.4/spider/enrichment.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:15:00.461361 spiderYa-0.1.4/spider/lrdb/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/lrdb/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8280 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/preprocess.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    26596 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/svi.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      996 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/trajectory.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2689 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/util.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       21 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/version.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    15772 2023-05-21 14:40:38.000000 spiderYa-0.1.4/spider/visualization.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:15:00.461361 spiderYa-0.1.4/spiderYa.egg-info/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 16:14:59.000000 spiderYa-0.1.4/spiderYa.egg-info/PKG-INFO
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1198 2023-05-21 16:15:00.000000 spiderYa-0.1.4/spiderYa.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 16:15:00.000000 spiderYa-0.1.4/spiderYa.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      308 2023-05-21 16:15:00.000000 spiderYa-0.1.4/spiderYa.egg-info/requires.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        7 2023-05-21 16:15:00.000000 spiderYa-0.1.4/spiderYa.egg-info/top_level.txt
```

### Comparing `spiderYa-0.1.3/LICENSE` & `spiderYa-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/PKG-INFO` & `spiderYa-0.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiderYa
-Version: 0.1.3
+Version: 0.1.4
 Summary: Identifying spatially variable interactions
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiderYa-0.1.3/setup.py` & `spiderYa-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 import os
-os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
+# os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spiderYa",
-    version="0.1.3",
+    version="0.1.4",
     author="Li Shiying",
     author_email="shiyingli7-c@my.cityu.edu.hk",
     description="Identifying spatially variable interactions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepomicslab/SPIDER",
     packages=setuptools.find_packages(),
```

### Comparing `spiderYa-0.1.3/spider/R_script/run_nnSVG.R` & `spiderYa-0.1.4/spider/R_script/run_nnSVG.R`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/R_script/run_spatalk.R` & `spiderYa-0.1.4/spider/R_script/run_spatalk.R`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SPIDER.py` & `spiderYa-0.1.4/spider/SPIDER.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/__init__.py` & `spiderYa-0.1.4/spider/SpatialDE/__init__.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/distance_cache.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/distance_cache.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/gpflow_helpers.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/gpflow_helpers.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/kernels.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/kernels.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/models.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/models.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/optimizer.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/optimizer.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/score_test.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/score_test.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/sm_kernel.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/sm_kernel.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/svca.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/svca.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/tf_dataset.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/tf_dataset.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/util.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/util.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/_internal/util_mixture.py` & `spiderYa-0.1.4/spider/SpatialDE/_internal/util_mixture.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/aeh.py` & `spiderYa-0.1.4/spider/SpatialDE/aeh.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/de_test.py` & `spiderYa-0.1.4/spider/SpatialDE/de_test.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/dp_hmrf.py` & `spiderYa-0.1.4/spider/SpatialDE/dp_hmrf.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/gaussian_process.py` & `spiderYa-0.1.4/spider/SpatialDE/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/io.py` & `spiderYa-0.1.4/spider/SpatialDE/io.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/SpatialDE/svca.py` & `spiderYa-0.1.4/spider/SpatialDE/svca.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/clustering.py` & `spiderYa-0.1.4/spider/clustering.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/enrichment.py` & `spiderYa-0.1.4/spider/enrichment.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/preprocess.py` & `spiderYa-0.1.4/spider/preprocess.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/svi.py` & `spiderYa-0.1.4/spider/svi.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/trajectory.py` & `spiderYa-0.1.4/spider/trajectory.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/util.py` & `spiderYa-0.1.4/spider/util.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spider/visualization.py` & `spiderYa-0.1.4/spider/visualization.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.3/spiderYa.egg-info/PKG-INFO` & `spiderYa-0.1.4/spiderYa.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiderYa
-Version: 0.1.3
+Version: 0.1.4
 Summary: Identifying spatially variable interactions
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiderYa-0.1.3/spiderYa.egg-info/SOURCES.txt` & `spiderYa-0.1.4/spiderYa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

