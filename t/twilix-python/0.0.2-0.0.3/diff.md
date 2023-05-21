# Comparing `tmp/twilix-python-0.0.2.tar.gz` & `tmp/twilix-python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilix-python-0.0.2.tar", last modified: Sat May 20 13:41:17 2023, max compression
+gzip compressed data, was "twilix-python-0.0.3.tar", last modified: Sat May 20 15:22:34 2023, max compression
```

## Comparing `twilix-python-0.0.2.tar` & `twilix-python-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 13:41:17.789842 twilix-python-0.0.2/
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-05-20 02:14:08.000000 twilix-python-0.0.2/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-20 13:41:17.789679 twilix-python-0.0.2/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      133 2023-05-20 11:36:18.000000 twilix-python-0.0.2/README.md
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-05-20 13:41:17.789908 twilix-python-0.0.2/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      377 2023-05-20 11:56:48.000000 twilix-python-0.0.2/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 13:41:17.787953 twilix-python-0.0.2/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      516 2023-05-20 11:33:00.000000 twilix-python-0.0.2/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      310 2023-05-20 06:21:57.000000 twilix-python-0.0.2/tests/test_semantic_search.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 13:41:17.788433 twilix-python-0.0.2/twilix/
--rw-r--r--   0 jackywong   (501) staff       (20)     1448 2023-05-20 11:58:43.000000 twilix-python-0.0.2/twilix/__init__.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 13:41:17.789487 twilix-python-0.0.2/twilix_python.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-20 13:41:17.000000 twilix-python-0.0.2/twilix_python.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      278 2023-05-20 13:41:17.000000 twilix-python-0.0.2/twilix_python.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-05-20 13:41:17.000000 twilix-python-0.0.2/twilix_python.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-05-20 13:41:17.000000 twilix-python-0.0.2/twilix_python.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        7 2023-05-20 13:41:17.000000 twilix-python-0.0.2/twilix_python.egg-info/top_level.txt
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 15:22:34.628758 twilix-python-0.0.3/
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-05-20 02:14:08.000000 twilix-python-0.0.3/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-20 15:22:34.628618 twilix-python-0.0.3/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      133 2023-05-20 11:36:18.000000 twilix-python-0.0.3/README.md
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-05-20 15:22:34.628805 twilix-python-0.0.3/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      377 2023-05-20 15:22:30.000000 twilix-python-0.0.3/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 15:22:34.627070 twilix-python-0.0.3/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      589 2023-05-20 15:04:38.000000 twilix-python-0.0.3/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      360 2023-05-20 15:10:35.000000 twilix-python-0.0.3/tests/test_semantic_search.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 15:22:34.627398 twilix-python-0.0.3/twilix/
+-rw-r--r--   0 jackywong   (501) staff       (20)     1468 2023-05-20 15:13:05.000000 twilix-python-0.0.3/twilix/__init__.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 15:22:34.628360 twilix-python-0.0.3/twilix_python.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-20 15:22:34.000000 twilix-python-0.0.3/twilix_python.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      278 2023-05-20 15:22:34.000000 twilix-python-0.0.3/twilix_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-05-20 15:22:34.000000 twilix-python-0.0.3/twilix_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-05-20 15:22:34.000000 twilix-python-0.0.3/twilix_python.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        7 2023-05-20 15:22:34.000000 twilix-python-0.0.3/twilix_python.egg-info/top_level.txt
```

### Comparing `twilix-python-0.0.2/LICENSE` & `twilix-python-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twilix-python-0.0.2/tests/test_crud.py` & `twilix-python-0.0.3/tests/test_crud.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Test for inserting data
 """
 import twilix
 from icecream import ic
 
-api_key = "j7UqObCMXFi4i1rQqBUdHidZ_K5fsHZkmf0h91HU9LM="
+# api_key = "j7UqObCMXFi4i1rQqBUdHidZ_K5fsHZkmf0h91HU9LM="
+api_key = "1f2B9oV_xbQvGbFcryiynNOEBwtFd_5YV6huRwVMHSA="
 
 twilix.api_key = api_key
 
 collection_name = "example2"
 
 docs = [
     {
         "answer": "This framework generates embeddings for each input sentence",
     },
     {
         "answer": "Sentences are passed as a list of string.",
     },
-    {"answer": "The quick brown fox jumps over the lazy dog."},
+    {
+        "answer": "The quick brown fox jumps over the lazy dog."
+    },
 ]
 
 result = twilix.add_objects(collection_name=collection_name, objects=docs)
 ic(result)
```

### Comparing `twilix-python-0.0.2/twilix/__init__.py` & `twilix-python-0.0.3/twilix/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 from icecream import ic
 
 # Initialize the api_key variable
 api_key = None
-base_url = "http://api.twilix.io"
+base_url = "https://api.twilix.io"
+# base_url = "http://localhost:8000"
 
 def set_api_key(key):
     global api_key
     api_key = key
 
 
 def make_post_request(endpoint: str, json: dict):
@@ -23,17 +24,17 @@
 def add_objects(collection_name: str, objects: list):
     return make_post_request(
         endpoint="/collection/bulk_insert",
         json={"collection_name": collection_name, "objects": objects},
     )
 
 
-def semantic_search(collection_name: str, query: str, fields_to_search: list = None):
+def search(collection_name: str, query: str, fields_to_search: list = None):
     return make_post_request(
-        endpoint="/collection/semantic_search",
+        endpoint="/collection/search",
         json={
             "collection_name": collection_name,
             "text": query,
             "fields_to_search": fields_to_search,
         },
     )
```

