# Comparing `tmp/agixt-1.1.55b0.tar.gz` & `tmp/agixt-1.1.56b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.55b0.tar", last modified: Sun May 21 04:12:06 2023, max compression
+gzip compressed data, was "agixt-1.1.56b0.tar", last modified: Sun May 21 06:11:14 2023, max compression
```

## Comparing `agixt-1.1.55b0.tar` & `agixt-1.1.56b0.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.575996 agixt-1.1.55b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 04:11:49.000000 agixt-1.1.55b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 04:11:49.000000 agixt-1.1.55b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-21 04:12:06.575996 agixt-1.1.55b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.571996 agixt-1.1.55b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.571996 agixt-1.1.55b0/agixt/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Config/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.575996 agixt-1.1.55b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.571996 agixt-1.1.55b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-21 04:12:06.000000 agixt-1.1.55b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-21 04:12:06.000000 agixt-1.1.55b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:12:06.000000 agixt-1.1.55b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-21 04:12:06.000000 agixt-1.1.55b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 04:12:06.000000 agixt-1.1.55b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.575996 agixt-1.1.55b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-21 04:11:49.000000 agixt-1.1.55b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 04:11:49.000000 agixt-1.1.55b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:12:06.575996 agixt-1.1.55b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 04:11:49.000000 agixt-1.1.55b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:14.632206 agixt-1.1.56b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 06:10:55.000000 agixt-1.1.56b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 06:10:55.000000 agixt-1.1.56b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-21 06:11:14.632206 agixt-1.1.56b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:14.628205 agixt-1.1.56b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:14.632206 agixt-1.1.56b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 06:10:55.000000 agixt-1.1.56b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:14.632206 agixt-1.1.56b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-21 06:11:14.000000 agixt-1.1.56b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-21 06:11:14.000000 agixt-1.1.56b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 06:11:14.000000 agixt-1.1.56b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-21 06:11:14.000000 agixt-1.1.56b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 06:11:14.000000 agixt-1.1.56b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 06:11:14.632206 agixt-1.1.56b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-21 06:10:55.000000 agixt-1.1.56b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 06:10:55.000000 agixt-1.1.56b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 06:11:14.632206 agixt-1.1.56b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 06:10:55.000000 agixt-1.1.56b0/setup.py
```

### Comparing `agixt-1.1.55b0/LICENSE` & `agixt-1.1.56b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/PKG-INFO` & `agixt-1.1.56b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.55b0
+Version: 1.1.56b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.55b0/agixt/AGiXT.py` & `agixt-1.1.56b0/agixt/AGiXT.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import asyncio
 import regex
 import json
 from datetime import datetime
-from Config.Agent import Agent
+from Agent import Agent
 from CustomPrompt import CustomPrompt
 from typing import List, Dict
 from duckduckgo_search import ddg
 from urllib.parse import urlparse
 
 
 class AGiXT:
@@ -400,15 +400,15 @@
         return [
             {"task_name": task_name} for task_name in new_tasks if task_name.strip()
         ]
 
     async def websearch_agent(
         self, task: str = "What are the latest breakthroughs in AI?", depth: int = 3
     ):
-        async def resursive_browsing(self, task, links):
+        async def resursive_browsing(task, links):
             try:
                 words = links.split()
                 links = [
                     word for word in words if urlparse(word).scheme in ["http", "https"]
                 ]
             except:
                 links = links
@@ -423,15 +423,15 @@
                     if url.startswith("http"):
                         print(f"Scraping: {url}")
                         if url not in self.browsed_links:
                             self.browsed_links.append(url)
                             (
                                 collected_data,
                                 link_list,
-                            ) = await self.memories.read_website(url)
+                            ) = await self.agent.memories.read_website(url)
                             if link_list is not None:
                                 if len(link_list) > 0:
                                     if len(link_list) > 5:
                                         link_list = link_list[:3]
                                     try:
                                         pick_a_link = self.run(
                                             task=task,
```

### Comparing `agixt-1.1.55b0/agixt/Chain.py` & `agixt-1.1.56b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/Commands.py` & `agixt-1.1.56b0/agixt/Commands.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,21 +55,25 @@
     def get_command_args(self, command_name: str):
         for command in self.available_commands:
             if command["friendly_name"] == command_name:
                 return command["args"]
         return None
 
     def load_commands(self):
+        try:
+            settings = self.agent_config["settings"]
+        except:
+            settings = {}
         commands = []
         command_files = glob.glob("commands/*.py")
         for command_file in command_files:
             module_name = os.path.splitext(os.path.basename(command_file))[0]
             module = importlib.import_module(f"commands.{module_name}")
             if issubclass(getattr(module, module_name), Commands):
-                command_class = getattr(module, module_name)()
+                command_class = getattr(module, module_name)(**settings)
                 if hasattr(command_class, "commands"):
                     for (
                         command_name,
                         command_function,
                     ) in command_class.commands.items():
                         params = self.get_command_params(command_function)
                         # Store the module along with the function name
@@ -80,18 +84,40 @@
                                 command_function.__name__,
                                 params,
                             )
                         )
         # Return the commands list
         return commands
 
+    def get_extension_settings(self):
+        settings = []
+        command_files = glob.glob("commands/*.py")
+        for command_file in command_files:
+            module_name = os.path.splitext(os.path.basename(command_file))[0]
+            module = importlib.import_module(f"commands.{module_name}")
+            if issubclass(getattr(module, module_name), Commands):
+                command_class = getattr(module, module_name)()
+                params = self.get_command_params(command_class.__init__)
+                # Remove self and kwargs from params
+                if "self" in params:
+                    del params["self"]
+                if "kwargs" in params:
+                    del params["kwargs"]
+                if params != {}:
+                    settings.append(list(params.keys()))
+        settings = [item for sublist in settings for item in sublist]
+        settings = list(set(settings))
+        return settings
+
     def get_command_params(self, func):
         params = {}
         sig = signature(func)
         for name, param in sig.parameters.items():
