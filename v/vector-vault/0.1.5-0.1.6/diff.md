# Comparing `tmp/vector_vault-0.1.5.tar.gz` & `tmp/vector_vault-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.1.5.tar", last modified: Sun May 21 05:22:39 2023, max compression
+gzip compressed data, was "vector_vault-0.1.6.tar", last modified: Sun May 21 05:38:35 2023, max compression
```

## Comparing `vector_vault-0.1.5.tar` & `vector_vault-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:22:39.417101 vector_vault-0.1.5/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.5/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11742 2023-05-21 05:22:39.416942 vector_vault-0.1.5/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    10990 2023-05-20 22:00:14.000000 vector_vault-0.1.5/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 05:22:39.417145 vector_vault-0.1.5/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1069 2023-05-21 05:20:01.000000 vector_vault-0.1.5/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:22:39.415803 vector_vault-0.1.5/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11742 2023-05-21 05:22:39.000000 vector_vault-0.1.5/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 05:22:39.000000 vector_vault-0.1.5/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 05:22:39.000000 vector_vault-0.1.5/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       53 2023-05-21 05:22:39.000000 vector_vault-0.1.5/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 05:22:39.000000 vector_vault-0.1.5/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:22:39.416744 vector_vault-0.1.5/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.5/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3660 2023-05-20 06:06:36.000000 vector_vault-0.1.5/vectorvault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3331 2023-05-20 04:21:10.000000 vector_vault-0.1.5/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1.5/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.5/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18493 2023-05-21 05:20:35.000000 vector_vault-0.1.5/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.5/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:38:35.423234 vector_vault-0.1.6/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.6/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11742 2023-05-21 05:38:35.423071 vector_vault-0.1.6/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    10990 2023-05-20 22:00:14.000000 vector_vault-0.1.6/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 05:38:35.423271 vector_vault-0.1.6/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1069 2023-05-21 05:38:29.000000 vector_vault-0.1.6/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:38:35.421935 vector_vault-0.1.6/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11742 2023-05-21 05:38:35.000000 vector_vault-0.1.6/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 05:38:35.000000 vector_vault-0.1.6/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 05:38:35.000000 vector_vault-0.1.6/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       53 2023-05-21 05:38:35.000000 vector_vault-0.1.6/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 05:38:35.000000 vector_vault-0.1.6/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:38:35.422894 vector_vault-0.1.6/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.6/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3660 2023-05-20 06:06:36.000000 vector_vault-0.1.6/vectorvault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 05:24:36.000000 vector_vault-0.1.6/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1.6/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.6/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18493 2023-05-21 05:20:35.000000 vector_vault-0.1.6/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.6/vectorvault/wrap.py
```

### Comparing `vector_vault-0.1.5/LICENSE` & `vector_vault-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.5/PKG-INFO` & `vector_vault-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.1.5
+Version: 0.1.6
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.1.5/README.md` & `vector_vault-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.5/setup.py` & `vector_vault-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-0.1.5/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.1.6/vector_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.1.5
+Version: 0.1.6
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.1.5/vectorvault/__init__.py` & `vector_vault-0.1.6/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.5/vectorvault/closedai.py` & `vector_vault-0.1.6/vectorvault/closedai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.5/vectorvault/cloudmanager.py` & `vector_vault-0.1.6/vectorvault/cloudmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
         # Create the OAuth credentials
         credentials = CustomCredentials(self.user, self.api)
 
         # Instantiates a client with the OAuth2 credentials
         self.storage_client = storage.Client(project='vectorvault-361ab', credentials=credentials)
         self.gcloud = self.storage_client.bucket(self.user)
+        print(f'Connected to Vault: {self.vault}')
 
     def vault_exists(self, vault_name):
         return storage.Blob(bucket=self.gcloud, name=vault_name).exists(self.storage_client)
 
     def upload_to_cloud(self, vault_name, content):
         blob = self.gcloud.blob(vault_name)
         blob.upload_from_string(content)
```

### Comparing `vector_vault-0.1.5/vectorvault/creds.py` & `vector_vault-0.1.6/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.5/vectorvault/download.py` & `vector_vault-0.1.6/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.5/vectorvault/vault.py` & `vector_vault-0.1.6/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.5/vectorvault/wrap.py` & `vector_vault-0.1.6/vectorvault/wrap.py`

 * *Files identical despite different names*

