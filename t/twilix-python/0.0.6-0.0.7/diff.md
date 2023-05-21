# Comparing `tmp/twilix-python-0.0.6.tar.gz` & `tmp/twilix-python-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilix-python-0.0.6.tar", last modified: Sun May 21 12:50:29 2023, max compression
+gzip compressed data, was "twilix-python-0.0.7.tar", last modified: Sun May 21 12:56:49 2023, max compression
```

## Comparing `twilix-python-0.0.6.tar` & `twilix-python-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:50:29.637443 twilix-python-0.0.6/
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-05-20 02:14:08.000000 twilix-python-0.0.6/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-21 12:50:29.637308 twilix-python-0.0.6/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      133 2023-05-21 12:30:44.000000 twilix-python-0.0.6/README.md
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-05-21 12:50:29.637490 twilix-python-0.0.6/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      377 2023-05-21 12:49:16.000000 twilix-python-0.0.6/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:50:29.635899 twilix-python-0.0.6/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      575 2023-05-21 12:28:10.000000 twilix-python-0.0.6/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      360 2023-05-20 15:30:28.000000 twilix-python-0.0.6/tests/test_semantic_search.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:50:29.636260 twilix-python-0.0.6/twilix/
--rw-r--r--   0 jackywong   (501) staff       (20)     3129 2023-05-21 12:49:51.000000 twilix-python-0.0.6/twilix/__init__.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:50:29.637111 twilix-python-0.0.6/twilix_python.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-21 12:50:29.000000 twilix-python-0.0.6/twilix_python.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      278 2023-05-21 12:50:29.000000 twilix-python-0.0.6/twilix_python.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-05-21 12:50:29.000000 twilix-python-0.0.6/twilix_python.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-05-21 12:50:29.000000 twilix-python-0.0.6/twilix_python.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        7 2023-05-21 12:50:29.000000 twilix-python-0.0.6/twilix_python.egg-info/top_level.txt
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:56:49.438958 twilix-python-0.0.7/
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-05-20 02:14:08.000000 twilix-python-0.0.7/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-21 12:56:49.438824 twilix-python-0.0.7/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      133 2023-05-21 12:51:49.000000 twilix-python-0.0.7/README.md
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-05-21 12:56:49.439001 twilix-python-0.0.7/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      377 2023-05-21 12:56:19.000000 twilix-python-0.0.7/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:56:49.437376 twilix-python-0.0.7/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      575 2023-05-21 12:28:10.000000 twilix-python-0.0.7/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      360 2023-05-20 15:30:28.000000 twilix-python-0.0.7/tests/test_semantic_search.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:56:49.437745 twilix-python-0.0.7/twilix/
+-rw-r--r--   0 jackywong   (501) staff       (20)     3331 2023-05-21 12:55:19.000000 twilix-python-0.0.7/twilix/__init__.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-21 12:56:49.438602 twilix-python-0.0.7/twilix_python.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-21 12:56:49.000000 twilix-python-0.0.7/twilix_python.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      278 2023-05-21 12:56:49.000000 twilix-python-0.0.7/twilix_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-05-21 12:56:49.000000 twilix-python-0.0.7/twilix_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-05-21 12:56:49.000000 twilix-python-0.0.7/twilix_python.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        7 2023-05-21 12:56:49.000000 twilix-python-0.0.7/twilix_python.egg-info/top_level.txt
```

### Comparing `twilix-python-0.0.6/LICENSE` & `twilix-python-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `twilix-python-0.0.6/tests/test_crud.py` & `twilix-python-0.0.7/tests/test_crud.py`

 * *Files identical despite different names*

### Comparing `twilix-python-0.0.6/twilix/__init__.py` & `twilix-python-0.0.7/twilix/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
 
 def make_get_request(endpoint: str, params: dict = None):
     headers = {
         "Authorization": f"Bearer {api_key}",
     }
     response = requests.get(base_url + endpoint, headers=headers, params=params)
-    ic(response.content.decode())
+    if response.status_code != 200:
+        ic(response.content.decode())
     response.raise_for_status()
     return response.json()
 
 
 def add_objects(collection_name: str, objects: list):
     return make_post_request(
         endpoint=f"/collection/{collection_name}/bulk_insert",
@@ -119,7 +120,14 @@
 
 
 def get_collection_schema(collection_name: str):
     """Get collection schema"""
     return make_get_request(
         endpoint=f"/collection/{collection_name}/schema",
     )
+
+
+def delete_collection(collection_name: str):
+    return make_delete_request(
+        endpoint=f"/collection/{collection_name}/delete",
+        json=None,
+    )
```

