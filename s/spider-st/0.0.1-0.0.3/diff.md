# Comparing `tmp/spider-st-0.0.1.tar.gz` & `tmp/spider-st-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spider-st-0.0.1.tar", last modified: Mon Apr 17 04:12:35 2023, max compression
+gzip compressed data, was "spider-st-0.0.3.tar", last modified: Sun May 21 05:40:41 2023, max compression
```

## Comparing `spider-st-0.0.1.tar` & `spider-st-0.0.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-17 04:12:34.000000 spider-st-0.0.1/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1068 2023-04-16 08:59:14.000000 spider-st-0.0.1/LICENSE
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      578 2023-04-17 04:12:34.000000 spider-st-0.0.1/PKG-INFO
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      170 2023-04-16 08:58:58.000000 spider-st-0.0.1/README.md
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       78 2023-04-17 04:12:35.000000 spider-st-0.0.1/setup.cfg
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1447 2023-04-17 04:12:19.000000 spider-st-0.0.1/setup.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-17 04:12:34.000000 spider-st-0.0.1/spider/
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-17 04:12:34.000000 spider-st-0.0.1/spider/R_script/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 14:21:50.000000 spider-st-0.0.1/spider/R_script/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      480 2023-04-16 08:56:04.000000 spider-st-0.0.1/spider/R_script/run_SPARKX.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      765 2023-04-16 08:56:04.000000 spider-st-0.0.1/spider/R_script/run_nnSVG.R
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8196 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SPIDER.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-17 04:12:34.000000 spider-st-0.0.1/spider/SpatialDE/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      802 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/__init__.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-17 04:12:34.000000 spider-st-0.0.1/spider/SpatialDE/_internal/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1156 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/distance_cache.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11731 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/gpflow_helpers.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3326 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/kernels.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11116 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/models.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1150 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/optimizer.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9297 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/score_test.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     5569 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/sm_kernel.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11625 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/svca.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1762 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/tf_dataset.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3700 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/util.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2067 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/_internal/util_mixture.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    14715 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/aeh.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8305 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/de_test.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    16006 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/dp_hmrf.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13415 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/gaussian_process.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3323 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/io.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6818 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/SpatialDE/svca.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       43 2023-04-16 08:57:16.000000 spider-st-0.0.1/spider/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2866 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/clustering.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9892 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/enrichment.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-17 04:12:34.000000 spider-st-0.0.1/spider/lrdb/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/lrdb/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13870 2023-04-16 13:53:53.000000 spider-st-0.0.1/spider/preprocess.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    26274 2023-04-16 14:26:50.000000 spider-st-0.0.1/spider/svi.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      996 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/trajectory.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2716 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/util.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       21 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/version.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    12002 2023-04-16 08:56:05.000000 spider-st-0.0.1/spider/visualization.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-17 04:12:34.000000 spider-st-0.0.1/spider_st.egg-info/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      578 2023-04-17 04:12:33.000000 spider-st-0.0.1/spider_st.egg-info/PKG-INFO
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1173 2023-04-17 04:12:34.000000 spider-st-0.0.1/spider_st.egg-info/SOURCES.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-04-17 04:12:33.000000 spider-st-0.0.1/spider_st.egg-info/dependency_links.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      296 2023-04-17 04:12:33.000000 spider-st-0.0.1/spider_st.egg-info/requires.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        7 2023-04-17 04:12:33.000000 spider-st-0.0.1/spider_st.egg-info/top_level.txt
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:40.359744 spider-st-0.0.3/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-21 05:33:01.000000 spider-st-0.0.3/LICENSE
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 05:40:40.359744 spider-st-0.0.3/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-21 05:33:01.000000 spider-st-0.0.3/README.md
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-21 05:40:41.103734 spider-st-0.0.3/setup.cfg
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1524 2023-05-21 05:35:16.000000 spider-st-0.0.3/setup.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:37.483785 spider-st-0.0.3/spider/
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:39.475757 spider-st-0.0.3/spider/R_script/
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/R_script/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      480 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/R_script/run_SPARKX.R
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      765 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/R_script/run_nnSVG.R
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/R_script/run_spatalk.R
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     6035 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/SPIDER.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:40.359744 spider-st-0.0.3/spider/SpatialDE/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.0.3/spider/SpatialDE/__init__.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:40.359744 spider-st-0.0.3/spider/SpatialDE/_internal/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/__init__.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/distance_cache.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/gpflow_helpers.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/kernels.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/models.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/optimizer.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/score_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/sm_kernel.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/svca.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/tf_dataset.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/util.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/util_mixture.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.0.3/spider/SpatialDE/aeh.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/de_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/dp_hmrf.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/gaussian_process.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/io.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/svca.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       26 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2958 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/clustering.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/enrichment.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:40.359744 spider-st-0.0.3/spider/lrdb/
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/lrdb/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     7467 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/preprocess.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    26510 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/svi.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      996 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/trajectory.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2689 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/util.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       21 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/version.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    15772 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/visualization.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:40.359744 spider-st-0.0.3/spider_st.egg-info/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 05:40:35.000000 spider-st-0.0.3/spider_st.egg-info/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1203 2023-05-21 05:40:35.000000 spider-st-0.0.3/spider_st.egg-info/SOURCES.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-21 05:40:35.000000 spider-st-0.0.3/spider_st.egg-info/dependency_links.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      296 2023-05-21 05:40:35.000000 spider-st-0.0.3/spider_st.egg-info/requires.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-21 05:40:35.000000 spider-st-0.0.3/spider_st.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spider-st-0.0.1/LICENSE` & `spider-st-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/PKG-INFO` & `spider-st-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.1
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spider-st-0.0.1/setup.py` & `spider-st-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import setuptools
+import os
+os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spider-st",
-    version="0.0.1",
+    version="0.0.3",
     author="Li Shiying",
     author_email="shiyingli7-c@my.cityu.edu.hk",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepomicslab/SPIDER",
     packages=setuptools.find_packages(),
