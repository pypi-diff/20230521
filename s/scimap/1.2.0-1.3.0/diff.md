# Comparing `tmp/scimap-1.2.0.tar.gz` & `tmp/scimap-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimap-1.2.0.tar", max compression
+gzip compressed data, was "scimap-1.3.0.tar", max compression
```

## Comparing `scimap-1.2.0.tar` & `scimap-1.3.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
--rw-r--r--   0        0        0     2240 2023-04-15 12:35:07.000000 scimap-1.2.0/README.md
--rw-r--r--   0        0        0     2369 2023-05-06 15:08:34.186630 scimap-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      299 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/__init__.py
--rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/__main__.py
--rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/cli/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-1.2.0/scimap/cli/_scimap_mcmicro.py
--rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-1.2.0/scimap/cli/test.py
--rw-r--r--   0        0        0      257 2022-07-04 23:50:44.000000 scimap-1.2.0/scimap/helpers/__init__.py
--rwxr-xr-x   0        0        0     6454 2022-05-01 02:47:57.000000 scimap-1.2.0/scimap/helpers/_addROI_omero.py
--rw-r--r--   0        0        0     6459 2022-05-01 03:13:26.000000 scimap-1.2.0/scimap/helpers/_add_roi_omero.py
--rw-r--r--   0        0        0    17875 2022-06-01 15:52:05.000000 scimap-1.2.0/scimap/helpers/_animate.py
--rwxr-xr-x   0        0        0     4944 2022-05-01 16:43:37.000000 scimap-1.2.0/scimap/helpers/_classify.py
--rw-r--r--   0        0        0     4835 2022-07-06 00:37:53.000000 scimap-1.2.0/scimap/helpers/_dropFeatures.py
--rwxr-xr-x   0        0        0     3830 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/helpers/_merge_adata_obs.py
--rwxr-xr-x   0        0        0     2276 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/helpers/_rename.py
--rw-r--r--   0        0        0     4855 2022-05-26 00:36:56.000000 scimap-1.2.0/scimap/helpers/_scimap_to_csv.py
--rwxr-xr-x   0        0        0     3141 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/helpers/add_roi_scatter.py
--rw-r--r--   0        0        0      504 2023-05-06 13:15:57.195162 scimap-1.2.0/scimap/plotting/__init__.py
--rw-r--r--   0        0        0    16440 2022-05-30 03:05:13.000000 scimap-1.2.0/scimap/plotting/_addROI_image.py
--rwxr-xr-x   0        0        0     5378 2021-07-02 16:14:28.000000 scimap-1.2.0/scimap/plotting/_cluster_plots.py
--rwxr-xr-x   0        0        0     6356 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/plotting/_foldchange.py
--rw-r--r--   0        0        0     8423 2022-05-26 00:26:48.000000 scimap-1.2.0/scimap/plotting/_gate_finder.py
--rw-r--r--   0        0        0     9403 2023-04-22 02:17:49.145882 scimap-1.2.0/scimap/plotting/_image_viewer.py
--rwxr-xr-x   0        0        0     6778 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/plotting/_pie.py
--rwxr-xr-x   0        0        0    12247 2022-08-05 18:19:47.000000 scimap-1.2.0/scimap/plotting/_spatial_distance.py
--rwxr-xr-x   0        0        0    10520 2022-07-28 19:28:59.000000 scimap-1.2.0/scimap/plotting/_spatial_interaction.py
--rwxr-xr-x   0        0        0     2837 2023-04-14 19:18:24.000000 scimap-1.2.0/scimap/plotting/_spatial_pscore.py
--rw-r--r--   0        0        0     1226 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/plotting/_spatial_scatter.py
--rwxr-xr-x   0        0        0     8776 2021-07-15 16:39:53.000000 scimap-1.2.0/scimap/plotting/_stacked_barplot.py
--rw-r--r--   0        0        0    11523 2022-05-29 22:46:02.000000 scimap-1.2.0/scimap/plotting/_umap.py
--rwxr-xr-x   0        0        0    17378 2021-07-12 17:49:48.000000 scimap-1.2.0/scimap/plotting/_voronoi.py
--rw-r--r--   0        0        0     8425 2023-05-06 15:02:41.773078 scimap-1.2.0/scimap/plotting/densityPlot2D.py
--rw-r--r--   0        0        0     3341 2020-04-01 13:37:18.000000 scimap-1.2.0/scimap/plotting/lasso_selector.py
--rw-r--r--   0        0        0      107 2023-04-20 01:30:26.953137 scimap-1.2.0/scimap/preprocessing/__init__.py
--rw-r--r--   0        0        0     5078 2023-04-21 02:03:50.459976 scimap-1.2.0/scimap/preprocessing/_combat.py
--rw-r--r--   0        0        0     9716 2022-05-29 01:57:56.000000 scimap-1.2.0/scimap/preprocessing/_mcmicro_to_scimap.py
--rw-r--r--   0        0        0    16550 2022-12-30 21:50:38.000000 scimap-1.2.0/scimap/preprocessing/_rescale.py
--rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tests/_data/example_data.csv
--rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tests/_data/example_data.h5ad
--rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tests/_data/phenotype_workflow.csv
--rwxr-xr-x   0        0        0     1268 2023-05-06 14:45:48.623561 scimap-1.2.0/scimap/tests/test_helpers.py
--rwxr-xr-x   0        0        0      984 2023-05-06 14:46:01.108135 scimap-1.2.0/scimap/tests/test_preprocessing.py
--rwxr-xr-x   0        0        0     4673 2023-05-06 14:46:08.191066 scimap-1.2.0/scimap/tests/test_tools.py
--rw-r--r--   0        0        0      581 2022-05-29 01:02:42.000000 scimap-1.2.0/scimap/tools/__init__.py
--rwxr-xr-x   0        0        0    20976 2021-07-02 14:30:55.000000 scimap-1.2.0/scimap/tools/_cluster.py
--rwxr-xr-x   0        0        0     7389 2022-05-17 01:33:44.000000 scimap-1.2.0/scimap/tools/_foldchange.py
--rw-r--r--   0        0        0    15522 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tools/_phenotype_cells.py
--rwxr-xr-x   0        0        0     8047 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tools/_spatial_aggregate.py
--rw-r--r--   0        0        0     7851 2022-05-05 01:01:59.000000 scimap-1.2.0/scimap/tools/_spatial_cluster.py
--rwxr-xr-x   0        0        0     7229 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tools/_spatial_count.py
--rw-r--r--   0        0        0     4909 2022-05-26 23:45:54.000000 scimap-1.2.0/scimap/tools/_spatial_distance.py
--rwxr-xr-x   0        0        0    10750 2022-05-15 00:55:32.000000 scimap-1.2.0/scimap/tools/_spatial_expression.py
--rw-r--r--   0        0        0    11448 2022-04-28 19:44:16.000000 scimap-1.2.0/scimap/tools/_spatial_interaction.py
--rw-r--r--   0        0        0     7863 2022-06-10 00:00:59.000000 scimap-1.2.0/scimap/tools/_spatial_lda.py
--rw-r--r--   0        0        0     9275 2023-04-14 19:20:19.000000 scimap-1.2.0/scimap/tools/_spatial_pscore.py
--rw-r--r--   0        0        0    18190 2022-06-04 15:12:26.000000 scimap-1.2.0/scimap/tools/_spatial_similarity_search.py
--rw-r--r--   0        0        0     3939 2022-06-06 16:53:31.000000 scimap-1.2.0/scimap/tools/_umap.py
--rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 scimap-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2240 2023-04-15 12:35:07.000000 scimap-1.3.0/README.md
+-rw-r--r--   0        0        0     2369 2023-05-21 01:05:13.360063 scimap-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      299 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/__init__.py
+-rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/__main__.py
+-rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/cli/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-1.3.0/scimap/cli/_scimap_mcmicro.py
+-rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-1.3.0/scimap/cli/test.py
+-rw-r--r--   0        0        0      257 2022-07-04 23:50:44.000000 scimap-1.3.0/scimap/helpers/__init__.py
+-rwxr-xr-x   0        0        0     6454 2022-05-01 02:47:57.000000 scimap-1.3.0/scimap/helpers/_addROI_omero.py
+-rw-r--r--   0        0        0     6459 2022-05-01 03:13:26.000000 scimap-1.3.0/scimap/helpers/_add_roi_omero.py
+-rw-r--r--   0        0        0    17875 2022-06-01 15:52:05.000000 scimap-1.3.0/scimap/helpers/_animate.py
+-rwxr-xr-x   0        0        0     4944 2022-05-01 16:43:37.000000 scimap-1.3.0/scimap/helpers/_classify.py
+-rw-r--r--   0        0        0     4835 2022-07-06 00:37:53.000000 scimap-1.3.0/scimap/helpers/_dropFeatures.py
+-rwxr-xr-x   0        0        0     3830 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/helpers/_merge_adata_obs.py
+-rwxr-xr-x   0        0        0     2276 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/helpers/_rename.py
+-rw-r--r--   0        0        0     4855 2022-05-26 00:36:56.000000 scimap-1.3.0/scimap/helpers/_scimap_to_csv.py
+-rwxr-xr-x   0        0        0     3141 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/helpers/add_roi_scatter.py
+-rw-r--r--   0        0        0      588 2023-05-21 00:55:17.808850 scimap-1.3.0/scimap/plotting/__init__.py
+-rw-r--r--   0        0        0    16440 2022-05-30 03:05:13.000000 scimap-1.3.0/scimap/plotting/_addROI_image.py
+-rwxr-xr-x   0        0        0     5378 2021-07-02 16:14:28.000000 scimap-1.3.0/scimap/plotting/_cluster_plots.py
+-rwxr-xr-x   0        0        0     6356 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/plotting/_foldchange.py
+-rw-r--r--   0        0        0     9508 2023-05-20 22:41:36.638128 scimap-1.3.0/scimap/plotting/_gate_finder.py
+-rw-r--r--   0        0        0     9403 2023-04-22 02:17:49.145882 scimap-1.3.0/scimap/plotting/_image_viewer.py
+-rwxr-xr-x   0        0        0     6778 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/plotting/_pie.py
+-rwxr-xr-x   0        0        0    12247 2022-08-05 18:19:47.000000 scimap-1.3.0/scimap/plotting/_spatial_distance.py
+-rwxr-xr-x   0        0        0    10520 2022-07-28 19:28:59.000000 scimap-1.3.0/scimap/plotting/_spatial_interaction.py
+-rwxr-xr-x   0        0        0     2837 2023-04-14 19:18:24.000000 scimap-1.3.0/scimap/plotting/_spatial_pscore.py
+-rw-r--r--   0        0        0     1226 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/plotting/_spatial_scatter.py
+-rwxr-xr-x   0        0        0     8776 2021-07-15 16:39:53.000000 scimap-1.3.0/scimap/plotting/_stacked_barplot.py
+-rw-r--r--   0        0        0    11523 2022-05-29 22:46:02.000000 scimap-1.3.0/scimap/plotting/_umap.py
+-rwxr-xr-x   0        0        0    17378 2021-07-12 17:49:48.000000 scimap-1.3.0/scimap/plotting/_voronoi.py
+-rw-r--r--   0        0        0     8513 2023-05-21 00:45:22.122325 scimap-1.3.0/scimap/plotting/densityPlot2D.py
+-rw-r--r--   0        0        0     8694 2023-05-21 00:57:39.732696 scimap-1.3.0/scimap/plotting/distPlot.py
+-rw-r--r--   0        0        0     3341 2020-04-01 13:37:18.000000 scimap-1.3.0/scimap/plotting/lasso_selector.py
+-rw-r--r--   0        0        0    11486 2023-05-21 00:55:01.189031 scimap-1.3.0/scimap/plotting/spatial_scatterPlot.py
+-rw-r--r--   0        0        0      107 2023-04-20 01:30:26.953137 scimap-1.3.0/scimap/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5078 2023-04-21 02:03:50.459976 scimap-1.3.0/scimap/preprocessing/_combat.py
+-rw-r--r--   0        0        0     9716 2022-05-29 01:57:56.000000 scimap-1.3.0/scimap/preprocessing/_mcmicro_to_scimap.py
+-rw-r--r--   0        0        0    16550 2022-12-30 21:50:38.000000 scimap-1.3.0/scimap/preprocessing/_rescale.py
+-rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tests/_data/example_data.csv
+-rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tests/_data/example_data.h5ad
+-rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tests/_data/phenotype_workflow.csv
+-rwxr-xr-x   0        0        0     1268 2023-05-06 14:45:48.623561 scimap-1.3.0/scimap/tests/test_helpers.py
+-rwxr-xr-x   0        0        0      984 2023-05-06 14:46:01.108135 scimap-1.3.0/scimap/tests/test_preprocessing.py
+-rwxr-xr-x   0        0        0     4673 2023-05-06 14:46:08.191066 scimap-1.3.0/scimap/tests/test_tools.py
+-rw-r--r--   0        0        0      581 2022-05-29 01:02:42.000000 scimap-1.3.0/scimap/tools/__init__.py
+-rwxr-xr-x   0        0        0    20976 2021-07-02 14:30:55.000000 scimap-1.3.0/scimap/tools/_cluster.py
+-rwxr-xr-x   0        0        0     7389 2022-05-17 01:33:44.000000 scimap-1.3.0/scimap/tools/_foldchange.py
+-rw-r--r--   0        0        0    15522 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tools/_phenotype_cells.py
+-rwxr-xr-x   0        0        0     8047 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tools/_spatial_aggregate.py
+-rw-r--r--   0        0        0     7851 2022-05-05 01:01:59.000000 scimap-1.3.0/scimap/tools/_spatial_cluster.py
+-rwxr-xr-x   0        0        0     7229 2021-07-01 20:47:33.000000 scimap-1.3.0/scimap/tools/_spatial_count.py
+-rw-r--r--   0        0        0     4909 2022-05-26 23:45:54.000000 scimap-1.3.0/scimap/tools/_spatial_distance.py
+-rwxr-xr-x   0        0        0    10750 2022-05-15 00:55:32.000000 scimap-1.3.0/scimap/tools/_spatial_expression.py
+-rw-r--r--   0        0        0    11448 2022-04-28 19:44:16.000000 scimap-1.3.0/scimap/tools/_spatial_interaction.py
+-rw-r--r--   0        0        0     7863 2022-06-10 00:00:59.000000 scimap-1.3.0/scimap/tools/_spatial_lda.py
+-rw-r--r--   0        0        0     9275 2023-04-14 19:20:19.000000 scimap-1.3.0/scimap/tools/_spatial_pscore.py
+-rw-r--r--   0        0        0    18190 2022-06-04 15:12:26.000000 scimap-1.3.0/scimap/tools/_spatial_similarity_search.py
+-rw-r--r--   0        0        0     3939 2022-06-06 16:53:31.000000 scimap-1.3.0/scimap/tools/_umap.py
+-rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 scimap-1.3.0/PKG-INFO
```

### Comparing `scimap-1.2.0/README.md` & `scimap-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/pyproject.toml` & `scimap-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "scimap"
-version = "1.2.0"
+version = "1.3.0"
 description = "Spatial Single-Cell Analysis Toolkit"
 
 license = "MIT"
 
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 
 readme = "README.md"
