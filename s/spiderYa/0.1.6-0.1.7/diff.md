# Comparing `tmp/spiderYa-0.1.6.tar.gz` & `tmp/spiderYa-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiderYa-0.1.6.tar", last modified: Sun May 21 16:44:24 2023, max compression
+gzip compressed data, was "spiderYa-0.1.7.tar", last modified: Sun May 21 17:14:55 2023, max compression
```

## Comparing `spiderYa-0.1.6.tar` & `spiderYa-0.1.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:44:24.003976 spiderYa-0.1.6/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1068 2023-05-21 14:40:37.000000 spiderYa-0.1.6/LICENSE
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 16:44:24.003976 spiderYa-0.1.6/PKG-INFO
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      170 2023-05-21 14:40:37.000000 spiderYa-0.1.6/README.md
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       78 2023-05-21 16:44:24.055975 spiderYa-0.1.6/setup.cfg
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1638 2023-05-21 16:44:00.000000 spiderYa-0.1.6/setup.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:44:03.152369 spiderYa-0.1.6/spider/
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:44:03.152369 spiderYa-0.1.6/spider/R_script/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/R_script/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      480 2023-05-21 14:40:41.000000 spiderYa-0.1.6/spider/R_script/run_SPARKX.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      765 2023-05-21 14:40:40.000000 spiderYa-0.1.6/spider/R_script/run_nnSVG.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2815 2023-05-21 14:40:41.000000 spiderYa-0.1.6/spider/R_script/run_spatalk.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6149 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/SPIDER.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:44:03.152369 spiderYa-0.1.6/spider/SpatialDE/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      802 2023-05-21 14:40:41.000000 spiderYa-0.1.6/spider/SpatialDE/__init__.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:44:03.152369 spiderYa-0.1.6/spider/SpatialDE/_internal/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1156 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/distance_cache.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11731 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/gpflow_helpers.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3326 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/kernels.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11116 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/models.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1150 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/optimizer.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9297 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/score_test.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     5569 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/sm_kernel.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11625 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/svca.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1762 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/tf_dataset.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3700 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/util.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2067 2023-05-21 14:40:45.000000 spiderYa-0.1.6/spider/SpatialDE/_internal/util_mixture.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    14715 2023-05-21 14:40:41.000000 spiderYa-0.1.6/spider/SpatialDE/aeh.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8305 2023-05-21 14:40:41.000000 spiderYa-0.1.6/spider/SpatialDE/de_test.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    16006 2023-05-21 14:40:41.000000 spiderYa-0.1.6/spider/SpatialDE/dp_hmrf.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13415 2023-05-21 14:40:41.000000 spiderYa-0.1.6/spider/SpatialDE/gaussian_process.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3323 2023-05-21 14:40:41.000000 spiderYa-0.1.6/spider/SpatialDE/io.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6818 2023-05-21 14:40:41.000000 spiderYa-0.1.6/spider/SpatialDE/svca.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       43 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2958 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/clustering.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9892 2023-05-21 14:40:37.000000 spiderYa-0.1.6/spider/enrichment.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:44:03.152369 spiderYa-0.1.6/spider/lrdb/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/lrdb/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)   125912 2023-04-16 08:56:05.000000 spiderYa-0.1.6/spider/lrdb/lrpairs.tsv
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)   212992 2023-05-21 16:44:03.356365 spiderYa-0.1.6/spider/lrdb/pathways.tsv
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8280 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/preprocess.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    26596 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/svi.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      996 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/trajectory.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2689 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/util.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       21 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/version.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    15772 2023-05-21 14:40:38.000000 spiderYa-0.1.6/spider/visualization.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 16:44:24.003976 spiderYa-0.1.6/spiderYa.egg-info/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 16:44:23.000000 spiderYa-0.1.6/spiderYa.egg-info/PKG-INFO
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1247 2023-05-21 16:44:23.000000 spiderYa-0.1.6/spiderYa.egg-info/SOURCES.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 16:44:23.000000 spiderYa-0.1.6/spiderYa.egg-info/dependency_links.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      308 2023-05-21 16:44:23.000000 spiderYa-0.1.6/spiderYa.egg-info/requires.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        7 2023-05-21 16:44:23.000000 spiderYa-0.1.6/spiderYa.egg-info/top_level.txt
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 17:14:55.421630 spiderYa-0.1.7/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1068 2023-05-21 14:40:37.000000 spiderYa-0.1.7/LICENSE
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 17:14:55.425630 spiderYa-0.1.7/PKG-INFO
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      170 2023-05-21 14:40:37.000000 spiderYa-0.1.7/README.md
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       78 2023-05-21 17:14:55.941620 spiderYa-0.1.7/setup.cfg
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1664 2023-05-21 17:14:52.000000 spiderYa-0.1.7/setup.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 17:14:55.281633 spiderYa-0.1.7/spider/
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 17:14:55.281633 spiderYa-0.1.7/spider/R_script/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/R_script/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      480 2023-05-21 14:40:41.000000 spiderYa-0.1.7/spider/R_script/run_SPARKX.R
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      765 2023-05-21 14:40:40.000000 spiderYa-0.1.7/spider/R_script/run_nnSVG.R
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2815 2023-05-21 14:40:41.000000 spiderYa-0.1.7/spider/R_script/run_spatalk.R
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6149 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/SPIDER.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 17:14:55.281633 spiderYa-0.1.7/spider/SpatialDE/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      802 2023-05-21 14:40:41.000000 spiderYa-0.1.7/spider/SpatialDE/__init__.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 17:14:55.285632 spiderYa-0.1.7/spider/SpatialDE/_internal/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1156 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/distance_cache.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11731 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/gpflow_helpers.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3326 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/kernels.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11116 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/models.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1150 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/optimizer.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9297 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/score_test.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     5569 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/sm_kernel.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11625 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/svca.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1762 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/tf_dataset.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3700 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/util.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2067 2023-05-21 14:40:45.000000 spiderYa-0.1.7/spider/SpatialDE/_internal/util_mixture.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    14715 2023-05-21 14:40:41.000000 spiderYa-0.1.7/spider/SpatialDE/aeh.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8305 2023-05-21 14:40:41.000000 spiderYa-0.1.7/spider/SpatialDE/de_test.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    16006 2023-05-21 14:40:41.000000 spiderYa-0.1.7/spider/SpatialDE/dp_hmrf.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13415 2023-05-21 14:40:41.000000 spiderYa-0.1.7/spider/SpatialDE/gaussian_process.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3323 2023-05-21 14:40:41.000000 spiderYa-0.1.7/spider/SpatialDE/io.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6818 2023-05-21 14:40:41.000000 spiderYa-0.1.7/spider/SpatialDE/svca.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       43 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2958 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/clustering.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9892 2023-05-21 14:40:37.000000 spiderYa-0.1.7/spider/enrichment.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 17:14:55.285632 spiderYa-0.1.7/spider/lrdb/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/lrdb/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)   125912 2023-04-16 08:56:05.000000 spiderYa-0.1.7/spider/lrdb/lrpairs.tsv
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069) 71272041 2023-04-16 08:56:04.000000 spiderYa-0.1.7/spider/lrdb/pathways.tsv
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8280 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/preprocess.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    26596 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/svi.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      996 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/trajectory.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2689 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/util.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       21 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/version.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    15772 2023-05-21 14:40:38.000000 spiderYa-0.1.7/spider/visualization.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-05-21 17:14:55.421630 spiderYa-0.1.7/spiderYa.egg-info/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      597 2023-05-21 17:14:55.000000 spiderYa-0.1.7/spiderYa.egg-info/PKG-INFO
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1247 2023-05-21 17:14:55.000000 spiderYa-0.1.7/spiderYa.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-05-21 17:14:55.000000 spiderYa-0.1.7/spiderYa.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      308 2023-05-21 17:14:55.000000 spiderYa-0.1.7/spiderYa.egg-info/requires.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        7 2023-05-21 17:14:55.000000 spiderYa-0.1.7/spiderYa.egg-info/top_level.txt
```

### Comparing `spiderYa-0.1.6/LICENSE` & `spiderYa-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/PKG-INFO` & `spiderYa-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiderYa
-Version: 0.1.6
+Version: 0.1.7
 Summary: Identifying spatially variable interactions
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiderYa-0.1.6/setup.py` & `spiderYa-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 # os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spiderYa",
-    version="0.1.6",
+    version="0.1.7",
     author="Li Shiying",
     author_email="shiyingli7-c@my.cityu.edu.hk",
     description="Identifying spatially variable interactions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepomicslab/SPIDER",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     
