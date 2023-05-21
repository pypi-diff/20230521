# Comparing `tmp/agixt-1.1.57b0.tar.gz` & `tmp/agixt-1.1.58b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.57b0.tar", last modified: Sun May 21 12:32:52 2023, max compression
+gzip compressed data, was "agixt-1.1.58b0.tar", last modified: Sun May 21 16:44:25 2023, max compression
```

## Comparing `agixt-1.1.57b0.tar` & `agixt-1.1.58b0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:52.987738 agixt-1.1.57b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 12:32:37.000000 agixt-1.1.57b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 12:32:37.000000 agixt-1.1.57b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 12:32:52.987738 agixt-1.1.57b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:52.987738 agixt-1.1.57b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/Commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:52.987738 agixt-1.1.57b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 12:32:37.000000 agixt-1.1.57b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:52.987738 agixt-1.1.57b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 12:32:52.000000 agixt-1.1.57b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-21 12:32:52.000000 agixt-1.1.57b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:32:52.000000 agixt-1.1.57b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-21 12:32:52.000000 agixt-1.1.57b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 12:32:52.000000 agixt-1.1.57b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:52.987738 agixt-1.1.57b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-21 12:32:37.000000 agixt-1.1.57b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 12:32:37.000000 agixt-1.1.57b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 12:32:52.987738 agixt-1.1.57b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 12:32:37.000000 agixt-1.1.57b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:44:25.587446 agixt-1.1.58b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 16:44:14.000000 agixt-1.1.58b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 16:44:14.000000 agixt-1.1.58b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 16:44:25.587446 agixt-1.1.58b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:44:25.587446 agixt-1.1.58b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    17509 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:44:25.587446 agixt-1.1.58b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 16:44:14.000000 agixt-1.1.58b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:44:25.587446 agixt-1.1.58b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 16:44:25.000000 agixt-1.1.58b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-21 16:44:25.000000 agixt-1.1.58b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 16:44:25.000000 agixt-1.1.58b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-21 16:44:25.000000 agixt-1.1.58b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 16:44:25.000000 agixt-1.1.58b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:44:25.587446 agixt-1.1.58b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-21 16:44:14.000000 agixt-1.1.58b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 16:44:14.000000 agixt-1.1.58b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 16:44:25.587446 agixt-1.1.58b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 16:44:14.000000 agixt-1.1.58b0/setup.py
```

### Comparing `agixt-1.1.57b0/LICENSE` & `agixt-1.1.58b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/PKG-INFO` & `agixt-1.1.58b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.57b0
+Version: 1.1.58b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.57b0/agixt/AGiXT.py` & `agixt-1.1.58b0/agixt/AGiXT.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,27 +123,29 @@
             execution_response = self.execution_agent(
                 execution_response=self.response,
                 task=task,
                 context_results=context_results,
                 **kwargs,
             )
             return_response = ""
-            if "response" in self.response:
-                # Turn it into json
+            try:
                 self.response = json.loads(self.response)
-                return_response = self.response["response"]
-            if "commands" in self.response:
-                if self.response["commands"] != {}:
+                if "response" in self.response:
+                    return_response = self.response["response"]
+                if "commands" in self.response:
+                    if self.response["commands"] != {}:
+                        return_response += (
+                            f"\n\nCommands Executed:\n{self.response['commands']}"
+                        )
+                if execution_response:
                     return_response += (
-                        f"\n\nCommands Executed:\n{self.response['commands']}"
+                        f"\n\nCommand Execution Response:\n{execution_response}"
                     )
-            if execution_response:
-                return_response += (
-                    f"\n\nCommand Execution Response:\n{execution_response}"
-                )
+            except:
+                return_response = self.response
             self.response = return_response
         print(f"Response: {self.response}")
         self.agent.memories.store_result(task, self.response)
         self.agent.log_interaction("USER", task)
         self.agent.log_interaction(self.agent_name, self.response)
         return self.response
```

### Comparing `agixt-1.1.57b0/agixt/Agent.py` & `agixt-1.1.58b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/Chain.py` & `agixt-1.1.58b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/Commands.py` & `agixt-1.1.58b0/agixt/Commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,31 +85,29 @@
                                 params,
                             )
                         )
         # Return the commands list
         return commands
 
     def get_extension_settings(self):
-        settings = []
+        settings = {}
         command_files = glob.glob("commands/*.py")
         for command_file in command_files:
             module_name = os.path.splitext(os.path.basename(command_file))[0]
             module = importlib.import_module(f"commands.{module_name}")
             if issubclass(getattr(module, module_name), Commands):
                 command_class = getattr(module, module_name)()
                 params = self.get_command_params(command_class.__init__)
                 # Remove self and kwargs from params
                 if "self" in params:
                     del params["self"]
                 if "kwargs" in params:
                     del params["kwargs"]
                 if params != {}:
-                    settings.append(list(params.keys()))
-        settings = [item for sublist in settings for item in sublist]
-        settings = list(set(settings))
+                    settings[module_name] = params
         return settings
 
     def get_command_params(self, func):
         params = {}
         sig = signature(func)
         for name, param in sig.parameters.items():
             if name == "self":
```

### Comparing `agixt-1.1.57b0/agixt/Config.py` & `agixt-1.1.58b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/CustomPrompt.py` & `agixt-1.1.58b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/Embedding.py` & `agixt-1.1.58b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/Memories.py` & `agixt-1.1.58b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/Tasks.py` & `agixt-1.1.58b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/app.py` & `agixt-1.1.58b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/__init__.py` & `agixt-1.1.58b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/azure.py` & `agixt-1.1.58b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/chatgpt.py` & `agixt-1.1.58b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/claude.py` & `agixt-1.1.58b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/fastchat.py` & `agixt-1.1.58b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/gpt4all.py` & `agixt-1.1.58b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/gpt4free.py` & `agixt-1.1.58b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.58b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/huggingchat.py` & `agixt-1.1.58b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/kobold.py` & `agixt-1.1.58b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/llamacpp.py` & `agixt-1.1.58b0/agixt/provider/llamacpp.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,32 +9,50 @@
 class LlamacppProvider:
     def __init__(
         self,
         MODEL_PATH: str = "",
         MAX_TOKENS: int = 2000,
         AI_TEMPERATURE: float = 0.7,
         AI_MODEL: str = "default",
+        GPU_LAYERS: int = 0,
+        BATCH_SIZE: int = 512,
+        THREADS: int = 0,
+        STOP_SEQUENCE: str = "\n",
         **kwargs
     ):
         self.requirements = ["llama-cpp-python"]
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
         self.AI_MODEL = AI_MODEL
+        self.GPU_LAYERS = GPU_LAYERS
+        self.BATCH_SIZE = BATCH_SIZE
+        self.THREADS = THREADS if THREADS != 0 else None
+        self.STOP_SEQUENCE = STOP_SEQUENCE
 
         if MODEL_PATH:
             try:
                 self.MAX_TOKENS = int(self.MAX_TOKENS)
             except:
                 self.MAX_TOKENS = 2000
 
         if os.path.isfile(MODEL_PATH):
-            self.model = Llama(model_path=MODEL_PATH, n_ctx=self.MAX_TOKENS * 2)
+            self.model = Llama(
+                model_path=MODEL_PATH,
+                n_ctx=(int(self.MAX_TOKENS) * 2),
+                n_gpu_layers=self.GPU_LAYERS,
+                n_batch=self.BATCH_SIZE,
+                n_threads=self.THREADS,
+            )
         else:
-            print("Failed to import model - not a file")
+            print("Unable to find model path.")
 
     def instruct(self, prompt, tokens: int = 0):
+        max_tokens = int(self.MAX_TOKENS) - tokens
+        if max_tokens < 1:
+            max_tokens = int(self.MAX_TOKENS)
+
         return self.model(
             prompt,
-            max_tokens=self.MAX_TOKENS,
-            stop=["\n"],
+            max_tokens=max_tokens,
+            stop=[self.STOP_SEQUENCE],
             temperature=float(self.AI_TEMPERATURE),
         )["choices"][0]["text"]
```

### Comparing `agixt-1.1.57b0/agixt/provider/oobabooga.py` & `agixt-1.1.58b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/openai.py` & `agixt-1.1.58b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/palm.py` & `agixt-1.1.58b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/provider/transformer.py` & `agixt-1.1.58b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt/requirements.txt` & `agixt-1.1.58b0/agixt/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #### This block includes deps for local providers - all may big dependencies due to torch
 --extra-index-url https://download.pytorch.org/whl/cpu torch
 chromadb
 git+https://github.com/huggingface/transformers
 sentence-transformers
-llama-cpp-python==0.1.48
+llama-cpp-python
 accelerate
 nomic
 ####
 argparse
 anthropic
 beautifulsoup4
 captcha-solver
```

### Comparing `agixt-1.1.57b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.58b0/agixt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.57b0
+Version: 1.1.58b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.57b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.58b0/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/agixt.egg-info/requires.txt` & `agixt-1.1.58b0/agixt.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 chromadb
 sentence-transformers
-llama-cpp-python==0.1.48
+llama-cpp-python
 accelerate
 nomic
 argparse
 anthropic
 beautifulsoup4
 captcha-solver
 docker
```

### Comparing `agixt-1.1.57b0/docs/README.md` & `agixt-1.1.58b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.57b0/setup.py` & `agixt-1.1.58b0/setup.py`

 * *Files identical despite different names*

