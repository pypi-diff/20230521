# Comparing `tmp/spiderYa-0.1.0.tar.gz` & `tmp/spiderYa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiderYa-0.1.0.tar", last modified: Sun May 21 14:43:58 2023, max compression
+gzip compressed data, was "spiderYa-0.1.1.tar", last modified: Sun May 21 15:06:35 2023, max compression
```

## Comparing `spiderYa-0.1.0.tar` & `spiderYa-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:43:57.951012 spiderYa-0.1.0/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1068 2023-05-21 14:40:37.000000 spiderYa-0.1.0/LICENSE
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 14:43:57.951012 spiderYa-0.1.0/PKG-INFO
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      170 2023-05-21 14:40:37.000000 spiderYa-0.1.0/README.md
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       78 2023-05-21 14:43:58.303005 spiderYa-0.1.0/setup.cfg
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1573 2023-05-21 14:43:35.000000 spiderYa-0.1.0/setup.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:43:57.803014 spiderYa-0.1.0/spider/
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:43:57.879013 spiderYa-0.1.0/spider/R_script/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/R_script/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      480 2023-05-21 14:40:41.000000 spiderYa-0.1.0/spider/R_script/run_SPARKX.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      765 2023-05-21 14:40:40.000000 spiderYa-0.1.0/spider/R_script/run_nnSVG.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2815 2023-05-21 14:40:41.000000 spiderYa-0.1.0/spider/R_script/run_spatalk.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6149 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/SPIDER.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:43:57.879013 spiderYa-0.1.0/spider/SpatialDE/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      802 2023-05-21 14:40:41.000000 spiderYa-0.1.0/spider/SpatialDE/__init__.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:43:57.951012 spiderYa-0.1.0/spider/SpatialDE/_internal/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1156 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/distance_cache.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11731 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/gpflow_helpers.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3326 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/kernels.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11116 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/models.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1150 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/optimizer.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9297 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/score_test.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     5569 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/sm_kernel.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11625 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/svca.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1762 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/tf_dataset.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3700 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/util.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2067 2023-05-21 14:40:45.000000 spiderYa-0.1.0/spider/SpatialDE/_internal/util_mixture.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    14715 2023-05-21 14:40:41.000000 spiderYa-0.1.0/spider/SpatialDE/aeh.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8305 2023-05-21 14:40:41.000000 spiderYa-0.1.0/spider/SpatialDE/de_test.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    16006 2023-05-21 14:40:41.000000 spiderYa-0.1.0/spider/SpatialDE/dp_hmrf.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13415 2023-05-21 14:40:41.000000 spiderYa-0.1.0/spider/SpatialDE/gaussian_process.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3323 2023-05-21 14:40:41.000000 spiderYa-0.1.0/spider/SpatialDE/io.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6818 2023-05-21 14:40:41.000000 spiderYa-0.1.0/spider/SpatialDE/svca.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       43 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2958 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/clustering.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9892 2023-05-21 14:40:37.000000 spiderYa-0.1.0/spider/enrichment.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:43:57.951012 spiderYa-0.1.0/spider/lrdb/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/lrdb/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8280 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/preprocess.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    26596 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/svi.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      996 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/trajectory.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2689 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/util.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       21 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/version.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    15772 2023-05-21 14:40:38.000000 spiderYa-0.1.0/spider/visualization.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:43:57.951012 spiderYa-0.1.0/spiderYa.egg-info/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 14:43:57.000000 spiderYa-0.1.0/spiderYa.egg-info/PKG-INFO
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1198 2023-05-21 14:43:57.000000 spiderYa-0.1.0/spiderYa.egg-info/SOURCES.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 14:43:57.000000 spiderYa-0.1.0/spiderYa.egg-info/dependency_links.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      303 2023-05-21 14:43:57.000000 spiderYa-0.1.0/spiderYa.egg-info/requires.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        7 2023-05-21 14:43:57.000000 spiderYa-0.1.0/spiderYa.egg-info/top_level.txt
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 15:06:35.338175 spiderYa-0.1.1/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1068 2023-05-21 14:40:37.000000 spiderYa-0.1.1/LICENSE
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 15:06:35.338175 spiderYa-0.1.1/PKG-INFO
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      170 2023-05-21 14:40:37.000000 spiderYa-0.1.1/README.md
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       78 2023-05-21 15:06:35.894165 spiderYa-0.1.1/setup.cfg
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1595 2023-05-21 15:06:18.000000 spiderYa-0.1.1/setup.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 15:06:35.134179 spiderYa-0.1.1/spider/
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 15:06:35.134179 spiderYa-0.1.1/spider/R_script/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/R_script/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      480 2023-05-21 14:40:41.000000 spiderYa-0.1.1/spider/R_script/run_SPARKX.R
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      765 2023-05-21 14:40:40.000000 spiderYa-0.1.1/spider/R_script/run_nnSVG.R
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2815 2023-05-21 14:40:41.000000 spiderYa-0.1.1/spider/R_script/run_spatalk.R
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6149 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/SPIDER.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 15:06:35.202178 spiderYa-0.1.1/spider/SpatialDE/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      802 2023-05-21 14:40:41.000000 spiderYa-0.1.1/spider/SpatialDE/__init__.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 15:06:35.202178 spiderYa-0.1.1/spider/SpatialDE/_internal/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1156 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/distance_cache.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11731 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/gpflow_helpers.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3326 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/kernels.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11116 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/models.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1150 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/optimizer.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9297 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/score_test.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     5569 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/sm_kernel.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11625 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/svca.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1762 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/tf_dataset.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3700 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/util.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2067 2023-05-21 14:40:45.000000 spiderYa-0.1.1/spider/SpatialDE/_internal/util_mixture.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    14715 2023-05-21 14:40:41.000000 spiderYa-0.1.1/spider/SpatialDE/aeh.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8305 2023-05-21 14:40:41.000000 spiderYa-0.1.1/spider/SpatialDE/de_test.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    16006 2023-05-21 14:40:41.000000 spiderYa-0.1.1/spider/SpatialDE/dp_hmrf.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13415 2023-05-21 14:40:41.000000 spiderYa-0.1.1/spider/SpatialDE/gaussian_process.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3323 2023-05-21 14:40:41.000000 spiderYa-0.1.1/spider/SpatialDE/io.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6818 2023-05-21 14:40:41.000000 spiderYa-0.1.1/spider/SpatialDE/svca.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       43 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2958 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/clustering.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9892 2023-05-21 14:40:37.000000 spiderYa-0.1.1/spider/enrichment.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 15:06:35.202178 spiderYa-0.1.1/spider/lrdb/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/lrdb/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8280 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/preprocess.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    26596 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/svi.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      996 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/trajectory.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2689 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/util.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       21 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/version.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    15772 2023-05-21 14:40:38.000000 spiderYa-0.1.1/spider/visualization.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 15:06:35.270177 spiderYa-0.1.1/spiderYa.egg-info/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 15:06:34.000000 spiderYa-0.1.1/spiderYa.egg-info/PKG-INFO
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1198 2023-05-21 15:06:35.000000 spiderYa-0.1.1/spiderYa.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 15:06:34.000000 spiderYa-0.1.1/spiderYa.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      314 2023-05-21 15:06:34.000000 spiderYa-0.1.1/spiderYa.egg-info/requires.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        7 2023-05-21 15:06:34.000000 spiderYa-0.1.1/spiderYa.egg-info/top_level.txt
```

### Comparing `spiderYa-0.1.0/LICENSE` & `spiderYa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/PKG-INFO` & `spiderYa-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiderYa
-Version: 0.1.0
+Version: 0.1.1
 Summary: Identifying spatially variable interactions
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiderYa-0.1.0/setup.py` & `spiderYa-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spiderYa",
-    version="0.1.0",
+    version="0.1.1",
     author="Li Shiying",
     author_email="shiyingli7-c@my.cityu.edu.hk",
     description="Identifying spatially variable interactions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepomicslab/SPIDER",
     packages=setuptools.find_packages(),
