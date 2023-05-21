# Comparing `tmp/spider-st-0.0.3.tar.gz` & `tmp/spider-st-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-st-0.0.3.tar", last modified: Sun May 21 05:40:41 2023, max compression
+gzip compressed data, was "spider-st-0.0.4.tar", last modified: Sun May 21 06:17:09 2023, max compression
```

## Comparing `spider-st-0.0.3.tar` & `spider-st-0.0.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:40.359744 spider-st-0.0.3/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-21 05:33:01.000000 spider-st-0.0.3/LICENSE
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 05:40:40.359744 spider-st-0.0.3/PKG-INFO
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-21 05:33:01.000000 spider-st-0.0.3/README.md
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-21 05:40:41.103734 spider-st-0.0.3/setup.cfg
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1524 2023-05-21 05:35:16.000000 spider-st-0.0.3/setup.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:37.483785 spider-st-0.0.3/spider/
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:39.475757 spider-st-0.0.3/spider/R_script/
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/R_script/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      480 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/R_script/run_SPARKX.R
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      765 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/R_script/run_nnSVG.R
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/R_script/run_spatalk.R
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     6035 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/SPIDER.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:40.359744 spider-st-0.0.3/spider/SpatialDE/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.0.3/spider/SpatialDE/__init__.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:40.359744 spider-st-0.0.3/spider/SpatialDE/_internal/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/__init__.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/distance_cache.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/gpflow_helpers.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/kernels.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/models.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/optimizer.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/score_test.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/sm_kernel.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/svca.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/tf_dataset.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/util.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/_internal/util_mixture.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.0.3/spider/SpatialDE/aeh.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/de_test.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/dp_hmrf.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/gaussian_process.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/io.py
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.0.3/spider/SpatialDE/svca.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       26 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2958 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/clustering.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/enrichment.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:40.359744 spider-st-0.0.3/spider/lrdb/
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/lrdb/__init__.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     7467 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/preprocess.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    26510 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/svi.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      996 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/trajectory.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2689 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/util.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       21 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/version.py
--rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    15772 2023-05-21 05:37:57.000000 spider-st-0.0.3/spider/visualization.py
-drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:40:40.359744 spider-st-0.0.3/spider_st.egg-info/
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 05:40:35.000000 spider-st-0.0.3/spider_st.egg-info/PKG-INFO
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1203 2023-05-21 05:40:35.000000 spider-st-0.0.3/spider_st.egg-info/SOURCES.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-21 05:40:35.000000 spider-st-0.0.3/spider_st.egg-info/dependency_links.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      296 2023-05-21 05:40:35.000000 spider-st-0.0.3/spider_st.egg-info/requires.txt
--rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-21 05:40:35.000000 spider-st-0.0.3/spider_st.egg-info/top_level.txt
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1068 2023-05-21 05:33:01.000000 spider-st-0.0.4/LICENSE
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 06:17:09.280198 spider-st-0.0.4/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      170 2023-05-21 05:33:01.000000 spider-st-0.0.4/README.md
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)       78 2023-05-21 06:17:09.556192 spider-st-0.0.4/setup.cfg
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1524 2023-05-21 06:16:53.000000 spider-st-0.0.4/setup.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.276198 spider-st-0.0.4/spider/
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/spider/R_script/
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/R_script/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      480 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/R_script/run_SPARKX.R
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      765 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/R_script/run_nnSVG.R
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2815 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/R_script/run_spatalk.R
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     6149 2023-05-21 06:13:17.000000 spider-st-0.0.4/spider/SPIDER.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/spider/SpatialDE/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      802 2023-01-15 09:48:37.000000 spider-st-0.0.4/spider/SpatialDE/__init__.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/spider/SpatialDE/_internal/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/__init__.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1156 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/distance_cache.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11731 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/gpflow_helpers.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3326 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/kernels.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11116 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/models.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1150 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/optimizer.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     9297 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/score_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     5569 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/sm_kernel.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    11625 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/svca.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1762 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/tf_dataset.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3700 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/util.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     2067 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/_internal/util_mixture.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    14715 2023-01-26 06:09:19.000000 spider-st-0.0.4/spider/SpatialDE/aeh.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     8305 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/de_test.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    16006 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/dp_hmrf.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)    13415 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/gaussian_process.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     3323 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/io.py
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     6818 2023-01-15 09:44:29.000000 spider-st-0.0.4/spider/SpatialDE/svca.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       26 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2958 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/clustering.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     9892 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/enrichment.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/spider/lrdb/
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/lrdb/__init__.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     8286 2023-05-21 06:13:32.000000 spider-st-0.0.4/spider/preprocess.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    26415 2023-05-21 06:13:39.000000 spider-st-0.0.4/spider/svi.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)      996 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/trajectory.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)     2689 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/util.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)       21 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/version.py
+-rwxrwxrwx   0 lishiying  (1035) lishiying  (1035)    15772 2023-05-21 05:37:57.000000 spider-st-0.0.4/spider/visualization.py
+drwxrwxr-x   0 lishiying  (1035) lishiying  (1035)        0 2023-05-21 06:17:09.280198 spider-st-0.0.4/spider_st.egg-info/
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      578 2023-05-21 06:17:08.000000 spider-st-0.0.4/spider_st.egg-info/PKG-INFO
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)     1203 2023-05-21 06:17:09.000000 spider-st-0.0.4/spider_st.egg-info/SOURCES.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        1 2023-05-21 06:17:08.000000 spider-st-0.0.4/spider_st.egg-info/dependency_links.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)      296 2023-05-21 06:17:08.000000 spider-st-0.0.4/spider_st.egg-info/requires.txt
+-rw-rw-r--   0 lishiying  (1035) lishiying  (1035)        7 2023-05-21 06:17:08.000000 spider-st-0.0.4/spider_st.egg-info/top_level.txt
```

### Comparing `spider-st-0.0.3/LICENSE` & `spider-st-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/PKG-INFO` & `spider-st-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spider-st-0.0.3/setup.py` & `spider-st-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 os.system("SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=TRUE")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spider-st",
-    version="0.0.3",
+    version="0.0.4",
     author="Li Shiying",
     author_email="shiyingli7-c@my.cityu.edu.hk",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepomicslab/SPIDER",
     packages=setuptools.find_packages(),