```

### Comparing `spider-st-0.0.1/spider/R_script/run_nnSVG.R` & `spider-st-0.0.3/spider/R_script/run_nnSVG.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/__init__.py` & `spider-st-0.0.3/spider/SpatialDE/__init__.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/distance_cache.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/distance_cache.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/gpflow_helpers.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/gpflow_helpers.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/kernels.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/kernels.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/models.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/models.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/optimizer.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/optimizer.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/score_test.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/score_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/sm_kernel.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/sm_kernel.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/svca.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/tf_dataset.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/tf_dataset.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/util.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/util.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/_internal/util_mixture.py` & `spider-st-0.0.3/spider/SpatialDE/_internal/util_mixture.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/aeh.py` & `spider-st-0.0.3/spider/SpatialDE/aeh.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/de_test.py` & `spider-st-0.0.3/spider/SpatialDE/de_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/dp_hmrf.py` & `spider-st-0.0.3/spider/SpatialDE/dp_hmrf.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/gaussian_process.py` & `spider-st-0.0.3/spider/SpatialDE/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/io.py` & `spider-st-0.0.3/spider/SpatialDE/io.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/SpatialDE/svca.py` & `spider-st-0.0.3/spider/SpatialDE/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/clustering.py` & `spider-st-0.0.3/spider/clustering.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 import scanpy as sc
 import pandas as pd
 import numpy as np
 
-def supervised_spot_clust(idata, adata, label, portion=0.1, n_cluster=None):
-    import umap, umap.plot
-    idata.uns['cell_meta'][label+'_int'] = idata.uns['cell_meta'][label].cat.codes
+def supervised_spot_clust(idata, adata, label, portion=0.1, n_cluster=None, n_neighbors=100, min_dist=1):
+    import umap
+    idata.uns['cell_meta'][label+'_int'] = idata.uns['cell_meta'][label].astype('category').cat.codes
     masked_target = idata.uns['cell_meta'][label+'_int']
     np.random.seed(52)
     masked_target[np.random.choice(len(idata.uns['cell_meta'][label]), size=int(len(idata.uns['cell_meta'][label]) * portion), replace=False)] = -1