```

### Comparing `scimap-1.2.0/scimap/cli/_scimap_mcmicro.py` & `scimap-1.3.0/scimap/cli/_scimap_mcmicro.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/cli/test.py` & `scimap-1.3.0/scimap/cli/test.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/helpers/_addROI_omero.py` & `scimap-1.3.0/scimap/helpers/_addROI_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/helpers/_add_roi_omero.py` & `scimap-1.3.0/scimap/helpers/_add_roi_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/helpers/_animate.py` & `scimap-1.3.0/scimap/helpers/_animate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/helpers/_classify.py` & `scimap-1.3.0/scimap/helpers/_classify.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/helpers/_dropFeatures.py` & `scimap-1.3.0/scimap/helpers/_dropFeatures.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/helpers/_merge_adata_obs.py` & `scimap-1.3.0/scimap/helpers/_merge_adata_obs.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/helpers/_rename.py` & `scimap-1.3.0/scimap/helpers/_rename.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/helpers/_scimap_to_csv.py` & `scimap-1.3.0/scimap/helpers/_scimap_to_csv.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/helpers/add_roi_scatter.py` & `scimap-1.3.0/scimap/helpers/add_roi_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_addROI_image.py` & `scimap-1.3.0/scimap/plotting/_addROI_image.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_cluster_plots.py` & `scimap-1.3.0/scimap/plotting/_cluster_plots.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_foldchange.py` & `scimap-1.3.0/scimap/plotting/_foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_gate_finder.py` & `scimap-1.3.0/scimap/preprocessing/_mcmicro_to_scimap.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,241 +1,240 @@
-#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Created on Tue May 12 23:47:52 2020
+# Created on Mon Mar  2 09:12:35 2020
 # @author: Ajit Johnson Nirmal
