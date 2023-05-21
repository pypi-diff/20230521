# Comparing `tmp/vector_vault-0.1.4.tar.gz` & `tmp/vector_vault-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.1.4.tar", last modified: Sat May 20 07:50:02 2023, max compression
+gzip compressed data, was "vector_vault-0.1.5.tar", last modified: Sun May 21 05:22:39 2023, max compression
```

## Comparing `vector_vault-0.1.4.tar` & `vector_vault-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 07:50:02.896703 vector_vault-0.1.4/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.4/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)     9736 2023-05-20 07:50:02.896551 vector_vault-0.1.4/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)     8971 2023-05-20 07:49:21.000000 vector_vault-0.1.4/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-20 07:50:02.896737 vector_vault-0.1.4/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1082 2023-05-20 07:49:52.000000 vector_vault-0.1.4/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 07:50:02.895711 vector_vault-0.1.4/vector_vault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.4/vector_vault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3660 2023-05-20 06:06:36.000000 vector_vault-0.1.4/vector_vault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3331 2023-05-20 04:21:10.000000 vector_vault-0.1.4/vector_vault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1.4/vector_vault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.4/vector_vault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18515 2023-05-20 06:46:35.000000 vector_vault-0.1.4/vector_vault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.4/vector_vault/wrap.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 07:50:02.896371 vector_vault-0.1.4/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)     9736 2023-05-20 07:50:02.000000 vector_vault-0.1.4/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      374 2023-05-20 07:50:02.000000 vector_vault-0.1.4/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-20 07:50:02.000000 vector_vault-0.1.4/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       53 2023-05-20 07:50:02.000000 vector_vault-0.1.4/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       13 2023-05-20 07:50:02.000000 vector_vault-0.1.4/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:22:39.417101 vector_vault-0.1.5/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.5/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11742 2023-05-21 05:22:39.416942 vector_vault-0.1.5/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    10990 2023-05-20 22:00:14.000000 vector_vault-0.1.5/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-21 05:22:39.417145 vector_vault-0.1.5/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1069 2023-05-21 05:20:01.000000 vector_vault-0.1.5/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:22:39.415803 vector_vault-0.1.5/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11742 2023-05-21 05:22:39.000000 vector_vault-0.1.5/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      367 2023-05-21 05:22:39.000000 vector_vault-0.1.5/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-21 05:22:39.000000 vector_vault-0.1.5/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       53 2023-05-21 05:22:39.000000 vector_vault-0.1.5/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-21 05:22:39.000000 vector_vault-0.1.5/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-21 05:22:39.416744 vector_vault-0.1.5/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.5/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3660 2023-05-20 06:06:36.000000 vector_vault-0.1.5/vectorvault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3331 2023-05-20 04:21:10.000000 vector_vault-0.1.5/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1.5/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.5/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18493 2023-05-21 05:20:35.000000 vector_vault-0.1.5/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.5/vectorvault/wrap.py
```

### Comparing `vector_vault-0.1.4/LICENSE` & `vector_vault-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.4/PKG-INFO` & `vector_vault-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.1.4
-Summary: Vector Vault: Simplified vector database management and secure cloud storage for data science and machine learning workflows.
-Home-page: http://github.com/John-Rood/vector_vault
+Version: 0.1.5
+Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
+Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-VectorVault is designed to simplify the process of working with vector databases. It allows users to manage vector databases efficiently, integrated and accessed seamlessly from the cloud. It's scalable, suitable for both small and large scale databases, and designed with a user-friendly interface. Furthermore, it simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" - simply and easily.
+VectorVault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. VectorVault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
 
-VectorVault was built with the goal of making complex work flows, that utilize vector databases for informed generative ai, simple and easy. By combining similarity vector search with generative ai chat, new possibilities for conversation and communication emerge. Product information can be added to a vault, and then when customers ask a product question, the right information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news and entertainment, to ai code reviews that reference documentation, and much more.
+VectorVault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledges, and much more.
 
 VectorVault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a VectorVault account in order to get your user id and api key for cloud access. If you don't already have one, you can sign up free at [VectorVault.io](https://vectorvault.io)
 
 This python library allows you to interact with VectorVault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
 
+<br>
 
 # Interact with your Vault:
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
 <br>
 `add_item` : Add item to the Vault
 <br>
