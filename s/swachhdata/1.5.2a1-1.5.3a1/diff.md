# Comparing `tmp/swachhdata-1.5.2a1-py3-none-any.whl.zip` & `tmp/swachhdata-1.5.3a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 26557 bytes, number of entries: 20
--rw-r--r--  2.0 unx      227 b- defN 23-May-21 04:19 swachhdata/__init__.py
+Zip file size: 26585 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      227 b- defN 23-May-21 04:33 swachhdata/__init__.py
 -rw-r--r--  2.0 unx      106 b- defN 23-May-21 04:19 swachhdata/compose/__init__.py
--rw-r--r--  2.0 unx     1140 b- defN 23-May-21 04:19 swachhdata/compose/core.py
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-21 04:49 swachhdata/compose/core.py
 -rw-r--r--  2.0 unx      131 b- defN 22-Jan-25 09:02 swachhdata/image/__init__.py
 -rw-r--r--  2.0 unx     7477 b- defN 22-Jan-25 09:02 swachhdata/image/_image.py
 -rw-r--r--  2.0 unx      173 b- defN 22-Jan-25 09:02 swachhdata/legacy/__init__.py
 -rw-r--r--  2.0 unx    15947 b- defN 23-Mar-10 23:37 swachhdata/legacy/_text.py
--rw-r--r--  2.0 unx     1013 b- defN 23-Mar-10 23:36 swachhdata/text/__init__.py
--rw-r--r--  2.0 unx     1058 b- defN 23-Mar-10 23:37 swachhdata/text/_base.py
+-rw-r--r--  2.0 unx     1083 b- defN 23-May-21 04:49 swachhdata/text/__init__.py
+-rw-r--r--  2.0 unx     1248 b- defN 23-May-21 04:49 swachhdata/text/_base.py
 -rw-r--r--  2.0 unx   105336 b- defN 23-Mar-10 23:38 swachhdata/text/_text.py
 -rw-r--r--  2.0 unx      642 b- defN 23-May-21 03:53 swachhdata/utils/__init__.py
 -rw-r--r--  2.0 unx      377 b- defN 23-May-21 03:02 swachhdata/utils/probe.py
 -rw-r--r--  2.0 unx     1149 b- defN 23-May-21 03:50 swachhdata/utils/recast.py
 -rw-r--r--  2.0 unx      480 b- defN 23-May-21 03:06 swachhdata/utils/tools.py
 -rw-r--r--  2.0 unx     1309 b- defN 23-May-21 04:10 swachhdata/utils/verify.py
--rw-rw-rw-  2.0 unx    17096 b- defN 23-May-21 04:20 swachhdata-1.5.2a1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2272 b- defN 23-May-21 04:20 swachhdata-1.5.2a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-21 04:20 swachhdata-1.5.2a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-21 04:20 swachhdata-1.5.2a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1659 b- defN 23-May-21 04:20 swachhdata-1.5.2a1.dist-info/RECORD
-20 files, 157695 bytes uncompressed, 23855 bytes compressed:  84.9%
+-rw-rw-rw-  2.0 unx    17096 b- defN 23-May-21 04:50 swachhdata-1.5.3a1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2272 b- defN 23-May-21 04:50 swachhdata-1.5.3a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 04:50 swachhdata-1.5.3a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-21 04:50 swachhdata-1.5.3a1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1659 b- defN 23-May-21 04:50 swachhdata-1.5.3a1.dist-info/RECORD
+20 files, 158051 bytes uncompressed, 23883 bytes compressed:  84.9%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: swachhdata/utils/tools.py
 Comment: 
 
 Filename: swachhdata/utils/verify.py
 Comment: 
 
-Filename: swachhdata-1.5.2a1.dist-info/LICENSE.txt
+Filename: swachhdata-1.5.3a1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: swachhdata-1.5.2a1.dist-info/METADATA
+Filename: swachhdata-1.5.3a1.dist-info/METADATA
 Comment: 
 
-Filename: swachhdata-1.5.2a1.dist-info/WHEEL
+Filename: swachhdata-1.5.3a1.dist-info/WHEEL
 Comment: 
 
-Filename: swachhdata-1.5.2a1.dist-info/top_level.txt
+Filename: swachhdata-1.5.3a1.dist-info/top_level.txt
 Comment: 
 
