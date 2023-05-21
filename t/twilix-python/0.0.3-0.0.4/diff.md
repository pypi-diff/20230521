# Comparing `tmp/twilix-python-0.0.3.tar.gz` & `tmp/twilix-python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilix-python-0.0.3.tar", last modified: Sat May 20 15:22:34 2023, max compression
+gzip compressed data, was "twilix-python-0.0.4.tar", last modified: Sun May 21 12:28:17 2023, max compression
```

## Comparing `twilix-python-0.0.3.tar` & `twilix-python-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 15:22:34.628758 twilix-python-0.0.3/
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-05-20 02:14:08.000000 twilix-python-0.0.3/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-20 15:22:34.628618 twilix-python-0.0.3/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      133 2023-05-20 11:36:18.000000 twilix-python-0.0.3/README.md
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-05-20 15:22:34.628805 twilix-python-0.0.3/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      377 2023-05-20 15:22:30.000000 twilix-python-0.0.3/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 15:22:34.627070 twilix-python-0.0.3/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      589 2023-05-20 15:04:38.000000 twilix-python-0.0.3/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      360 2023-05-20 15:10:35.000000 twilix-python-0.0.3/tests/test_semantic_search.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 15:22:34.627398 twilix-python-0.0.3/twilix/
--rw-r--r--   0 jackywong   (501) staff       (20)     1468 2023-05-20 15:13:05.000000 twilix-python-0.0.3/twilix/__init__.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 15:22:34.628360 twilix-python-0.0.3/twilix_python.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-20 15:22:34.000000 twilix-python-0.0.3/twilix_python.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      278 2023-05-20 15:22:34.000000 twilix-python-0.0.3/twilix_python.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-05-20 15:22:34.000000 twilix-python-0.0.3/twilix_python.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-05-20 15:22:34.000000 twilix-python-0.0.3/twilix_python.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        7 2023-05-20 15:22:34.000000 twilix-python-0.0.3/twilix_python.egg-info/top_level.txt
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:28:17.275436 twilix-python-0.0.4/
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-05-20 02:14:08.000000 twilix-python-0.0.4/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-21 12:28:17.275286 twilix-python-0.0.4/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      133 2023-05-20 15:30:27.000000 twilix-python-0.0.4/README.md
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-05-21 12:28:17.275485 twilix-python-0.0.4/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      377 2023-05-21 11:54:37.000000 twilix-python-0.0.4/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:28:17.273874 twilix-python-0.0.4/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      575 2023-05-21 12:28:10.000000 twilix-python-0.0.4/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      360 2023-05-20 15:30:28.000000 twilix-python-0.0.4/tests/test_semantic_search.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:28:17.274261 twilix-python-0.0.4/twilix/
+-rw-r--r--   0 jackywong   (501) staff       (20)     3149 2023-05-21 12:28:08.000000 twilix-python-0.0.4/twilix/__init__.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:28:17.275089 twilix-python-0.0.4/twilix_python.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-21 12:28:17.000000 twilix-python-0.0.4/twilix_python.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      278 2023-05-21 12:28:17.000000 twilix-python-0.0.4/twilix_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-05-21 12:28:17.000000 twilix-python-0.0.4/twilix_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-05-21 12:28:17.000000 twilix-python-0.0.4/twilix_python.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        7 2023-05-21 12:28:17.000000 twilix-python-0.0.4/twilix_python.egg-info/top_level.txt
```

### Comparing `twilix-python-0.0.3/LICENSE` & `twilix-python-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twilix-python-0.0.3/tests/test_crud.py` & `twilix-python-0.0.4/tests/test_crud.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,12 @@
 docs = [
     {
         "answer": "This framework generates embeddings for each input sentence",
     },
     {
         "answer": "Sentences are passed as a list of string.",
     },
-    {
-        "answer": "The quick brown fox jumps over the lazy dog."
-    },
+    {"answer": "The quick brown fox jumps over the lazy dog."},
 ]
 
 result = twilix.add_objects(collection_name=collection_name, objects=docs)
 ic(result)
```

### Comparing `twilix-python-0.0.3/twilix/__init__.py` & `twilix-python-0.0.4/twilix/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,56 +2,124 @@
 from icecream import ic
 
 # Initialize the api_key variable
 api_key = None
 base_url = "https://api.twilix.io"
 # base_url = "http://localhost:8000"
 
+
 def set_api_key(key):
     global api_key
     api_key = key
 
 
-def make_post_request(endpoint: str, json: dict):
+def make_post_request(endpoint: str, json: dict, params: dict = None):
+    headers = {
+        "Authorization": f"Bearer {api_key}",
+    }
+    response = requests.post(
+        base_url + endpoint, headers=headers, json=json, params=params
+    )
+    if response.status_code != 200:
+        ic(response.content.decode())
+    response.raise_for_status()
+    return response.json()
+
+
+def make_delete_request(endpoint: str, json: dict):
     headers = {
         "Authorization": f"Bearer {api_key}",
     }
-    response = requests.post(base_url + endpoint, headers=headers, json=json)
+    response = requests.delete(base_url + endpoint, headers=headers, json=json)
+    ic(response.content.decode())
+    response.raise_for_status()
+    return response.json()
+
+
+def make_get_request(endpoint: str, params: dict = None):
+    headers = {
+        "Authorization": f"Bearer {api_key}",
+    }
+    response = requests.get(base_url + endpoint, headers=headers, params=params)
     ic(response.content.decode())
     response.raise_for_status()
     return response.json()
 
 
 def add_objects(collection_name: str, objects: list):
     return make_post_request(
-        endpoint="/collection/bulk_insert",
-        json={"collection_name": collection_name, "objects": objects},
+        endpoint=f"/collection/{collection_name}/bulk_insert",
+        json={"objects": objects},
     )
 
 
 def search(collection_name: str, query: str, fields_to_search: list = None):
     return make_post_request(
-        endpoint="/collection/search",
+        endpoint=f"/collection/{collection_name}/search",
         json={
-            "collection_name": collection_name,
             "text": query,
             "fields_to_search": fields_to_search,
         },
     )
 
 
-def ask(
+def answer(
     collection_name: str,
     query: str,
     fields_to_search: list = None,
     include_reference_documents: bool = False,
 ):
     return make_post_request(
-        endpoint="/collection/ask_question",
+        endpoint=f"/collection/{collection_name}/answer",
         json={
-            "collection_name": collection_name,
             "text": query,
             "fields_to_search": fields_to_search,
             "include_reference_documents": include_reference_documents,
         },
     )
 
+
+def delete_object(collection_name: str, object_id: str):
+    """Delete an object"""
+    return make_delete_request(
+        endpoint=f"/collection/{collection_name}/object/delete",
+        json={"object_id": object_id},
+    )
+
+
+def list_collections():
+    """List collections"""
+    return make_get_request(
+        endpoint="/collection/list",
+    )
+
+
+def list_objects(collection_name: str):
+    """List documents"""
+    return make_post_request(
+        f"/collection/{collection_name}/list",
+        json=None,
+    )
+
+
+def graphql(graphql_query: str):
+    """GraphQL"""
+    return make_post_request(
+        endpoint=f"/graphql",
+        json={
+            "graphql_query": graphql_query,
+        },
+    )
+
+
+def get_number_of_objects(collection_name: str):
+    """Number of documents"""
+    return make_get_request(
+        endpoint=f"/collection/{collection_name}/number_of_objects",
+    )
+
+
+def get_collection_schema(collection_name: str):
+    """Get collection schema"""
+    return make_get_request(
+        endpoint=f"/collection/{collection_name}/schema",
+    )
```