+
 """
 !!! abstract "Short Description"
-    `sm.pl.gate_finder`: The function opens the OME-TIFF image inside Napari and overlays points to help with the 
-    identifying manual gates for each marker. Use the `sm.pp.rescale` function to apply the identified gates to your data.
+    `sm.pp.mcmicro_to_scimap`: The function allows users to directly import the output from [mcmicro](https://mcmicro.org/) 
+    into `scimap`.
 
 ## Function
 """
 
-try:
-    import napari
-except:
-    pass
-
-import pandas as pd
-import tifffile as tiff
+# Import library
 import numpy as np
-
-import dask.array as da
-from dask.cache import Cache
-import zarr
-import os
-
-cache = Cache(2e9)  # Leverage two gigabytes of memory
-cache.register()
-
-def gate_finder (image_path, adata, marker_of_interest, from_gate = 6, to_gate = 8, increment = 0.1,
-                 markers=None, channel_names = 'default', flip_y=True,
-                 x_coordinate='X_centroid',y_coordinate='Y_centroid',
-                 point_size=10,imageid='imageid',subset=None,seg_mask=None,**kwargs):
+import anndata as ad
+import pandas as pd
+import argparse
+import sys
+import pathlib
+
+
+def main(argv=sys.argv):
+    parser = argparse.ArgumentParser(
+        description='The function allows users to directly import the output from mcmicro'
+    )
+    parser.add_argument(
+        '--feature_table_path', nargs='*', required=True, 
+        help='List of path to the single-cell feature tables. Each Image should have a unique path supplied.'
+    )
+    parser.add_argument(
+        '--remove_dna', action='store_true', required=False,  default=True,
+        help='Remove the DNA channels from the final output. Looks for channels with the string dna in it.'
+    )
+    parser.add_argument(
+        '--remove_string_from_name', type=str, required=False, default=None,
+        help='Used to celan up channel names. If a string is given, that particular string will be removed from all marker names. If multiple images are passed, just use the string that appears in the first image.'
+    )
+    parser.add_argument(
+        '--log', required=False, default=True,
+        help='Log the data (log1p transformation will be applied).'
+    )
+    parser.add_argument(
+        '--drop_markers', nargs='*', required=False, default=None,
+        help='List of markers to drop from the analysis. e.g. ["CD3D", "CD20"]'
+    )
+    parser.add_argument(
+        '--random_sample', type=int, required=False, default=None,
+        help='Randomly sub-sample the data with the desired number of cells.'
+    )
+    parser.add_argument(
+        '--unique_CellId', required=False, default=True,
+        help='By default, the function creates a unique name for each cell/row by combining the `CellId` and `imageid`. If you wish not to perform this operation please pass `False`. The function will use whatever is under `CellId`. In which case, please be careful to pass unique `CellId` especially when loading multiple datasets togeather.'
+    )
+    parser.add_argument(
+        '--CellId', type=str, required=False, default='CellID',
+        help='Name of the column that contains the cell ID.'
+    )
+    parser.add_argument(
+        '--split', type=str, required=False, default='X_centroid',
+        help='To split the CSV into counts table and meta data, pass in the name of the column that immediately follows the marker quantification.'
+    )
+    parser.add_argument( 
+        '--custom_imageid', type=str, required=False, default=None,
+        help='Pass a user defined Image ID. By default the name of the CSV file is used.'
+    )
+    parser.add_argument(
+        '--min_cells', type=int, required=False, default=None,
+        help='If these many cells are not in the image, the image will be dropped. Particulary useful when importing multiple images.'
+    )
+    parser.add_argument(
+        '--output_dir', type=str, required=False, default=None,
+        help='Path to output directory.'
+    )
+    args = parser.parse_args(argv[1:])
+    print(vars(args))
+    mcmicro_to_scimap(**vars(args))
+
+
+
+
+def mcmicro_to_scimap (feature_table_path,remove_dna=True,remove_string_from_name=None,
+                        log=True,drop_markers=None,random_sample=None, unique_CellId=True,
+                        CellId='CellID',split='X_centroid',custom_imageid=None,
+                        min_cells=None, output_dir=None):
     """
 Parameters:
-    image_path : string  
-        Location to the image file.
 
-    adata : Ann Data Object  
+    feature_table_path : list  
+        List of path to the single-cell spatial feature tables. Each Image should have a unique path supplied.
 
-    marker_of_interest : string  
-        Marker for which gate is to be defined e.g. 'CD45'.
+    remove_dna : bool, optional  
+        Remove the DNA channels from the final output. Looks for channels with the string 'dna' in it.
 
-    from_gate : int, optional  
-        Start value gate of interest.
+    remove_string_from_name : string, optional  
+        Used to celan up channel names. If a string is given, that particular string will be removed from all marker names.
+        If multiple images are passed, just use the string that appears in the first image.
 
-    to_gate : int, optional  
-        End value of the gate of interest.
-        
-    flip_y : bool, optional  
-        Flip the Y-axis if needed. Some algorithms output the XY with the Y-coordinates flipped.
-        If the image overlays do not align to the cells, try again by setting this to `False`.
+    log : bool, optional  
+        Log the data (log1p transformation will be applied).
 
-    increment : float, optional  
-        Increments between the start and end values.
+    drop_markers : list, optional  
+        List of markers to drop from the analysis. e.g. ["CD3D", "CD20"].
 
-    markers : string, optional  
-        Additional markers to be included in the plot for evaluation.
+    random_sample : int, optional  
+        Randomly sub-sample the data with the desired number of cells.
 
-    channel_names : list, optional  
-        List of channels in the image in the exact order as image. The default is `adata.uns['all_markers']`
+    CellId : string, optional  
+        Name of the column that contains the cell ID.
 
-    x_coordinate : string, optional  
-        X axis coordinate column name in AnnData object.
+    unique_CellId: bool, optional  
+        By default, the function creates a unique name for each cell/row by combining the 
+        `CellId` and `imageid`. If you wish not to perform this operation please pass `False`.
+        The function will use whatever is under `CellId`. In which case, please be careful to pass unique `CellId`
+        especially when loading multiple datasets togeather.  
 
-    y_coordinate : string, optional  
-        Y axis coordinate column name in AnnData object.
+    split : string, optional  
+        To split the CSV into counts table and meta data, pass in the name of the column
+        that immediately follows the marker quantification.
 
-    point_size : int, optional  
-        point size in the napari plot.
+    custom_imageid: string, optional  
+        Pass a user defined Image ID. By default the name of the CSV file is used.
 
-    imageid : string, optional  
-        Column name of the column containing the image id.
+    min_cells: int, optional  
+        If these many cells are not in the image, the image will be dropped.
+        Particulary useful when importing multiple images.
 
-    subset : string, optional  
-        imageid of a single image to be subsetted for analyis.
+    output_dir: string, optional  
+        Path to output directory. 
 
-    seg_mask : string, optional  
-        Location to the segmentation mask file.
+Returns:
+
+    AnnData Object
 
-    **kwargs  
-        Other arguments that can be passed to napari viewer.
 
 Example:
 ```python
-    image_path = '/Users/aj/Desktop/ptcl_tma/image.ome.tif'
-    sm.pl.gate_finder (image_path, adata, marker_of_interest='CD45',
-                 from_gate = 6, to_gate = 8, increment = 0.1,
-                 markers=['DNA10'], channel_names = 'default',
-                 x_coordinate='X_position',y_coordinate='Y_position',point_size=10,
-                 subset= '77', seg_mask=None)
+feature_table_path = ['/Users/aj/whole_sections/PTCL1_450.csv',
+                  '/Users/aj/whole_sections/PTCL2_552.csv']
+adata = sm.pp.mcmicro_to_scimap (feature_table_path, drop_markers= ['CD21', 'ACTIN'], random_sample=5000)
 ```
     """
