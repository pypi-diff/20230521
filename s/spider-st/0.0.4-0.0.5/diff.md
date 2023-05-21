# Comparing `tmp/spider-st-0.0.4.tar.gz` & `tmp/spider-st-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-st-0.0.4.tar", last modified: Sun May 21 06:17:09 2023, max compression
+gzip compressed data, was "spider-st-0.0.5.tar", last modified: Sun May 21 06:55:07 2023, max compression
```

## Comparing `spider-st-0.0.4.tar` & `spider-st-0.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-21 05:33:01.000000 spider-st-0.0.4/LICENSE
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 06:17:09.280198 spider-st-0.0.4/PKG-INFO
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-21 05:33:01.000000 spider-st-0.0.4/README.md
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-21 06:17:09.556192 spider-st-0.0.4/setup.cfg
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1524 2023-05-21 06:16:53.000000 spider-st-0.0.4/setup.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.276198 spider-st-0.0.4/spider/
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/spider/R_script/
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/R_script/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      480 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/R_script/run_SPARKX.R
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      765 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/R_script/run_nnSVG.R
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/R_script/run_spatalk.R
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     6149 2023-05-21 06:13:17.000000 spider-st-0.0.4/spider/SPIDER.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/spider/SpatialDE/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.0.4/spider/SpatialDE/__init__.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/spider/SpatialDE/_internal/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/__init__.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/distance_cache.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/gpflow_helpers.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/kernels.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/models.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/optimizer.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/score_test.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/sm_kernel.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/svca.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/tf_dataset.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/util.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/util_mixture.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.0.4/spider/SpatialDE/aeh.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/de_test.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/dp_hmrf.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/gaussian_process.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/io.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/svca.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       26 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2958 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/clustering.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/enrichment.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/spider/lrdb/
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/lrdb/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     8286 2023-05-21 06:13:32.000000 spider-st-0.0.4/spider/preprocess.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    26415 2023-05-21 06:13:39.000000 spider-st-0.0.4/spider/svi.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      996 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/trajectory.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2689 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/util.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       21 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/version.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    15772 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/visualization.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/spider_st.egg-info/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 06:17:08.000000 spider-st-0.0.4/spider_st.egg-info/PKG-INFO
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1203 2023-05-21 06:17:09.000000 spider-st-0.0.4/spider_st.egg-info/SOURCES.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-21 06:17:08.000000 spider-st-0.0.4/spider_st.egg-info/dependency_links.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      296 2023-05-21 06:17:08.000000 spider-st-0.0.4/spider_st.egg-info/requires.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-21 06:17:08.000000 spider-st-0.0.4/spider_st.egg-info/top_level.txt
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.634099 spider-st-0.0.5/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-21 05:33:01.000000 spider-st-0.0.5/LICENSE
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 06:55:07.634099 spider-st-0.0.5/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-21 05:33:01.000000 spider-st-0.0.5/README.md
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-21 06:55:07.642098 spider-st-0.0.5/setup.cfg
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1531 2023-05-21 06:55:01.000000 spider-st-0.0.5/setup.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.630099 spider-st-0.0.5/spider/
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.630099 spider-st-0.0.5/spider/R_script/
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/R_script/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      480 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/R_script/run_SPARKX.R
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      765 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/R_script/run_nnSVG.R
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/R_script/run_spatalk.R
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     6149 2023-05-21 06:51:11.000000 spider-st-0.0.5/spider/SPIDER.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.630099 spider-st-0.0.5/spider/SpatialDE/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.0.5/spider/SpatialDE/__init__.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.634099 spider-st-0.0.5/spider/SpatialDE/_internal/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/__init__.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/distance_cache.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/gpflow_helpers.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/kernels.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/models.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/optimizer.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/score_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/sm_kernel.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/svca.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/tf_dataset.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/util.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/util_mixture.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.0.5/spider/SpatialDE/aeh.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/de_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/dp_hmrf.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/gaussian_process.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/io.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/svca.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       26 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2958 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/clustering.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/enrichment.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.634099 spider-st-0.0.5/spider/lrdb/
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/lrdb/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     8286 2023-05-21 06:13:32.000000 spider-st-0.0.5/spider/preprocess.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    26415 2023-05-21 06:13:39.000000 spider-st-0.0.5/spider/svi.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      996 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/trajectory.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2689 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/util.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       21 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/version.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    15772 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/visualization.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.634099 spider-st-0.0.5/spider_st.egg-info/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 06:55:07.000000 spider-st-0.0.5/spider_st.egg-info/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1203 2023-05-21 06:55:07.000000 spider-st-0.0.5/spider_st.egg-info/SOURCES.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-21 06:55:07.000000 spider-st-0.0.5/spider_st.egg-info/dependency_links.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      302 2023-05-21 06:55:07.000000 spider-st-0.0.5/spider_st.egg-info/requires.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-21 06:55:07.000000 spider-st-0.0.5/spider_st.egg-info/top_level.txt
```

### Comparing `spider-st-0.0.4/LICENSE` & `spider-st-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/PKG-INFO` & `spider-st-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spider-st-0.0.4/setup.py` & `spider-st-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spider-st",
-    version="0.0.4",
+    version="0.0.5",
     author="Li Shiying",
     author_email="shiyingli7-c@my.cityu.edu.hk",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepomicslab/SPIDER",
     packages=setuptools.find_packages(),
