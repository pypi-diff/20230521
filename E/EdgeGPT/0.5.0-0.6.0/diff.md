# Comparing `tmp/EdgeGPT-0.5.0.tar.gz` & `tmp/EdgeGPT-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.5.0.tar", last modified: Sun May 21 08:22:09 2023, max compression
+gzip compressed data, was "EdgeGPT-0.6.0.tar", last modified: Sun May 21 11:49:53 2023, max compression
```

## Comparing `EdgeGPT-0.5.0.tar` & `EdgeGPT-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:22:09.811892 EdgeGPT-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-21 08:21:34.000000 EdgeGPT-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 08:22:09.811892 EdgeGPT-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-21 08:22:09.000000 EdgeGPT-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 08:22:09.811892 EdgeGPT-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-21 08:21:34.000000 EdgeGPT-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:22:09.811892 EdgeGPT-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:22:09.811892 EdgeGPT-0.5.0/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 08:22:09.000000 EdgeGPT-0.5.0/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 08:22:09.000000 EdgeGPT-0.5.0/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 08:22:09.000000 EdgeGPT-0.5.0/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 08:22:09.000000 EdgeGPT-0.5.0/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 08:22:09.000000 EdgeGPT-0.5.0/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-21 08:22:09.000000 EdgeGPT-0.5.0/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-05-21 08:21:34.000000 EdgeGPT-0.5.0/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-21 08:21:34.000000 EdgeGPT-0.5.0/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:49:53.955881 EdgeGPT-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-21 11:49:18.000000 EdgeGPT-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 11:49:53.955881 EdgeGPT-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-21 11:49:53.000000 EdgeGPT-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 11:49:53.955881 EdgeGPT-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-21 11:49:18.000000 EdgeGPT-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:49:53.955881 EdgeGPT-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:49:53.955881 EdgeGPT-0.6.0/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 11:49:53.000000 EdgeGPT-0.6.0/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 11:49:53.000000 EdgeGPT-0.6.0/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:49:53.000000 EdgeGPT-0.6.0/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 11:49:53.000000 EdgeGPT-0.6.0/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 11:49:53.000000 EdgeGPT-0.6.0/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-21 11:49:53.000000 EdgeGPT-0.6.0/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    37812 2023-05-21 11:49:18.000000 EdgeGPT-0.6.0/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-21 11:49:18.000000 EdgeGPT-0.6.0/src/ImageGen.py
```

### Comparing `EdgeGPT-0.5.0/LICENSE` & `EdgeGPT-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.5.0/PKG-INFO` & `EdgeGPT-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.5.0
+Version: 0.6.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `EdgeGPT-0.5.0/README.md` & `EdgeGPT-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.5.0/setup.py` & `EdgeGPT-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.5.0",
+    version="0.6.0",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.5.0/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.6.0/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.5.0
+Version: 0.6.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `EdgeGPT-0.5.0/src/EdgeGPT.py` & `EdgeGPT-0.6.0/src/EdgeGPT.py`

 * *Files 11% similar despite different names*

```diff
@@ -289,14 +289,15 @@
     Conversation API
     """
 
     def __init__(
         self,
         proxy: str | None = None,
         async_mode: bool = False,
+        cookies: list[dict] | None = None,
     ) -> None:
         if async_mode:
             return
         self.struct: dict = {
             "conversationId": None,
             "clientId": None,
             "conversationSignature": None,
@@ -314,14 +315,17 @@
         if proxy is not None and proxy.startswith("socks5h://"):
             proxy = "socks5://" + proxy[len("socks5h://") :]
         self.session = httpx.Client(
             proxies=proxy,
             timeout=30,
             headers=HEADERS_INIT_CONVER,
         )
+        if cookies:
+            for cookie in cookies:
+                self.session.cookies.set(cookie["name"], cookie["value"])
         # Send GET request
         response = self.session.get(
             url=os.environ.get("BING_PROXY_URL")
             or "https://edgeservices.bing.com/edgesvc/turing/conversation/create",
         )
         if response.status_code != 200:
             response = self.session.get(
@@ -340,14 +344,15 @@
             ) from exc
         if self.struct["result"]["value"] == "UnauthorizedRequest":
             raise NotAllowedToAccess(self.struct["result"]["message"])
 
     @staticmethod
     async def create(
         proxy: str | None = None,
+        cookies: list[dict] | None = None,
     ) -> _Conversation:
         self = _Conversation(async_mode=True)
         self.struct = {
             "conversationId": None,
             "clientId": None,
             "conversationSignature": None,
             "result": {"value": "Success", "message": None},
@@ -360,19 +365,25 @@
             or os.environ.get("https_proxy")
             or os.environ.get("HTTPS_PROXY")
             or None
         )
         if proxy is not None and proxy.startswith("socks5h://"):
             proxy = "socks5://" + proxy[len("socks5h://") :]
         transport = httpx.AsyncHTTPTransport(retries=10)
+        # Convert cookie format to httpx format
+        if cookies:
+            formatted_cookies = httpx.Cookies()
+            for cookie in cookies:
+                formatted_cookies.set(cookie["name"], cookie["value"])
         async with httpx.AsyncClient(
             proxies=proxy,
             timeout=30,
             headers=HEADERS_INIT_CONVER,
             transport=transport,
+            cookies=formatted_cookies,
         ) as client:
             # Send GET request
             response = await client.get(
                 url=os.environ.get("BING_PROXY_URL")
                 or "https://edgeservices.bing.com/edgesvc/turing/conversation/create",
             )
             if response.status_code != 200:
@@ -396,25 +407,31 @@
 
 
 class _ChatHub:
     """
     Chat API
     """
 
-    def __init__(self, conversation: _Conversation, proxy: str = None) -> None:
+    def __init__(
+        self,
+        conversation: _Conversation,
+        proxy: str = None,
+        cookies: list[dict] | None = None,
+    ) -> None:
         self.session: aiohttp.ClientSession | None = None
         self.wss: aiohttp.ClientWebSocketResponse | None = None
         self.request: _ChatHubRequest
         self.loop: bool
         self.task: asyncio.Task
         self.request = _ChatHubRequest(
             conversation_signature=conversation.struct["conversationSignature"],
             client_id=conversation.struct["clientId"],
             conversation_id=conversation.struct["conversationId"],
         )
+        self.cookies = cookies
         self.proxy: str = proxy
 
     async def ask_stream(
         self,
         prompt: str,
         wss_link: str,
         conversation_style: CONVERSATION_STYLE_TYPE = None,
@@ -424,14 +441,15 @@
         search_result: bool = False,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         timeout = aiohttp.ClientTimeout(total=30)
         self.session = aiohttp.ClientSession(timeout=timeout)
+
         if self.wss and not self.wss.closed:
             await self.wss.close()
         # Check if websocket is closed
         self.wss = await self.session.ws_connect(
             wss_link,
             headers=HEADERS,
             ssl=ssl_context,
@@ -586,30 +604,34 @@
     """
     Combines everything to make it seamless
     """
 
     def __init__(
         self,
         proxy: str | None = None,
+        cookies: list[dict] | None = None,
     ) -> None:
         self.proxy: str | None = proxy
         self.chat_hub: _ChatHub = _ChatHub(
-            _Conversation(self.proxy),
+            _Conversation(self.proxy, cookies=cookies),
             proxy=self.proxy,
+            cookies=cookies,
         )
 
     @staticmethod
     async def create(
         proxy: str | None = None,
+        cookies: list[dict] | None = None,
     ):
         self = Chatbot.__new__(Chatbot)
         self.proxy = proxy
         self.chat_hub = _ChatHub(
-            await _Conversation.create(self.proxy),
+            await _Conversation.create(self.proxy, cookies=cookies),
             proxy=self.proxy,
+            cookies=cookies,
         )
         return self
 
     async def ask(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
@@ -715,15 +737,19 @@
 
 async def async_main(args: argparse.Namespace) -> None:
     """
     Main function
     """
     print("Initializing...")
     print("Enter `alt+enter` or `escape+enter` to send a message")
-    bot = await Chatbot.create(proxy=args.proxy)
+    # Read and parse cookies
+    cookies = None
+    if args.cookie_file:
+        cookies = json.loads(open(args.cookie_file).read())
+    bot = await Chatbot.create(proxy=args.proxy, cookies=cookies)
     session = _create_session()
     completer = _create_completer(["!help", "!exit", "!reset"])
     initial_prompt = args.prompt
 
     while True:
         print("\nYou:")
         if initial_prompt:
@@ -830,14 +856,21 @@
     parser.add_argument(
         "--prompt",
         type=str,
         default="",
         required=False,
         help="prompt to start with",
     )
+    parser.add_argument(
+        "--cookie-file",
+        type=str,
+        default="",
+        required=False,
+        help="path to cookie file",
+    )
     args = parser.parse_args()
     asyncio.run(async_main(args))
 
 
 class Cookie:
     """
     Convenience class for Bing Cookie files, data, and configuration. This Class
```

