# Comparing `tmp/revChatGPT-5.0.4.tar.gz` & `tmp/revChatGPT-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-5.0.4.tar", last modified: Sun May 21 03:26:49 2023, max compression
+gzip compressed data, was "revChatGPT-5.1.0.tar", last modified: Sun May 21 04:20:11 2023, max compression
```

## Comparing `revChatGPT-5.0.4.tar` & `revChatGPT-5.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-21 03:26:48.000000 revChatGPT-5.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 03:26:49.156279 revChatGPT-5.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    49926 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-05-21 03:26:49.000000 revChatGPT-5.0.4/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-21 03:26:49.000000 revChatGPT-5.0.4/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:26:49.000000 revChatGPT-5.0.4/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-21 03:26:49.000000 revChatGPT-5.0.4/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 03:26:49.000000 revChatGPT-5.0.4/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:26:49.152279 revChatGPT-5.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-21 03:26:16.000000 revChatGPT-5.0.4/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:20:11.631576 revChatGPT-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-21 04:20:11.631576 revChatGPT-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-21 04:20:11.000000 revChatGPT-5.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 04:20:11.631576 revChatGPT-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:20:11.627575 revChatGPT-5.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:20:11.631576 revChatGPT-5.1.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    50857 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:20:11.631576 revChatGPT-5.1.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:20:11.631576 revChatGPT-5.1.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-21 04:20:11.000000 revChatGPT-5.1.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-21 04:20:11.000000 revChatGPT-5.1.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:20:11.000000 revChatGPT-5.1.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-21 04:20:11.000000 revChatGPT-5.1.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 04:20:11.000000 revChatGPT-5.1.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:20:11.631576 revChatGPT-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-21 04:19:31.000000 revChatGPT-5.1.0/tests/test_recipient.py
```

### Comparing `revChatGPT-5.0.4/LICENSE` & `revChatGPT-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.4/PKG-INFO` & `revChatGPT-5.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.0.4
+Version: 5.1.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -26,15 +26,15 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
-Status: Working but unmaintained. 
+Status: Working but unmaintained.
 
 [![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
 
 # Installation
 
 ```
 python -m pip install --upgrade revChatGPT
@@ -48,15 +48,15 @@
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
 V1 uses a cloudflare bypass proxy to make life convenient for everyone. The proxy is open source: https://github.com/acheong08/ChatGPT-Proxy-V4
-    
+
 To set your own deployed proxy, set the environment variable `CHATGPT_BASE_URL` to `https://yourproxy.com/api/`
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
@@ -93,22 +93,24 @@
 #### - Optional configuration:
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
-  "paid": false,
-  "model": "gpt-4" // gpt-4-browsing, text-davinci-002-render-sha, gpt-4
+  "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
+  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"] // Wolfram Alpha example
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
+Plugin IDs can be found [here](./docs/plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled
+
 ## Usage
 
 ### Command line
 
 `python3 -m revChatGPT.V1`
 
 ```
@@ -162,14 +164,16 @@
 
 #### All API methods
 
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
+<details>
+
 <summary>
 
 # V3 Official Chat API
 
 > Recently released by OpenAI
 >
 > - Paid
```

### Comparing `revChatGPT-5.0.4/README.md` & `revChatGPT-5.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
-Status: Working but unmaintained. 
+Status: Working but unmaintained.
 
 [![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
 
 # Installation
 
 ```
 python -m pip install --upgrade revChatGPT
@@ -26,15 +26,15 @@
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
 V1 uses a cloudflare bypass proxy to make life convenient for everyone. The proxy is open source: https://github.com/acheong08/ChatGPT-Proxy-V4
-    
+
 To set your own deployed proxy, set the environment variable `CHATGPT_BASE_URL` to `https://yourproxy.com/api/`
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
@@ -71,22 +71,24 @@
 #### - Optional configuration:
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
-  "paid": false,
-  "model": "gpt-4" // gpt-4-browsing, text-davinci-002-render-sha, gpt-4
+  "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
+  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"] // Wolfram Alpha example
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
+Plugin IDs can be found [here](./docs/plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled
+
 ## Usage
 
 ### Command line
 
 `python3 -m revChatGPT.V1`
 
 ```
@@ -140,14 +142,16 @@
 
 #### All API methods
 
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
+<details>
+
 <summary>
 
 # V3 Official Chat API
 
 > Recently released by OpenAI
 >
 > - Paid
```

### Comparing `revChatGPT-5.0.4/setup.py` & `revChatGPT-5.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="5.0.4",
+    version="5.1.0",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-5.0.4/src/revChatGPT/V1.py` & `revChatGPT-5.1.0/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,18 @@
         base_url: str | None = None,
     ) -> None:
         """Initialize a chatbot
 
         Args:
             config (dict[str, str]): Login and proxy info. Example:
                 {
-                    "email": "OpenAI account email",
-                    "password": "OpenAI account password",
                     "access_token": "<access_token>"
                     "proxy": "<proxy_url_string>",
+                    "model": "<model_name>",
+                    "plugin": "<plugin_id>",
                 }
                 More details on these are available at https://github.com/acheong08/ChatGPT#configuration
             conversation_id (str | None, optional): Id of the conversation to continue on. Defaults to None.
             parent_id (str | None, optional): Id of the previous response message to continue on. Defaults to None.
             session_client (_type_, optional): _description_. Defaults to None.
 
         Raises:
@@ -386,22 +386,22 @@
                 raise ValueError(f"Field missing. Details: {str(line)}")
             if line.get("message").get("author").get("role") != "assistant":
                 continue
 
             cid = line["conversation_id"]
             pid = line["message"]["id"]
             metadata = line["message"].get("metadata", {})
-            author = metadata.get("author", {})
             message_exists = False
+            author = {}
             if line.get("message"):
+                author = metadata.get("author", {}) or line["message"].get("author", {})
                 if line["message"].get("content"):
                     if line["message"]["content"].get("parts"):
                         if len(line["message"]["content"]["parts"]) > 0:
                             message_exists = True
-
             message: str = (
                 line["message"]["content"]["parts"][0] if message_exists else ""
             )
             model = metadata.get("model_slug", None)
             finish_details = metadata.get("finish_details", {"type": None})["type"]
             yield {
                 "author": author,
@@ -434,14 +434,15 @@
 
     @logger(is_timed=True)
     def post_messages(
         self,
         messages: list[dict],
         conversation_id: str | None = None,
         parent_id: str | None = None,
+        plugin_ids: list = [],
         model: str | None = None,
         auto_continue: bool = False,
         timeout: float = 360,
         **kwargs,
     ) -> Generator[dict, None, None]:
         """Ask a question to the chatbot
         Args:
@@ -501,28 +502,32 @@
         data = {
             "action": "next",
             "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model or self.config.get("model") or "text-davinci-002-render-sha",
         }
+        plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
+        if len(plugin_ids) > 0 and not conversation_id:
+            data["plugin_ids"] = plugin_ids
 
         yield from self.__send_request(
             data,
             timeout=timeout,
             auto_continue=auto_continue,
         )
 
     @logger(is_timed=True)
     def ask(
         self,
         prompt: str,
         conversation_id: str | None = None,
         parent_id: str = "",
         model: str = "",
+        plugin_ids: list = [],
         auto_continue: bool = False,
         timeout: float = 360,
         **kwargs,
     ) -> Generator[dict, None, None]:
         """Ask a question to the chatbot
         Args:
             prompt (str): The question
@@ -552,14 +557,15 @@
             },
         ]
 
         yield from self.post_messages(
             messages,
             conversation_id=conversation_id,
             parent_id=parent_id,
+            plugin_ids=plugin_ids,
             model=model,
             auto_continue=auto_continue,
             timeout=timeout,
         )
 
     @logger(is_timed=True)
     def continue_write(
@@ -775,14 +781,29 @@
         :param num: Integer. The number of messages to rollback
         :return: None
         """
         for _ in range(num):
             self.conversation_id = self.conversation_id_prev_queue.pop()
             self.parent_id = self.parent_id_prev_queue.pop()
 
+    @logger(is_timed=True)
+    def get_plugins(self, offset: int = 0, limit: int = 250, status: str = "approved"):
+        url = f"{self.base_url}aip/p?offset={offset}&limit={limit}&statuses={status}"
+        response = self.session.get(url)
+        self.__check_response(response)
+        # Parse as JSON
+        return json.loads(response.text)
+
+    @logger(is_timed=True)
+    def install_plugin(self, plugin_id: str):
+        url = f"{self.base_url}aip/p/{plugin_id}/user-settings"
+        payload = {"is_installed": True}
+        response = self.session.patch(url, data=json.dumps(payload))
+        self.__check_response(response)
+
 
 class AsyncChatbot(Chatbot):
     """Async Chatbot class for ChatGPT"""
 
     def __init__(
         self,
         config: dict,
@@ -1337,30 +1358,30 @@
 
             print()
             print(f"{bcolors.OKGREEN + bcolors.BOLD}Chatbot: {bcolors.ENDC}")
             if chatbot.config.get("model") == "gpt-4-browsing":
                 print("Browsing takes a while, please wait...")
             prev_text = ""
             for data in chatbot.post_messages([msg], auto_continue=True):
-                result = data
-                if data.get("author").get("role") == "tool":
+                if data["recipient"] != "all":
                     continue
+                result = data
                 message = data["message"][len(prev_text) :]
                 print(message, end="", flush=True)
                 prev_text = data["message"]
             print(bcolors.ENDC)
             print()
 
             if result.get("citations", False):
                 print(
                     f"{bcolors.WARNING + bcolors.BOLD}Citations: {bcolors.ENDC}",
                 )
                 for citation in result["citations"]:
                     print(
-                        f'{citation["metadata"]["title"]}: {citation["metadata"]["url"]}'
+                        f'{citation["metadata"]["title"]}: {citation["metadata"]["url"]}',
                     )
                 print()
 
             msg = {}
             if not result.get("end_turn", True):
                 times += 1
                 if times >= 5:
```

### Comparing `revChatGPT-5.0.4/src/revChatGPT/V3.py` & `revChatGPT-5.1.0/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.4/src/revChatGPT/__init__.py` & `revChatGPT-5.1.0/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.4/src/revChatGPT/__main__.py` & `revChatGPT-5.1.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.4/src/revChatGPT/config/enable_internet.json` & `revChatGPT-5.1.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.4/src/revChatGPT/recipient.py` & `revChatGPT-5.1.0/src/revChatGPT/recipient.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.4/src/revChatGPT/typings.py` & `revChatGPT-5.1.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.4/src/revChatGPT/utils.py` & `revChatGPT-5.1.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.4/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-5.1.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.0.4
+Version: 5.1.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -26,15 +26,15 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
-Status: Working but unmaintained. 
+Status: Working but unmaintained.
 
 [![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
 
 # Installation
 
 ```
 python -m pip install --upgrade revChatGPT
@@ -48,15 +48,15 @@
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
 V1 uses a cloudflare bypass proxy to make life convenient for everyone. The proxy is open source: https://github.com/acheong08/ChatGPT-Proxy-V4
-    
+
 To set your own deployed proxy, set the environment variable `CHATGPT_BASE_URL` to `https://yourproxy.com/api/`
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
@@ -93,22 +93,24 @@
 #### - Optional configuration:
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
-  "paid": false,
-  "model": "gpt-4" // gpt-4-browsing, text-davinci-002-render-sha, gpt-4
+  "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
+  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"] // Wolfram Alpha example
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
+Plugin IDs can be found [here](./docs/plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled
+
 ## Usage
 
 ### Command line
 
 `python3 -m revChatGPT.V1`
 
 ```
@@ -162,14 +164,16 @@
 
 #### All API methods
 
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
+<details>
+
 <summary>
 
 # V3 Official Chat API
 
 > Recently released by OpenAI
 >
 > - Paid
```

### Comparing `revChatGPT-5.0.4/tests/test_recipient.py` & `revChatGPT-5.1.0/tests/test_recipient.py`

 * *Files identical despite different names*

