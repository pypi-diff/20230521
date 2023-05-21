# Comparing `tmp/spider-st-0.0.5.tar.gz` & `tmp/spider-st-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-st-0.0.5.tar", last modified: Sun May 21 06:55:07 2023, max compression
+gzip compressed data, was "spider-st-0.0.6.tar", last modified: Sun May 21 07:22:35 2023, max compression
```

## Comparing `spider-st-0.0.5.tar` & `spider-st-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.634099 spider-st-0.0.5/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-21 05:33:01.000000 spider-st-0.0.5/LICENSE
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 06:55:07.634099 spider-st-0.0.5/PKG-INFO
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-21 05:33:01.000000 spider-st-0.0.5/README.md
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-21 06:55:07.642098 spider-st-0.0.5/setup.cfg
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1531 2023-05-21 06:55:01.000000 spider-st-0.0.5/setup.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.630099 spider-st-0.0.5/spider/
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.630099 spider-st-0.0.5/spider/R_script/
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/R_script/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      480 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/R_script/run_SPARKX.R
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      765 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/R_script/run_nnSVG.R
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/R_script/run_spatalk.R
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     6149 2023-05-21 06:51:11.000000 spider-st-0.0.5/spider/SPIDER.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.630099 spider-st-0.0.5/spider/SpatialDE/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.0.5/spider/SpatialDE/__init__.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.634099 spider-st-0.0.5/spider/SpatialDE/_internal/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/__init__.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/distance_cache.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/gpflow_helpers.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/kernels.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/models.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/optimizer.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/score_test.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/sm_kernel.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/svca.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/tf_dataset.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/util.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/_internal/util_mixture.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.0.5/spider/SpatialDE/aeh.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/de_test.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/dp_hmrf.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/gaussian_process.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/io.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.0.5/spider/SpatialDE/svca.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       26 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2958 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/clustering.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/enrichment.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.634099 spider-st-0.0.5/spider/lrdb/
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/lrdb/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     8286 2023-05-21 06:13:32.000000 spider-st-0.0.5/spider/preprocess.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    26415 2023-05-21 06:13:39.000000 spider-st-0.0.5/spider/svi.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      996 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/trajectory.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2689 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/util.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       21 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/version.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    15772 2023-05-21 05:37:57.000000 spider-st-0.0.5/spider/visualization.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:55:07.634099 spider-st-0.0.5/spider_st.egg-info/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 06:55:07.000000 spider-st-0.0.5/spider_st.egg-info/PKG-INFO
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1203 2023-05-21 06:55:07.000000 spider-st-0.0.5/spider_st.egg-info/SOURCES.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-21 06:55:07.000000 spider-st-0.0.5/spider_st.egg-info/dependency_links.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      302 2023-05-21 06:55:07.000000 spider-st-0.0.5/spider_st.egg-info/requires.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-21 06:55:07.000000 spider-st-0.0.5/spider_st.egg-info/top_level.txt
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.562501 spider-st-0.0.6/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-21 05:33:01.000000 spider-st-0.0.6/LICENSE
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 07:22:35.562501 spider-st-0.0.6/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-21 05:33:01.000000 spider-st-0.0.6/README.md
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-21 07:22:35.670499 spider-st-0.0.6/setup.cfg
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1552 2023-05-21 07:22:10.000000 spider-st-0.0.6/setup.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.478503 spider-st-0.0.6/spider/
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.522502 spider-st-0.0.6/spider/R_script/
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/R_script/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      480 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/R_script/run_SPARKX.R
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      765 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/R_script/run_nnSVG.R
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/R_script/run_spatalk.R
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     6149 2023-05-21 07:21:38.000000 spider-st-0.0.6/spider/SPIDER.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.522502 spider-st-0.0.6/spider/SpatialDE/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.0.6/spider/SpatialDE/__init__.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.562501 spider-st-0.0.6/spider/SpatialDE/_internal/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/__init__.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/distance_cache.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/gpflow_helpers.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/kernels.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/models.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/optimizer.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/score_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/sm_kernel.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/svca.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/tf_dataset.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/util.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/_internal/util_mixture.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.0.6/spider/SpatialDE/aeh.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/de_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/dp_hmrf.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/gaussian_process.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/io.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.0.6/spider/SpatialDE/svca.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       26 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2958 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/clustering.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/enrichment.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.562501 spider-st-0.0.6/spider/lrdb/
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/lrdb/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     8286 2023-05-21 06:13:32.000000 spider-st-0.0.6/spider/preprocess.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    26620 2023-05-21 07:21:19.000000 spider-st-0.0.6/spider/svi.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      996 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/trajectory.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2689 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/util.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       21 2023-05-21 07:21:25.000000 spider-st-0.0.6/spider/version.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    15772 2023-05-21 05:37:57.000000 spider-st-0.0.6/spider/visualization.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 07:22:35.562501 spider-st-0.0.6/spider_st.egg-info/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 07:22:35.000000 spider-st-0.0.6/spider_st.egg-info/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1203 2023-05-21 07:22:35.000000 spider-st-0.0.6/spider_st.egg-info/SOURCES.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-21 07:22:35.000000 spider-st-0.0.6/spider_st.egg-info/dependency_links.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      313 2023-05-21 07:22:35.000000 spider-st-0.0.6/spider_st.egg-info/requires.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-21 07:22:35.000000 spider-st-0.0.6/spider_st.egg-info/top_level.txt
```

### Comparing `spider-st-0.0.5/LICENSE` & `spider-st-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/PKG-INFO` & `spider-st-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spider-st-0.0.5/setup.py` & `spider-st-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spider-st",
-    version="0.0.5",
+    version="0.0.6",
     author="Li Shiying",
     author_email="shiyingli7-c@my.cityu.edu.hk",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepomicslab/SPIDER",
     packages=setuptools.find_packages(),