+    
+    # feature_table_path list or string
+    if isinstance(feature_table_path, str):
+        feature_table_path = [feature_table_path]
+    feature_table_path = [pathlib.Path(p) for p in feature_table_path]
+
+    # Import data based on the location provided
+    def load_process_data (image):
+        # Print the data that is being processed
+        print(f"Loading {image.name}")
+        d = pd.read_csv(image)
+        # If the data does not have a unique image ID column, add one.
+        if 'imageid' not in d.columns:
+            if custom_imageid is not None:
+                imid = custom_imageid
+            else:
+                #imid = random.randint(1000000,9999999)
+                imid = image.stem
+            d['imageid'] = imid
+        # Unique name for the data
+        if unique_CellId is True:
+            d.index = d['imageid'].astype(str)+'_'+d[CellId].astype(str)
+        else:
+            d.index = d[CellId]
+            
+        # move image id and cellID column to end
+        cellid_col = [col for col in d.columns if col != CellId] + [CellId]; d = d[cellid_col]
+        imageid_col = [col for col in d.columns if col != 'imageid'] + ['imageid']; d = d[imageid_col]
+        # If there is INF replace with zero
+        d = d.replace([np.inf, -np.inf], 0)
+        # Return data
+        return d
+    # Apply function to all images and create a master dataframe
+    r_load_process_data = lambda x: load_process_data(image=x) # Create lamda function
+    all_data = list(map(r_load_process_data, list(feature_table_path))) # Apply function
+
+    # Merge all the data into a single large dataframe
+    for i in range(len(all_data)):
+        all_data[i].columns = all_data[0].columns
+    entire_data = pd.concat(all_data, axis=0, sort=False)
+    
+    # Randomly sample the data
+    if random_sample is not None:
+        entire_data = entire_data.sample(n=random_sample,replace=False)
+
+    #Remove the images that contain less than a defined threshold of cells (min_cells)
+    if min_cells is not None:
+        to_drop = entire_data['imageid'].value_counts()[entire_data['imageid'].value_counts() < min_cells].index
+        entire_data = entire_data[~entire_data['imageid'].isin(to_drop)]
+        print('Removed Images that contained less than '+str(min_cells)+' cells: '+ str(to_drop.values))
+
+    # Split the data into expression data and meta data
+    # Step-1 (Find the index of the column with name Area)
+    split_idx = entire_data.columns.get_loc(split)
+    meta = entire_data.iloc [:,split_idx:]
+    # Step-2 (select only the expression values)
+    entire_data = entire_data.iloc [:,:split_idx]
+
+    # Rename the columns of the data
+    if remove_string_from_name is not None:
+        entire_data.columns = entire_data.columns.str.replace(remove_string_from_name, '')
+
+    # Save a copy of the column names in the uns space of ANNDATA
+    markers = list(entire_data.columns)
+
+    # Remove DNA channels
+    if remove_dna is True:
+        entire_data = entire_data.loc[:,~entire_data.columns.str.contains('dna', case=False)]
+
+    # Drop unnecessary markers
+    if drop_markers is not None:
+        if isinstance(drop_markers, str):
+            drop_markers = [drop_markers]
+        entire_data = entire_data.drop(columns=drop_markers)
+
+    # Create an anndata object
+    adata = ad.AnnData(entire_data)
+    adata.obs = meta
+    adata.uns['all_markers'] = markers
 
