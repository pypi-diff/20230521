# Comparing `tmp/timeslime-1.5.4-py3-none-any.whl.zip` & `tmp/timeslime-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 14557 bytes, number of entries: 19
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-03 17:08 timeslime/__init__.py
--rw-r--r--  2.0 unx       52 b- defN 22-Mar-03 17:08 timeslime/__main__.py
--rw-r--r--  2.0 unx     6904 b- defN 22-Mar-03 17:08 timeslime/cli.py
--rw-r--r--  2.0 unx     1974 b- defN 22-Mar-03 17:08 timeslime/models.py
--rw-r--r--  2.0 unx     4429 b- defN 22-Mar-03 17:08 timeslime/serializer.py
--rw-r--r--  2.0 unx      489 b- defN 22-Mar-03 17:08 timeslime/handler/__init__.py
--rw-r--r--  2.0 unx     5997 b- defN 22-Mar-03 17:08 timeslime/handler/database_handler.py
--rw-r--r--  2.0 unx     1565 b- defN 22-Mar-03 17:08 timeslime/handler/ntp_server_handler.py
--rw-r--r--  2.0 unx     4287 b- defN 22-Mar-03 17:08 timeslime/handler/settings_handler.py
--rw-r--r--  2.0 unx     1092 b- defN 22-Mar-03 17:08 timeslime/handler/state_handler.py
--rw-r--r--  2.0 unx     7315 b- defN 22-Mar-03 17:08 timeslime/handler/timeslime_handler.py
--rw-r--r--  2.0 unx     5328 b- defN 22-Mar-03 17:08 timeslime/handler/timeslime_server_handler.py
--rw-rw-rw-  2.0 unx      534 b- defN 22-Mar-03 17:08 timeslime/update/1.2_to_1.3.sql
--rw-rw-rw-  2.0 unx     1072 b- defN 22-Mar-03 17:11 timeslime-1.5.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2797 b- defN 22-Mar-03 17:11 timeslime-1.5.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Mar-03 17:11 timeslime-1.5.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 22-Mar-03 17:11 timeslime-1.5.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 22-Mar-03 17:11 timeslime-1.5.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1617 b- defN 22-Mar-03 17:11 timeslime-1.5.4.dist-info/RECORD
-19 files, 45609 bytes uncompressed, 11889 bytes compressed:  73.9%
+Zip file size: 14639 bytes, number of entries: 19
+-rw-r--r--  2.0 unx        0 b- defN 23-May-21 18:19 timeslime/__init__.py
+-rw-r--r--  2.0 unx       52 b- defN 23-May-21 18:19 timeslime/__main__.py
+-rw-r--r--  2.0 unx     6904 b- defN 23-May-21 18:19 timeslime/cli.py
+-rw-r--r--  2.0 unx     1983 b- defN 23-May-21 18:19 timeslime/models.py
+-rw-r--r--  2.0 unx     4429 b- defN 23-May-21 18:19 timeslime/serializer.py
+-rw-r--r--  2.0 unx      489 b- defN 23-May-21 18:19 timeslime/handler/__init__.py
+-rw-r--r--  2.0 unx     5997 b- defN 23-May-21 18:19 timeslime/handler/database_handler.py
+-rw-r--r--  2.0 unx     1565 b- defN 23-May-21 18:19 timeslime/handler/ntp_server_handler.py
+-rw-r--r--  2.0 unx     4287 b- defN 23-May-21 18:19 timeslime/handler/settings_handler.py
+-rw-r--r--  2.0 unx     1092 b- defN 23-May-21 18:19 timeslime/handler/state_handler.py
+-rw-r--r--  2.0 unx     7315 b- defN 23-May-21 18:19 timeslime/handler/timeslime_handler.py
+-rw-r--r--  2.0 unx     5328 b- defN 23-May-21 18:19 timeslime/handler/timeslime_server_handler.py
+-rw-rw-rw-  2.0 unx      534 b- defN 23-May-21 18:19 timeslime/update/1.2_to_1.3.sql
+-rw-rw-rw-  2.0 unx     1072 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3073 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1617 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/RECORD
+19 files, 45893 bytes uncompressed, 11971 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: timeslime/handler/timeslime_server_handler.py
 Comment: 
 
 Filename: timeslime/update/1.2_to_1.3.sql
 Comment: 
 
-Filename: timeslime-1.5.4.dist-info/LICENSE
+Filename: timeslime-1.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: timeslime-1.5.4.dist-info/METADATA
+Filename: timeslime-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: timeslime-1.5.4.dist-info/WHEEL
+Filename: timeslime-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: timeslime-1.5.4.dist-info/entry_points.txt
+Filename: timeslime-1.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: timeslime-1.5.4.dist-info/top_level.txt
+Filename: timeslime-1.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: timeslime-1.5.4.dist-info/RECORD
+Filename: timeslime-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## timeslime/models.py

```diff
@@ -30,15 +30,15 @@
 
         table_name = "settings"
 
 
 class SettingResponse:
     """setting response model"""
 
-    settings: list
+    settings: list[Setting]
     request_time: datetime
 
 
 class Timespan(Model):
     """timespan model"""
 
     id = UUIDField(primary_key=True, default=uuid4)
```

