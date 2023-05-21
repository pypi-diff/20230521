# Comparing `tmp/revChatGPT-5.0.3.tar.gz` & `tmp/revChatGPT-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-5.0.3.tar", last modified: Wed May 17 12:06:24 2023, max compression
+gzip compressed data, was "revChatGPT-5.0.4.tar", last modified: Sun May 21 03:26:49 2023, max compression
```

## Comparing `revChatGPT-5.0.3.tar` & `revChatGPT-5.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:06:24.275362 revChatGPT-5.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-17 12:06:24.275362 revChatGPT-5.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-17 12:06:24.000000 revChatGPT-5.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 12:06:24.275362 revChatGPT-5.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:06:24.271362 revChatGPT-5.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:06:24.271362 revChatGPT-5.0.3/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    48993 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:06:24.275362 revChatGPT-5.0.3/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:06:24.275362 revChatGPT-5.0.3/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-17 12:06:24.000000 revChatGPT-5.0.3/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-17 12:06:24.000000 revChatGPT-5.0.3/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:06:24.000000 revChatGPT-5.0.3/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-17 12:06:24.000000 revChatGPT-5.0.3/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 12:06:24.000000 revChatGPT-5.0.3/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:06:24.275362 revChatGPT-5.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-17 12:05:55.000000 revChatGPT-5.0.3/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-21 03:26:48.000000 revChatGPT-5.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 03:26:49.156279 revChatGPT-5.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    49926 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-05-21 03:26:49.000000 revChatGPT-5.0.4/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-21 03:26:49.000000 revChatGPT-5.0.4/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:26:49.000000 revChatGPT-5.0.4/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-21 03:26:49.000000 revChatGPT-5.0.4/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 03:26:49.000000 revChatGPT-5.0.4/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/tests/test_recipient.py
```

### Comparing `revChatGPT-5.0.3/LICENSE` & `revChatGPT-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.3/PKG-INFO` & `revChatGPT-5.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.0.3
+Version: 5.0.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -47,16 +47,14 @@
 
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
-~~Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.~~
-    
 V1 uses a cloudflare bypass proxy to make life convenient for everyone. The proxy is open source: https://github.com/acheong08/ChatGPT-Proxy-V4
     
 To set your own deployed proxy, set the environment variable `CHATGPT_BASE_URL` to `https://yourproxy.com/api/`
 
 </summary>
 
 ## Rate limits
@@ -96,23 +94,20 @@
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "paid": false,
-  "collect_analytics": true,
-  "model": "gpt-4"
+  "model": "gpt-4" // gpt-4-browsing, text-davinci-002-render-sha, gpt-4
 }
 ```
 
-Analytics is disabled by default. Set `collect_analytics` to `true` to enable it.
-
-3. Save this as `$HOME/.config/revChatGPT/config.json`
-4. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
+1. Save this as `$HOME/.config/revChatGPT/config.json`
+2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 ## Usage
 
 ### Command line
 
 `python3 -m revChatGPT.V1`
```

### Comparing `revChatGPT-5.0.3/README.md` & `revChatGPT-5.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,14 @@
 
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
-~~Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.~~
-    
 V1 uses a cloudflare bypass proxy to make life convenient for everyone. The proxy is open source: https://github.com/acheong08/ChatGPT-Proxy-V4
     
 To set your own deployed proxy, set the environment variable `CHATGPT_BASE_URL` to `https://yourproxy.com/api/`
 
 </summary>
 
 ## Rate limits
@@ -74,23 +72,20 @@
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "paid": false,
-  "collect_analytics": true,
-  "model": "gpt-4"
+  "model": "gpt-4" // gpt-4-browsing, text-davinci-002-render-sha, gpt-4
 }
 ```
 
-Analytics is disabled by default. Set `collect_analytics` to `true` to enable it.
-
-3. Save this as `$HOME/.config/revChatGPT/config.json`
-4. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
+1. Save this as `$HOME/.config/revChatGPT/config.json`
+2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 ## Usage
 
 ### Command line
 
 `python3 -m revChatGPT.V1`
```

### Comparing `revChatGPT-5.0.3/setup.py` & `revChatGPT-5.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="5.0.3",
+    version="5.0.4",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-5.0.3/src/revChatGPT/V1.py` & `revChatGPT-5.0.4/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,14 @@
         Args:
             config (dict[str, str]): Login and proxy info. Example:
                 {
                     "email": "OpenAI account email",
                     "password": "OpenAI account password",
                     "access_token": "<access_token>"
                     "proxy": "<proxy_url_string>",
-                    "paid": True/False, # whether this is a plus account
                 }
                 More details on these are available at https://github.com/acheong08/ChatGPT#configuration
             conversation_id (str | None, optional): Id of the conversation to continue on. Defaults to None.
             parent_id (str | None, optional): Id of the previous response message to continue on. Defaults to None.
             session_client (_type_, optional): _description_. Defaults to None.
 
         Raises:
@@ -383,28 +382,41 @@
                 line = json.loads(line)
             except json.decoder.JSONDecodeError:
                 continue
             if not self.__check_fields(line):
                 raise ValueError(f"Field missing. Details: {str(line)}")
             if line.get("message").get("author").get("role") != "assistant":
                 continue
-            message: str = line["message"]["content"]["parts"][0]
+
             cid = line["conversation_id"]
             pid = line["message"]["id"]
             metadata = line["message"].get("metadata", {})
