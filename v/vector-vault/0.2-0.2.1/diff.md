# Comparing `tmp/vector_vault-0.2.tar.gz` & `tmp/vector_vault-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.2.tar", last modified: Sun May 21 06:24:42 2023, max compression
+gzip compressed data, was "vector_vault-0.2.1.tar", last modified: Sun May 21 06:32:31 2023, max compression
```

## Comparing `vector_vault-0.2.tar` & `vector_vault-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:24:42.038416 vector_vault-0.2/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11735 2023-05-21 06:24:42.038227 vector_vault-0.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 06:24:42.038458 vector_vault-0.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1064 2023-05-21 06:24:31.000000 vector_vault-0.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:24:42.036744 vector_vault-0.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11735 2023-05-21 06:24:42.000000 vector_vault-0.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 06:24:42.000000 vector_vault-0.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 06:24:42.000000 vector_vault-0.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-21 06:24:42.000000 vector_vault-0.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 06:24:42.000000 vector_vault-0.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:24:42.038019 vector_vault-0.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.2/vectorvault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 06:23:42.000000 vector_vault-0.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18588 2023-05-21 06:23:37.000000 vector_vault-0.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:32:30.999871 vector_vault-0.2.1/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.1/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 06:32:30.999677 vector_vault-0.2.1/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2.1/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 06:32:30.999910 vector_vault-0.2.1/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-21 06:32:23.000000 vector_vault-0.2.1/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:32:30.998264 vector_vault-0.2.1/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 06:32:30.000000 vector_vault-0.2.1/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 06:32:30.000000 vector_vault-0.2.1/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 06:32:30.000000 vector_vault-0.2.1/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-21 06:32:30.000000 vector_vault-0.2.1/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 06:32:30.000000 vector_vault-0.2.1/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 06:32:30.999487 vector_vault-0.2.1/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.1/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3951 2023-05-21 06:21:17.000000 vector_vault-0.2.1/vectorvault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 06:23:42.000000 vector_vault-0.2.1/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-21 06:14:10.000000 vector_vault-0.2.1/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.1/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18832 2023-05-21 06:31:42.000000 vector_vault-0.2.1/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.1/vectorvault/wrap.py
```

### Comparing `vector_vault-0.2/LICENSE` & `vector_vault-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2/PKG-INFO` & `vector_vault-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.2
+Version: 0.2.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.2/README.md` & `vector_vault-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2/setup.py` & `vector_vault-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.2",
+    version="0.2.1",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-0.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.2.1/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.2
+Version: 0.2.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `vector_vault-0.2/vectorvault/__init__.py` & `vector_vault-0.2.1/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2/vectorvault/closedai.py` & `vector_vault-0.2.1/vectorvault/closedai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2/vectorvault/cloudmanager.py` & `vector_vault-0.2.1/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2/vectorvault/creds.py` & `vector_vault-0.2.1/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2/vectorvault/download.py` & `vector_vault-0.2.1/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2/vectorvault/vault.py` & `vector_vault-0.2.1/vectorvault/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,16 @@
         self.items.clear()
 
         if self.verbose:
             print("save vectors time --- %s seconds ---" % (time.time() - start_time))
 
 
     def delete(self):
-        print('Deleting started. Note: this can take a while for large datasets')
+        if self.verbose == True:
+                print('Deleting started. Note: this can take a while for large datasets')
         # Clear the local vector data
         self.vectors = AnnoyIndex(self.dims, 'angular')
         self.items.clear()
         self.x = 0
         self.cloud_manager.delete()
         print('Vault deleted')
     
@@ -230,15 +231,16 @@
     def add(self, text: str, meta: dict = None, name: str = None):
         """
             If your text length lenght is greater than 15000 characters, Vault.split_text(your_text)  
             will automatically be added
         """
 
         if len(text) > 14000:
-            print('Text length too long. Using the built-in "split_text()" function to get a list of text segments') 
+            if self.verbose == True:
+                print('Text length too long. Using the built-in "split_text()" function to get a list of text segments') 
             texts = self.split_text(text) # returns list of text segments
         else:
             texts = [text]
 
         for text in texts:
             self.add_item(text)
 
@@ -330,23 +332,25 @@
             for i in range(num_batches)
         ]
         
         # max 350,000 tokens per minute - max requests per minute = 3500
         if self.first_run == False:
             trip_time = float(start_time - self.last_time)
             req_min = 60 / trip_time # 1 min (60) / time between requests (trip_time)
-            projected_chars_per_min = req_min * text_len
-            rate_ratio = projected_chars_per_min / 350000
-            print(f'Projected Characters per min:{projected_chars_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {text_len}')
+            projected_tokens_per_min = req_min * text_len
+            rate_ratio = projected_tokens_per_min / 350000
+            if self.verbose == True:
+                print(f'Projected Tokens per min:{projected_tokens_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {text_len}')
             # 1 min divided by the cap per min and the total we are sending now and factor in the last trip time
             self.needed_sleep_time = 60 / (350000 / text_len) - trip_time 
             if self.needed_sleep_time < 0:
                 self.needed_sleep_time = 0
 
-            print(f'Time calc to sleep: {self.needed_sleep_time}')
+            if self.verbose == True:
+                print(f'Time calc to sleep: {self.needed_sleep_time}')
             if req_min > 3500:
                 time.sleep(1)
 
         # Process the batches in parallel using ThreadPoolExecutor
         with ThreadPoolExecutor() as executor:
             process_batch_with_params = lambda batch_text_chunks: self.process_batch(batch_text_chunks, never_stop, loop_timeout)
             batch_embeddings_list = list(executor.map(process_batch_with_params, batches_text_chunks))
@@ -429,22 +433,24 @@
         response = ''
         for segment in inputs:
             start_time = time.time()
             seg_len = self.closedai.get_tokens(segment)
             # max 90,000 tokens per minute | max requests per minute = 3500
             trip_time = float(start_time - self.last_chat_time)
             req_min = 60 / trip_time # 1 min (60) / time between requests (trip_time)
-            projected_chars_per_min = req_min * seg_len
-            rate_ratio = projected_chars_per_min / 90000
-            print(f'Projected Characters per min:{projected_chars_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {seg_len}')
+            projected_tokens_per_min = req_min * seg_len
+            rate_ratio = projected_tokens_per_min / 90000
+            if self.verbose == True:
+                print(f'Projected Tokens per min:{projected_tokens_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {seg_len}')
             # 1 min divided by the cap per min and the total we are sending now and factor in the last trip time
             self.needed_sleep_time = 60 / (90000 / seg_len) - trip_time 
             if self.needed_sleep_time < 0:
                 self.needed_sleep_time = 0
-            print(f'Time calc to sleep: {self.needed_sleep_time}')
+            if self.verbose == True:
+                print(f'Time calc to sleep: {self.needed_sleep_time}')
 
             if expansion:
                 iq = f"be direct and short. Question: {segment} \n The intent of this question is to: "
                 intent_expansion = self.closedai.llm(iq)
                 kq = f"be general, direct, and short. Don't give an answer, only topics this question falls under to this question: {segment}"
                 knowledge_expansion = self.closedai.llm(kq)
                 segment = f'question_intent: {intent_expansion} | {knowledge_expansion}\n\
```

### Comparing `vector_vault-0.2/vectorvault/wrap.py` & `vector_vault-0.2.1/vectorvault/wrap.py`

 * *Files identical despite different names*

