# Comparing `tmp/swachhdata-1.5.1a1-py3-none-any.whl.zip` & `tmp/swachhdata-1.5.2a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 26488 bytes, number of entries: 20
--rw-r--r--  2.0 unx      227 b- defN 23-May-21 04:10 swachhdata/__init__.py
--rw-r--r--  2.0 unx       66 b- defN 23-May-21 03:53 swachhdata/compose/__init__.py
--rw-r--r--  2.0 unx      937 b- defN 23-May-21 03:52 swachhdata/compose/core.py
+Zip file size: 26557 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      227 b- defN 23-May-21 04:19 swachhdata/__init__.py
+-rw-r--r--  2.0 unx      106 b- defN 23-May-21 04:19 swachhdata/compose/__init__.py
+-rw-r--r--  2.0 unx     1140 b- defN 23-May-21 04:19 swachhdata/compose/core.py
 -rw-r--r--  2.0 unx      131 b- defN 22-Jan-25 09:02 swachhdata/image/__init__.py
 -rw-r--r--  2.0 unx     7477 b- defN 22-Jan-25 09:02 swachhdata/image/_image.py
 -rw-r--r--  2.0 unx      173 b- defN 22-Jan-25 09:02 swachhdata/legacy/__init__.py
 -rw-r--r--  2.0 unx    15947 b- defN 23-Mar-10 23:37 swachhdata/legacy/_text.py
 -rw-r--r--  2.0 unx     1013 b- defN 23-Mar-10 23:36 swachhdata/text/__init__.py
 -rw-r--r--  2.0 unx     1058 b- defN 23-Mar-10 23:37 swachhdata/text/_base.py
 -rw-r--r--  2.0 unx   105336 b- defN 23-Mar-10 23:38 swachhdata/text/_text.py
 -rw-r--r--  2.0 unx      642 b- defN 23-May-21 03:53 swachhdata/utils/__init__.py
 -rw-r--r--  2.0 unx      377 b- defN 23-May-21 03:02 swachhdata/utils/probe.py
 -rw-r--r--  2.0 unx     1149 b- defN 23-May-21 03:50 swachhdata/utils/recast.py
 -rw-r--r--  2.0 unx      480 b- defN 23-May-21 03:06 swachhdata/utils/tools.py
 -rw-r--r--  2.0 unx     1309 b- defN 23-May-21 04:10 swachhdata/utils/verify.py
--rw-rw-rw-  2.0 unx    17096 b- defN 23-May-21 04:10 swachhdata-1.5.1a1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2272 b- defN 23-May-21 04:10 swachhdata-1.5.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-21 04:10 swachhdata-1.5.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-21 04:10 swachhdata-1.5.1a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1657 b- defN 23-May-21 04:10 swachhdata-1.5.1a1.dist-info/RECORD
-20 files, 157450 bytes uncompressed, 23786 bytes compressed:  84.9%
+-rw-rw-rw-  2.0 unx    17096 b- defN 23-May-21 04:20 swachhdata-1.5.2a1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2272 b- defN 23-May-21 04:20 swachhdata-1.5.2a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 04:20 swachhdata-1.5.2a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-21 04:20 swachhdata-1.5.2a1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1659 b- defN 23-May-21 04:20 swachhdata-1.5.2a1.dist-info/RECORD
+20 files, 157695 bytes uncompressed, 23855 bytes compressed:  84.9%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: swachhdata/utils/tools.py
 Comment: 
 
 Filename: swachhdata/utils/verify.py
 Comment: 
 
-Filename: swachhdata-1.5.1a1.dist-info/LICENSE.txt
+Filename: swachhdata-1.5.2a1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: swachhdata-1.5.1a1.dist-info/METADATA
+Filename: swachhdata-1.5.2a1.dist-info/METADATA
 Comment: 
 
-Filename: swachhdata-1.5.1a1.dist-info/WHEEL
+Filename: swachhdata-1.5.2a1.dist-info/WHEEL
 Comment: 
 
-Filename: swachhdata-1.5.1a1.dist-info/top_level.txt
+Filename: swachhdata-1.5.2a1.dist-info/top_level.txt
 Comment: 
 
-Filename: swachhdata-1.5.1a1.dist-info/RECORD
+Filename: swachhdata-1.5.2a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swachhdata/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = '1.5.1a1'
+__version__ = '1.5.2a1'
 __author__ = 'Kritik Seth'
 __maintainer__ = __author__
 __license__ = 'Mozilla Public License Version 2.0'
 __url__ = 'https://swachhdata.readthedocs.io/'
 __connect__ = 'https://www.kritikseth.com/'
```

## swachhdata/compose/__init__.py

```diff
@@ -1,7 +1,9 @@
 from .core import (
+    BaseTextDatum,
     TextDatum
 )
 
 __all__ = [
+    'BaseTextDatum',
     'TextDatum'
 ]
```

## swachhdata/compose/core.py

```diff
@@ -7,15 +7,15 @@
     fetch_num_rows
 )
 
 from ..utils.probe import (
     probe_string_data
 )
 
-class TextDatum:
+class BaseTextDatum:
 
     """
     Data formatter, converts heterogenous text data types to homogenous list of string(s).
 
     Parameters
     ----------
     data / X : pandas.core.frame.DataFrame / pandas.core.series.Series / numpy.ndarray
@@ -38,8 +38,17 @@
         return self.__data
 
     @data.setter
     def data(self, text):
         self.__data = probe_string_data(text)
     
     def recast(self):
-        self.__data = probe_string_data(self.__data)
+        self.__data = probe_string_data(self.__data)
+
+class TextDatum(BaseTextDatum):
+
+    def __init__(self, text):
+        super().__init__(text)
+    
+    def __add__(self, other):
+        data = self.data + other.data
+        return TextDatum(data)
```

## Comparing `swachhdata-1.5.1a1.dist-info/LICENSE.txt` & `swachhdata-1.5.2a1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `swachhdata-1.5.1a1.dist-info/METADATA` & `swachhdata-1.5.2a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swachhdata
-Version: 1.5.1a1
+Version: 1.5.2a1
 Summary: Data cleaning made easy with swachhdata
 Home-page: https://swachhdata.readthedocs.io/
 Author: Kritik Seth
 Author-email: sethkritik@gmail.com
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swachhdata Version: 1.5.1a1 Summary: Data cleaning
+Metadata-Version: 2.1 Name: swachhdata Version: 1.5.2a1 Summary: Data cleaning
 made easy with swachhdata Home-page: https://swachhdata.readthedocs.io/ Author:
 Kritik Seth Author-email: sethkritik@gmail.com Classifier: Natural Language ::
 English Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL
 2.0) Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 6 - Mature Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: regex (>=2019.12.20) Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: tqdm (>=4.41.1) Requires-Dist: beautifulsoup4 (>=4.6.3)
```