@@ -46,15 +47,15 @@
 <br>
 `get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
 
 
 <br>
 <br>
 
-Basic usage:
+## Basic usage:
 ```
 from vector_vault import Vault
 
 # Create an instance of the Vault class - a new vault will be created if name does not exist
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='name_of_your_vault)
 
 # Some text data we want to store
@@ -89,29 +90,29 @@
 vault.save()
 ```
 
 <br>
 <br>
 
 vault.add() is cool. You can add any length of text, even a full book...and it will be all automatically split and processed.
-vault.get_vectors() is also cool, because you can vault.add() as much as you want, then when you're done, process all the vectors at once with a vault.get_vectors() - Internally batch processes vector embeddings with OpenAI's text embeddings ada 002, and comes with auto rate-limiting and concurrent requests for maximum speed
+vault.get_vectors() is also cool, because you can vault.add() as much as you want, then when you're done, process all the vectors at once with a vault.get_vectors() - Internally batches vector embeddings with OpenAI's text embeddings ada 002, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 ```
 vault.add(insanely_large_text_data)
 vault.get_vectors() 
 vault.save() 
 ```
-
+^ these three lines execute fast and can be called as often as you like. For example: `add`, `get_vectors`, and `save` can be used mid conversation to add every message to the vault one at a time as they comes in.
 
 
 <br>
 <br>
 
-## When you want to use the vault later:
+## Use the vault later:
 ```
 similar_data = vault.get_similar(text_input) # returns a list with 4 results
 similar_data = vault.get_similar(text_input, n = 10) # returns 10 results
 
 # Print each similar item 
 for result in similar_data:
     print(result['data'])
@@ -119,21 +120,21 @@
 
 
 <br>
 
 ## Use the get_chat() function to get a response from chatgpt
 The following searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the context
 ```
-user_input = "This text is going to be used find contextually similar references in the vault"
+question = "This text is going to be used find contextually similar references in the vault"
 
-answer = vault.get_chat(user_input, get_context=True)  
+answer = vault.get_chat(question, get_context=True)  
 print(answer)
 
-# The following line will just send chatgpt the user_input and not interact with the vault in any way
-answer = vault.get_chat(user_input) 
+# The following line will send chatgpt the question for response and not interact with the vault in any way
+answer = vault.get_chat(question) 
 ```
 
 
 <br>
 <br>
 
 # Change Vault
@@ -205,15 +206,15 @@
 
 # print context:
 for item in vault_response['context']['results']:
     print("\n\n", f"item {item['metadata']['item_id']}")
     print(item['data'])
 ```
 
-## Summarize:
+# Summarize Anything:
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
 ```
 summary = vault.get_chat(text, summary=True)
 ```
 
 <br>
 <br>
@@ -272,9 +273,57 @@
 print("Question:", user_input2, "\n\nAnswer:", vault_response2)
 ```
 >> Question: 
 How do I use it? 
  
 >>Answer: 
 You can use it by...
->>
+
+
+
+<br>
+<br>
+<br>
+
+# Build an AI Cusomter Service Chat Bot
+In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
+
+<br>
+
+### Create the Customer Service Vault
+```
+from vector_vault import Vault
+
+os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
+
+vault = Vault(user='your_user_id', api_key='your_api_key', vault='Customer Service')
+
+with open('customer_service.txt', 'r') as f:
+    vault.add(f.read())
+
+vault.get_vectors()
+
+vault.save()
+```
+
+<br>
+
+And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` function with `get_context=True`. The call `get_chat(text, get_context=True)` will take the customer's question, search the vault, find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
+
+```
+question = 'customer question text string'
+
+answer = vault.get_chat(question, get_context=True)
+```
+
+That's all it takes to create an ai customer service chatbot that responds to your customers as well as any support rep!
+
+
+<br>
+<br>
+
+If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
+
+Happy coding.
+
+
```