-Filename: swachhdata-1.5.2a1.dist-info/RECORD
+Filename: swachhdata-1.5.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swachhdata/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = '1.5.2a1'
+__version__ = '1.5.3a1'
 __author__ = 'Kritik Seth'
 __maintainer__ = __author__
 __license__ = 'Mozilla Public License Version 2.0'
 __url__ = 'https://swachhdata.readthedocs.io/'
 __connect__ = 'https://www.kritikseth.com/'
```

## swachhdata/compose/core.py

```diff
@@ -25,14 +25,18 @@
     def __init__(self, text=None):
         
         dtype_check = verify_valid_dtype_text(text)
         ndim_check = verify_valid_ndim_text(text)
 
         self.__data = None
         self.data = text
+        self.__base_text_datum = None
+    
+    def __str__(self):
+        return str(self.data)
     
     def __len__(self):
         return fetch_num_rows(self.__data)
 
     @property
     def data(self):
         return self.__data
```

## swachhdata/text/__init__.py

```diff
@@ -12,14 +12,18 @@
 from ._text import PunctuationRecast
 from ._text import StemmingRecast
 from ._text import LemmatizationRecast
 from ._text import TokenisationRecast
 from ._text import TextRecast
 from ._text import RecastPipeline
 
+from ._base import (
+    BaseTextRecast
+)
+
 
 __all__ = [
     'urlRecast',
     'htmlRecast',
     'EscapeSequenceRecast',
     'MentionRecast',
     'ContractionsRecast',
@@ -30,9 +34,10 @@
     'NumberRecast',
     'AlphabetRecast',
     'PunctuationRecast',
     'StemmingRecast',
     'LemmatizationRecast',
     'TokenisationRecast',
     'TextRecast',
-    'RecastPipeline'
+    'RecastPipeline',
+    'BaseTextRecast'
 ]
```

## swachhdata/text/_base.py

```diff
@@ -1,23 +1,9 @@
-import re
 import pandas
-from tqdm.auto import trange, tqdm
-from bs4 import BeautifulSoup
-from html import unescape
-import contractions
-import nltk
-nltk.download('popular', quiet=True)
-import spacy
-from gensim.parsing.preprocessing import remove_stopwords
-import num2words
-import unicodedata
-import string
-import json
-import textblob
-
+from ..compose.core import BaseTextDatum
 
 class TextFormatter:
     """
     Base Data Formatter for all recasts in swachhdata.text module
 
     Accepted text input format:
         * string
@@ -26,20 +12,45 @@
     """
 
     def __init__(self):
         
         self._dtype = None
         self._text = None
         self._count = None
-
     
     def __text_formatter(self):
         
         self._count = len(self._text)
 
         if self._dtype == pandas.core.series.Series:
             self._text = self._text.tolist()
             self._dtype = type(self._text)
 
         if self._dtype == str:
             self._count = len(self._text.split())
-            self._dtype = type(self._text)
+            self._dtype = type(self._text)
+
+class BaseTextRecast(BaseTextDatum):
+
+    def __init__(self):
+        """
+        Initialize
+        """
+    
+    def setup(self, data)
+        """
+        Setup
+        """
+        if hasattr(data, '__base_text_datum'):
+            self.__dict__.update(data.__dict__)
+        else:
+            self.data = data
+    
+    def recast(self):
+        """
+        Recast
+        """
+    
+    def setup_recast(self):
+        """
+        Setup & Recast
+        """
```

## Comparing `swachhdata-1.5.2a1.dist-info/LICENSE.txt` & `swachhdata-1.5.3a1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `swachhdata-1.5.2a1.dist-info/METADATA` & `swachhdata-1.5.3a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swachhdata
-Version: 1.5.2a1
+Version: 1.5.3a1
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
-Metadata-Version: 2.1 Name: swachhdata Version: 1.5.2a1 Summary: Data cleaning
+Metadata-Version: 2.1 Name: swachhdata Version: 1.5.3a1 Summary: Data cleaning
 made easy with swachhdata Home-page: https://swachhdata.readthedocs.io/ Author:
 Kritik Seth Author-email: sethkritik@gmail.com Classifier: Natural Language ::
 English Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL
 2.0) Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 6 - Mature Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: regex (>=2019.12.20) Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: tqdm (>=4.41.1) Requires-Dist: beautifulsoup4 (>=4.6.3)
```

