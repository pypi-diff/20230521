# Comparing `tmp/vector_vault-0.1.6.tar.gz` & `tmp/vector_vault-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.1.6.tar", last modified: Sun May 21 05:38:35 2023, max compression
+gzip compressed data, was "vector_vault-0.1.7.tar", last modified: Sun May 21 05:55:43 2023, max compression
```

## Comparing `vector_vault-0.1.6.tar` & `vector_vault-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:38:35.423234 vector_vault-0.1.6/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.6/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11742 2023-05-21 05:38:35.423071 vector_vault-0.1.6/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    10990 2023-05-20 22:00:14.000000 vector_vault-0.1.6/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 05:38:35.423271 vector_vault-0.1.6/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1069 2023-05-21 05:38:29.000000 vector_vault-0.1.6/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:38:35.421935 vector_vault-0.1.6/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11742 2023-05-21 05:38:35.000000 vector_vault-0.1.6/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 05:38:35.000000 vector_vault-0.1.6/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 05:38:35.000000 vector_vault-0.1.6/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       53 2023-05-21 05:38:35.000000 vector_vault-0.1.6/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 05:38:35.000000 vector_vault-0.1.6/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:38:35.422894 vector_vault-0.1.6/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.6/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3660 2023-05-20 06:06:36.000000 vector_vault-0.1.6/vectorvault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 05:24:36.000000 vector_vault-0.1.6/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1.6/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.6/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18493 2023-05-21 05:20:35.000000 vector_vault-0.1.6/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.6/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:55:43.102021 vector_vault-0.1.7/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.7/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 05:55:43.101852 vector_vault-0.1.7/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.1.7/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 05:55:43.102058 vector_vault-0.1.7/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-21 05:46:49.000000 vector_vault-0.1.7/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:55:43.100699 vector_vault-0.1.7/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-21 05:55:43.000000 vector_vault-0.1.7/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 05:55:43.000000 vector_vault-0.1.7/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 05:55:43.000000 vector_vault-0.1.7/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-21 05:55:43.000000 vector_vault-0.1.7/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 05:55:43.000000 vector_vault-0.1.7/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:55:43.101682 vector_vault-0.1.7/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.7/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3945 2023-05-21 05:43:48.000000 vector_vault-0.1.7/vectorvault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3382 2023-05-21 05:24:36.000000 vector_vault-0.1.7/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1.7/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.7/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18588 2023-05-21 05:52:53.000000 vector_vault-0.1.7/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.7/vectorvault/wrap.py
```

### Comparing `vector_vault-0.1.6/LICENSE` & `vector_vault-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.6/PKG-INFO` & `vector_vault-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.1.6
+Version: 0.1.7
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -49,15 +49,15 @@
 
 
 <br>
 <br>
 
 ## Basic usage:
 ```
-from vector_vault import Vault
+from vectorvault import Vault
 
 # Create an instance of the Vault class - a new vault will be created if name does not exist
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='name_of_your_vault)
 
 # Some text data we want to store
 text_data = 'some data'
 
@@ -228,15 +228,15 @@
 vault_response = vault.get_chat(user_input, get_context=True, return_context=True)
 
 answer = vault_response['response']
 print("Question:", user_input, "\n\nAnswer:", answer)
 
 # show the context used to generate the answer
 for item in vault_response['context']['results']:
-    print("\n\n", f"item {item['metadata']['item_index']}")
+    print("\n\n", f"item {item['metadata']['item_id']}")
     print(item['data'])
 
 ```
 
 >> Question: 
 What is a token broker? 
  
@@ -287,15 +287,15 @@
 # Build an AI Cusomter Service Chat Bot
 In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
-from vector_vault import Vault
+from vectorvault import Vault
 
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='Customer Service')
 
 with open('customer_service.txt', 'r') as f:
     vault.add(f.read())