-    # If no raw data is available make a copy
-    if adata.raw is None:
+    # Add log data
+    if log is True:
         adata.raw = adata
+        adata.X = np.log1p(adata.X)
 
-    # Copy of the raw data if it exisits
-    if adata.raw is not None:
-        adata.X = adata.raw.X
-
-    # Make a copy of the data with the marker of interest
-    data = pd.DataFrame(np.log1p(adata.X), columns = adata.var.index, index= adata.obs.index)[[marker_of_interest]]
-
-    # Generate a dataframe with various gates
-    def gate (g, d):
-        dd = d.values
-        dd = np.where(dd < g, np.nan, dd)
-        np.warnings.filterwarnings('ignore')
-        dd = np.where(dd > g, 1, dd)
-        dd = pd.DataFrame(dd, index = d.index, columns = ['gate-' + str(g)])
-        return dd
-
-    # Identify the list of increments
-    inc = list(np.arange (from_gate, to_gate, increment))
-    inc = [round(num,3) for num in inc]
-
-    # Apply the function
-    r_gate = lambda x: gate(g=x, d=data) # Create lamda function
-    gated_data = list(map(r_gate, inc)) # Apply function
-    # Concat all the results into a single dataframe
-    gates = pd.concat(gated_data, axis=1)
-    
-    # Plot only the Image that is requested
-    if subset is not None:
-        adata = adata[adata.obs[imageid] == subset]
-        
-    # Recover the channel names from adata
-    if channel_names == 'default':
-        channel_names = adata.uns['all_markers']
-    else:
-        channel_names = channel_names
-
-    # if markers is a string convert to list
-    if isinstance(markers, str):
-        markers = [markers]
-        
-    # Index of the marker of interest and corresponding names
-    if markers is not None:
-        markers.extend([marker_of_interest])
-        idx = np.where(np.isin(channel_names,markers))[0]
-        channel_names = [channel_names[i] for i in idx]
-    else:
-        idx = list(range(len(channel_names)))
-        channel_names = channel_names
-
-
-    # Load the segmentation mask
-    if seg_mask is not None:
-        seg_m = tiff.imread(seg_mask)
-        if (len(seg_m.shape) > 2) and (seg_m.shape[0] > 1):
-            seg_m = seg_m[0]
-        
+    # Save data if requested
+    if output_dir is not None:
+        output_dir = pathlib.Path(output_dir)
+        output_dir.mkdir(exist_ok=True, parents=True)
+        imid = feature_table_path[0].stem
+        adata.write(output_dir / f'{imid}.h5ad')
+        #adata.write(str(output_dir) + '/' + imid + '.h5ad')
+    else:    
+        # Return data
+        return adata
 
