# Comparing `tmp/swachhdata-1.5.0a1-py3-none-any.whl.zip` & `tmp/swachhdata-1.5.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 26485 bytes, number of entries: 20
--rw-r--r--  2.0 unx      227 b- defN 23-May-21 03:55 swachhdata/__init__.py
+Zip file size: 26488 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      227 b- defN 23-May-21 04:10 swachhdata/__init__.py
 -rw-r--r--  2.0 unx       66 b- defN 23-May-21 03:53 swachhdata/compose/__init__.py
 -rw-r--r--  2.0 unx      937 b- defN 23-May-21 03:52 swachhdata/compose/core.py
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
--rw-r--r--  2.0 unx     1309 b- defN 23-May-21 03:40 swachhdata/utils/verify.py
--rw-rw-rw-  2.0 unx    17096 b- defN 23-May-21 04:05 swachhdata-1.5.0a1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2272 b- defN 23-May-21 04:05 swachhdata-1.5.0a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-21 04:05 swachhdata-1.5.0a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-21 04:05 swachhdata-1.5.0a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1657 b- defN 23-May-21 04:05 swachhdata-1.5.0a1.dist-info/RECORD
-20 files, 157450 bytes uncompressed, 23783 bytes compressed:  84.9%
+-rw-r--r--  2.0 unx     1309 b- defN 23-May-21 04:10 swachhdata/utils/verify.py
+-rw-rw-rw-  2.0 unx    17096 b- defN 23-May-21 04:10 swachhdata-1.5.1a1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2272 b- defN 23-May-21 04:10 swachhdata-1.5.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 04:10 swachhdata-1.5.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-21 04:10 swachhdata-1.5.1a1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1657 b- defN 23-May-21 04:10 swachhdata-1.5.1a1.dist-info/RECORD
+20 files, 157450 bytes uncompressed, 23786 bytes compressed:  84.9%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: swachhdata/utils/tools.py
 Comment: 
 
 Filename: swachhdata/utils/verify.py
 Comment: 
 
-Filename: swachhdata-1.5.0a1.dist-info/LICENSE.txt
+Filename: swachhdata-1.5.1a1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: swachhdata-1.5.0a1.dist-info/METADATA
+Filename: swachhdata-1.5.1a1.dist-info/METADATA
 Comment: 
 
-Filename: swachhdata-1.5.0a1.dist-info/WHEEL
+Filename: swachhdata-1.5.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: swachhdata-1.5.0a1.dist-info/top_level.txt
+Filename: swachhdata-1.5.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: swachhdata-1.5.0a1.dist-info/RECORD
+Filename: swachhdata-1.5.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swachhdata/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = '1.5.0a1'
+__version__ = '1.5.1a1'
 __author__ = 'Kritik Seth'
 __maintainer__ = __author__
 __license__ = 'Mozilla Public License Version 2.0'
 __url__ = 'https://swachhdata.readthedocs.io/'
 __connect__ = 'https://www.kritikseth.com/'
```

## swachhdata/utils/verify.py

 * *Ordering differences only*

```diff
@@ -1,15 +1,10 @@
 import pandas
 import numpy
 
-from .tools import (
-    fetch_num_columns,
-    fetch_array_dim
-)
-
 def verify_array(data):
     return isinstance(data, numpy.ndarray)
 
 def verify_dataframe(data):
     return isinstance(data, pandas.core.frame.DataFrame) 
 
 def verify_series(data):
@@ -17,14 +12,19 @@
 
 def verify_list(data):
     return isinstance(data, list)
 
 def verify_str(data):
     return isinstance(data, str)
 
+from .tools import (
+    fetch_num_columns,
+    fetch_array_dim
+)
+
 def verify_valid_ndim_text(data):
     if verify_dataframe(data):
         if fetch_num_columns != 1:
             raise ValueError(
                     f'Expected 1 column in pandas.core.DataFrame, got {fetch_num_columns(data)}'
                 )
     elif verify_array(data):
```

## Comparing `swachhdata-1.5.0a1.dist-info/LICENSE.txt` & `swachhdata-1.5.1a1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `swachhdata-1.5.0a1.dist-info/METADATA` & `swachhdata-1.5.1a1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swachhdata
-Version: 1.5.0a1
+Version: 1.5.1a1
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
-Metadata-Version: 2.1 Name: swachhdata Version: 1.5.0a1 Summary: Data cleaning
+Metadata-Version: 2.1 Name: swachhdata Version: 1.5.1a1 Summary: Data cleaning
 made easy with swachhdata Home-page: https://swachhdata.readthedocs.io/ Author:
 Kritik Seth Author-email: sethkritik@gmail.com Classifier: Natural Language ::
 English Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL
 2.0) Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 6 - Mature Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: regex (>=2019.12.20) Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: tqdm (>=4.41.1) Requires-Dist: beautifulsoup4 (>=4.6.3)
```