### Comparing `vector_vault-0.1.4/README.md` & `vector_vault-0.1.5/vector_vault.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,35 @@
-VectorVault is designed to simplify the process of working with vector databases. It allows users to manage vector databases efficiently, integrated and accessed seamlessly from the cloud. It's scalable, suitable for both small and large scale databases, and designed with a user-friendly interface. Furthermore, it simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" - simply and easily.
+Metadata-Version: 2.1
+Name: vector-vault
+Version: 0.1.5
+Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
+Home-page: https://github.com/John-Rood/VectorVault
+Author: VectorVault.io
+Author-email: john@johnrood.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-VectorVault was built with the goal of making complex work flows, that utilize vector databases for informed generative ai, simple and easy. By combining similarity vector search with generative ai chat, new possibilities for conversation and communication emerge. Product information can be added to a vault, and then when customers ask a product question, the right information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news and entertainment, to ai code reviews that reference documentation, and much more.
+VectorVault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. VectorVault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
+
+VectorVault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledges, and much more.
 
 VectorVault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a VectorVault account in order to get your user id and api key for cloud access. If you don't already have one, you can sign up free at [VectorVault.io](https://vectorvault.io)
 
 This python library allows you to interact with VectorVault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
 
+<br>
 
 # Interact with your Vault:
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
 <br>
 `add_item` : Add item to the Vault
 <br>
@@ -27,15 +47,15 @@
 <br>
 `get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
 
 
 <br>
 <br>
 
-Basic usage:
+## Basic usage:
 ```
 from vector_vault import Vault
 
 # Create an instance of the Vault class - a new vault will be created if name does not exist
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='name_of_your_vault)
 
 # Some text data we want to store
@@ -70,29 +90,29 @@
 vault.save()
 ```
 
 <br>
 <br>
 
 vault.add() is cool. You can add any length of text, even a full book...and it will be all automatically split and processed.
-vault.get_vectors() is also cool, because you can vault.add() as much as you want, then when you're done, process all the vectors at once with a vault.get_vectors() - Internally batch processes vector embeddings with OpenAI's text embeddings ada 002, and comes with auto rate-limiting and concurrent requests for maximum speed
+vault.get_vectors() is also cool, because you can vault.add() as much as you want, then when you're done, process all the vectors at once with a vault.get_vectors() - Internally batches vector embeddings with OpenAI's text embeddings ada 002, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 ```
 vault.add(insanely_large_text_data)
 vault.get_vectors() 
 vault.save() 
 ```
-
+^ these three lines execute fast and can be called as often as you like. For example: `add`, `get_vectors`, and `save` can be used mid conversation to add every message to the vault one at a time as they comes in.
 
 
 <br>
 <br>
 
-## When you want to use the vault later:
+## Use the vault later:
 ```
 similar_data = vault.get_similar(text_input) # returns a list with 4 results
 similar_data = vault.get_similar(text_input, n = 10) # returns 10 results
 
 # Print each similar item 
 for result in similar_data:
     print(result['data'])
@@ -100,21 +120,21 @@
 
 
 <br>
 
 ## Use the get_chat() function to get a response from chatgpt
 The following searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the context
 ```
-user_input = "This text is going to be used find contextually similar references in the vault"
+question = "This text is going to be used find contextually similar references in the vault"
 
-answer = vault.get_chat(user_input, get_context=True)  
+answer = vault.get_chat(question, get_context=True)  
 print(answer)
 
-# The following line will just send chatgpt the user_input and not interact with the vault in any way
-answer = vault.get_chat(user_input) 
+# The following line will send chatgpt the question for response and not interact with the vault in any way
+answer = vault.get_chat(question) 
 ```
 
 
 <br>
 <br>
 
 # Change Vault
@@ -186,15 +206,15 @@
 
 # print context:
 for item in vault_response['context']['results']:
     print("\n\n", f"item {item['metadata']['item_id']}")
     print(item['data'])
 ```
 
-## Summarize:
+# Summarize Anything:
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
 ```
 summary = vault.get_chat(text, summary=True)
 ```
 
 <br>
 <br>
@@ -253,8 +273,57 @@
 print("Question:", user_input2, "\n\nAnswer:", vault_response2)
 ```
 >> Question: 
 How do I use it? 
  
 >>Answer: 
 You can use it by...
->>
+
+
+
+<br>
+<br>
+<br>
+
+# Build an AI Cusomter Service Chat Bot
+In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
+
+<br>
+
+### Create the Customer Service Vault
+```
+from vector_vault import Vault
+
+os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
+
+vault = Vault(user='your_user_id', api_key='your_api_key', vault='Customer Service')
+
+with open('customer_service.txt', 'r') as f:
+    vault.add(f.read())
+
+vault.get_vectors()
+
+vault.save()
+```
+
+<br>
+
+And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` function with `get_context=True`. The call `get_chat(text, get_context=True)` will take the customer's question, search the vault, find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
+
+```
+question = 'customer question text string'
+
+answer = vault.get_chat(question, get_context=True)
+```
+
+That's all it takes to create an ai customer service chatbot that responds to your customers as well as any support rep!
+
+
+<br>
+<br>
+
+If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
+
+Happy coding.
+
+
+
```