-    embedding = umap.UMAP(n_neighbors=100, min_dist=1,random_state=52).fit_transform(idata.uns['cell_pattern'], y=masked_target)
+    embedding = umap.UMAP(n_neighbors=n_neighbors, min_dist=min_dist,random_state=52).fit_transform(idata.uns['cell_pattern'], y=masked_target)
     adata.obsm['X_umap'] = embedding
     sc.pp.neighbors(adata, n_neighbors=20, use_rep='X_umap')
     sc.tl.draw_graph(adata)
     flag = 1
     res_max = 10
     res_min = 0.0001
     res = 0.05
     if not n_cluster:
         k = len(idata.uns['cell_meta'][label].unique())
     else:
         k = n_cluster
+    repeat = 0
     while (flag):
         sc.tl.leiden(adata, resolution=res)
+        repeat+=1
         # print(len(adata.obs['leiden'].unique()), res)
-        if (len(adata.obs['leiden'].unique()) == k) | (res < 0) | (res > 10):
+        if (len(adata.obs['leiden'].unique()) == k) | (res < 0) | (res > 10) | (repeat > 1000):
             flag = 0
         elif len(adata.obs['leiden'].unique()) < k:
             res_min = res
             res = (res+res_max)/2
         else:
             res_max = res
             res = (res+res_min)/2
     adata.obs['leiden_supervised'] = adata.obs['leiden']
     
             
 def unsupervised_spot_clust(idata, adata, n_cluster=None):
-    import umap, umap.plot
+    import umap
 
     embedding = umap.UMAP(n_neighbors=100, min_dist=1,random_state=52).fit_transform(idata.uns['cell_pattern'])
     adata.obsm['X_umap'] = embedding
     sc.pp.neighbors(adata, n_neighbors=20, use_rep='X_umap')
     sc.tl.draw_graph(adata)
     flag = 1
     res_max = 10
```

### Comparing `spider-st-0.0.1/spider/enrichment.py` & `spider-st-0.0.3/spider/enrichment.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/svi.py` & `spider-st-0.0.3/spider/svi.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,33 +7,65 @@
 import squidpy as sq
 import warnings
 warnings.filterwarnings('ignore')
 import time
 from importlib import resources
 
 def abstract(idata, n_neighbors=10):
+    # Method: Building abstract interfaces with self-organizing map
     from somde import SomNode
     df = idata.to_df().T
     corinfo = idata.obs
     corinfo["total_count"]=df.sum(0)
     X=corinfo[['row','col']].values.astype(np.float32)
     som = SomNode(X,n_neighbors)
     ndf,ninfo = som.mtx(df)
     meta_idata = anndata.AnnData(ndf.T)
     meta_idata.obs[['row', 'col', 'total_count']] = ninfo.to_numpy(dtype=float)
     meta_idata.obsm['spatial'] = meta_idata.obs[['row', 'col']].to_numpy()
     idata = som_mapping(som, idata, df)
     return som, idata, meta_idata
 
+def som_mapping(som, idata, df):
+    bsmc = som.som.bmus
+    soml = []
+    for i in np.arange(bsmc.shape[0]):
+        u,v = bsmc[i]
+        soml.append(v*som.somn+u)
+    idata.obs['som_node'] = -1
+    ids = np.sort(np.unique(np.array(soml)))
+    count = 0
+    for i in ids:
+        idata.obs.loc[df.loc[:,np.array(soml)==i].columns,'som_node'] = count
+        count += 1
+    return idata
+
+def meta_pattern_to_idata(idata, meta_idata):
+    idata.obsm['pattern_score'] = meta_idata.obsm['pattern_score'][idata.obs['som_node'].to_numpy()]  
+    idata.var = meta_idata.var
+    idata.uns['nnSVG'] = meta_idata.uns['nnSVG']
+    idata.uns['SOMDE'] = meta_idata.uns['SOMDE']
+    idata.uns['SpatialDE'] = meta_idata.uns['SpatialDE']
+    idata.uns['SPARKX'] = meta_idata.uns['SPARKX']
+    idata.uns['scGCO'] = meta_idata.uns['scGCO']
+    idata.uns['moranI'] = meta_idata.uns['moranI']
+    idata.uns['gearyC'] = meta_idata.uns['gearyC']
+    print(f'Added key pattern_score in idata.obsm')   
+
 def find_svi(idata, out_f, overwrite, som=None):
