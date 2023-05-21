# Comparing `tmp/sleepyask-6.0.0.tar.gz` & `tmp/sleepyask-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nocet\OneDrive\Documents\Projects\one_thing\naggingGPT\dist\.tmp-57ovnsc3\sleepyask-6.0.0.tar", last modified: Sun May 21 07:51:55 2023, max compression
+gzip compressed data, was "sleepyask-6.0.1.tar", last modified: Sun May 21 07:56:55 2023, max compression
```

## Comparing `sleepyask-6.0.0.tar` & `sleepyask-6.0.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 07:51:55.000000 sleepyask-6.0.0/
--rw-rw-rw-   0        0        0      378 2023-05-21 07:51:55.000000 sleepyask-6.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-05-21 07:51:25.000000 sleepyask-6.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 07:51:55.000000 sleepyask-6.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/naggpt/
--rw-rw-rw-   0        0        0        0 2023-05-19 08:52:03.000000 sleepyask-6.0.0/src/naggpt/__init__.py
--rw-rw-rw-   0        0        0     2515 2023-05-21 07:44:34.000000 sleepyask-6.0.0/src/naggpt/nag.py
-drwxrwxrwx   0        0        0        0 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/
--rw-rw-rw-   0        0        0      378 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:56:55.054703 sleepyask-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 07:56:44.000000 sleepyask-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 07:56:55.054703 sleepyask-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-21 07:56:44.000000 sleepyask-6.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-21 07:56:44.000000 sleepyask-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 07:56:55.054703 sleepyask-6.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:56:55.054703 sleepyask-6.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:56:55.054703 sleepyask-6.0.1/src/sleepyask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:56:44.000000 sleepyask-6.0.1/src/sleepyask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-21 07:56:44.000000 sleepyask-6.0.1/src/sleepyask/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:56:55.054703 sleepyask-6.0.1/src/sleepyask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 07:56:55.000000 sleepyask-6.0.1/src/sleepyask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-21 07:56:55.000000 sleepyask-6.0.1/src/sleepyask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 07:56:55.000000 sleepyask-6.0.1/src/sleepyask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 07:56:55.000000 sleepyask-6.0.1/src/sleepyask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 07:56:55.000000 sleepyask-6.0.1/src/sleepyask.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sleepyask-6.0.0/pyproject.toml` & `sleepyask-6.0.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "sleepyask"
-version = "6.0.0"
-authors = [
-  { name="hwelsters", email="redacted@redacted.redacted" },
-]
-description = "A small tool for automating collecting data from ChatGPT"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = []
-dependencies = [
-  'openai-async>=0.0.3'
-]
-
-[project.urls]
-"Homepage" = "https://github.com/hwelsters/sleepyask"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "sleepyask"
+version = "6.0.1"
+authors = [
+  { name="hwelsters", email="redacted@redacted.redacted" },
+]
+description = "A small tool for automating collecting data from ChatGPT"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = []
+dependencies = [
+  'openai-async>=0.0.3'
+]
+
+[project.urls]
+"Homepage" = "https://github.com/hwelsters/sleepyask"
 "Bug Tracker" = "https://github.com/hwelsters/sleepyask/issues"