@@ -56,10 +56,10 @@
         'umap-learn',
         'statsmodels',
         'importlib',
         'scprep',
         'squidpy',
         'magic-impute',
         'NaiveDE',
-        'gpflow',
+        'gpflow>= 2.12',
     ],
 )
```

### Comparing `spider-st-0.0.4/spider/R_script/run_nnSVG.R` & `spider-st-0.0.5/spider/R_script/run_nnSVG.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/R_script/run_spatalk.R` & `spider-st-0.0.5/spider/R_script/run_spatalk.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SPIDER.py` & `spider-st-0.0.5/spider/SPIDER.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/__init__.py` & `spider-st-0.0.5/spider/SpatialDE/__init__.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/distance_cache.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/distance_cache.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/gpflow_helpers.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/gpflow_helpers.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/kernels.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/kernels.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/models.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/models.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/optimizer.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/optimizer.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/score_test.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/score_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/sm_kernel.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/sm_kernel.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/svca.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/tf_dataset.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/tf_dataset.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/util.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/util.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/_internal/util_mixture.py` & `spider-st-0.0.5/spider/SpatialDE/_internal/util_mixture.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/aeh.py` & `spider-st-0.0.5/spider/SpatialDE/aeh.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/de_test.py` & `spider-st-0.0.5/spider/SpatialDE/de_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/dp_hmrf.py` & `spider-st-0.0.5/spider/SpatialDE/dp_hmrf.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/gaussian_process.py` & `spider-st-0.0.5/spider/SpatialDE/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/io.py` & `spider-st-0.0.5/spider/SpatialDE/io.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/SpatialDE/svca.py` & `spider-st-0.0.5/spider/SpatialDE/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/clustering.py` & `spider-st-0.0.5/spider/clustering.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/enrichment.py` & `spider-st-0.0.5/spider/enrichment.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/preprocess.py` & `spider-st-0.0.5/spider/preprocess.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/svi.py` & `spider-st-0.0.5/spider/svi.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/trajectory.py` & `spider-st-0.0.5/spider/trajectory.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/util.py` & `spider-st-0.0.5/spider/util.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider/visualization.py` & `spider-st-0.0.5/spider/visualization.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.4/spider_st.egg-info/PKG-INFO` & `spider-st-0.0.5/spider_st.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spider-st-0.0.4/spider_st.egg-info/SOURCES.txt` & `spider-st-0.0.5/spider_st.egg-info/SOURCES.txt`

 * *Files identical despite different names*