### Comparing `vector_vault-0.1.4/setup.py` & `vector_vault-0.1.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
-    description="Vector Vault: Simplified vector database management and secure cloud storage for data science and machine learning workflows.",
+    description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
-    url="http://github.com/John-Rood/vector_vault",
+    url="https://github.com/John-Rood/VectorVault",
     classifiers=[
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     install_requires=[
         'numpy',
-        'openai',
-        'annoy',
-        'google-cloud-storage',
         'requests',
         'bs4',
+        'google-cloud-storage',
+        'annoy',
+        'openai',
         # add any other dependencies your package needs
     ],
 )
```

### Comparing `vector_vault-0.1.4/vector_vault/__init__.py` & `vector_vault-0.1.5/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.4/vector_vault/closedai.py` & `vector_vault-0.1.5/vectorvault/closedai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.4/vector_vault/cloudmanager.py` & `vector_vault-0.1.5/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.4/vector_vault/creds.py` & `vector_vault-0.1.5/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.4/vector_vault/download.py` & `vector_vault-0.1.5/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.4/vector_vault/vault.py` & `vector_vault-0.1.5/vectorvault/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,22 +178,22 @@
 
         # Create a return dictionary
         return_dict = {
             "results": results
         }
 
         if self.verbose == True:
-            print(f"get {num_items} items back --- %s seconds ---" % (time.time() - start_time))
+            print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time))
 
         return return_dict
     
 
-    def get_similar(self, text, num_items: int = 4):
+    def get_similar(self, text, n: int = 4):
         vector = self.process_batch([text], never_stop=False, loop_timeout=180)[0]