## Comparing `swachhdata-1.5.0a1.dist-info/RECORD` & `swachhdata-1.5.1a1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-swachhdata/__init__.py,sha256=OZ8Vy7BqCbxLKBnc1R71oRJvDlRv43lpxLBWmSbkeCQ,227
+swachhdata/__init__.py,sha256=GanQ9TkAR83bP9_oXTyBJUZPKv8gCEaXmHCGmgiHEYE,227
 swachhdata/compose/__init__.py,sha256=fYvifIgd34JznO9LQRptjNVM2uaFo28nbPMc7Zf_BD0,66
 swachhdata/compose/core.py,sha256=iaxOHhZQwYbXiKncQMQVv4psdLCNMw3NBJZ5V4jO0eY,937
 swachhdata/image/__init__.py,sha256=m6pEvV60cN9cj5G-mMsr27F41s6A-IbPNIpmSwFvSmE,131
 swachhdata/image/_image.py,sha256=9RkuFHcWZOSVXWByBfvCnO6hhB19KLwia4QErqr6SY8,7477
 swachhdata/legacy/__init__.py,sha256=MQGn-ahr-9jjg4T_hp1Btl39mSAuw7qw359evKHUnjk,173
 swachhdata/legacy/_text.py,sha256=lQqrPQunEwCeNf0hUBrxBBIp3e7iX-WRovYb0kHi1_4,15947
 swachhdata/text/__init__.py,sha256=EAhE1VtfSqNEg9hUblZUYBIXk28pFAwJLBCnGtLpULg,1013
 swachhdata/text/_base.py,sha256=niUOhSY7TGk1Y4QXZHoWeIm02EbGXuacvC2o8MXQguk,1058
 swachhdata/text/_text.py,sha256=MmDmJrVtxKN5_P-FYhUq-4L5urRIvyOIixCpZRQgRlA,105336
 swachhdata/utils/__init__.py,sha256=1ZH0VgYFVYuf0jTP8ncCxPxDnHBOEQ8OZgjy-iuvYlU,642
 swachhdata/utils/probe.py,sha256=Gms2hRnfGB-VN7DOov-AJWMHtJICbHiwlDQo51N3YCM,377
 swachhdata/utils/recast.py,sha256=1J7WCQ8evbEJ_1OBkq8j8mLMVxOwMf9LK1weZPmvBm4,1149
 swachhdata/utils/tools.py,sha256=1K9ekx8Lqt15GY7RuEH5-wgL_TtMEkEYyevN9KrP03I,480
-swachhdata/utils/verify.py,sha256=cPqLGMSi3kOWZUmraZzKHJC1OpAHyZaybG79c7BpFIM,1309
-swachhdata-1.5.0a1.dist-info/LICENSE.txt,sha256=k0P1sbYupRWlxoESvbYq2UzoMW6MXA84LltqR-4mEo4,17096
-swachhdata-1.5.0a1.dist-info/METADATA,sha256=KvWmLYHQhIYmUJemNVd6mR-c-PBb7UcYV_YWthqDqdE,2272
-swachhdata-1.5.0a1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-swachhdata-1.5.0a1.dist-info/top_level.txt,sha256=UPLFTkg5MwIkJLZzEOsLnndE5jByl-BGbZ0_Z40oq0Y,11
-swachhdata-1.5.0a1.dist-info/RECORD,,
+swachhdata/utils/verify.py,sha256=2GVec_gRGR5cPzvaxxFc5uFn1YKJQ_uk1fU-_BshNYs,1309
+swachhdata-1.5.1a1.dist-info/LICENSE.txt,sha256=k0P1sbYupRWlxoESvbYq2UzoMW6MXA84LltqR-4mEo4,17096
+swachhdata-1.5.1a1.dist-info/METADATA,sha256=e7rOZz-rg7e0U1qu5LimQrIgMBhX0dNdaLEgpTvYsUg,2272
+swachhdata-1.5.1a1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+swachhdata-1.5.1a1.dist-info/top_level.txt,sha256=UPLFTkg5MwIkJLZzEOsLnndE5jByl-BGbZ0_Z40oq0Y,11
+swachhdata-1.5.1a1.dist-info/RECORD,,
```