```

### Comparing `spider-st-0.0.3/spider/R_script/run_nnSVG.R` & `spider-st-0.0.4/spider/R_script/run_nnSVG.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/R_script/run_spatalk.R` & `spider-st-0.0.4/spider/R_script/run_spatalk.R`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SPIDER.py` & `spider-st-0.0.4/spider/SPIDER.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,75 +17,75 @@
         self.er = enrichment
         self.vis = visualization
         self.util = util
         self.traj = trajectory
         pass
 
     def prep(self,
-            adata_input, work_dir, 
+            adata_input, work_dir, R_path,
             no_spatalk=False,
             cluster_key='type', 
             is_human=True, 
             n_neighs=6, 
-            coord_type='grid', 
+            coord_type='generic', 
             imputation=True,
             overwrite=False,
     ):
         adata = adata_input.copy()
         del adata_input
         # detect cci
 
         # Step 1
-        pairs = preprocess.find_pairs(adata, coord_type, n_neighs)
-        pairs_meta = preprocess.meta(adata, cluster_key, pairs)
+        interface_cell_pair, interface_meta = preprocess.find_interfaces(adata, coord_type=coord_type, n_neighs=n_neighs, cluster_key=cluster_key)
         # Step 2
-        lr_raw = preprocess.subset_lr(adata, no_spatalk, work_dir, cluster_key, is_human, overwrite)
+        lr_raw = preprocess.subset_lr(adata, no_spatalk, work_dir, cluster_key, is_human, overwrite, R_path)
         lr_df, adata = preprocess.subset_adata(adata, lr_raw)
-        score = preprocess.score(adata, lr_df, pairs, imputation)
+        score = preprocess.score(adata, lr_df, interface_cell_pair, imputation)
         # Idata object construction
-        idata = preprocess.idata_construct(score, pairs_meta, lr_df, lr_raw, adata)
+        idata = preprocess.idata_construct(score, interface_meta, lr_df, lr_raw, adata)
         return idata
 
-    def find_svi(self, idata, out_f, abstract=True, overwrite=False, n_neighbors=10, threshold=0.01, pattern_prune_threshold=0.0001):
+    def find_svi(self, idata, out_f, R_path, abstract=True, overwrite=False, n_neighbors=10, threshold=0.01, pattern_prune_threshold=0.0001):
         from os.path import exists
         from os import mkdir
         if not exists(out_f):
             print(f'Creating folder {out_f}')
             mkdir(out_f)
         if len(idata) < 200:
             print('number of interface is less than 200, skipping abstraction')
             abstract=False
         if abstract:
             som, idata, meta_idata = svi.abstract(idata, n_neighbors)
-            svi.find_svi(meta_idata,out_f,overwrite, som=som) #generating results
+            svi.find_svi(meta_idata,out_f, overwrite, R_path, som=som) #generating results
             print('finished running all SVI tests')
             svi_df, svi_df_strict = svi.combine_SVI(meta_idata,threshold=threshold)
             if (overwrite) | (not exists(f'{out_f}pattern.csv')):
                 svi.SVI_patterns(meta_idata, svi_df_strict, pattern_prune_threshold=pattern_prune_threshold)
                 pd.DataFrame(meta_idata.obsm['pattern_score']).to_csv(f'{out_f}pattern.csv')
                 meta_idata.var.to_csv(f'{out_f}membership.csv')
             else:
                 meta_idata.obsm['pattern_score'] = pd.read_csv(f'{out_f}pattern.csv', index_col=0).to_numpy()
                 meta_idata.var = pd.read_csv(f'{out_f}membership.csv', index_col=0)
             svi.meta_pattern_to_idata(idata, meta_idata)
             pd.DataFrame(meta_idata.obsm['pattern_score']).to_csv(f'{out_f}full_pattern.csv')
         else:
-            svi.find_svi(idata, out_f,overwrite) #generating results
+            svi.find_svi(idata, out_f, R_path, overwrite) #generating results
             svi_df, svi_df_strict = svi.combine_SVI(idata,threshold=threshold)
             if (overwrite) | (not exists(f'{out_f}pattern.csv')):
                 svi.SVI_patterns(idata, svi_df_strict, pattern_prune_threshold=pattern_prune_threshold)
                 pd.DataFrame(idata.obsm['pattern_score']).to_csv(f'{out_f}pattern.csv')
                 idata.var.to_csv(f'{out_f}membership.csv')
             else:
                 idata.obsm['pattern_score'] = pd.read_csv(f'{out_f}pattern.csv', index_col=0)
                 idata.var = pd.read_csv(f'{out_f}membership.csv', index_col=0)   
+            meta_idata = None
         idata.var[[f'pattern_correlation_{x}' for x in range(idata.obsm['pattern_score'].shape[1])]] = 0
         corr_df=pd.concat([idata[:,idata.var['is_svi']==1].to_df(),pd.DataFrame(idata.obsm['pattern_score'],index=idata.obs_names)],axis=1).corr().loc[idata[:,idata.var['is_svi']==1].var_names, range(idata.obsm['pattern_score'].shape[1])]
         idata.var.loc[idata[:,idata.var['is_svi']==1].var_names, [f'pattern_correlation_{x}' for x in range(idata.obsm['pattern_score'].shape[1])]] = corr_df.to_numpy()
-        return idata, None
+        return idata, meta_idata
         
     def cell_transform(self, idata, adata, label=None):
         from scanpy.tools import rank_genes_groups
         import anndata
         adata = adata[adata.obs_names.isin(idata.uns['cell_meta'].index)]
         util.scored_spot_interface(idata)
         util.interaction_spot_interface(idata)
```