@@ -22,14 +22,15 @@
     ],
     
    package_data={'spider': ['lrdb/*.tsv'],
                  'spider': ['R_script/*.R']},
     
     install_requires=[
         'anndata>=0.8.0',
+        'numpy',
         'cellrank',
         'fa2',
         'gseapy',
         'h5py',
         'igraph',
         'leidenalg',
         'louvain',
@@ -43,15 +44,15 @@
         'pygco',
         'scanpy',
         'scgco',
         'scikit-learn',
         'scipy',
         'scvelo',
         'seaborn',
-        'sklearn',
+        'scikit-learn',
         'somde',
         'somoclu',
         # 'spaotsc',
         'spatialde',
         'stlearn',
         'umap-learn',
         'statsmodels',
```

### Comparing `spiderYa-0.1.0/spider/R_script/run_nnSVG.R` & `spiderYa-0.1.1/spider/R_script/run_nnSVG.R`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/R_script/run_spatalk.R` & `spiderYa-0.1.1/spider/R_script/run_spatalk.R`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SPIDER.py` & `spiderYa-0.1.1/spider/SPIDER.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/__init__.py` & `spiderYa-0.1.1/spider/SpatialDE/__init__.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/distance_cache.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/distance_cache.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/gpflow_helpers.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/gpflow_helpers.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/kernels.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/kernels.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/models.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/models.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/optimizer.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/optimizer.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/score_test.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/score_test.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/sm_kernel.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/sm_kernel.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/svca.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/svca.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/tf_dataset.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/tf_dataset.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/util.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/util.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/_internal/util_mixture.py` & `spiderYa-0.1.1/spider/SpatialDE/_internal/util_mixture.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/aeh.py` & `spiderYa-0.1.1/spider/SpatialDE/aeh.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/de_test.py` & `spiderYa-0.1.1/spider/SpatialDE/de_test.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/dp_hmrf.py` & `spiderYa-0.1.1/spider/SpatialDE/dp_hmrf.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/gaussian_process.py` & `spiderYa-0.1.1/spider/SpatialDE/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/io.py` & `spiderYa-0.1.1/spider/SpatialDE/io.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/SpatialDE/svca.py` & `spiderYa-0.1.1/spider/SpatialDE/svca.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/clustering.py` & `spiderYa-0.1.1/spider/clustering.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/enrichment.py` & `spiderYa-0.1.1/spider/enrichment.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/preprocess.py` & `spiderYa-0.1.1/spider/preprocess.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/svi.py` & `spiderYa-0.1.1/spider/svi.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/trajectory.py` & `spiderYa-0.1.1/spider/trajectory.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/util.py` & `spiderYa-0.1.1/spider/util.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spider/visualization.py` & `spiderYa-0.1.1/spider/visualization.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.0/spiderYa.egg-info/PKG-INFO` & `spiderYa-0.1.1/spiderYa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiderYa
-Version: 0.1.0
+Version: 0.1.1
 Summary: Identifying spatially variable interactions
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiderYa-0.1.0/spiderYa.egg-info/SOURCES.txt` & `spiderYa-0.1.1/spiderYa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