@@ -56,10 +56,11 @@
         'umap-learn',
         'statsmodels',
         'importlib',
         'scprep',
         'squidpy',
         'magic-impute',
         'NaiveDE',
-        'gpflow>= 2.12',
+        'gpflow',
+        'tensorflow>=2.12',
     ],
 )
```

### Comparing `spider-st-0.0.5/spider/R_script/run_nnSVG.R` & `spider-st-0.0.6/spider/R_script/run_nnSVG.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/R_script/run_spatalk.R` & `spider-st-0.0.6/spider/R_script/run_spatalk.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SPIDER.py` & `spider-st-0.0.6/spider/SPIDER.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/__init__.py` & `spider-st-0.0.6/spider/SpatialDE/__init__.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/distance_cache.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/distance_cache.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/gpflow_helpers.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/gpflow_helpers.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/kernels.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/kernels.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/models.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/models.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/optimizer.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/optimizer.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/score_test.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/score_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/sm_kernel.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/sm_kernel.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/svca.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/tf_dataset.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/tf_dataset.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/util.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/util.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/_internal/util_mixture.py` & `spider-st-0.0.6/spider/SpatialDE/_internal/util_mixture.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/aeh.py` & `spider-st-0.0.6/spider/SpatialDE/aeh.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/de_test.py` & `spider-st-0.0.6/spider/SpatialDE/de_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/dp_hmrf.py` & `spider-st-0.0.6/spider/SpatialDE/dp_hmrf.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/gaussian_process.py` & `spider-st-0.0.6/spider/SpatialDE/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/io.py` & `spider-st-0.0.6/spider/SpatialDE/io.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/SpatialDE/svca.py` & `spider-st-0.0.6/spider/SpatialDE/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/clustering.py` & `spider-st-0.0.6/spider/clustering.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/enrichment.py` & `spider-st-0.0.6/spider/enrichment.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/preprocess.py` & `spider-st-0.0.6/spider/preprocess.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/svi.py` & `spider-st-0.0.6/spider/svi.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,16 @@
                 n_jobs=10,
             )
             idata.uns['moranI_time'] = time.time()-t0
             idata.uns['moranI'].to_csv(f'{work_dir}moranI.csv')
         result = pd.read_csv(f'{work_dir}moranI.csv', index_col=0)
         idata.uns['moranI'] = result
         print(f'Added key moranI in idata.uns')
-    except:
+    except Exception as e:
+        print(e)
         pass
 
 def svi_geary(idata, work_dir,overwrite=False):
     try:
         t0=time.time()
         n_perms=1000
         if (overwrite) | (not exists( f'{work_dir}gearyC.csv')):
@@ -99,15 +100,16 @@
                 n_jobs=10,
             )
             idata.uns['gearyC_time'] = time.time()-t0
             idata.uns['gearyC'].to_csv(f'{work_dir}gearyC.csv')
         result = pd.read_csv(f'{work_dir}gearyC.csv', index_col=0)
         idata.uns['gearyC'] = result
         print(f'Added key gearyC in idata.uns')
-    except:
+    except Exception as e:
+        print(e)
         pass
 
 def svi_nnSVG(idata, work_dir, R_path, overwrite=False):
     try:
         count_f = f'{work_dir}idata_count.csv'
         meta_f = f'{work_dir}idata_meta.csv'
         if (overwrite) | ((not exists(count_f)) & (not exists(meta_f))):
