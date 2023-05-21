# Comparing `tmp/vector_vault-0.1.9.tar.gz` & `tmp/vector_vault-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.1.9.tar", last modified: Sun May 21 06:22:05 2023, max compression
+gzip compressed data, was "vector_vault-0.2.tar", last modified: Sun May 21 06:24:42 2023, max compression
```

## Comparing `vector_vault-0.1.9.tar` & `vector_vault-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:22:05.433378 vector_vault-0.1.9/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.9/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 06:22:05.433205 vector_vault-0.1.9/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.1.9/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 06:22:05.433419 vector_vault-0.1.9/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-21 06:21:58.000000 vector_vault-0.1.9/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:22:05.432169 vector_vault-0.1.9/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 06:22:05.000000 vector_vault-0.1.9/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 06:22:05.000000 vector_vault-0.1.9/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 06:22:05.000000 vector_vault-0.1.9/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-21 06:22:05.000000 vector_vault-0.1.9/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 06:22:05.000000 vector_vault-0.1.9/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:22:05.433035 vector_vault-0.1.9/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      672 2023-05-21 06:21:21.000000 vector_vault-0.1.9/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.1.9/vectorvault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3381 2023-05-21 06:14:11.000000 vector_vault-0.1.9/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.1.9/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.9/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18586 2023-05-21 06:21:23.000000 vector_vault-0.1.9/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.9/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:24:42.038416 vector_vault-0.2/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11735 2023-05-21 06:24:42.038227 vector_vault-0.2/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 06:24:42.038458 vector_vault-0.2/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1064 2023-05-21 06:24:31.000000 vector_vault-0.2/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:24:42.036744 vector_vault-0.2/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11735 2023-05-21 06:24:42.000000 vector_vault-0.2/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 06:24:42.000000 vector_vault-0.2/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 06:24:42.000000 vector_vault-0.2/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-21 06:24:42.000000 vector_vault-0.2/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 06:24:42.000000 vector_vault-0.2/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:24:42.038019 vector_vault-0.2/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.2/vectorvault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 06:23:42.000000 vector_vault-0.2/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.2/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18588 2023-05-21 06:23:37.000000 vector_vault-0.2/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2/vectorvault/wrap.py
```

### Comparing `vector_vault-0.1.9/LICENSE` & `vector_vault-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.9/PKG-INFO` & `vector_vault-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.1.9
+Version: 0.2
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.1.9/README.md` & `vector_vault-0.2/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.9/setup.py` & `vector_vault-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.1.9",
+    version="0.2",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-0.1.9/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.2/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.1.9
+Version: 0.2
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.1.9/vectorvault/__init__.py` & `vector_vault-0.2/vectorvault/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 # herein are proprietary to Vector Vault
 # and its suppliers and may be covered by U.S. and Foreign Patents,
 # patents in process, and are protected by trade secret or copyright law.
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
-from vault import Vault
-from download import download_url
-from wrap import wrap
+from .vault import Vault
+from .download import download_url
+from .wrap import wrap
```

### Comparing `vector_vault-0.1.9/vectorvault/closedai.py` & `vector_vault-0.2/vectorvault/closedai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.9/vectorvault/cloudmanager.py` & `vector_vault-0.2/vectorvault/cloudmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
 import tempfile
 import os
 import json
-from creds import CustomCredentials
+from .creds import CustomCredentials
 from google.cloud import storage
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 
 class CloudManager:
     def __init__(self, user: str, api_key: str, vault: str):
         self.user = user
```

### Comparing `vector_vault-0.1.9/vectorvault/creds.py` & `vector_vault-0.2/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.9/vectorvault/download.py` & `vector_vault-0.2/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.9/vectorvault/vault.py` & `vector_vault-0.2/vectorvault/vault.py`

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
-from cloudmanager import CloudManager
-from closedai import ClosedAI
+from .cloudmanager import CloudManager
+from .closedai import ClosedAI
 
 
 class Vault:
     def __init__(self, user: str, api_key: str, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = AnnoyIndex(dims, 'angular')
         self.dims = dims
```

### Comparing `vector_vault-0.1.9/vectorvault/wrap.py` & `vector_vault-0.2/vectorvault/wrap.py`

 * *Files identical despite different names*