### Comparing `spider-st-0.0.3/spider/SpatialDE/__init__.py` & `spider-st-0.0.4/spider/SpatialDE/__init__.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/distance_cache.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/distance_cache.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/gpflow_helpers.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/gpflow_helpers.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/kernels.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/kernels.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/models.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/models.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/optimizer.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/optimizer.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/score_test.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/score_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/sm_kernel.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/sm_kernel.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/svca.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/tf_dataset.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/tf_dataset.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/util.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/util.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/_internal/util_mixture.py` & `spider-st-0.0.4/spider/SpatialDE/_internal/util_mixture.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/aeh.py` & `spider-st-0.0.4/spider/SpatialDE/aeh.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/de_test.py` & `spider-st-0.0.4/spider/SpatialDE/de_test.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/dp_hmrf.py` & `spider-st-0.0.4/spider/SpatialDE/dp_hmrf.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/gaussian_process.py` & `spider-st-0.0.4/spider/SpatialDE/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/io.py` & `spider-st-0.0.4/spider/SpatialDE/io.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/SpatialDE/svca.py` & `spider-st-0.0.4/spider/SpatialDE/svca.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/clustering.py` & `spider-st-0.0.4/spider/clustering.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/enrichment.py` & `spider-st-0.0.4/spider/enrichment.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/preprocess.py` & `spider-st-0.0.4/spider/preprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from scipy.spatial import Delaunay
 from sklearn.decomposition import PCA,NMF
 import anndata 
 from importlib import resources
 
 
 # detect cci