@@ -119,14 +121,15 @@
                 os.system(str(f'/bin/bash -c "{R_path} -f {pw_fn} {count_f} {meta_f} {work_dir}"'))
             idata.uns['nnSVG_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}nnSVG.csv', index_col=0)
         idata.uns['nnSVG'] = result
         print(f'Added key nnSVG in idata.uns')
     except Exception as e:
         print(e)
+        pass
     
 def scGCO_sv(locs, data_norm, cellGraph, gmmDict, smooth_factor=10, unary_scale_factor=100, label_cost=10, algorithm='expansion'):
     from itertools import repeat
     from functools import reduce
     import operator
     import statsmodels.stats.multitest as multi
     import scGCO
@@ -177,15 +180,16 @@
             gmmDict= scGCO.gmm_model(data_norm)
             result_df= scGCO_sv(locs, data_norm, cellGraph,gmmDict)
             scGCO.write_result_to_csv(result_df, f'{work_dir}scGCO.csv')
             idata.uns['scGCO_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}scGCO.csv')
         idata.uns['scGCO'] = result
         print(f'Added key scGCO in idata.uns')
-    except:
+    except Exception as e:
+        print(e)
         pass
     
 def svi_SPARKX(idata, work_dir, R_path, overwrite=False):
     try:
         count_f = f'{work_dir}idata_count.csv'
         meta_f = f'{work_dir}idata_meta.csv'
         if (overwrite) | ((not exists(count_f)) & (not exists(meta_f))):
@@ -195,15 +199,16 @@
             t0=time.time()
             with resources.path("spider_local.R_script", "run_SPARKX.R") as pw_fn:
                 os.system(str(f'/bin/bash -c "{R_path} -f {pw_fn} {count_f} {meta_f} {work_dir}"'))
             idata.uns['SPARKX_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}SPARKX.csv', index_col=0)
         idata.uns['SPARKX'] = result
         print(f'Added key SPARKX in idata.uns')
-    except:
+    except Exception as e:
+        print(e)
         pass
     
 def svi_SpatialDE2(idata, work_dir, overwrite=False):
     try:
         # if (overwrite) | (not exists(f'{work_dir}SpatialDE.csv')) | (not exists(f'{work_dir}SpatialDE_individual.csv')):
         if (overwrite) | (not exists(f'{work_dir}SpatialDE.csv')):
             print('in')
@@ -213,15 +218,16 @@
             svg_full = pd.concat([svg_full.set_index('gene'), individual.loc[individual.groupby('gene').lengthscale.idxmin()].set_index('gene')], axis=1)
             svg_full.to_csv(f'{work_dir}SpatialDE.csv')
             individual.to_csv(f'{work_dir}SpatialDE_individual.csv')
             idata.uns['SpatialDE2_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}SpatialDE.csv', index_col=0)
         idata.uns['SpatialDE'] = result
         print(f'Added key SpatialDE in idata.uns')
-    except:
+    except Exception as e:
+        print(e)
         pass 
     
 def svi_SOMDE(idata, work_dir, overwrite=False, som=None):
     try:
         if (overwrite) | (not exists(f'{work_dir}SOMDE.csv')):
             t0=time.time()
             if som is None:
@@ -235,15 +241,16 @@
             nres = som.norm()
             result, SVnum =som.run()
             result.to_csv(f'{work_dir}SOMDE.csv')
             idata.uns['SOMDE_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}SOMDE.csv', index_col=0)
         idata.uns['SOMDE'] = result
         print(f'Added key SOMDE in idata.uns')
-    except:
+    except Exception as e:
+        print(e)
         pass
     
 def combine_SVI(idata, threshold):
     svi_df, svi_df_strict = combine_SVI_strict(idata,threshold=threshold)
     if len(svi_df_strict) < 10:
         print('Detected SVI number is less than 10, falling back to relaxed filtering.')
         svi_df, svi_df_strict = combine_SVI_Fisher(idata,threshold=threshold)
```

### Comparing `spider-st-0.0.5/spider/trajectory.py` & `spider-st-0.0.6/spider/trajectory.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/util.py` & `spider-st-0.0.6/spider/util.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider/visualization.py` & `spider-st-0.0.6/spider/visualization.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.5/spider_st.egg-info/PKG-INFO` & `spider-st-0.0.6/spider_st.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spider-st-0.0.5/spider_st.egg-info/SOURCES.txt` & `spider-st-0.0.6/spider_st.egg-info/SOURCES.txt`

 * *Files identical despite different names*