## Comparing `timeslime-1.5.4.dist-info/LICENSE` & `timeslime-1.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `timeslime-1.5.4.dist-info/METADATA` & `timeslime-1.6.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: timeslime
-Version: 1.5.4
-Summary: UNKNOWN
+Version: 1.6.0
 Author: Christian Decker
 Author-email: christian.decker@lookslikematrix.de
 License: MIT
 Project-URL: Donate, https://www.buymeacoffee.com/lookslikematrix
 Project-URL: Source Code, https://gitlab.com/lookslikematrix/timeslime
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests (==2.27.1)
-Requires-Dist: click (==8.0.3)
-Requires-Dist: peewee (==3.14.8)
-Requires-Dist: dbus-python (==1.2.18) ; platform_system == "Linux"
+Requires-Dist: requests (==2.30.0)
+Requires-Dist: click (==8.1.3)
+Requires-Dist: peewee (==3.16.2)
+Requires-Dist: dbus-python (==1.3.2) ; platform_system == "Linux"
 
 # timeslime
 
 It's a tool to track your time.
 
 ## Install
 
@@ -71,8 +69,23 @@
 
 You can delete settings via the CL. For example:
 
 ~~~bash
 timeslime settings --key timeslime_server --delete
 ~~~
 
+## Getting started
 
+~~~bash
+git clone https://gitlab.com/lookslikematrix/timeslime.git
+cd timeslime
+pipenv install --dev
+pipenv shell
+pytest tests -m "not server"
+~~~
+
+Test with timeslime server.
+
+~~~bash
+docker run -d -p 8000:8000 --name timeslime-server lookslikematrix/timeslime-server:v1.4.8
+pytest tests
+~~~
```

## Comparing `timeslime-1.5.4.dist-info/RECORD` & `timeslime-1.6.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 timeslime/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 timeslime/__main__.py,sha256=D-c9Wts6p0sR6ES-shgtXLmF1nVCS_53ixj0OJ9IsMU,52
 timeslime/cli.py,sha256=me63ItWNoME_Tc9mklpi5SCva_f_PkE3bBuTRGFtVO0,6904
-timeslime/models.py,sha256=x9WEKEBVV_0yJEpxXDZ_yVVDo6dW19xmdYx5-QDMFCE,1974
+timeslime/models.py,sha256=maP58Mclu1aQgtEBAgdcf6U3iOAY4JxvRQoooJiDDLk,1983
 timeslime/serializer.py,sha256=M9V3jR722miV7IoXkxcjKVUfP1UOKIkQXzqwHZJqbhg,4429
 timeslime/handler/__init__.py,sha256=DgB8v_mx-6g0vIT5HBIO0GYCRbmBviytzDoT_eib4AI,489
 timeslime/handler/database_handler.py,sha256=f1hucZy8FUYMmR096TREf-dOgw5qES82pI8W4BHiKj8,5997
 timeslime/handler/ntp_server_handler.py,sha256=da6K6OX10MxvZaFDe5uHpjMGaEKpq0T7ew3x2SP8naQ,1565
 timeslime/handler/settings_handler.py,sha256=e59rOUrmBKnP7D8JbKXIAf0QI7QUXh_mkYtZyJCuObU,4287
 timeslime/handler/state_handler.py,sha256=4NbHzLnddWpPBqKZiQeMbJiF9DTc-2gDyB1gO7J6xx8,1092
 timeslime/handler/timeslime_handler.py,sha256=3Mg1JM5oRtGf-5AJm0vVPiIhb-zhNO02ZPmeUZHO0dk,7315
 timeslime/handler/timeslime_server_handler.py,sha256=4pmMifFKQHYGI9u-MQ-0jg7oninHzBY9Kv_vRugAAAI,5328
 timeslime/update/1.2_to_1.3.sql,sha256=LLuT0LCA9W4J-5kGuiqxJ9rEgq8cSr94v1GLC-oIRBA,534
-timeslime-1.5.4.dist-info/LICENSE,sha256=LiRYlunBxa9UIPdfV7F9IRSRSISLC7bCz-DubILGtgs,1072
-timeslime-1.5.4.dist-info/METADATA,sha256=7mgtGf12JwWlh2_lxJ3NqiI7P93xBexTy-dx6YLdZp8,2797
-timeslime-1.5.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-timeslime-1.5.4.dist-info/entry_points.txt,sha256=7i17KGeXCO0BSnIWyRwEfceSgacIX4J3L2gZQzsCUeA,55
-timeslime-1.5.4.dist-info/top_level.txt,sha256=kToBlgsTKvfE41ILjN4v6ZIQYLxFlROmu21LJPKmz8M,10
-timeslime-1.5.4.dist-info/RECORD,,
+timeslime-1.6.0.dist-info/LICENSE,sha256=LiRYlunBxa9UIPdfV7F9IRSRSISLC7bCz-DubILGtgs,1072
+timeslime-1.6.0.dist-info/METADATA,sha256=0WhEHNcjGUS22PaKvTdi686Nwa-erNVzd3IxhpkZTpI,3073
+timeslime-1.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+timeslime-1.6.0.dist-info/entry_points.txt,sha256=MT9_31puJx5fzANMynwiNIhyhYsl0KWKYNkzK8PZB-g,54
+timeslime-1.6.0.dist-info/top_level.txt,sha256=kToBlgsTKvfE41ILjN4v6ZIQYLxFlROmu21LJPKmz8M,10
+timeslime-1.6.0.dist-info/RECORD,,
```