-def cci_spatalk(adata, work_dir, cluster_key, is_human, out_f):
+def cci_spatalk(adata, work_dir, cluster_key, is_human, out_f, R_path):
     import os
     count_f = f'{work_dir}/adata_count.csv'
     meta_f = f'{work_dir}/adata_meta.csv'
     df = adata.to_df()
     df.index = "C"+df.index
     df.to_csv(count_f)
     meta = adata.obs[cluster_key].reset_index()
@@ -28,15 +28,16 @@
     if not pd.api.types.is_string_dtype(meta.celltype.dtype):
         meta.celltype = "T"+meta.celltype.astype('str')
     meta.celltype = meta.celltype.str.replace(' ', '_')
     meta.celltype = meta.celltype.str.replace('-', '_')
     meta.to_csv(meta_f)
     species = 'Human' if is_human else 'Mouse'
     with resources.path("spider_local.R_script", "run_spatalk.R") as pw_fn:
-        os.system(str(f'/bin/bash -c "source /etc/profile;module load GCC/11.2.0 OpenMPI/4.1.1 R/4.2.0 Anaconda3/2022.05 R-bundle-Bioconductor/3.15-R-4.2.0;R -f {pw_fn} {count_f} {meta_f} {species} {out_f}"'))
+        os.system(str(f'/bin/bash -c "{R_path} -f {pw_fn} {count_f} {meta_f} {species} {out_f}"'))
+        # os.system(str(f'/bin/bash -c "source /etc/profile;module load GCC/11.2.0 OpenMPI/4.1.1 R/4.2.0 Anaconda3/2022.05 R-bundle-Bioconductor/3.15-R-4.2.0;R -f {pw_fn} {count_f} {meta_f} {species} {out_f}"'))
     
 # imputation
 def impute_MAGIC(adata):
     magic_op = magic.MAGIC(n_jobs=5)
     inp = adata.to_df()
     inp = scprep.normalize.library_size_normalize(inp)
     inp = scprep.transform.sqrt(inp)
@@ -54,23 +55,23 @@
     cell_meta = adata.obs.loc[unique_cells]
     idata.uns['cell_meta'] = cell_meta
     # quality check
     sc.pp.calculate_qc_metrics(idata, inplace=True, percent_top=None)
     sc.pp.filter_genes(idata, min_cells=5)
     sc.pp.filter_cells(idata, min_genes=1)
     idata.obsm['spatial'] = idata.obs[['row', 'col']].to_numpy()
-    print(f'Construct idata with {idata.shape[0]} interactions and {idata.shape[1]} LR pairs.')
+    print(f'Construct idata with {idata.shape[0]} interfaces and {idata.shape[1]} LR pairs.')
     return idata
 
-def subset_lr(adata, no_spatalk, work_dir, cluster_key, is_human, overwrite):
+def subset_lr(adata, no_spatalk, work_dir, cluster_key, is_human, overwrite, R_path):
     from os.path import exists
     if not no_spatalk:
         out_f = f'{work_dir}/spatalk'
         if overwrite | (not exists(f'{out_f}_lrpair.csv')):
