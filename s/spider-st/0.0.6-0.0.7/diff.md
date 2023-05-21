# Comparing `tmp/spider-st-0.0.6.tar.gz` & `tmp/spider-st-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-st-0.0.6.tar", last modified: Sun May 21 07:22:35 2023, max compression
+gzip compressed data, was "spider-st-0.0.7.tar", last modified: Sun May 21 07:42:13 2023, max compression
```

## Comparing `spider-st-0.0.6.tar` & `spider-st-0.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.562501 spider-st-0.0.6/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-21 05:33:01.000000 spider-st-0.0.6/LICENSE
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 07:22:35.562501 spider-st-0.0.6/PKG-INFO
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-21 05:33:01.000000 spider-st-0.0.6/README.md
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-21 07:22:35.670499 spider-st-0.0.6/setup.cfg
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1552 2023-05-21 07:22:10.000000 spider-st-0.0.6/setup.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.478503 spider-st-0.0.6/spider/
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.522502 spider-st-0.0.6/spider/R_script/
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/R_script/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      480 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/R_script/run_SPARKX.R
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      765 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/R_script/run_nnSVG.R
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/R_script/run_spatalk.R
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     6149 2023-05-21 07:21:38.000000 spider-st-0.0.6/spider/SPIDER.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.522502 spider-st-0.0.6/spider/SpatialDE/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.0.6/spider/SpatialDE/__init__.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.562501 spider-st-0.0.6/spider/SpatialDE/_internal/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/__init__.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/distance_cache.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/gpflow_helpers.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/kernels.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/models.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/optimizer.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/score_test.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/sm_kernel.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/svca.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/tf_dataset.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/util.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/util_mixture.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.0.6/spider/SpatialDE/aeh.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/de_test.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/dp_hmrf.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/gaussian_process.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/io.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/svca.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       26 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2958 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/clustering.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/enrichment.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.562501 spider-st-0.0.6/spider/lrdb/
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/lrdb/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     8286 2023-05-21 06:13:32.000000 spider-st-0.0.6/spider/preprocess.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    26620 2023-05-21 07:21:19.000000 spider-st-0.0.6/spider/svi.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      996 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/trajectory.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2689 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/util.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       21 2023-05-21 07:21:25.000000 spider-st-0.0.6/spider/version.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    15772 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/visualization.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.562501 spider-st-0.0.6/spider_st.egg-info/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 07:22:35.000000 spider-st-0.0.6/spider_st.egg-info/PKG-INFO
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1203 2023-05-21 07:22:35.000000 spider-st-0.0.6/spider_st.egg-info/SOURCES.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-21 07:22:35.000000 spider-st-0.0.6/spider_st.egg-info/dependency_links.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      313 2023-05-21 07:22:35.000000 spider-st-0.0.6/spider_st.egg-info/requires.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-21 07:22:35.000000 spider-st-0.0.6/spider_st.egg-info/top_level.txt
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:42:10.843992 spider-st-0.0.7/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-21 05:33:01.000000 spider-st-0.0.7/LICENSE
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      598 2023-05-21 07:42:10.843992 spider-st-0.0.7/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-21 05:33:01.000000 spider-st-0.0.7/README.md
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-21 07:42:13.207947 spider-st-0.0.7/setup.cfg
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1572 2023-05-21 07:42:00.000000 spider-st-0.0.7/setup.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:42:10.839992 spider-st-0.0.7/spider/
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:42:10.839992 spider-st-0.0.7/spider/R_script/
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.7/spider/R_script/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      480 2023-05-21 05:37:57.000000 spider-st-0.0.7/spider/R_script/run_SPARKX.R
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      765 2023-05-21 05:37:57.000000 spider-st-0.0.7/spider/R_script/run_nnSVG.R
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-21 05:37:57.000000 spider-st-0.0.7/spider/R_script/run_spatalk.R
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     6149 2023-05-21 07:21:38.000000 spider-st-0.0.7/spider/SPIDER.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:42:10.839992 spider-st-0.0.7/spider/SpatialDE/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.0.7/spider/SpatialDE/__init__.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:42:10.843992 spider-st-0.0.7/spider/SpatialDE/_internal/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/__init__.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/distance_cache.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/gpflow_helpers.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/kernels.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/models.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/optimizer.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/score_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/sm_kernel.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/svca.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/tf_dataset.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/util.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/_internal/util_mixture.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.0.7/spider/SpatialDE/aeh.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/de_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/dp_hmrf.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/gaussian_process.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/io.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.0.7/spider/SpatialDE/svca.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       43 2023-05-21 07:39:43.000000 spider-st-0.0.7/spider/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2958 2023-05-21 05:37:57.000000 spider-st-0.0.7/spider/clustering.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-21 05:37:57.000000 spider-st-0.0.7/spider/enrichment.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:42:10.843992 spider-st-0.0.7/spider/lrdb/
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.7/spider/lrdb/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     8286 2023-05-21 06:13:32.000000 spider-st-0.0.7/spider/preprocess.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    26620 2023-05-21 07:21:19.000000 spider-st-0.0.7/spider/svi.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      996 2023-05-21 05:37:57.000000 spider-st-0.0.7/spider/trajectory.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2689 2023-05-21 05:37:57.000000 spider-st-0.0.7/spider/util.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       21 2023-05-21 07:21:25.000000 spider-st-0.0.7/spider/version.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    15772 2023-05-21 05:37:57.000000 spider-st-0.0.7/spider/visualization.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:42:10.843992 spider-st-0.0.7/spider_st.egg-info/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      598 2023-05-21 07:42:08.000000 spider-st-0.0.7/spider_st.egg-info/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1203 2023-05-21 07:42:08.000000 spider-st-0.0.7/spider_st.egg-info/SOURCES.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-21 07:42:08.000000 spider-st-0.0.7/spider_st.egg-info/dependency_links.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      313 2023-05-21 07:42:08.000000 spider-st-0.0.7/spider_st.egg-info/requires.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-21 07:42:08.000000 spider-st-0.0.7/spider_st.egg-info/top_level.txt
```

### Comparing `spider-st-0.0.6/LICENSE` & `spider-st-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/PKG-INFO` & `spider-st-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.6
-Summary: A small example package
+Version: 0.0.7
+Summary: Identifying spatially variable interactions
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `spider-st-0.0.6/setup.py` & `spider-st-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spider-st",
-    version="0.0.6",
+    version="0.0.7",
     author="Li Shiying",
     author_email="shiyingli7-c@my.cityu.edu.hk",
-    description="A small example package",
+    description="Identifying spatially variable interactions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepomicslab/SPIDER",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `spider-st-0.0.6/spider/R_script/run_nnSVG.R` & `spider-st-0.0.7/spider/R_script/run_nnSVG.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/R_script/run_spatalk.R` & `spider-st-0.0.7/spider/R_script/run_spatalk.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SPIDER.py` & `spider-st-0.0.7/spider/SPIDER.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/__init__.py` & `spider-st-0.0.7/spider/SpatialDE/__init__.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/distance_cache.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/distance_cache.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/gpflow_helpers.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/gpflow_helpers.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/kernels.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/kernels.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/models.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/models.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/optimizer.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/optimizer.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/score_test.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/score_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/sm_kernel.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/sm_kernel.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/svca.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/tf_dataset.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/tf_dataset.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/util.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/util.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/_internal/util_mixture.py` & `spider-st-0.0.7/spider/SpatialDE/_internal/util_mixture.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/aeh.py` & `spider-st-0.0.7/spider/SpatialDE/aeh.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/de_test.py` & `spider-st-0.0.7/spider/SpatialDE/de_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/dp_hmrf.py` & `spider-st-0.0.7/spider/SpatialDE/dp_hmrf.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/gaussian_process.py` & `spider-st-0.0.7/spider/SpatialDE/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/io.py` & `spider-st-0.0.7/spider/SpatialDE/io.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/SpatialDE/svca.py` & `spider-st-0.0.7/spider/SpatialDE/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/clustering.py` & `spider-st-0.0.7/spider/clustering.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/enrichment.py` & `spider-st-0.0.7/spider/enrichment.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/preprocess.py` & `spider-st-0.0.7/spider/preprocess.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/svi.py` & `spider-st-0.0.7/spider/svi.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/trajectory.py` & `spider-st-0.0.7/spider/trajectory.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/util.py` & `spider-st-0.0.7/spider/util.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider/visualization.py` & `spider-st-0.0.7/spider/visualization.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.6/spider_st.egg-info/PKG-INFO` & `spider-st-0.0.7/spider_st.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.6
-Summary: A small example package
+Version: 0.0.7
+Summary: Identifying spatially variable interactions
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `spider-st-0.0.6/spider_st.egg-info/SOURCES.txt` & `spider-st-0.0.7/spider_st.egg-info/SOURCES.txt`

 * *Files identical despite different names*