```

### Comparing `vector_vault-0.1.6/README.md` & `vector_vault-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 <br>
 <br>
 
 ## Basic usage:
 ```
-from vector_vault import Vault
+from vectorvault import Vault
 
 # Create an instance of the Vault class - a new vault will be created if name does not exist
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='name_of_your_vault)
 
 # Some text data we want to store
 text_data = 'some data'
 
@@ -209,15 +209,15 @@
 vault_response = vault.get_chat(user_input, get_context=True, return_context=True)
 
 answer = vault_response['response']
 print("Question:", user_input, "\n\nAnswer:", answer)
 
 # show the context used to generate the answer
 for item in vault_response['context']['results']:
-    print("\n\n", f"item {item['metadata']['item_index']}")
+    print("\n\n", f"item {item['metadata']['item_id']}")
     print(item['data'])
 
 ```
 
 >> Question: 
 What is a token broker? 
  
@@ -268,15 +268,15 @@
 # Build an AI Cusomter Service Chat Bot
 In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
-from vector_vault import Vault
+from vectorvault import Vault
 
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='Customer Service')
 
 with open('customer_service.txt', 'r') as f:
     vault.add(f.read())
```

### Comparing `vector_vault-0.1.6/setup.py` & `vector_vault-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
@@ -22,10 +22,11 @@
     install_requires=[
         'numpy',
         'requests',
         'bs4',
         'google-cloud-storage',
         'annoy',
         'openai',
-        # add any other dependencies your package needs
+        'tiktoken',
+        # any other dependencies
     ],
 )
```

### Comparing `vector_vault-0.1.6/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.1.7/vector_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.1.6
+Version: 0.1.7
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -49,15 +49,15 @@
 
 
 <br>
 <br>
 
 ## Basic usage:
 ```
-from vector_vault import Vault
+from vectorvault import Vault
 
 # Create an instance of the Vault class - a new vault will be created if name does not exist
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='name_of_your_vault)
 
 # Some text data we want to store
 text_data = 'some data'
 
@@ -228,15 +228,15 @@
 vault_response = vault.get_chat(user_input, get_context=True, return_context=True)
 
 answer = vault_response['response']
 print("Question:", user_input, "\n\nAnswer:", answer)
 
 # show the context used to generate the answer
 for item in vault_response['context']['results']:
-    print("\n\n", f"item {item['metadata']['item_index']}")
+    print("\n\n", f"item {item['metadata']['item_id']}")
     print(item['data'])
 
 ```
 
 >> Question: 
 What is a token broker? 
  
@@ -287,15 +287,15 @@
 # Build an AI Cusomter Service Chat Bot
 In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
-from vector_vault import Vault
+from vectorvault import Vault
 
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='Customer Service')
 
 with open('customer_service.txt', 'r') as f:
     vault.add(f.read())
```

### Comparing `vector_vault-0.1.6/vectorvault/__init__.py` & `vector_vault-0.1.7/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.6/vectorvault/closedai.py` & `vector_vault-0.1.7/vectorvault/closedai.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # and its suppliers and may be covered by U.S. and Foreign Patents,
 # patents in process, and are protected by trade secret or copyright law.
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
 import openai
+import tiktoken
 
 class ClosedAI:
     def __init__(self) -> None:
         pass
 
     # This function returns a ChatGPT completion based on a provided input.
     def llm(self, user_input, history=None, model='gpt-3.5-turbo'):
@@ -84,7 +85,12 @@
         response = openai.ChatCompletion.create(
             model=model,
             messages=[{"role": "user", "content": f"Summarize the following: {user_input}"}]
         )
         # The API responds with a 'choices' array containing the 'message' object.
         return response['choices'][0]['message']['content']
 
+    def get_tokens(string: str, encoding_name: str = "cl100k_base") -> int:
+        """Returns the number of tokens in a text string."""
+        encoding = tiktoken.get_encoding(encoding_name)
+        num_tokens = len(encoding.encode(string))
+        return num_tokens
```

### Comparing `vector_vault-0.1.6/vectorvault/cloudmanager.py` & `vector_vault-0.1.7/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.6/vectorvault/creds.py` & `vector_vault-0.1.7/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.6/vectorvault/download.py` & `vector_vault-0.1.7/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.6/vectorvault/vault.py` & `vector_vault-0.1.7/vectorvault/vault.py`

 * *Files 4% similar despite different names*

```diff
@@ -316,34 +316,33 @@
         
         time.sleep(self.needed_sleep_time)
         
         texts = []
         text_len = 0
         for item in self.items:
             text = item['text']