-            cci_spatalk(adata, work_dir, cluster_key, is_human, out_f)
+            cci_spatalk(adata, work_dir, cluster_key, is_human, out_f, R_path)
         else:
             print(f'{out_f}_lrpair.csv already exists, skipping spatalk.')
     try:
         print('using spatalk result')
         lr_raw = pd.read_csv(f'{out_f}_lrpair.csv', index_col=0).sort_values('score')
         lr_raw = lr_raw.drop_duplicates(subset=['ligand', 'receptor'], keep="last")
     except:
@@ -93,38 +94,50 @@
     sub_exp_rev = exp_ref[np.concatenate((r, l))].to_numpy()
     edge_exp_both = np.multiply(sub_exp[pairs[0]], sub_exp_rev[pairs[1]])
     # equation 2 in the manuscript
     print('scoring')
     score = lr_df['score'].to_numpy()*np.sqrt(np.maximum(edge_exp_both[:, :int(len(l))], edge_exp_both[:, int(len(l)):]))
     return score
 
+def find_interfaces(adata, coord_type, n_neighs, cluster_key):
+        pairs = find_pairs(adata, coord_type=coord_type, n_neighs=n_neighs)
+        pairs_meta = meta(adata, cluster_key, pairs)
+        return pairs, pairs_meta
+
 def subset_adata(adata, lr_df):
     genes = adata.var_names.tolist()
     lr_df = lr_df[lr_df['ligand'].isin(genes) & lr_df['receptor'].isin(genes)]
     lr_df.index = lr_df['ligand'] + "_" + lr_df['receptor']
     l = lr_df['ligand'].to_numpy().flatten()
     r = lr_df['receptor'].to_numpy().flatten()
     unique_lr = np.unique(np.concatenate((l, r)))
     adata = adata[:, adata.var_names.isin(unique_lr)]
     sc.pp.filter_genes(adata, min_cells=1)
-    sc.pp.filter_cells(adata, min_genes=1)
     sc.pp.normalize_total(adata, target_sum=1e4)
     genes = adata.var_names.tolist()
     lr_df = lr_df[lr_df['ligand'].isin(genes) & lr_df['receptor'].isin(genes)]
     return lr_df, adata
 
-def find_pairs(adata, coord_type='grid', n_neighs=6):
-    from squidpy.gr import spatial_neighbors
+def find_pairs(adata, coord_type='generic', n_neighs=6):
+    from sklearn.metrics import pairwise_distances
     from scipy.sparse import triu
-    if coord_type == 'grid':
+    from scipy.spatial import Delaunay
+    from squidpy.gr import spatial_neighbors
+    if coord_type=='grid':    
         spatial_neighbors(adata, coord_type=coord_type, n_neighs=n_neighs)
+        return np.transpose(triu(adata.obsp['spatial_connectivities']).nonzero()).T
     else:
+        print('non grid coordinate')
         spatial_neighbors(adata, coord_type=coord_type, delaunay=True, n_neighs=n_neighs)
-    return np.transpose(triu(adata.obsp['spatial_connectivities']).nonzero()).T
-
+        potential_pairs = np.transpose(triu(adata.obsp['spatial_connectivities']).nonzero()).T
+        print('distance cutoff')
+        d = np.linalg.norm(adata.obsm['spatial'][potential_pairs[0]]-adata.obsm['spatial'][potential_pairs[1]], axis=1)
+        d = (d - d.mean()) / d.std()**2
+        potential_pairs = potential_pairs[:, d <= d.std()]
+        return potential_pairs
 
 def meta(adata, cluster_key, pairs):
     # get label
     pairs_meta = pd.DataFrame()
     pairs_meta['A'] = adata.obs_names[pairs[0]]
     pairs_meta['B'] = adata.obs_names[pairs[1]]
     pairs_meta[['A_row', 'A_col']] = adata.obsm['spatial'][pairs[0]]
