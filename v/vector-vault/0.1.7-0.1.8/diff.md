# Comparing `tmp/vector_vault-0.1.7.tar.gz` & `tmp/vector_vault-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.1.7.tar", last modified: Sun May 21 05:55:43 2023, max compression
+gzip compressed data, was "vector_vault-0.1.8.tar", last modified: Sun May 21 06:15:52 2023, max compression
```

## Comparing `vector_vault-0.1.7.tar` & `vector_vault-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:55:43.102021 vector_vault-0.1.7/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.7/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 05:55:43.101852 vector_vault-0.1.7/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.1.7/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 05:55:43.102058 vector_vault-0.1.7/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-21 05:46:49.000000 vector_vault-0.1.7/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:55:43.100699 vector_vault-0.1.7/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 05:55:43.000000 vector_vault-0.1.7/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 05:55:43.000000 vector_vault-0.1.7/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 05:55:43.000000 vector_vault-0.1.7/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-21 05:55:43.000000 vector_vault-0.1.7/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 05:55:43.000000 vector_vault-0.1.7/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:55:43.101682 vector_vault-0.1.7/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.7/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3945 2023-05-21 05:43:48.000000 vector_vault-0.1.7/vectorvault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 05:24:36.000000 vector_vault-0.1.7/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1.7/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.7/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18588 2023-05-21 05:52:53.000000 vector_vault-0.1.7/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.7/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:15:52.565750 vector_vault-0.1.8/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.8/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 06:15:52.565595 vector_vault-0.1.8/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.1.8/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 06:15:52.565786 vector_vault-0.1.8/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-21 06:15:48.000000 vector_vault-0.1.8/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:15:52.564348 vector_vault-0.1.8/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 06:15:52.000000 vector_vault-0.1.8/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 06:15:52.000000 vector_vault-0.1.8/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 06:15:52.000000 vector_vault-0.1.8/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-21 06:15:52.000000 vector_vault-0.1.8/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 06:15:52.000000 vector_vault-0.1.8/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:15:52.565284 vector_vault-0.1.8/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.8/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:15:12.000000 vector_vault-0.1.8/vectorvault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3381 2023-05-21 06:14:11.000000 vector_vault-0.1.8/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.1.8/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.8/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18586 2023-05-21 06:14:15.000000 vector_vault-0.1.8/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.8/vectorvault/wrap.py
```

### Comparing `vector_vault-0.1.7/LICENSE` & `vector_vault-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.7/PKG-INFO` & `vector_vault-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.1.7
+Version: 0.1.8
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.1.7/README.md` & `vector_vault-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.7/setup.py` & `vector_vault-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-0.1.7/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.1.8/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.1.7
+Version: 0.1.8
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.1.7/vectorvault/__init__.py` & `vector_vault-0.1.8/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.7/vectorvault/closedai.py` & `vector_vault-0.1.8/vectorvault/closedai.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,12 +85,12 @@
         response = openai.ChatCompletion.create(
             model=model,
             messages=[{"role": "user", "content": f"Summarize the following: {user_input}"}]
         )
         # The API responds with a 'choices' array containing the 'message' object.
         return response['choices'][0]['message']['content']
 
-    def get_tokens(string: str, encoding_name: str = "cl100k_base") -> int:
+    def get_tokens(self, string: str, encoding_name: str = "cl100k_base") -> int:
         """Returns the number of tokens in a text string."""
         encoding = tiktoken.get_encoding(encoding_name)
         num_tokens = len(encoding.encode(string))
         return num_tokens
```

### Comparing `vector_vault-0.1.7/vectorvault/cloudmanager.py` & `vector_vault-0.1.8/vectorvault/cloudmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
 import tempfile
 import os
 import json
-from .creds import CustomCredentials
+from creds import CustomCredentials
 from google.cloud import storage
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 
 class CloudManager:
     def __init__(self, user: str, api_key: str, vault: str):
         self.user = user
```

### Comparing `vector_vault-0.1.7/vectorvault/creds.py` & `vector_vault-0.1.8/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.7/vectorvault/download.py` & `vector_vault-0.1.8/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.7/vectorvault/vault.py` & `vector_vault-0.1.8/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import datetime
 import time
 import json
 import re
 import openai
 from annoy import AnnoyIndex
 from concurrent.futures import ThreadPoolExecutor
-from .cloudmanager import CloudManager
-from .closedai import ClosedAI
+from cloudmanager import CloudManager
+from closedai import ClosedAI
 
 
 class Vault:
     def __init__(self, user: str, api_key: str, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = AnnoyIndex(dims, 'angular')
         self.dims = dims
```

### Comparing `vector_vault-0.1.7/vectorvault/wrap.py` & `vector_vault-0.1.8/vectorvault/wrap.py`

 * *Files identical despite different names*