+            if name == "self":
+                continue
             if param.default == Parameter.empty:
                 params[name] = None
             else:
                 params[name] = param.default
         return params
 
     def find_command(self, command_name: str):
```

### Comparing `agixt-1.1.55b0/agixt/Config/Agent.py` & `agixt-1.1.56b0/agixt/Agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 import uuid
 import shutil
 import importlib
 import yaml
 from pathlib import Path
 from inspect import signature, Parameter
 from provider import Provider
-from Config import Config
 from Memories import Memories
 from Commands import Commands
 
 
-class Agent(Config):
+class Agent:
     def __init__(self, agent_name=None):
         # General Configuration
         self.agent_name = agent_name if agent_name is not None else "AGiXT"
         # Need to get the following from the agent config file:
         self.AGENT_CONFIG = self.get_agent_config()
         self.available_commands = Commands(self.AGENT_CONFIG).get_available_commands()
         self.execute = Commands(self.AGENT_CONFIG).execute_command
```

### Comparing `agixt-1.1.55b0/agixt/CustomPrompt.py` & `agixt-1.1.56b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/Embedding.py` & `agixt-1.1.56b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/Memories.py` & `agixt-1.1.56b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/Tasks.py` & `agixt-1.1.56b0/agixt/Tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from AGiXT import AGiXT
 import re
-from Config.Agent import Agent
+from Agent import Agent
 from collections import deque
 
 
 class Tasks:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
         self.agent = Agent(self.agent_name)
@@ -68,15 +68,15 @@
                 task = self.task_list.popleft()
             if task["task_name"] == "None" or task["task_name"] == "None.":
                 break
             self.update_output_list(
                 f"\nExecuting task {task['task_id']}: {task['task_name']}\n"
             )
             if smart:
-                result = self.smart_instruct(
+                result = AGiXT(self.agent_name).smart_instruct(
                     task=task["task_name"],
                     shots=3,
                     async_exec=async_exec,
                     **kwargs,
                 )
             else:
                 result = AGiXT(self.agent_name).instruction_agent(
```

### Comparing `agixt-1.1.55b0/agixt/app.py` & `agixt-1.1.56b0/agixt/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uvicorn
 from fastapi import FastAPI, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from pydantic import BaseModel
 from Config import Config
 from AGiXT import AGiXT
-from Config.Agent import Agent
+from Agent import Agent
 from Commands import Commands
 from Chain import Chain
 from CustomPrompt import CustomPrompt
 import threading
 from typing import Optional, Dict, List, Any
 from provider import get_provider_options
 from Embedding import get_embedding_providers
```

### Comparing `agixt-1.1.55b0/agixt/provider/__init__.py` & `agixt-1.1.56b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/azure.py` & `agixt-1.1.56b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/bing.py` & `agixt-1.1.56b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/claude.py` & `agixt-1.1.56b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/fastchat.py` & `agixt-1.1.56b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/gpt4all.py` & `agixt-1.1.56b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/gpt4free.py` & `agixt-1.1.56b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.56b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/huggingchat.py` & `agixt-1.1.56b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/kobold.py` & `agixt-1.1.56b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/llamacpp.py` & `agixt-1.1.56b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/oobabooga.py` & `agixt-1.1.56b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/openai.py` & `agixt-1.1.56b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/palm.py` & `agixt-1.1.56b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/provider/transformer.py` & `agixt-1.1.56b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/agixt/requirements.txt` & `agixt-1.1.56b0/agixt/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 jsonschema
 openai
 playwright
 playsound==1.2.2
 pre-commit
 pytz
 pynacl
-python-dotenv
 python-git
 PyGithub
 selenium
 sendgrid
 tiktoken
 tweepy
 webdriver_manager
```

### Comparing `agixt-1.1.55b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.56b0/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.55b0
+Version: 1.1.56b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.55b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.56b0/agixt.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 LICENSE
 MANIFEST.in
 pyproject.toml
 setup.py
 agixt/AGiXT.py
+agixt/Agent.py
 agixt/Chain.py
 agixt/Commands.py
+agixt/Config.py
 agixt/CustomPrompt.py
 agixt/Embedding.py
 agixt/Memories.py
 agixt/Tasks.py
 agixt/__init__.py
 agixt/app.py
 agixt/requirements.txt
 agixt/streamlit.py
 agixt/version
 agixt.egg-info/PKG-INFO
 agixt.egg-info/SOURCES.txt
 agixt.egg-info/dependency_links.txt
 agixt.egg-info/requires.txt
 agixt.egg-info/top_level.txt
-agixt/Config/Agent.py
-agixt/Config/__init__.py
 agixt/provider/__init__.py
 agixt/provider/azure.py
 agixt/provider/bard.py
 agixt/provider/bing.py
 agixt/provider/claude.py
 agixt/provider/fastchat.py
 agixt/provider/gpt4all.py
```

### Comparing `agixt-1.1.55b0/agixt.egg-info/requires.txt` & `agixt-1.1.56b0/agixt.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 jsonschema
 openai
 playwright
 playsound==1.2.2
 pre-commit
 pytz
 pynacl
-python-dotenv
 python-git
 PyGithub
 selenium
 sendgrid
 tiktoken
 tweepy
 webdriver_manager
```

### Comparing `agixt-1.1.55b0/docs/README.md` & `agixt-1.1.56b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.55b0/setup.py` & `agixt-1.1.56b0/setup.py`

 * *Files identical despite different names*