## Comparing `swachhdata-1.5.2a1.dist-info/RECORD` & `swachhdata-1.5.3a1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-swachhdata/__init__.py,sha256=YxUwCa69MA6Rhgs6UvGkTXCaSTd4Sgj0wdmvBKya_y0,227
+swachhdata/__init__.py,sha256=gOGYxlxN2Clj4imPYLo-sCwbh7YgnbPVtpdKXrlx3EM,227
 swachhdata/compose/__init__.py,sha256=9NKRJN3d38FxfExXwK8L1jfi5IMI5jKqfEtFLt97LO8,106
-swachhdata/compose/core.py,sha256=xhUFzyLbo5fEYgSlb0PR5BC-ClTXzZ09GiHtRCR3QKY,1140
+swachhdata/compose/core.py,sha256=KJUUMFg-mW5329nO2RkWh0gZq-KW2Q_Vp407mn1w78Y,1236
 swachhdata/image/__init__.py,sha256=m6pEvV60cN9cj5G-mMsr27F41s6A-IbPNIpmSwFvSmE,131
 swachhdata/image/_image.py,sha256=9RkuFHcWZOSVXWByBfvCnO6hhB19KLwia4QErqr6SY8,7477
 swachhdata/legacy/__init__.py,sha256=MQGn-ahr-9jjg4T_hp1Btl39mSAuw7qw359evKHUnjk,173
 swachhdata/legacy/_text.py,sha256=lQqrPQunEwCeNf0hUBrxBBIp3e7iX-WRovYb0kHi1_4,15947
-swachhdata/text/__init__.py,sha256=EAhE1VtfSqNEg9hUblZUYBIXk28pFAwJLBCnGtLpULg,1013
-swachhdata/text/_base.py,sha256=niUOhSY7TGk1Y4QXZHoWeIm02EbGXuacvC2o8MXQguk,1058
+swachhdata/text/__init__.py,sha256=Yv-lTK8yimzHxXI7FH2cRuhqBMby9UL_GK1Obf8zaNs,1083
+swachhdata/text/_base.py,sha256=_GTaw1SDB9hntP7eMztSXyBWz-kSRvw4-Slyoyz5sRk,1248
 swachhdata/text/_text.py,sha256=MmDmJrVtxKN5_P-FYhUq-4L5urRIvyOIixCpZRQgRlA,105336
 swachhdata/utils/__init__.py,sha256=1ZH0VgYFVYuf0jTP8ncCxPxDnHBOEQ8OZgjy-iuvYlU,642
 swachhdata/utils/probe.py,sha256=Gms2hRnfGB-VN7DOov-AJWMHtJICbHiwlDQo51N3YCM,377
 swachhdata/utils/recast.py,sha256=1J7WCQ8evbEJ_1OBkq8j8mLMVxOwMf9LK1weZPmvBm4,1149
 swachhdata/utils/tools.py,sha256=1K9ekx8Lqt15GY7RuEH5-wgL_TtMEkEYyevN9KrP03I,480
 swachhdata/utils/verify.py,sha256=2GVec_gRGR5cPzvaxxFc5uFn1YKJQ_uk1fU-_BshNYs,1309
-swachhdata-1.5.2a1.dist-info/LICENSE.txt,sha256=k0P1sbYupRWlxoESvbYq2UzoMW6MXA84LltqR-4mEo4,17096
-swachhdata-1.5.2a1.dist-info/METADATA,sha256=ZbRjtb17KpseqxX8a0bC1E0Jc6M2Ja5MlpoZ8MT--0c,2272
-swachhdata-1.5.2a1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-swachhdata-1.5.2a1.dist-info/top_level.txt,sha256=UPLFTkg5MwIkJLZzEOsLnndE5jByl-BGbZ0_Z40oq0Y,11
-swachhdata-1.5.2a1.dist-info/RECORD,,
+swachhdata-1.5.3a1.dist-info/LICENSE.txt,sha256=k0P1sbYupRWlxoESvbYq2UzoMW6MXA84LltqR-4mEo4,17096
+swachhdata-1.5.3a1.dist-info/METADATA,sha256=LWr7oEWwTmBO20cziVpfbAAEFq-qfbYZDRYnQyl0Rvg,2272
+swachhdata-1.5.3a1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+swachhdata-1.5.3a1.dist-info/top_level.txt,sha256=UPLFTkg5MwIkJLZzEOsLnndE5jByl-BGbZ0_Z40oq0Y,11
+swachhdata-1.5.3a1.dist-info/RECORD,,
```