```

### Comparing `spider-st-0.0.3/spider/svi.py` & `spider-st-0.0.4/spider/svi.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,31 +38,32 @@
         idata.obs.loc[df.loc[:,np.array(soml)==i].columns,'som_node'] = count
         count += 1
     return idata
 
 def meta_pattern_to_idata(idata, meta_idata):
     idata.obsm['pattern_score'] = meta_idata.obsm['pattern_score'][idata.obs['som_node'].to_numpy()]  
     idata.var = meta_idata.var
+    print(meta_idata)
     idata.uns['nnSVG'] = meta_idata.uns['nnSVG']
     idata.uns['SOMDE'] = meta_idata.uns['SOMDE']
     idata.uns['SpatialDE'] = meta_idata.uns['SpatialDE']
     idata.uns['SPARKX'] = meta_idata.uns['SPARKX']
     idata.uns['scGCO'] = meta_idata.uns['scGCO']
     idata.uns['moranI'] = meta_idata.uns['moranI']
     idata.uns['gearyC'] = meta_idata.uns['gearyC']
     print(f'Added key pattern_score in idata.obsm')   
 
-def find_svi(idata, out_f, overwrite, som=None):
+def find_svi(idata, out_f, overwrite, R_path, som=None):
     # Method: Identifying spatially variable LR interactions
     # Gaussian models
-    svi_nnSVG(idata,out_f,overwrite)
+    svi_nnSVG(idata,out_f,R_path,overwrite)
     svi_SOMDE(idata,out_f,overwrite, som=som)
     svi_SpatialDE2(idata,out_f,overwrite)
     # Non-parametric covariance test
-    svi_SPARKX(idata,out_f,overwrite)
+    svi_SPARKX(idata,out_f,R_path,overwrite)
     # HMRF
     svi_scGCO(idata,out_f,overwrite)
     # baseline auto-correlation metrics
     svi_moran(idata,out_f,overwrite)
     svi_geary(idata,out_f,overwrite)
 
 def svi_moran(idata, work_dir, overwrite=False):
@@ -101,31 +102,31 @@
             idata.uns['gearyC'].to_csv(f'{work_dir}gearyC.csv')
         result = pd.read_csv(f'{work_dir}gearyC.csv', index_col=0)
         idata.uns['gearyC'] = result
         print(f'Added key gearyC in idata.uns')
     except:
         pass
 
-def svi_nnSVG(idata, work_dir, overwrite=False):
+def svi_nnSVG(idata, work_dir, R_path, overwrite=False):
     try:
         count_f = f'{work_dir}idata_count.csv'
         meta_f = f'{work_dir}idata_meta.csv'
         if (overwrite) | ((not exists(count_f)) & (not exists(meta_f))):
             idata.to_df().to_csv(count_f)
             idata.obs[['row', 'col']].to_csv(meta_f)
         if (overwrite) | (not exists( f'{work_dir}nnSVG.csv')):
             t0=time.time()
-            with resources.path("spider.R_script", "run_nnSVG.R") as pw_fn:
-                os.system(str(f'/bin/bash -c "source /etc/profile;module load GCC/11.2.0 OpenMPI/4.1.1 R/4.2.0 Anaconda3/2022.05 R-bundle-Bioconductor/3.15-R-4.2.0;R -f {pw_fn} {count_f} {meta_f} {work_dir}"'))
+            with resources.path("spider_local.R_script", "run_nnSVG.R") as pw_fn:
+                os.system(str(f'/bin/bash -c "{R_path} -f {pw_fn} {count_f} {meta_f} {work_dir}"'))
             idata.uns['nnSVG_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}nnSVG.csv', index_col=0)
         idata.uns['nnSVG'] = result
         print(f'Added key nnSVG in idata.uns')
-    except:
-        pass
+    except Exception as e:
+        print(e)
     
 def scGCO_sv(locs, data_norm, cellGraph, gmmDict, smooth_factor=10, unary_scale_factor=100, label_cost=10, algorithm='expansion'):
     from itertools import repeat
     from functools import reduce
     import operator
     import statsmodels.stats.multitest as multi
     import scGCO
@@ -179,37 +180,38 @@
             idata.uns['scGCO_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}scGCO.csv')
         idata.uns['scGCO'] = result
         print(f'Added key scGCO in idata.uns')
     except:
         pass
     