-        return self.get_items_by_vector(vector, num_items)
+        return self.get_items_by_vector(vector, n)
 
 
     def add_item(self, text: str, meta: dict = None, name: str = None):
         """
             If your text length lenght is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
@@ -457,15 +457,15 @@
                 try:
                     if summary and not get_context:
                         response += self.closedai.summarize(segment, model=model)
                     elif get_context and not summary:
                         user_input = segment + history if history_search else segment
                         if len(user_input) > 15000:
                             user_input = user_input[-15000:]
-                        context = self.get_similar(user_input, n_context)
+                        context = self.get_similar(user_input, n=n_context)
                         response = self.closedai.llm_w_context(segment, context, history, model=model)
                     else:
                         response = self.closedai.llm(segment, history, model=model)
                     break
                 except Exception as e:
                     print(f"API Error: {e}. Sleeping 15 seconds")
                     time.sleep(15)
```

### Comparing `vector_vault-0.1.4/vector_vault/wrap.py` & `vector_vault-0.1.5/vectorvault/wrap.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.4/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,16 @@
-Metadata-Version: 2.1
-Name: vector-vault
-Version: 0.1.4
-Summary: Vector Vault: Simplified vector database management and secure cloud storage for data science and machine learning workflows.
-Home-page: http://github.com/John-Rood/vector_vault
-Author: VectorVault.io
-Author-email: john@johnrood.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
+VectorVault is designed to simplify the process of working with vector databases. It allows users to vectorize datasets efficiently, and access them seamlessly from the cloud. It's scalable and suitable for both small and large scale projects. VectorVault has been designed with a user-friendly interface to make the process of working with vector databases easy and let you focus on what matters. It simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" 
 
-VectorVault is designed to simplify the process of working with vector databases. It allows users to manage vector databases efficiently, integrated and accessed seamlessly from the cloud. It's scalable, suitable for both small and large scale databases, and designed with a user-friendly interface. Furthermore, it simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" - simply and easily.
-
-VectorVault was built with the goal of making complex work flows, that utilize vector databases for informed generative ai, simple and easy. By combining similarity vector search with generative ai chat, new possibilities for conversation and communication emerge. Product information can be added to a vault, and then when customers ask a product question, the right information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news and entertainment, to ai code reviews that reference documentation, and much more.
+VectorVault was built with the goal of making generative ai work flows simple and easy. By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledges, and much more.
 
 VectorVault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a VectorVault account in order to get your user id and api key for cloud access. If you don't already have one, you can sign up free at [VectorVault.io](https://vectorvault.io)
 
 This python library allows you to interact with VectorVault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
 
+<br>
 
 # Interact with your Vault:
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
 <br>
 `add_item` : Add item to the Vault
 <br>
@@ -46,15 +28,15 @@
 <br>
 `get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
 
 
 <br>
 <br>
 
-Basic usage:
+## Basic usage:
 ```
 from vector_vault import Vault
 
 # Create an instance of the Vault class - a new vault will be created if name does not exist
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='name_of_your_vault)
 
 # Some text data we want to store
@@ -89,29 +71,29 @@
 vault.save()
 ```
 
 <br>
 <br>
 
 vault.add() is cool. You can add any length of text, even a full book...and it will be all automatically split and processed.
-vault.get_vectors() is also cool, because you can vault.add() as much as you want, then when you're done, process all the vectors at once with a vault.get_vectors() - Internally batch processes vector embeddings with OpenAI's text embeddings ada 002, and comes with auto rate-limiting and concurrent requests for maximum speed
+vault.get_vectors() is also cool, because you can vault.add() as much as you want, then when you're done, process all the vectors at once with a vault.get_vectors() - Internally batches vector embeddings with OpenAI's text embeddings ada 002, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 ```
 vault.add(insanely_large_text_data)
 vault.get_vectors() 
 vault.save() 
 ```
-
+^ these three lines execute fast and can be called as often as you like. For example: `add`, `get_vectors`, and `save` can be used mid conversation to add every message to the vault one at a time as they comes in.
 
 
 <br>
 <br>
 
-## When you want to use the vault later:
+## Use the vault later:
 ```
 similar_data = vault.get_similar(text_input) # returns a list with 4 results
 similar_data = vault.get_similar(text_input, n = 10) # returns 10 results
 
 # Print each similar item 
 for result in similar_data:
     print(result['data'])
@@ -119,21 +101,21 @@
 
 
 <br>
 
 ## Use the get_chat() function to get a response from chatgpt
 The following searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the context
 ```
-user_input = "This text is going to be used find contextually similar references in the vault"
+question = "This text is going to be used find contextually similar references in the vault"
 
-answer = vault.get_chat(user_input, get_context=True)  
+answer = vault.get_chat(question, get_context=True)  
 print(answer)
 
-# The following line will just send chatgpt the user_input and not interact with the vault in any way
-answer = vault.get_chat(user_input) 
+# The following line will send chatgpt the question for response and not interact with the vault in any way
+answer = vault.get_chat(question) 
 ```
 
 
 <br>
 <br>
 
 # Change Vault
@@ -205,15 +187,15 @@
 
 # print context:
 for item in vault_response['context']['results']:
     print("\n\n", f"item {item['metadata']['item_id']}")
     print(item['data'])
 ```
 
-## Summarize:
+# Summarize Anything:
 You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
 ```
 summary = vault.get_chat(text, summary=True)
 ```
 
 <br>
 <br>
@@ -272,9 +254,55 @@
 print("Question:", user_input2, "\n\nAnswer:", vault_response2)
 ```
 >> Question: 
 How do I use it? 
  
 >>Answer: 
 You can use it by...
->>
+
+
+
+<br>
+<br>
+<br>
+
+# Build an AI Cusomter Service Chat Bot
+In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
+
+<br>
+
+### Create the Customer Service Vault
+```
+from vector_vault import Vault
+
+os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
+
+vault = Vault(user='your_user_id', api_key='your_api_key', vault='Customer Service')
+
+with open('customer_service.txt', 'r') as f:
+    vault.add(f.read())
+
+vault.get_vectors()
+
+vault.save()
+```
+
+<br>
+
+And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` function with `get_context=True`. The call `get_chat(text, get_context=True)` will take the customer's question, search the vault, find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
+
+```
+question = 'customer question text string'
+
+answer = vault.get_chat(question, get_context=True)
+```
+
+That's all it takes to create an ai customer service chatbot that responds to your customers as well as any support rep!
+
+
+<br>
+<br>
+
+If have any questions, leave a comment. Open the "examples" folder and try out the Google Colab tutorials we have.
+
+Happy coding.
```