+    # Method: Identifying spatially variable LR interactions
+    # Gaussian models
     svi_nnSVG(idata,out_f,overwrite)
-    svi_scGCO(idata,out_f,overwrite)
     svi_SOMDE(idata,out_f,overwrite, som=som)
-    svi_SPARKX(idata,out_f,overwrite)
     svi_SpatialDE2(idata,out_f,overwrite)
+    # Non-parametric covariance test
+    svi_SPARKX(idata,out_f,overwrite)
+    # HMRF
+    svi_scGCO(idata,out_f,overwrite)
+    # baseline auto-correlation metrics
     svi_moran(idata,out_f,overwrite)
     svi_geary(idata,out_f,overwrite)
 
 def svi_moran(idata, work_dir, overwrite=False):
     try:
         t0=time.time()
         n_perms=1000
@@ -87,30 +119,14 @@
             idata.uns['nnSVG_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}nnSVG.csv', index_col=0)
         idata.uns['nnSVG'] = result
         print(f'Added key nnSVG in idata.uns')
     except:
         pass
     
-def svi_trendsceek(idata, work_dir, overwrite=False):
-    try:
-        count_f = f'{work_dir}idata_count.csv'
-        meta_f = f'{work_dir}idata_meta.csv'
-        if (overwrite) | ((not exists(count_f)) & (not exists(meta_f))):
-            idata.to_df().to_csv(count_f)
-            idata.obs[['row', 'col']].to_csv(meta_f)
-        if (overwrite) | (not exists( f'{work_dir}trendsceek.csv')):
-            with resources.path("spider.R_script", "run_trendsceek.R") as pw_fn:
-                os.system(str(f'/bin/bash -c "source /etc/profile;module load GCC/11.2.0 OpenMPI/4.1.1 R/4.2.0 Anaconda3/2022.05 R-bundle-Bioconductor/3.15-R-4.2.0;R -f {pw_fn} {count_f} {meta_f} {work_dir}"'))
-        result = pd.read_csv(f'{work_dir}trendsceek.csv', index_col=0)
-        idata.uns['trendsceek'] = result
-        print(f'Added key trendsceek in idata.uns')
-    except:
-        pass
-    
 def scGCO_sv(locs, data_norm, cellGraph, gmmDict, smooth_factor=10, unary_scale_factor=100, label_cost=10, algorithm='expansion'):
     from itertools import repeat
     from functools import reduce
     import operator
     import statsmodels.stats.multitest as multi
     import scGCO
 
@@ -196,16 +212,15 @@
             svg_full.to_csv(f'{work_dir}SpatialDE.csv')
             individual.to_csv(f'{work_dir}SpatialDE_individual.csv')
             idata.uns['SpatialDE2_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}SpatialDE.csv', index_col=0)
         idata.uns['SpatialDE'] = result
         print(f'Added key SpatialDE in idata.uns')
     except:
-        pass
-    
+        pass 
     
 def svi_SOMDE(idata, work_dir, overwrite=False, som=None):
     try:
         if (overwrite) | (not exists(f'{work_dir}SOMDE.csv')):
             t0=time.time()
             if som is None:
                 from somde import SomNode
@@ -254,15 +269,15 @@
     df = pd.concat(df, axis=1).fillna(1)
     
     arr = [combine_pvalues(x, method='fisher')[1] for x in df.to_numpy()]
     df['adj_pvalue'] = arr
     df_sub = df[df['adj_pvalue']<threshold]
     # df_sub = df_sub.loc[np.intersect1d(df_sub.index, idata.uns['SOMDE']['g'])]
     print(f'{len(df_sub)}/{len(df)} SVIs identified (threshold={threshold}).')
-    idata.varm['svi'] = df.loc[idata.var_names]
+    idata.uns['svi'] = df
     idata.var['is_svi'] = 0
     idata.var.loc[df_sub.index, 'is_svi'] = 1
     return df, df_sub
 
 def combine_SVI_strict(idata, threshold=0.01):
     methods = np.array(['SOMDE', 'SpatialDE', 'SPARKX', 'nnSVG', 'scGCO', 'gearyC', 'moranI'])[np.isin(['SOMDE', 'SpatialDE', 'SPARKX', 'nnSVG', 'scGCO', 'gearyC', 'moranI'],list(idata.uns.keys()))]
     print(f'Using the results from SVI identification methods: {methods}')