-    ##########################################################################
-    # Visulaisation using Napari
-    
-    # load OME TIFF
-    if os.path.isfile(image_path) is True: 
-        # Load the image    
-        image = tiff.TiffFile(image_path, is_ome=False)
-        z = zarr.open(image.aszarr(), mode='r') # convert image to Zarr array
-        # Identify the number of pyramids and number of channels
-        n_levels = len(image.series[0].levels) # pyramid  
-        # If and if not pyramids are available
-        if n_levels > 1:
-            pyramid = [da.from_zarr(z[i]) for i in range(n_levels)]
-            multiscale = True
-        else:
-            pyramid = da.from_zarr(z)
-            multiscale = False   
-        # subset channels of interest
-        if markers is not None:
-            if n_levels > 1:
-                for i in range(n_levels-1):
-                    pyramid[i] = pyramid[i][idx, :, :]
-                n_channels = pyramid[0].shape[0] # identify the number of channels
-            else:
-                pyramid = pyramid[idx, :, :]
-                n_channels = pyramid.shape[0] # identify the number of channels
-        else:
-            if n_levels > 1:
-                n_channels = pyramid[0].shape[0]
-            else:
-                n_channels = pyramid.shape[0]\
-        # check if channel names have been passed to all channels
-        if channel_names is not None:
-            assert n_channels == len(channel_names), (
-                f'number of channel names ({len(channel_names)}) must '
-                f'match number of channels ({n_channels})'
-            )
-
-        # Load the viewer
-        viewer = napari.view_image(
-        pyramid,
-        channel_axis = 0,
-        multiscale=multiscale,
-        name = None if channel_names is None else channel_names,
-        visible = False, **kwargs)
-
-
-    # Operations on the ZARR image
-    # check the format of image
-    if os.path.isfile(image_path) is False: 
-        #print(image_path)
-        viewer = napari.Viewer()
-        viewer.open(image_path, multiscale=True,
-                    visible=False,
-                    name = None if channel_names is None else channel_names)
-
-    # Add the seg mask
-    if seg_mask is not None:
-        viewer.add_labels(seg_m, name='segmentation mask', visible=False)
-
-    # subset the gates to include only the image of interest
-    gates = gates.loc[adata.obs.index,]
-
-    # Add gating layer
-    def add_phenotype_layer (adata, gates, phenotype_layer,x,y,viewer,point_size):
-        cells = gates[gates[phenotype_layer] == 1].index
-        coordinates = adata[cells]
-        # Flip Y axis if needed
-        if flip_y is True:
-            coordinates = pd.DataFrame({'y': coordinates.obs[y],'x': coordinates.obs[x]})
-        else:  
-            coordinates = pd.DataFrame({'x': coordinates.obs[x],'y': coordinates.obs[y]})
-        #points = coordinates.values.tolist()
-        points = coordinates.values
-        #import time
-        #start = time.time()
-        viewer.add_points(points, size=point_size, face_color='white',visible=False,name=phenotype_layer)
-        #stop = time.time()
-        #print(stop-start)
-        
-
-    # Run the function on all gating layer
-    for i in gates.columns:
-        add_phenotype_layer (adata=adata, gates=gates, 
-                             phenotype_layer=i, x=x_coordinate, y=y_coordinate, 
-                             viewer=viewer, point_size=point_size)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `scimap-1.2.0/scimap/plotting/_image_viewer.py` & `scimap-1.3.0/scimap/plotting/_image_viewer.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_pie.py` & `scimap-1.3.0/scimap/plotting/_pie.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_spatial_distance.py` & `scimap-1.3.0/scimap/plotting/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_spatial_interaction.py` & `scimap-1.3.0/scimap/plotting/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_spatial_pscore.py` & `scimap-1.3.0/scimap/plotting/_spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_spatial_scatter.py` & `scimap-1.3.0/scimap/plotting/_spatial_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_stacked_barplot.py` & `scimap-1.3.0/scimap/plotting/_stacked_barplot.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_umap.py` & `scimap-1.3.0/scimap/plotting/_umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/_voronoi.py` & `scimap-1.3.0/scimap/plotting/_voronoi.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/plotting/densityPlot2D.py` & `scimap-1.3.0/scimap/plotting/densityPlot2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from matplotlib import cm
 from matplotlib.colors import LogNorm
 mpl.rcParams['pdf.fonttype'] = 42
 
 
 def densityPlot2D (adata, 
                    markerA,  markerB=None, 
-                   layers=None, 
+                   layer=None, 
                    subset=None, 
                    imageid='imageid', 
                    ncols=None, 
                    cmap='jet', 
                    figsize=(3, 3), 
                    hline = 'auto', vline = 'auto',
                    fontsize=None, 
@@ -49,15 +49,15 @@
     markerA (str): 
         The name of the first marker whose expression will be plotted.
 
     markerB (list, optional): 
         The name of the second marker or a list of second markers whose expression will be plotted. 
         If not provided, a 2D density plot of `markerA` against all markers in the dataset will be plotted.
 
-    layers (str or list of str, optional): 
+    layer (str or list of str, optional): 
         The layer in adata.layers that contains the expression data to use. 
         If None, adata.X is used. use `raw` to use the data stored in `adata.raw.X`
 
     subset (list, optional):  
         `imageid` of a single or multiple images to be subsetted for plotting purposes.
 
     imageid (str, optional):  
@@ -69,18 +69,20 @@
     cmap (str, optional):  
         The name of the colormap to use. Defaults to 'jet'.
 
     figsize (tuple, optional):  
         The size of the figure in inches.
 
     hline (float or 'auto', optional):  
-        The y-coordinate of the horizontal line to plot. If set to `None`, a horizontal line is not plotted.
+        The y-coordinate of the horizontal line to plot. If set to `None`, a horizontal line is not plotted. 
+        Use 'auto' to draw a vline at the center point. 
 
     vline (float or 'auto', optional):  
-        The x-coordinate of the vertical line to plot. If set to `None`, a vertical line is not plotted.
+        The x-coordinate of the vertical line to plot. If set to `None`, a vertical line is not plotted. 
+        Use 'auto' to draw a vline at the center point. 
 
     fontsize (int, optional):  
         The size of the font of the axis labels.
 
     dpi (int, optional):  
         The DPI of the figure. Use this to control the point size. Lower the dpi, larger the point size.
 
@@ -128,33 +130,31 @@
     cp = copy.copy(cm.get_cmap(cmap))
     cp.set_under(alpha=0)
     
     # subset data if neede
     if subset is not None:
         if isinstance (subset, str):
             subset = [subset]
-        if layers == 'raw':
+        if layer == 'raw':
             bdata=adata.copy()
             bdata.X = adata.raw.X
             bdata = bdata[bdata.obs[imageid].isin(subset)]
         else:
             bdata=adata.copy()
             bdata = bdata[bdata.obs[imageid].isin(subset)]
     else:
         bdata=adata.copy()
               
     # isolate the data
-    if layers is None:
+    if layer is None:
         data = pd.DataFrame(bdata.X, index=bdata.obs.index, columns=bdata.var.index)
-    elif layers == 'raw':
+    elif layer == 'raw':
         data = pd.DataFrame(bdata.raw.X, index=bdata.obs.index, columns=bdata.var.index)
     else:
-        data = pd.DataFrame(
-            bdata.layers[layers], index=bdata.obs.index, columns=bdata.var.index
-        )
+        data = pd.DataFrame(bdata.layers[layer], index=bdata.obs.index, columns=bdata.var.index)
     
     # keep only columns that are required
     x = data[markerA]
     
     if markerB is None:
         y = data.drop(markerA, axis=1)
     else:
```

