# Comparing `tmp/vector_vault-0.2.2.tar.gz` & `tmp/vector_vault-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.2.2.tar", last modified: Sun May 21 18:30:51 2023, max compression
+gzip compressed data, was "vector_vault-0.2.3.tar", last modified: Sun May 21 18:37:17 2023, max compression
```

## Comparing `vector_vault-0.2.2.tar` & `vector_vault-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 18:30:51.070410 vector_vault-0.2.2/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 18:30:51.070210 vector_vault-0.2.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 18:30:51.070460 vector_vault-0.2.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-21 18:30:47.000000 vector_vault-0.2.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 18:30:51.067772 vector_vault-0.2.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 18:30:51.000000 vector_vault-0.2.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 18:30:51.000000 vector_vault-0.2.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 18:30:51.000000 vector_vault-0.2.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-21 18:30:51.000000 vector_vault-0.2.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 18:30:51.000000 vector_vault-0.2.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 18:30:51.069793 vector_vault-0.2.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.2.2/vectorvault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 06:23:42.000000 vector_vault-0.2.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.2.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18868 2023-05-21 18:30:31.000000 vector_vault-0.2.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 18:37:17.107588 vector_vault-0.2.3/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.3/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 18:37:17.107430 vector_vault-0.2.3/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2.3/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 18:37:17.107635 vector_vault-0.2.3/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-21 18:37:11.000000 vector_vault-0.2.3/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 18:37:17.106001 vector_vault-0.2.3/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 18:37:17.000000 vector_vault-0.2.3/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 18:37:17.000000 vector_vault-0.2.3/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 18:37:17.000000 vector_vault-0.2.3/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-21 18:37:17.000000 vector_vault-0.2.3/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 18:37:17.000000 vector_vault-0.2.3/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 18:37:17.107249 vector_vault-0.2.3/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.3/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.2.3/vectorvault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 06:23:42.000000 vector_vault-0.2.3/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.2.3/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.3/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18832 2023-05-21 18:36:59.000000 vector_vault-0.2.3/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.3/vectorvault/wrap.py
```

### Comparing `vector_vault-0.2.2/LICENSE` & `vector_vault-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.2/PKG-INFO` & `vector_vault-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.2.2
+Version: 0.2.3
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.2.2/README.md` & `vector_vault-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.2/setup.py` & `vector_vault-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-0.2.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.2.3/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.2.2
+Version: 0.2.3
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.2.2/vectorvault/__init__.py` & `vector_vault-0.2.3/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.2/vectorvault/closedai.py` & `vector_vault-0.2.3/vectorvault/closedai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.2/vectorvault/cloudmanager.py` & `vector_vault-0.2.3/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.2/vectorvault/creds.py` & `vector_vault-0.2.3/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.2/vectorvault/download.py` & `vector_vault-0.2.3/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.2/vectorvault/vault.py` & `vector_vault-0.2.3/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,16 +312,14 @@
         start_time = time.time()
         if not self.last_time:
             self.last_time = start_time - 1
         
         if not self.needed_sleep_time:
             self.needed_sleep_time = 0
         
-        self.check_index()
-        
         time.sleep(self.needed_sleep_time)
         
         texts = []
         text_len = 0
         for item in self.items:
             text = item['text']
             text_len += self.closedai.get_tokens(text)
```

### Comparing `vector_vault-0.2.2/vectorvault/wrap.py` & `vector_vault-0.2.3/vectorvault/wrap.py`

 * *Files identical despite different names*