```

### Comparing `sleepyask-6.0.0/src/naggpt/nag.py` & `sleepyask-6.0.1/src/sleepyask/chat.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import time
-import queue
-import json
-import asyncio
-
-from openai_async import openai_async
-
-# TODO: Shouldn't be that hard to extend to other OpenAI functions but chat is the only one I'm familiar with atm
-class Nagger:
-    """
-    This class provides functions which use ayncio to ask multiple questions to ChatGPT simultaneously.
-    This allows users to aggregate a large number of responses from ChatGPT.
-    """
-
-    def __init__(self, configs : dict ={}, rate_limit: int = 5, api_key: str = "", timeout: int = 100, out_path : str = ""):
-        """
-        `configs` a dict containing parameters which will be part of the payload such as model, temperature, etc
-        `rate_limit` the maximum number of questions you would like to ask a minute.
-        `api_key` OpenAI API key
-        `timeout` the amount of time to wait before timing out
-        `out_path` the path in which the responses will be outputted
-        """
-        self.configs = configs
-        self.rate_limit = rate_limit
-        self.api_key = api_key
-        self.timeout = timeout
-        self.out_path = out_path
-
-    def start(self, question_list):
-        """
-        `question_list` list of questions to ask ChatGPT
-        """
-        asyncio.run(self.__start(question_list))
-
-    async def __start(self, question_list):
-        self.succeed = 0
-        self.file_lock = asyncio.Lock()
-        self.question_queue = queue.Queue()
-        for question in question_list: self.question_queue.put(question)
-
-        while self.succeed < len(question_list):
-            tasks = [self.async_nag(self.question_queue.get()) for _ in range(self.rate_limit)]
-            await asyncio.gather(*tasks)
-
-            if self.succeed < len(question_list): time.sleep(60)
-
-    async def log(self, response):
-        await self.file_lock.acquire()
-
-        with open(self.out_path, "a") as outfile:
-            outfile.write(json.dumps(response))
-            outfile.write("\n")
-        self.succeed += 1
-        self.file_lock.release()
-
-    async def async_nag(self, question):
-        try:
-            payload = {"messages": [{"role": "user", "content": question}], **self.configs}
-            response = await openai_async.chat_complete(payload=payload, api_key=self.api_key, timeout=self.timeout)
-            
-            if response.status_code != 200: raise ValueError("Should be 200")
-
-            await self.log(response.text)
+import time
+import queue
+import json
+import asyncio
+
+from openai_async import openai_async
+
+# TODO: Shouldn't be that hard to extend to other OpenAI functions but chat is the only one I'm familiar with atm
+class Sleepyask:
+    """
+    This class provides functions which use ayncio to ask multiple questions to ChatGPT simultaneously.
+    This allows users to aggregate a large number of responses from ChatGPT.
+    """
+
+    def __init__(self, configs : dict ={}, rate_limit: int = 5, api_key: str = "", timeout: int = 100, out_path : str = ""):
+        """
+        `configs` a dict containing parameters which will be part of the payload such as model, temperature, etc
+        `rate_limit` the maximum number of questions you would like to ask a minute.
+        `api_key` OpenAI API key
+        `timeout` the amount of time to wait before timing out
+        `out_path` the path in which the responses will be outputted
+        """
+        self.configs = configs
+        self.rate_limit = rate_limit
+        self.api_key = api_key
+        self.timeout = timeout
+        self.out_path = out_path
+
+    def start(self, question_list):
+        """
+        `question_list` list of questions to ask ChatGPT
+        """
+        asyncio.run(self.__start(question_list))
+
+    async def __start(self, question_list):
+        self.succeed = 0
+        self.file_lock = asyncio.Lock()
+        self.question_queue = queue.Queue()
+        for question in question_list: self.question_queue.put(question)
+
+        while self.succeed < len(question_list):
+            tasks = [self.async_ask(self.question_queue.get()) for _ in range(self.rate_limit)]
+            await asyncio.gather(*tasks)
+
+            if self.succeed < len(question_list): time.sleep(60)
+
+    async def log(self, response):
+        await self.file_lock.acquire()
+
+        with open(self.out_path, "a") as outfile:
+            outfile.write(json.dump(response))
+            outfile.write("\n")
+        self.succeed += 1
+        self.file_lock.release()
+
+    async def async_ask(self, question):
+        try:
+            payload = {"messages": [{"role": "user", "content": question}], **self.configs}
+            response = await openai_async.chat_complete(payload=payload, api_key=self.api_key, timeout=self.timeout)
+            
+            if response.status_code != 200: raise ValueError("Should be 200")
+
+            await self.log(response.text)
         except: self.question_queue.put(question)
```