-            text_len += len(text)
+            text_len += self.closedai.get_tokens(text)
             texts.append(text)
         num_batches = int(np.ceil(len(texts) / batch_size))
 
         # Prepare the text chunks for all batches
         batches_text_chunks = [
             texts[i * batch_size:min((i + 1) * batch_size, len(texts))]
             for i in range(num_batches)
         ]
         
         # max 350,000 tokens per minute - max requests per minute = 3500
-        # 1 token ~= 4 char - aka 1,400,000 char per min
         if self.first_run == False:
             trip_time = float(start_time - self.last_time)
             req_min = 60 / trip_time # 1 min (60) / time between requests (trip_time)
             projected_chars_per_min = req_min * text_len
-            rate_ratio = projected_chars_per_min / 1500000
+            rate_ratio = projected_chars_per_min / 350000
             print(f'Projected Characters per min:{projected_chars_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {text_len}')
             # 1 min divided by the cap per min and the total we are sending now and factor in the last trip time
-            self.needed_sleep_time = 60 / (1500000 / text_len) - trip_time 
+            self.needed_sleep_time = 60 / (350000 / text_len) - trip_time 
             if self.needed_sleep_time < 0:
                 self.needed_sleep_time = 0
 
             print(f'Time calc to sleep: {self.needed_sleep_time}')
             if req_min > 3500:
                 time.sleep(1)
 
@@ -416,34 +415,33 @@
             self.needed_sleep_time = 0
         
         if not history:
             history = ''
         
         time.sleep(self.needed_sleep_time)
 
-        if len(text) > 15000:
+        if self.closedai.get_tokens(text) > 4000:
             if summary:
                 inputs = self.split_text(text, 14500)
             else:
                 inputs = self.split_text(text)
         else:
             inputs = [text]
         response = ''
         for segment in inputs:
             start_time = time.time()
-            seg_len = len(segment)
+            seg_len = self.closedai.get_tokens(segment)
             # max 90,000 tokens per minute | max requests per minute = 3500
-            # 1 token ~= 4 char - aka 360,000 char per min
             trip_time = float(start_time - self.last_chat_time)
             req_min = 60 / trip_time # 1 min (60) / time between requests (trip_time)
             projected_chars_per_min = req_min * seg_len
-            rate_ratio = projected_chars_per_min / 360000
+            rate_ratio = projected_chars_per_min / 90000
             print(f'Projected Characters per min:{projected_chars_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {seg_len}')
             # 1 min divided by the cap per min and the total we are sending now and factor in the last trip time
-            self.needed_sleep_time = 60 / (360000 / seg_len) - trip_time 
+            self.needed_sleep_time = 60 / (90000 / seg_len) - trip_time 
             if self.needed_sleep_time < 0:
                 self.needed_sleep_time = 0
             print(f'Time calc to sleep: {self.needed_sleep_time}')
 
             if expansion:
                 iq = f"be direct and short. Question: {segment} \n The intent of this question is to: "
                 intent_expansion = self.closedai.llm(iq)
@@ -455,15 +453,17 @@
 
             while True:
                 try:
                     if summary and not get_context:
                         response += self.closedai.summarize(segment, model=model)
                     elif get_context and not summary:
                         user_input = segment + history if history_search else segment
-                        if len(user_input) > 15000:
+                        if self.closedai.get_tokens(user_input) > 4000:
+                            user_input = user_input[-16000:]
+                        if self.closedai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         context = self.get_similar(user_input, n=n_context)
                         response = self.closedai.llm_w_context(segment, context, history, model=model)
                     else:
                         response = self.closedai.llm(segment, history, model=model)
                     break
                 except Exception as e:
```

### Comparing `vector_vault-0.1.6/vectorvault/wrap.py` & `vector_vault-0.1.7/vectorvault/wrap.py`

 * *Files identical despite different names*

