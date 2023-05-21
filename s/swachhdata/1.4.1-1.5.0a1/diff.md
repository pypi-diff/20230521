# Comparing `tmp/swachhdata-1.4.1-py3-none-any.whl.zip` & `tmp/swachhdata-1.5.0a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,22 @@
-Zip file size: 23495 bytes, number of entries: 13
--rw-r--r--  2.0 unx      225 b- defN 23-Mar-11 04:04 swachhdata/__init__.py
+Zip file size: 26485 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      227 b- defN 23-May-21 03:55 swachhdata/__init__.py
+-rw-r--r--  2.0 unx       66 b- defN 23-May-21 03:53 swachhdata/compose/__init__.py
+-rw-r--r--  2.0 unx      937 b- defN 23-May-21 03:52 swachhdata/compose/core.py
 -rw-r--r--  2.0 unx      131 b- defN 22-Jan-25 09:02 swachhdata/image/__init__.py
 -rw-r--r--  2.0 unx     7477 b- defN 22-Jan-25 09:02 swachhdata/image/_image.py
 -rw-r--r--  2.0 unx      173 b- defN 22-Jan-25 09:02 swachhdata/legacy/__init__.py
 -rw-r--r--  2.0 unx    15947 b- defN 23-Mar-10 23:37 swachhdata/legacy/_text.py
 -rw-r--r--  2.0 unx     1013 b- defN 23-Mar-10 23:36 swachhdata/text/__init__.py
 -rw-r--r--  2.0 unx     1058 b- defN 23-Mar-10 23:37 swachhdata/text/_base.py
 -rw-r--r--  2.0 unx   105336 b- defN 23-Mar-10 23:38 swachhdata/text/_text.py
--rw-rw-rw-  2.0 unx    17096 b- defN 23-Mar-11 06:10 swachhdata-1.4.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2307 b- defN 23-Mar-11 06:10 swachhdata-1.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-11 06:10 swachhdata-1.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-11 06:10 swachhdata-1.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1068 b- defN 23-Mar-11 06:10 swachhdata-1.4.1.dist-info/RECORD
-13 files, 151934 bytes uncompressed, 21717 bytes compressed:  85.7%
+-rw-r--r--  2.0 unx      642 b- defN 23-May-21 03:53 swachhdata/utils/__init__.py
+-rw-r--r--  2.0 unx      377 b- defN 23-May-21 03:02 swachhdata/utils/probe.py
+-rw-r--r--  2.0 unx     1149 b- defN 23-May-21 03:50 swachhdata/utils/recast.py
+-rw-r--r--  2.0 unx      480 b- defN 23-May-21 03:06 swachhdata/utils/tools.py
+-rw-r--r--  2.0 unx     1309 b- defN 23-May-21 03:40 swachhdata/utils/verify.py
+-rw-rw-rw-  2.0 unx    17096 b- defN 23-May-21 04:05 swachhdata-1.5.0a1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2272 b- defN 23-May-21 04:05 swachhdata-1.5.0a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 04:05 swachhdata-1.5.0a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-21 04:05 swachhdata-1.5.0a1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1657 b- defN 23-May-21 04:05 swachhdata-1.5.0a1.dist-info/RECORD
+20 files, 157450 bytes uncompressed, 23783 bytes compressed:  84.9%
```

## zipnote {}

```diff
@@ -1,10 +1,16 @@
 Filename: swachhdata/__init__.py
 Comment: 
 
+Filename: swachhdata/compose/__init__.py
+Comment: 
+
+Filename: swachhdata/compose/core.py
+Comment: 
+
 Filename: swachhdata/image/__init__.py
 Comment: 
 
 Filename: swachhdata/image/_image.py
 Comment: 
 
 Filename: swachhdata/legacy/__init__.py
@@ -18,23 +24,38 @@
 
 Filename: swachhdata/text/_base.py
 Comment: 
 
 Filename: swachhdata/text/_text.py
 Comment: 
 
-Filename: swachhdata-1.4.1.dist-info/LICENSE.txt
+Filename: swachhdata/utils/__init__.py
+Comment: 
+
+Filename: swachhdata/utils/probe.py
+Comment: 
+
+Filename: swachhdata/utils/recast.py
+Comment: 
+
+Filename: swachhdata/utils/tools.py
+Comment: 
+
+Filename: swachhdata/utils/verify.py
+Comment: 
+
+Filename: swachhdata-1.5.0a1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: swachhdata-1.4.1.dist-info/METADATA
+Filename: swachhdata-1.5.0a1.dist-info/METADATA
 Comment: 
 
-Filename: swachhdata-1.4.1.dist-info/WHEEL
+Filename: swachhdata-1.5.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: swachhdata-1.4.1.dist-info/top_level.txt
+Filename: swachhdata-1.5.0a1.dist-info/top_level.txt
 Comment: 
 