@@ -277,30 +292,29 @@
         elif i == 'nnSVG':
             df.append(idata.uns[i][['padj']].rename(columns = {'padj': i}))
         elif i == 'scGCO':
             df.append(idata.uns[i].set_index(idata.uns['scGCO'].columns[0])[['fdr']].rename(columns = {'fdr': i}))
     df = pd.concat(df, axis=1).fillna(1)
     df_sub = df[(df<threshold).all(axis=1)]
     print(f'{len(df_sub)}/{len(df)} SVIs identified (threshold={threshold}).')
-    idata.varm['svi'] = df.loc[idata.var_names]
+    idata.uns['svi'] = df
     idata.var['is_svi'] = 0
     idata.var.loc[df_sub.index, 'is_svi'] = 1
     return df, df_sub
 
 def combine_SVI_somde(idata, threshold=0.01):
     print(f'Using the SOMDE results')
     df = idata.uns['SOMDE'].set_index('g')[['pval']].rename(columns = {'pval': 'SOMDE'}).fillna(1)
     df_sub = df[(df<threshold).all(axis=1)]
     print(f'{len(df_sub)}/{len(df)} SVIs identified (threshold={threshold}).')
-    idata.varm['svi'] = df.loc[idata.var_names]
+    idata.uns['svi'] = df
     idata.var['is_svi'] = 0
     idata.var.loc[df_sub.index, 'is_svi'] = 1
     return df, df_sub
     