-   package_data={'spider': ['lrdb/*.tsv'],
-                 'spider': ['R_script/*.R']},
+    # package_dir={"": "spider"},
+    
+    package_data={'lrdb': ['*.tsv'],
+                 'R_script': ['*.R']},
     
     install_requires=[
         'anndata>=0.8.0',
         'numpy',
         'Cython',
         'cellrank',
         'fa2',
```

### Comparing `spiderYa-0.1.6/spider/R_script/run_nnSVG.R` & `spiderYa-0.1.7/spider/R_script/run_nnSVG.R`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/R_script/run_spatalk.R` & `spiderYa-0.1.7/spider/R_script/run_spatalk.R`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SPIDER.py` & `spiderYa-0.1.7/spider/SPIDER.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/__init__.py` & `spiderYa-0.1.7/spider/SpatialDE/__init__.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/distance_cache.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/distance_cache.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/gpflow_helpers.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/gpflow_helpers.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/kernels.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/kernels.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/models.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/models.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/optimizer.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/optimizer.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/score_test.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/score_test.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/sm_kernel.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/sm_kernel.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/svca.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/svca.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/tf_dataset.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/tf_dataset.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/util.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/util.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/_internal/util_mixture.py` & `spiderYa-0.1.7/spider/SpatialDE/_internal/util_mixture.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/aeh.py` & `spiderYa-0.1.7/spider/SpatialDE/aeh.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/de_test.py` & `spiderYa-0.1.7/spider/SpatialDE/de_test.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/dp_hmrf.py` & `spiderYa-0.1.7/spider/SpatialDE/dp_hmrf.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/gaussian_process.py` & `spiderYa-0.1.7/spider/SpatialDE/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/io.py` & `spiderYa-0.1.7/spider/SpatialDE/io.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/SpatialDE/svca.py` & `spiderYa-0.1.7/spider/SpatialDE/svca.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/clustering.py` & `spiderYa-0.1.7/spider/clustering.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/enrichment.py` & `spiderYa-0.1.7/spider/enrichment.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/lrdb/lrpairs.tsv` & `spiderYa-0.1.7/spider/lrdb/lrpairs.tsv`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/preprocess.py` & `spiderYa-0.1.7/spider/preprocess.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/svi.py` & `spiderYa-0.1.7/spider/svi.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/trajectory.py` & `spiderYa-0.1.7/spider/trajectory.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/util.py` & `spiderYa-0.1.7/spider/util.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spider/visualization.py` & `spiderYa-0.1.7/spider/visualization.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.1.6/spiderYa.egg-info/PKG-INFO` & `spiderYa-0.1.7/spiderYa.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiderYa
-Version: 0.1.6
+Version: 0.1.7
 Summary: Identifying spatially variable interactions
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiderYa-0.1.6/spiderYa.egg-info/SOURCES.txt` & `spiderYa-0.1.7/spiderYa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

