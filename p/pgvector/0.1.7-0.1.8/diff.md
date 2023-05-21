# Comparing `tmp/pgvector-0.1.7-py2.py3-none-any.whl.zip` & `tmp/pgvector-0.1.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7525 bytes, number of entries: 11
+Zip file size: 7559 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      272 b- defN 21-Jun-23 06:42 pgvector/asyncpg/__init__.py
--rw-r--r--  2.0 unx     2333 b- defN 22-Jan-14 19:08 pgvector/django/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 23-May-13 19:32 pgvector/django/__init__.py
 -rw-r--r--  2.0 unx     1743 b- defN 23-May-10 04:14 pgvector/psycopg/__init__.py
 -rw-r--r--  2.0 unx      881 b- defN 21-Jun-13 19:29 pgvector/psycopg2/__init__.py
 -rw-r--r--  2.0 unx     1033 b- defN 22-May-23 01:12 pgvector/sqlalchemy/__init__.py
 -rw-r--r--  2.0 unx     1305 b- defN 21-Jun-23 02:28 pgvector/utils/__init__.py
--rw-r--r--  2.0 unx     1083 b- defN 23-May-11 21:56 pgvector-0.1.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6462 b- defN 23-May-11 21:56 pgvector-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-11 21:56 pgvector-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-11 21:56 pgvector-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      904 b- defN 23-May-11 21:56 pgvector-0.1.7.dist-info/RECORD
-11 files, 16135 bytes uncompressed, 5993 bytes compressed:  62.9%
+-rw-r--r--  2.0 unx     1083 b- defN 23-May-21 00:32 pgvector-0.1.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6462 b- defN 23-May-21 00:32 pgvector-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-21 00:32 pgvector-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-21 00:32 pgvector-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      904 b- defN 23-May-21 00:32 pgvector-0.1.8.dist-info/RECORD
+11 files, 16236 bytes uncompressed, 6027 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pgvector/sqlalchemy/__init__.py
 Comment: 
 
 Filename: pgvector/utils/__init__.py
 Comment: 
 
-Filename: pgvector-0.1.7.dist-info/LICENSE.txt
+Filename: pgvector-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pgvector-0.1.7.dist-info/METADATA
+Filename: pgvector-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: pgvector-0.1.7.dist-info/WHEEL
+Filename: pgvector-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: pgvector-0.1.7.dist-info/top_level.txt
+Filename: pgvector-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pgvector-0.1.7.dist-info/RECORD
+Filename: pgvector-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pgvector/django/__init__.py

```diff
@@ -7,15 +7,15 @@
 
 
 class VectorExtension(CreateExtension):
     def __init__(self):
         self.name = 'vector'
 
 
-# https://docs.djangoproject.com/en/3.2/howto/custom-model-fields/
+# https://docs.djangoproject.com/en/4.2/howto/custom-model-fields/
 class VectorField(Field):
     description = 'Vector'
 
     def __init__(self, *args, dimensions=None, **kwargs):
         self.dimensions = dimensions
         super().__init__(*args, **kwargs)
 
@@ -35,14 +35,17 @@
 
     def to_python(self, value):
         return from_db(value)
 
     def get_prep_value(self, value):
         return to_db(value)
 
+    def value_to_string(self, obj):
+        return self.get_prep_value(self.value_from_object(obj))
+
 
 class IvfflatIndex(PostgresIndex):
     suffix = 'ivfflat'
 
     def __init__(self, *expressions, lists=None, **kwargs):
         self.lists = lists
         super().__init__(*expressions, **kwargs)
```

## Comparing `pgvector-0.1.7.dist-info/LICENSE.txt` & `pgvector-0.1.8.dist-info/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021-2022 Andrew Kane
+Copyright (c) 2021-2023 Andrew Kane
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `pgvector-0.1.7.dist-info/METADATA` & `pgvector-0.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgvector
-Version: 0.1.7
+Version: 0.1.8
 Summary: pgvector support for Python
 Home-page: https://github.com/pgvector/pgvector-python
 Author: Andrew Kane
 Author-email: andrew@ankane.org
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

## Comparing `pgvector-0.1.7.dist-info/RECORD` & `pgvector-0.1.8.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pgvector/asyncpg/__init__.py,sha256=VffBZUNIwvinQdh0lIYoSWgSQq57nFkpj9VhPjp11QQ,272
-pgvector/django/__init__.py,sha256=vqCrNBuQ-Big2ijRp8V5quBapwEVBDWWUS6X9Qc-bT8,2333
+pgvector/django/__init__.py,sha256=8OX-LD3QpZD4a7a4vKVNSRXw9mbQlhHDTHQFhPpDe1M,2434
 pgvector/psycopg/__init__.py,sha256=BjyTM_VGtl3RB-Fh4gPBppr8LutuH7hR3l0C7MJYMyw,1743
 pgvector/psycopg2/__init__.py,sha256=w_uHyKJzHMI79IyKYwFv6CK_k1RI1X6sWiML55Wo4b4,881
 pgvector/sqlalchemy/__init__.py,sha256=LUEkR6UIxW_o6fmjRKQmasMm6ZkyylnkW7VDMWyi-EI,1033
 pgvector/utils/__init__.py,sha256=udvrI2Gl5cjO-eXYkb5opTDUFs0indJIPQJ9qgpH-j4,1305
-pgvector-0.1.7.dist-info/LICENSE.txt,sha256=acu4JLgUota7RWrziCwZFkNMxioYF78_0xbbpn6o3Jg,1083
-pgvector-0.1.7.dist-info/METADATA,sha256=AjFk4Am3xHde_WuzpKYj4AFbccs0AGneNVKJ3RTy678,6462
-pgvector-0.1.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-pgvector-0.1.7.dist-info/top_level.txt,sha256=xGGaXFRcSRHEhn0HS1FN_UjCWr1G-WSPgxx4a0NJc0M,9
-pgvector-0.1.7.dist-info/RECORD,,
+pgvector-0.1.8.dist-info/LICENSE.txt,sha256=3Nr5vwERQHKYiiQHzy_AO2HurO6I3TonpJlYOmwbmcI,1083
+pgvector-0.1.8.dist-info/METADATA,sha256=CWy0YjvD3twmA6Kp90wY8Nykvf9bjf7cWQE948E3jbs,6462
+pgvector-0.1.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+pgvector-0.1.8.dist-info/top_level.txt,sha256=xGGaXFRcSRHEhn0HS1FN_UjCWr1G-WSPgxx4a0NJc0M,9
+pgvector-0.1.8.dist-info/RECORD,,
```

