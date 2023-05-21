# Comparing `tmp/sleepyask-6.0.1.tar.gz` & `tmp/sleepyask-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyask-6.0.1.tar", last modified: Sun May 21 07:56:55 2023, max compression
+gzip compressed data, was "sleepyask-6.1.0.tar", last modified: Sun May 21 08:04:02 2023, max compression
```

## Comparing `sleepyask-6.0.1.tar` & `sleepyask-6.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:56:55.054703 sleepyask-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 07:56:44.000000 sleepyask-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 07:56:55.054703 sleepyask-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-21 07:56:44.000000 sleepyask-6.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-21 07:56:44.000000 sleepyask-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 07:56:55.054703 sleepyask-6.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:56:55.054703 sleepyask-6.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:56:55.054703 sleepyask-6.0.1/src/sleepyask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:56:44.000000 sleepyask-6.0.1/src/sleepyask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-21 07:56:44.000000 sleepyask-6.0.1/src/sleepyask/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:56:55.054703 sleepyask-6.0.1/src/sleepyask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 07:56:55.000000 sleepyask-6.0.1/src/sleepyask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-21 07:56:55.000000 sleepyask-6.0.1/src/sleepyask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 07:56:55.000000 sleepyask-6.0.1/src/sleepyask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 07:56:55.000000 sleepyask-6.0.1/src/sleepyask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 07:56:55.000000 sleepyask-6.0.1/src/sleepyask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:04:02.049187 sleepyask-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 08:03:47.000000 sleepyask-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 08:04:02.049187 sleepyask-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-21 08:03:47.000000 sleepyask-6.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-21 08:03:47.000000 sleepyask-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 08:04:02.049187 sleepyask-6.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:04:02.049187 sleepyask-6.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:04:02.049187 sleepyask-6.1.0/src/sleepyask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:03:47.000000 sleepyask-6.1.0/src/sleepyask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-21 08:03:47.000000 sleepyask-6.1.0/src/sleepyask/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:04:02.049187 sleepyask-6.1.0/src/sleepyask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 08:04:02.000000 sleepyask-6.1.0/src/sleepyask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-21 08:04:02.000000 sleepyask-6.1.0/src/sleepyask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 08:04:02.000000 sleepyask-6.1.0/src/sleepyask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 08:04:02.000000 sleepyask-6.1.0/src/sleepyask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 08:04:02.000000 sleepyask-6.1.0/src/sleepyask.egg-info/top_level.txt
```

### Comparing `sleepyask-6.0.1/LICENSE` & `sleepyask-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepyask-6.0.1/PKG-INFO` & `sleepyask-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 6.0.1
+Version: 6.1.0
 Summary: A small tool for automating collecting data from ChatGPT
 Author-email: hwelsters <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/hwelsters/sleepyask
 Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sleepyask Version: 6.0.1 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 6.1.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
```

### Comparing `sleepyask-6.0.1/README.md` & `sleepyask-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sleepyask-6.0.1/pyproject.toml` & `sleepyask-6.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sleepyask"
-version = "6.0.1"
+version = "6.1.0"
 authors = [
   { name="hwelsters", email="redacted@redacted.redacted" },
 ]
 description = "A small tool for automating collecting data from ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = []
```

### Comparing `sleepyask-6.0.1/src/sleepyask/chat.py` & `sleepyask-6.1.0/src/sleepyask/chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,57 +8,71 @@
 # TODO: Shouldn't be that hard to extend to other OpenAI functions but chat is the only one I'm familiar with atm
 class Sleepyask:
     """
     This class provides functions which use ayncio to ask multiple questions to ChatGPT simultaneously.
     This allows users to aggregate a large number of responses from ChatGPT.
     """
 
-    def __init__(self, configs : dict ={}, rate_limit: int = 5, api_key: str = "", timeout: int = 100, out_path : str = ""):
+    def __init__(self, configs : dict ={}, rate_limit: int = 5, api_key: str = "", timeout: int = 100, out_path : str = "", verbose: bool = False):
         """
         `configs` a dict containing parameters which will be part of the payload such as model, temperature, etc
         `rate_limit` the maximum number of questions you would like to ask a minute.
         `api_key` OpenAI API key
         `timeout` the amount of time to wait before timing out
         `out_path` the path in which the responses will be outputted
         """
         self.configs = configs
         self.rate_limit = rate_limit
         self.api_key = api_key
         self.timeout = timeout
         self.out_path = out_path
+        self.verbose = verbose
 
     def start(self, question_list):
         """
         `question_list` list of questions to ask ChatGPT
         """
         asyncio.run(self.__start(question_list))
 
     async def __start(self, question_list):
         self.succeed = 0
         self.file_lock = asyncio.Lock()
         self.question_queue = queue.Queue()
         for question in question_list: self.question_queue.put(question)
 
+        question_index = 0
+
         while self.succeed < len(question_list):
-            tasks = [self.async_ask(self.question_queue.get()) for _ in range(self.rate_limit)]
+            tasks = []
+            for _ in range(self.rate_limit):
+                tasks.append(self.async_ask(self.question_queue.get(), question_index))
+                question_index += 1 
+
             await asyncio.gather(*tasks)
 
             if self.succeed < len(question_list): time.sleep(60)
 
     async def log(self, response):
         await self.file_lock.acquire()
 
         with open(self.out_path, "a") as outfile:
             outfile.write(json.dump(response))
             outfile.write("\n")
+
         self.succeed += 1
         self.file_lock.release()
 
-    async def async_ask(self, question):
+    async def async_ask(self, question, question_index):
         try:
+            if self.verbose: print(f"[sleepyask] INFO | ID {question_index} | ASKING: {question}")
+
             payload = {"messages": [{"role": "user", "content": question}], **self.configs}
             response = await openai_async.chat_complete(payload=payload, api_key=self.api_key, timeout=self.timeout)
             
-            if response.status_code != 200: raise ValueError("Should be 200")
+            if response.status_code != 200: 
+                if self.verbose: print(f"[sleepyask] INFO | ID {question_index} | {response.status_code}")
+                raise ValueError("Should be 200")
 
             await self.log(response.text)
-        except: self.question_queue.put(question)
+        except: 
+            if self.verbose: print(f"[sleepyask] INFO | ID {question_index} | ERROR")
+            self.question_queue.put(question)
```

### Comparing `sleepyask-6.0.1/src/sleepyask.egg-info/PKG-INFO` & `sleepyask-6.1.0/src/sleepyask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 6.0.1
+Version: 6.1.0
 Summary: A small tool for automating collecting data from ChatGPT
 Author-email: hwelsters <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/hwelsters/sleepyask
 Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sleepyask Version: 6.0.1 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 6.1.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
```