+            author = metadata.get("author", {})
+            message_exists = False
+            if line.get("message"):
+                if line["message"].get("content"):
+                    if line["message"]["content"].get("parts"):
+                        if len(line["message"]["content"]["parts"]) > 0:
+                            message_exists = True
+
+            message: str = (
+                line["message"]["content"]["parts"][0] if message_exists else ""
+            )
             model = metadata.get("model_slug", None)
             finish_details = metadata.get("finish_details", {"type": None})["type"]
             yield {
+                "author": author,
                 "message": message,
                 "conversation_id": cid,
                 "parent_id": pid,
                 "model": model,
                 "finish_details": finish_details,
                 "end_turn": line["message"].get("end_turn", True),
                 "recipient": line["message"].get("recipient", "all"),
+                "citations": metadata.get("citations", []),
             }
 
         self.conversation_mapping[cid] = pid
         if pid is not None:
             self.parent_id = pid
         if cid is not None:
             self.conversation_id = cid
@@ -445,14 +457,15 @@
                 "message": str,
                 "conversation_id": str,
                 "parent_id": str,
                 "model": str,
                 "finish_details": str, # "max_tokens" or "stop"
                 "end_turn": bool,
                 "recipient": str,
+                "citations": list[dict],
             }
         """
         if parent_id and not conversation_id:
             raise t.Error(
                 source="User",
                 message="conversation_id must be set once parent_id is set",
                 code=t.ErrorType.USER_ERROR,
@@ -486,21 +499,15 @@
                 parent_id = str(uuid.uuid4())
 
         data = {
             "action": "next",
             "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
-            "model": model
-            or self.config.get("model")
-            or (
-                "text-davinci-002-render-paid"
-                if self.config.get("paid")
-                else "text-davinci-002-render-sha"
-            ),
+            "model": model or self.config.get("model") or "text-davinci-002-render-sha",
         }
 
         yield from self.__send_request(
             data,
             timeout=timeout,
             auto_continue=auto_continue,
         )
@@ -1326,23 +1333,37 @@
                 print(
                     f"{bcolors.OKCYAN + bcolors.BOLD}{result['recipient'] if result['recipient'] != 'user' else 'You'}: {bcolors.ENDC}",
                 )
                 print(msg["content"]["parts"][0])
 
             print()
             print(f"{bcolors.OKGREEN + bcolors.BOLD}Chatbot: {bcolors.ENDC}")
+            if chatbot.config.get("model") == "gpt-4-browsing":
+                print("Browsing takes a while, please wait...")
             prev_text = ""
             for data in chatbot.post_messages([msg], auto_continue=True):
                 result = data
+                if data.get("author").get("role") == "tool":
+                    continue
                 message = data["message"][len(prev_text) :]
                 print(message, end="", flush=True)
                 prev_text = data["message"]
             print(bcolors.ENDC)
             print()
 
+            if result.get("citations", False):
+                print(
+                    f"{bcolors.WARNING + bcolors.BOLD}Citations: {bcolors.ENDC}",
+                )
+                for citation in result["citations"]:
+                    print(
+                        f'{citation["metadata"]["title"]}: {citation["metadata"]["url"]}'
+                    )
+                print()
+
             msg = {}
             if not result.get("end_turn", True):
                 times += 1
                 if times >= 5:
                     continue
                 api = plugins.get(result["recipient"])
                 if not api:
```

### Comparing `revChatGPT-5.0.3/src/revChatGPT/V3.py` & `revChatGPT-5.0.4/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.3/src/revChatGPT/__init__.py` & `revChatGPT-5.0.4/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.3/src/revChatGPT/__main__.py` & `revChatGPT-5.0.4/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.3/src/revChatGPT/config/enable_internet.json` & `revChatGPT-5.0.4/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.3/src/revChatGPT/recipient.py` & `revChatGPT-5.0.4/src/revChatGPT/recipient.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.3/src/revChatGPT/typings.py` & `revChatGPT-5.0.4/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.3/src/revChatGPT/utils.py` & `revChatGPT-5.0.4/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.3/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-5.0.4/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.0.3
+Version: 5.0.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -47,16 +47,14 @@
 
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
-~~Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.~~
-    
 V1 uses a cloudflare bypass proxy to make life convenient for everyone. The proxy is open source: https://github.com/acheong08/ChatGPT-Proxy-V4
     
 To set your own deployed proxy, set the environment variable `CHATGPT_BASE_URL` to `https://yourproxy.com/api/`
 
 </summary>
 
 ## Rate limits
@@ -96,23 +94,20 @@
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "paid": false,
-  "collect_analytics": true,
-  "model": "gpt-4"
+  "model": "gpt-4" // gpt-4-browsing, text-davinci-002-render-sha, gpt-4
 }
 ```
 
-Analytics is disabled by default. Set `collect_analytics` to `true` to enable it.
-
-3. Save this as `$HOME/.config/revChatGPT/config.json`
-4. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
+1. Save this as `$HOME/.config/revChatGPT/config.json`
+2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 ## Usage
 
 ### Command line
 
 `python3 -m revChatGPT.V1`
```

### Comparing `revChatGPT-5.0.3/tests/test_recipient.py` & `revChatGPT-5.0.4/tests/test_recipient.py`

 * *Files identical despite different names*