### Comparing `scimap-1.2.0/scimap/plotting/lasso_selector.py` & `scimap-1.3.0/scimap/plotting/lasso_selector.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/preprocessing/_combat.py` & `scimap-1.3.0/scimap/preprocessing/_combat.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/preprocessing/_rescale.py` & `scimap-1.3.0/scimap/preprocessing/_rescale.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tests/_data/example_data.csv` & `scimap-1.3.0/scimap/tests/_data/example_data.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tests/_data/example_data.h5ad` & `scimap-1.3.0/scimap/tests/_data/example_data.h5ad`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tests/_data/phenotype_workflow.csv` & `scimap-1.3.0/scimap/tests/_data/phenotype_workflow.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tests/test_helpers.py` & `scimap-1.3.0/scimap/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tests/test_preprocessing.py` & `scimap-1.3.0/scimap/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tests/test_tools.py` & `scimap-1.3.0/scimap/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/__init__.py` & `scimap-1.3.0/scimap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_cluster.py` & `scimap-1.3.0/scimap/tools/_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_foldchange.py` & `scimap-1.3.0/scimap/tools/_foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_phenotype_cells.py` & `scimap-1.3.0/scimap/tools/_phenotype_cells.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_spatial_aggregate.py` & `scimap-1.3.0/scimap/tools/_spatial_aggregate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_spatial_cluster.py` & `scimap-1.3.0/scimap/tools/_spatial_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_spatial_count.py` & `scimap-1.3.0/scimap/tools/_spatial_count.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_spatial_distance.py` & `scimap-1.3.0/scimap/tools/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_spatial_expression.py` & `scimap-1.3.0/scimap/tools/_spatial_expression.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_spatial_interaction.py` & `scimap-1.3.0/scimap/tools/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_spatial_lda.py` & `scimap-1.3.0/scimap/tools/_spatial_lda.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_spatial_pscore.py` & `scimap-1.3.0/scimap/tools/_spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_spatial_similarity_search.py` & `scimap-1.3.0/scimap/tools/_spatial_similarity_search.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/scimap/tools/_umap.py` & `scimap-1.3.0/scimap/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.2.0/PKG-INFO` & `scimap-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scimap
-Version: 1.2.0
+Version: 1.3.0
 Summary: Spatial Single-Cell Analysis Toolkit
 Home-page: https://pypi.org/project/scimap/
 License: MIT
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.7,<3.11
```

