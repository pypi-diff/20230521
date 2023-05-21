# Comparing `tmp/Orange3-Tools-0.0.5.tar.gz` & `tmp/Orange3-Tools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-Tools-0.0.5.tar", last modified: Sun May 21 09:28:59 2023, max compression
+gzip compressed data, was "Orange3-Tools-0.0.7.tar", last modified: Sun May 21 19:38:21 2023, max compression
```

## Comparing `Orange3-Tools-0.0.5.tar` & `Orange3-Tools-0.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.017232 Orange3-Tools-0.0.5/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)    35801 2023-03-07 11:54:58.000000 Orange3-Tools-0.0.5/LICENSE
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.010184 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/
--rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/PKG-INFO
--rw-r--r--   0 julioj.melero   (501) staff       (20)     1092 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)       98 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/entry_points.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-17 10:38:08.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/not-zip-safe
--rw-r--r--   0 julioj.melero   (501) staff       (20)      200 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/requires.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)       14 2023-05-21 09:28:58.000000 Orange3-Tools-0.0.5/Orange3_Tools.egg-info/top_level.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-21 09:28:59.017091 Orange3-Tools-0.0.5/PKG-INFO
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      100 2023-04-13 16:55:45.000000 Orange3-Tools-0.0.5/README.md
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.010615 Orange3-Tools-0.0.5/orangecontrib/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      169 2023-04-11 17:27:18.000000 Orange3-Tools-0.0.5/orangecontrib/__init__.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)    20713 2023-05-18 08:25:22.000000 Orange3-Tools-0.0.5/orangecontrib/functions.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.010983 Orange3-Tools-0.0.5/orangecontrib/tools/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      654 2023-04-11 19:26:01.000000 Orange3-Tools-0.0.5/orangecontrib/tools/__init__.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.013987 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     6713 2023-04-16 09:22:31.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/MySqlOrange.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     9754 2023-04-16 15:10:09.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/Pairsplot.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     7281 2023-04-16 09:57:24.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/Scatterplot.py
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     1091 2023-04-13 17:01:11.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/__init__.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 09:28:59.016785 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/
--rw-r--r--   0 julioj.melero   (501) staff       (20)    14469 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/ARIMA.svg
--rw-------   0 julioj.melero   (501) staff       (20)     1513 2023-04-16 09:12:55.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Barchart.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     9756 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Correlogram.svg
--rw-------   0 julioj.melero   (501) staff       (20)    15156 2023-04-16 09:04:28.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Pairs.svg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     5586 2023-04-11 16:37:34.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)    10454 2023-04-16 09:14:11.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/category.svg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3595 2023-03-08 12:27:13.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/mysql-orange.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     4964 2023-04-11 17:00:16.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/sscater.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     5418 2023-05-21 09:26:14.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owcorrelogram.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)    30238 2023-05-19 17:23:52.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owsarima.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     9733 2023-05-20 11:28:08.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owstationarity.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     2212 2023-04-13 16:39:56.000000 Orange3-Tools-0.0.5/orangecontrib/tools/widgets/utils.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)       38 2023-05-21 09:28:59.017277 Orange3-Tools-0.0.5/setup.cfg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3576 2023-05-21 09:28:46.000000 Orange3-Tools-0.0.5/setup.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 19:38:21.185778 Orange3-Tools-0.0.7/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)    35801 2023-03-07 11:54:58.000000 Orange3-Tools-0.0.7/LICENSE
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 19:38:21.180830 Orange3-Tools-0.0.7/Orange3_Tools.egg-info/
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-21 19:38:21.000000 Orange3-Tools-0.0.7/Orange3_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     1092 2023-05-21 19:38:21.000000 Orange3-Tools-0.0.7/Orange3_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-21 19:38:21.000000 Orange3-Tools-0.0.7/Orange3_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       98 2023-05-21 19:38:21.000000 Orange3-Tools-0.0.7/Orange3_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-17 10:38:08.000000 Orange3-Tools-0.0.7/Orange3_Tools.egg-info/not-zip-safe
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      200 2023-05-21 19:38:21.000000 Orange3-Tools-0.0.7/Orange3_Tools.egg-info/requires.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       14 2023-05-21 19:38:21.000000 Orange3-Tools-0.0.7/Orange3_Tools.egg-info/top_level.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-21 19:38:21.185656 Orange3-Tools-0.0.7/PKG-INFO
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      100 2023-04-13 16:55:45.000000 Orange3-Tools-0.0.7/README.md
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 19:38:21.181163 Orange3-Tools-0.0.7/orangecontrib/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      169 2023-04-11 17:27:18.000000 Orange3-Tools-0.0.7/orangecontrib/__init__.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    20713 2023-05-18 08:25:22.000000 Orange3-Tools-0.0.7/orangecontrib/functions.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 19:38:21.181542 Orange3-Tools-0.0.7/orangecontrib/tools/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      654 2023-04-11 19:26:01.000000 Orange3-Tools-0.0.7/orangecontrib/tools/__init__.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 19:38:21.183483 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     6713 2023-04-16 09:22:31.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/MySqlOrange.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9754 2023-04-16 15:10:09.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/Pairsplot.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     7281 2023-04-16 09:57:24.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/Scatterplot.py
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     1091 2023-04-13 17:01:11.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/__init__.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-21 19:38:21.185377 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    14469 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/ARIMA.svg
+-rw-------   0 julioj.melero   (501) staff       (20)     1513 2023-04-16 09:12:55.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/Barchart.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9756 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/Correlogram.svg
+-rw-------   0 julioj.melero   (501) staff       (20)    15156 2023-04-16 09:04:28.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/Pairs.svg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     5586 2023-04-11 16:37:34.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    10454 2023-04-16 09:14:11.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/category.svg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3595 2023-03-08 12:27:13.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/mysql-orange.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     4964 2023-04-11 17:00:16.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/sscater.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     5418 2023-05-21 09:26:14.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/owcorrelogram.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     5010 2023-05-21 18:13:55.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/owsarima.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9735 2023-05-21 18:28:42.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/owstationarity.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     2212 2023-04-13 16:39:56.000000 Orange3-Tools-0.0.7/orangecontrib/tools/widgets/utils.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       38 2023-05-21 19:38:21.185819 Orange3-Tools-0.0.7/setup.cfg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3576 2023-05-21 19:38:12.000000 Orange3-Tools-0.0.7/setup.py
```

### Comparing `Orange3-Tools-0.0.5/LICENSE` & `Orange3-Tools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/Orange3_Tools.egg-info/SOURCES.txt` & `Orange3-Tools-0.0.7/Orange3_Tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/functions.py` & `Orange3-Tools-0.0.7/orangecontrib/functions.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/__init__.py` & `Orange3-Tools-0.0.7/orangecontrib/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/MySqlOrange.py` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/MySqlOrange.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/Pairsplot.py` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/Pairsplot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/Scatterplot.py` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/Scatterplot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/__init__.py` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/ARIMA.svg` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/ARIMA.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Barchart.svg` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/Barchart.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Correlogram.svg` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/Correlogram.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Pairs.svg` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/Pairs.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/category.svg` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/category.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/mysql-orange.svg` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/mysql-orange.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/icons/sscater.svg` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/icons/sscater.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owcorrelogram.py` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/owcorrelogram.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/owstationarity.py` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/owstationarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                 val=round(value,2)
             else:
                 val=round(value,3)
             tmp_result[label]=str(val)
         for key in result[4]:
             key1 = "Critical Value ({0})".format(key)
             tmp_result[key1] = str(round(result[4][key],3))
-        if ((result[0] < result[4]["5%"])&(result[1]<0.05)):
+        if ((result[0] < result[4]["5%"])&(result[1]<=0.05)):
             tmp_result['<font color=\'green\' > Reject Ho </font>']="<font color=\'green\' >Time Series is Stationary</font>"
         else:
             tmp_result['<font color=\'red\' > Failed to Reject Ho </font>']="<font color=\"red\" > Time Series is Non-Stationary</font>"
         return tmp_result
 
     def kpss_test(self,data):
         tmp_result={}
@@ -149,15 +149,15 @@
                 val=round(value,2)
             else:
                 val=round(value,3)
             tmp_result[label]=str(round(value,3))
         for key in result[3]:
             key1 = "Critical Value ({0})".format(key)
             tmp_result[key1] = str(result[3][key])
-        if ((result[0] < result[3]["5%"])&(result[1]<0.05)):
+        if ((result[0] < result[3]["5%"])&(result[1]<=0.05)):
             tmp_result['<font color=\'green\'> Reject Ho </font>']="<font color=\'green\' > Time Series is Stationary</font>"
         else:
             tmp_result['<font color=\'red\' > Failed to Reject Ho </font>']="<font color=\"red\" > Time Series is Non-Stationary</font>"
         return tmp_result
 
 
     def init_model(self):
```

### Comparing `Orange3-Tools-0.0.5/orangecontrib/tools/widgets/utils.py` & `Orange3-Tools-0.0.7/orangecontrib/tools/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.5/setup.py` & `Orange3-Tools-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from os import path, walk
 from setuptools import setup, find_packages
 from setuptools.dist import Distribution
 
 NAME = "Orange3-Tools"
 
-VERSION = "0.0.5"
+VERSION = "0.0.7"
 
 DESCRIPTION = "Tools para Asignatura Big Data Master EERR"
 LONG_DESCRIPTION = ""
 
 LICENSE = "GPL-3.0"
 
 KEYWORDS = (
```