-Filename: swachhdata-1.4.1.dist-info/RECORD
+Filename: swachhdata-1.5.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swachhdata/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = '1.4.1'
+__version__ = '1.5.0a1'
 __author__ = 'Kritik Seth'
 __maintainer__ = __author__
 __license__ = 'Mozilla Public License Version 2.0'
 __url__ = 'https://swachhdata.readthedocs.io/'
 __connect__ = 'https://www.kritikseth.com/'
```

## Comparing `swachhdata-1.4.1.dist-info/LICENSE.txt` & `swachhdata-1.5.0a1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `swachhdata-1.4.1.dist-info/METADATA` & `swachhdata-1.5.0a1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swachhdata
-Version: 1.4.1
+Version: 1.5.0a1
 Summary: Data cleaning made easy with swachhdata
 Home-page: https://swachhdata.readthedocs.io/
 Author: Kritik Seth
 Author-email: sethkritik@gmail.com
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 
 ![](https://raw.githubusercontent.com/swachhdata/swachhdata/main/logo/sd-cover.png)
 
 # swachhdata
 
 [![pypi package](https://badge.fury.io/py/swachhdata.svg)](https://pypi.org/project/swachhdata)
 [![Downloads](https://static.pepy.tech/personalized-badge/swachhdata?period=total&units=international_system&left_color=gray&right_color=blue&left_text=Downloads)](https://pepy.tech/project/swachhdata)
-[![GitHub last commit](https://img.shields.io/github/last-commit/kritikseth/swachhdata.svg)](https://github.com/swachhdata/swachhdata/)
+![GitHub last commit](https://img.shields.io/github/last-commit/swachhdata/swachhdata?color=green)
 [![GitHub](https://img.shields.io/github/license/kritikseth/swachhdata.svg)](https://github.com/kritikseth/swachhdata/blob/master/LICENSE)
 
 * Simple and efficient tools for cleaning and transforming data
 * Accessible to everybody, and reusable in various contexts
 * Open source, commercially usable - MPL-2.0 license
 
 ## Documentation-
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swachhdata Version: 1.4.1 Summary: Data cleaning
+Metadata-Version: 2.1 Name: swachhdata Version: 1.5.0a1 Summary: Data cleaning
 made easy with swachhdata Home-page: https://swachhdata.readthedocs.io/ Author:
 Kritik Seth Author-email: sethkritik@gmail.com Classifier: Natural Language ::
 English Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL
 2.0) Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 6 - Mature Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: regex (>=2019.12.20) Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: tqdm (>=4.41.1) Requires-Dist: beautifulsoup4 (>=4.6.3)
@@ -12,19 +12,18 @@
 (>=0.15.3) Requires-Dist: requests (>=2.23.0) Requires-Dist: opencv-python
 (>=4.1.2.30) Requires-Dist: tweepy (>=3.6.0) ![](https://
 raw.githubusercontent.com/swachhdata/swachhdata/main/logo/sd-cover.png) #
 swachhdata [![pypi package](https://badge.fury.io/py/swachhdata.svg)](https://
 pypi.org/project/swachhdata) [![Downloads](https://static.pepy.tech/
 personalized-badge/
 swachhdata?period=total&units=international_system&left_color=gray&right_color=blue&left_text=Downloads)]
-(https://pepy.tech/project/swachhdata) [![GitHub last commit](https://
-img.shields.io/github/last-commit/kritikseth/swachhdata.svg)](https://
-github.com/swachhdata/swachhdata/) [![GitHub](https://img.shields.io/github/
-license/kritikseth/swachhdata.svg)](https://github.com/kritikseth/swachhdata/
-blob/master/LICENSE) * Simple and efficient tools for cleaning and transforming
-data * Accessible to everybody, and reusable in various contexts * Open source,
-commercially usable - MPL-2.0 license ## Documentation- * https://
-swachhdata.readthedocs.io/en/latest/ * [Examples](https://
-colab.research.google.com/drive/
+(https://pepy.tech/project/swachhdata) ![GitHub last commit](https://
+img.shields.io/github/last-commit/swachhdata/swachhdata?color=green) [![GitHub]
+(https://img.shields.io/github/license/kritikseth/swachhdata.svg)](https://
+github.com/kritikseth/swachhdata/blob/master/LICENSE) * Simple and efficient
+tools for cleaning and transforming data * Accessible to everybody, and
+reusable in various contexts * Open source, commercially usable - MPL-2.0
+license ## Documentation- * https://swachhdata.readthedocs.io/en/latest/ *
+[Examples](https://colab.research.google.com/drive/
 1IH7ve5xoQ4vLyrRP4HvTCYBlj1Ub1GGS?usp=sharing#scrollTo=3Seymy37xQk4) ## Author-
 [Kritik_Seth]
    [https://visitor-badge.glitch.me/badge?page_id=swachhdata.visitor-badge]
```