-
 def eva_SVI(idata, svi_df_strict):
     import seaborn as sns
     dfs = [
         -idata.uns['gearyC'][['C']],
         idata.uns['moranI'][['I']],
         idata.uns['SOMDE'].set_index('g')['FSV'],
         idata.uns['nnSVG']['LR_stat'],
@@ -322,20 +336,22 @@
     
 class dotdict(dict):
     """dot.notation access to dictionary attributes"""
     __getattr__ = dict.get
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
+# SVI pattern generation with Gaussian process mixture model
 def SVI_patterns(idata, svi_df_strict, iter=1000, pattern_prune_threshold=1e-8):
     from spider import SpatialDE as SpatialDE2
     allsignifgenes = svi_df_strict.index.to_numpy()
     if 'lengthscale' in idata.uns['SpatialDE'].columns:
         l=idata.uns['SpatialDE'].loc[allsignifgenes]['lengthscale'].to_list()
         if len(np.unique(l)) < 2:
+            allsignifgenes = np.intersect1d(allsignifgenes, idata.uns['SOMDE']['g'].to_numpy())
             l=idata.uns['SOMDE'].set_index('g').loc[allsignifgenes]['l'].to_list()
     else:
         l=idata.uns['SOMDE'].set_index('g').loc[allsignifgenes]['l'].to_list()
     pattern_number = 1000
     if len(np.unique(l)) <= 1:
         pattern_number = -1
     for count in range(5):
@@ -362,14 +378,18 @@
 
     print(f'eventually found {pattern_number} patterns')
     idata.var['label'] = -1
     idata.var.loc[allsignifgenes, 'label'] = upper_patterns.labels
     idata.var[[f'pattern_membership_{x}' for x in range(upper_patterns.pattern_probabilities.shape[1])]] = 0
     idata.var.loc[allsignifgenes, [f'pattern_membership_{x}' for x in range(upper_patterns.pattern_probabilities.shape[1])]] = upper_patterns.pattern_probabilities
     idata.obsm['pattern_score'] = upper_patterns.patterns
+    idata.var[[f'pattern_correlation_{x}' for x in range(idata.obsm['pattern_score'].shape[1])]] = 0
+    corr_df=pd.concat([idata.to_df(),pd.DataFrame(idata.obsm['pattern_score'],index=idata.obs_names)],axis=1).corr().loc[idata.var_names, range(idata.obsm['pattern_score'].shape[1])]
+    idata.var[[f'pattern_correlation_{x}' for x in range(idata.obsm['pattern_score'].shape[1])]] = corr_df.to_numpy()
+
     
 def SVI_patterns_v1(idata, svi_df_strict, components=5):
     import NaiveDE
     import SpatialDE
     df = idata.to_df().T.loc[svi_df_strict.index]
     corinfo = idata.obs
     corinfo["total_counts"]=df.sum(0)
@@ -377,39 +397,21 @@
     norm_expr = NaiveDE.stabilize(df).T
     resid_expr = NaiveDE.regress_out(corinfo, norm_expr.T, 'np.log(total_counts)').T
     print('finished regression')
     results = SpatialDE.run(X,resid_expr)
     print('finished fitting')
     histology_results, patterns, prob = spatial_patterns(X, resid_expr, results, C=components,l=results['l'].median()+0.5, verbosity=1)
     return histology_results, patterns, prob
-
-def som_mapping(som, idata, df):
-    bsmc = som.som.bmus
-    soml = []
-    for i in np.arange(bsmc.shape[0]):
-        u,v = bsmc[i]
-        soml.append(v*som.somn+u)
-    idata.obs['som_node'] = -1
-    ids = np.sort(np.unique(np.array(soml)))
-    count = 0
-    for i in ids:
-        idata.obs.loc[df.loc[:,np.array(soml)==i].columns,'som_node'] = count
-        count += 1
-    return idata
-
-def meta_pattern_to_idata(idata, meta_idata):
-    idata.obsm['pattern_score'] = meta_idata.obsm['pattern_score'][idata.obs['som_node'].to_numpy()]  
-    print(f'Added key pattern_score in idata.obsm')     
     
 def idata_pattern_to_spot(idata):
     belonging = {}
     cells = idata.uns['cell_meta'].index
     for i in cells:
         belonging[i] = []
-    for pair in idata.obs.reset_index()[['index','A', 'B']].to_numpy():
+    for pair in idata.obs.reset_index()[['index', 'A', 'B']].to_numpy():
         belonging[pair[1]].append(pair[0])
         belonging[pair[2]].append(pair[0])
     score = pd.DataFrame(idata.obsm['pattern_score'], index=idata.obs_names)
     df = pd.concat([score.loc[belonging[c]].mean() for c in cells], axis=1).T     
     df.index = cells
     idata.uns['cell_pattern'] = df
     print(f'Added key cell_pattern in idata.uns')   
@@ -470,15 +472,14 @@
 
 def ELBO(Y, r, m, s2e, K, K_0, s2e_0, pi=None):
     L = ln_P_YZms(Y, r, m, s2e, pi) + ln_P_Z(r, pi) + ln_P_mu(m, K) \
         - ln_Q_Z(r, r) - ln_Q_mu(K_0, r, s2e_0)
     
     return L
 
-
 def factor(K):
     S, U = np.linalg.eigh(K)
     # .clip removes negative eigenvalues
     return U, np.clip(S, 1e-8, None)
 
 def ln_Q_mu(K, Z, s2e):
     ''' Expecation of ln Q(mu)
```

### Comparing `spider-st-0.0.1/spider/trajectory.py` & `spider-st-0.0.3/spider/trajectory.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.1/spider/util.py` & `spider-st-0.0.3/spider/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     idata.obs[f'A_label_{clust_key}'] = node_labels_text.loc[idata.obs['A']].astype(str).to_numpy()
     idata.obs[f'B_label_{clust_key}'] = node_labels_text.loc[idata.obs['B']].astype(str).to_numpy()
     node_labels = idata.uns['cell_meta'][clust_key].astype('category').cat.codes
     idata.obs[f'A_label_int_{clust_key}'] = node_labels.loc[idata.obs['A']].to_numpy()
     idata.obs[f'B_label_int_{clust_key}'] = node_labels.loc[idata.obs['B']].to_numpy()
     idata.obs['label_1'] = idata.obs[f'A_label_int_{clust_key}'].astype(str) + idata.obs[f'B_label_int_{clust_key}'].astype(str)
     idata.obs['label_2'] = idata.obs[f'B_label_int_{clust_key}'].astype(str) + idata.obs[f'A_label_int_{clust_key}'].astype(str)
-    idata.obs['label_int_{clust_key}'] = idata.obs[['label_1', 'label_2']].astype(int).max(axis=1).astype(str).astype('category')
+    idata.obs[f'label_{clust_key}_int'] = idata.obs[['label_1', 'label_2']].astype(int).max(axis=1).astype(str).astype('category')
     label_1 = idata.obs[f'A_label_{clust_key}'].astype(str) + '_' + idata.obs[f'B_label_{clust_key}'].astype(str).to_numpy()
     label_2 = idata.obs[f'B_label_{clust_key}'].astype(str) + '_' + idata.obs[f'A_label_{clust_key}'].astype(str).to_numpy()
     pick = idata.obs[['label_1', 'label_2']].astype(int).idxmax(axis=1).to_numpy()
     text_label = [label_1[i] if x=='label_1' else label_2[i] for i,x in enumerate(pick)]
     idata.obs[f'label_{clust_key}'] = text_label
     idata.obs[f'label_{clust_key}'] = idata.obs[f'label_{clust_key}'].astype('category')
     print(f'Added key label_{clust_key} in idata.obs')
@@ -27,25 +27,23 @@
         belonging[pair[1]].append(pair[0])
         belonging[pair[2]].append(pair[0])
     score = pd.DataFrame(idata.obsm['pattern_score'], index=idata.obs_names)
     df = pd.concat([score.loc[belonging[c]].mean() for c in cells], axis=1).T     
     df.index = cells
     idata.uns['cell_pattern'] = df
     print(f'Added key cell_pattern in idata.uns')
-    return df
 
 def interaction_spot_interface(idata):       
     belonging = {}
     cells = idata.uns['cell_meta'].index
     for i in cells:
         belonging[i] = []
     for pair in idata.obs.reset_index()[['index','A', 'B']].to_numpy():
         belonging[pair[1]].append(pair[0])
         belonging[pair[2]].append(pair[0])
     score = idata.to_df()
     df = pd.concat([score.loc[belonging[c]].mean() for c in cells], axis=1).T     
     df.index = cells
     idata.uns['cell_score'] = df
     print(f'Added key cell_score in idata.uns')
-    return df
```

### Comparing `spider-st-0.0.1/spider/visualization.py` & `spider-st-0.0.3/spider/visualization.py`

 * *Files 13% similar despite different names*

```diff
@@ -238,8 +238,87 @@
     
 def plot_projection(idata, save=None):
     import scvelo as scv
     scv.pl.velocity_embedding_stream(
         idata, color="label", vkey="T_fwd_spatial", basis="spatial", legend_loc="right",
         recompute=False,V=idata.obsm['T_fwd_spatial'],smooth=1.5,
         save=save
-    )
+    )
+    
+def draw_diff(adata, idata, title, is_human=True,top=200):
+    from matplotlib_venn import venn3,venn3_circles
+    import gseapy
+
+    organism = 'Human' if is_human else 'Mouse'
+    pathway_db = 'KEGG_2021_Human' if is_human else 'KEGG_2019_Mouse'
+    
+    pathway_dfs=[]
+
+    print(organism, pathway_db)
+
+    genelist = adata.uns['moranI'][:top].index.to_list()
+    enr_res_gene = gseapy.enrichr(gene_list=genelist,
+                            cutoff=0.01,
+                            organism=organism,
+                            gene_sets=pathway_db)
+    gene_pw_list = enr_res_gene.res2d[enr_res_gene.res2d['P-value']<0.01].Term.to_numpy()
+    enr_res_gene.res2d['group']='SVG'
+    pathway_dfs.append(enr_res_gene.res2d[enr_res_gene.res2d['P-value']<0.01])
+    
+    
+    human_lr = load_lr_df(is_human)
+    l = human_lr['ligand'].to_numpy().flatten()
+    r = human_lr['receptor'].to_numpy().flatten()
+    unique_lr_human = np.unique(np.concatenate((l, r)))
+    genelist_lr = adata.uns['moranI'].loc[np.intersect1d(unique_lr_human,adata.uns['moranI'].index)].sort_values('I',ascending=False)[:top].index.to_list()
+    enr_res_gene = gseapy.enrichr(gene_list=genelist_lr,
+                            cutoff=0.01,
+                            organism=organism,
+                            gene_sets=pathway_db)
+    gene_lr_list = enr_res_gene.res2d[enr_res_gene.res2d['P-value']<0.01].Term.to_numpy()
+    enr_res_gene.res2d['group']='LR genes'
+    pathway_dfs.append(enr_res_gene.res2d[enr_res_gene.res2d['P-value']<0.01])
+
+    interaction_list = idata.uns['moranI'][:top].index.to_list()
+    gene_list_lri = np.unique(np.concatenate([x.split('_') for x in interaction_list])).tolist()
+    enr_res = gseapy.enrichr(gene_list=gene_list_lri,
+                                cutoff=0.01,
+                                organism=organism,
+                                gene_sets=pathway_db)
+    lri_pw_list = enr_res.res2d[enr_res.res2d['P-value']<0.01].Term.to_numpy()
+    enr_res.res2d['group']='SVI genes'
+    pathway_dfs.append(enr_res.res2d[enr_res.res2d['P-value']<0.01])
+
+    fig = plt.figure(figsize=(12, 4))
+    fig.suptitle(title, fontsize=15)
+    plt.subplot(1, 3, 1)
+    moran_df = adata.uns['moranI'][:top]
+    moran_df['label'] = 'SVG'
+    moran_df_lr = adata.uns['moranI'].loc[genelist_lr]
+    moran_df_lr['label'] = 'LR genes'
+    moran_df_svi = adata.uns['moranI'].loc[np.intersect1d(gene_list_lri,adata.uns['moranI'].index)]
+    moran_df_svi['label'] = 'SVI genes'
+    df = pd.concat([moran_df, moran_df_lr,moran_df_svi])
+    print(moran_df.I.mean(),moran_df_lr.I.mean(), moran_df_svi.I.mean())
+    sns.boxplot(data=df, x="label", y="I", order=["SVI genes", "LR genes",  "SVG",], palette={"SVI genes":"#098154","LR genes":  "#069af3",  "SVG": "#c72e29"})
+    plt.title('Moran I')
+    
+    plt.subplot(1, 3, 2)
+    g=venn3(subsets = [set(gene_list_lri),set(genelist_lr),set(genelist)], #绘图数据集
+        set_labels = ('SVI genes', "LR genes",'SVG'), #设置组名
+        set_colors=("#098154","#069af3","#c72e29"),#设置圈的颜色，中间颜色不能修改
+        alpha=0.6,#透明度
+        normalize_to=1.0,#venn图占据figure的比例，1.0为占满
+       )
+    plt.title('Gene Overlap')
+    plt.subplot(1, 3, 3)
+    g=venn3(subsets = [set(lri_pw_list),set(gene_lr_list),set(gene_pw_list)], #绘图数据集
+        set_labels = ('SVI genes', "LR genes",'SVG'), #设置组名
+        set_colors=("#098154","#069af3","#c72e29"),#设置圈的颜色，中间颜色不能修改
+        alpha=0.6,#透明度
+        normalize_to=1.0,#venn图占据figure的比例，1.0为占满
+       )
+    plt.title('Enriched Pathway Overlap')
+    
+    merged_df = pd.concat(pathway_dfs)
+
+    return merged_df,lri_pw_list,gene_lr_list,gene_pw_list
```

### Comparing `spider-st-0.0.1/spider_st.egg-info/PKG-INFO` & `spider-st-0.0.3/spider_st.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.1
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spider-st-0.0.1/spider_st.egg-info/SOURCES.txt` & `spider-st-0.0.3/spider_st.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 spider/trajectory.py
 spider/util.py
 spider/version.py
 spider/visualization.py
 spider/R_script/__init__.py
 spider/R_script/run_SPARKX.R
 spider/R_script/run_nnSVG.R
+spider/R_script/run_spatalk.R
 spider/SpatialDE/__init__.py
 spider/SpatialDE/aeh.py
 spider/SpatialDE/de_test.py
 spider/SpatialDE/dp_hmrf.py
 spider/SpatialDE/gaussian_process.py
 spider/SpatialDE/io.py
 spider/SpatialDE/svca.py
```