-def svi_SPARKX(idata, work_dir, overwrite=False):
+def svi_SPARKX(idata, work_dir, R_path, overwrite=False):
     try:
         count_f = f'{work_dir}idata_count.csv'
         meta_f = f'{work_dir}idata_meta.csv'
         if (overwrite) | ((not exists(count_f)) & (not exists(meta_f))):
             idata.to_df().to_csv(count_f)
             idata.obs[['row', 'col']].to_csv(meta_f)
         if (overwrite) | (not exists( f'{work_dir}SPARKX.csv')):
             t0=time.time()
-            with resources.path("spider.R_script", "run_SPARKX.R") as pw_fn:
-                os.system(str(f'/bin/bash -c "source /etc/profile;module load GCC/11.2.0 OpenMPI/4.1.1 R/4.2.0 Anaconda3/2022.05 R-bundle-Bioconductor/3.15-R-4.2.0;R -f {pw_fn} {count_f} {meta_f} {work_dir}"'))
+            with resources.path("spider_local.R_script", "run_SPARKX.R") as pw_fn:
+                os.system(str(f'/bin/bash -c "{R_path} -f {pw_fn} {count_f} {meta_f} {work_dir}"'))
             idata.uns['SPARKX_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}SPARKX.csv', index_col=0)
         idata.uns['SPARKX'] = result
         print(f'Added key SPARKX in idata.uns')
     except:
         pass
     
 def svi_SpatialDE2(idata, work_dir, overwrite=False):
     try:
         # if (overwrite) | (not exists(f'{work_dir}SpatialDE.csv')) | (not exists(f'{work_dir}SpatialDE_individual.csv')):
         if (overwrite) | (not exists(f'{work_dir}SpatialDE.csv')):
-            from spider import SpatialDE as SpatialDE2
+            print('in')
+            from spider_local import SpatialDE as SpatialDE2
             t0=time.time()
             svg_full, individual = SpatialDE2.test(idata, omnibus=False)
             svg_full = pd.concat([svg_full.set_index('gene'), individual.loc[individual.groupby('gene').lengthscale.idxmin()].set_index('gene')], axis=1)
             svg_full.to_csv(f'{work_dir}SpatialDE.csv')
             individual.to_csv(f'{work_dir}SpatialDE_individual.csv')
             idata.uns['SpatialDE2_time'] = time.time()-t0
         result = pd.read_csv(f'{work_dir}SpatialDE.csv', index_col=0)
@@ -338,15 +340,15 @@
     """dot.notation access to dictionary attributes"""
     __getattr__ = dict.get
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
 # SVI pattern generation with Gaussian process mixture model
 def SVI_patterns(idata, svi_df_strict, iter=1000, pattern_prune_threshold=1e-8):
-    from spider import SpatialDE as SpatialDE2
+    from spider_local import SpatialDE as SpatialDE2
     allsignifgenes = svi_df_strict.index.to_numpy()
     if 'lengthscale' in idata.uns['SpatialDE'].columns:
         l=idata.uns['SpatialDE'].loc[allsignifgenes]['lengthscale'].to_list()
         if len(np.unique(l)) < 2:
             allsignifgenes = np.intersect1d(allsignifgenes, idata.uns['SOMDE']['g'].to_numpy())
             l=idata.uns['SOMDE'].set_index('g').loc[allsignifgenes]['l'].to_list()
     else:
```

### Comparing `spider-st-0.0.3/spider/trajectory.py` & `spider-st-0.0.4/spider/trajectory.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/util.py` & `spider-st-0.0.4/spider/util.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider/visualization.py` & `spider-st-0.0.4/spider/visualization.py`

 * *Files identical despite different names*

### Comparing `spider-st-0.0.3/spider_st.egg-info/PKG-INFO` & `spider-st-0.0.4/spider_st.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-st
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/deepomicslab/SPIDER
 Author: Li Shiying
 Author-email: shiyingli7-c@my.cityu.edu.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spider-st-0.0.3/spider_st.egg-info/SOURCES.txt` & `spider-st-0.0.4/spider_st.egg-info/SOURCES.txt`

 * *Files identical despite different names*

