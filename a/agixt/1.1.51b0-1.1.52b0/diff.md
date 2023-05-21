# Comparing `tmp/agixt-1.1.51b0.tar.gz` & `tmp/agixt-1.1.52b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.51b0.tar", last modified: Sat May 20 21:50:24 2023, max compression
+gzip compressed data, was "agixt-1.1.52b0.tar", last modified: Sun May 21 00:41:02 2023, max compression
```

## Comparing `agixt-1.1.51b0.tar` & `agixt-1.1.52b0.tar`

### file list

```diff
@@ -1,51 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:50:24.919453 agixt-1.1.51b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 21:50:14.000000 agixt-1.1.51b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-20 21:50:14.000000 agixt-1.1.51b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-05-20 21:50:24.919453 agixt-1.1.51b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:50:24.911453 agixt-1.1.51b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-20 21:50:14.000000 agixt-1.1.51b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 21:50:14.000000 agixt-1.1.51b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 21:50:24.919453 agixt-1.1.51b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-20 21:50:14.000000 agixt-1.1.51b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:50:24.911453 agixt-1.1.51b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:50:24.915453 agixt-1.1.51b0/src/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    25222 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/Commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:50:24.915453 agixt-1.1.51b0/src/agixt/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/Config/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:50:24.919453 agixt-1.1.51b0/src/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/smartchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/smartinstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 21:50:14.000000 agixt-1.1.51b0/src/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:50:24.915453 agixt-1.1.51b0/src/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-05-20 21:50:24.000000 agixt-1.1.51b0/src/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 21:50:24.000000 agixt-1.1.51b0/src/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 21:50:24.000000 agixt-1.1.51b0/src/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-20 21:50:24.000000 agixt-1.1.51b0/src/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 21:50:24.000000 agixt-1.1.51b0/src/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.542321 agixt-1.1.52b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 00:40:48.000000 agixt-1.1.52b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 00:40:48.000000 agixt-1.1.52b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-05-21 00:41:02.542321 agixt-1.1.52b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.534321 agixt-1.1.52b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-21 00:40:48.000000 agixt-1.1.52b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 00:40:48.000000 agixt-1.1.52b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:41:02.542321 agixt-1.1.52b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-21 00:40:48.000000 agixt-1.1.52b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.534321 agixt-1.1.52b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.538321 agixt-1.1.52b0/src/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.538321 agixt-1.1.52b0/src/agixt/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Config/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.542321 agixt-1.1.52b0/src/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.538321 agixt-1.1.52b0/src/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-05-21 00:41:02.000000 agixt-1.1.52b0/src/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-21 00:41:02.000000 agixt-1.1.52b0/src/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:41:02.000000 agixt-1.1.52b0/src/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-21 00:41:02.000000 agixt-1.1.52b0/src/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 00:41:02.000000 agixt-1.1.52b0/src/agixt.egg-info/top_level.txt
```

### Comparing `agixt-1.1.51b0/LICENSE` & `agixt-1.1.52b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/PKG-INFO` & `agixt-1.1.52b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.51b0
+Version: 1.1.52b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.51b0/docs/README.md` & `agixt-1.1.52b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/setup.py` & `agixt-1.1.52b0/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/Chain.py` & `agixt-1.1.52b0/src/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/Commands.py` & `agixt-1.1.52b0/src/agixt/Commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import importlib
 import os
+import glob
 from inspect import signature, Parameter
-from Config.Agent import Agent
 
 
 class Commands:
-    def __init__(self, agent_name: str = "AGiXT", load_commands_flag: bool = True):
-        if agent_name == "undefined":
-            self.agent_name = "AGiXT"
-        else:
-            self.agent_name = agent_name
-        self.CFG = Agent(self.agent_name)
-        self.agent_folder = self.CFG.create_agent_folder(self.agent_name)
-        # self.agent_config_file = self.CFG.create_agent_config_file(self.agent_folder)
-        self.agent_config = self.CFG.load_agent_config(self.agent_name)
+    def __init__(self, agent_config, load_commands_flag: bool = True):
+        self.agent_config = agent_config
         if load_commands_flag:
             self.commands = self.load_commands()
         else:
             self.commands = []
         self.available_commands = self.get_available_commands()
 
     def get_available_commands(self):
@@ -63,15 +56,15 @@
         for command in self.available_commands:
             if command["friendly_name"] == command_name:
                 return command["args"]
         return None
 
     def load_commands(self):
         commands = []
-        command_files = self.CFG.load_command_files()
+        command_files = glob.glob("commands/*.py")
         for command_file in command_files:
             module_name = os.path.splitext(os.path.basename(command_file))[0]
             module = importlib.import_module(f"commands.{module_name}")
             if issubclass(getattr(module, module_name), Commands):
                 command_class = getattr(module, module_name)()
                 if hasattr(command_class, "commands"):
                     for (
```

### Comparing `agixt-1.1.51b0/src/agixt/Config/Agent.py` & `agixt-1.1.52b0/src/agixt/Config/Agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 import json
 import glob
 import uuid
 import shutil
 import importlib
 import yaml
 from pathlib import Path
-from dotenv import load_dotenv
 from inspect import signature, Parameter
 from provider import Provider
 from Config import Config
-
-load_dotenv()
+from Memories import Memories
+from Commands import Commands
 
 
 class Agent(Config):
     def __init__(self, agent_name=None):
         # General Configuration
-        self.AGENT_NAME = agent_name if agent_name is not None else "AGiXT"
+        self.agent_name = agent_name if agent_name is not None else "AGiXT"
         # Need to get the following from the agent config file:
         self.AGENT_CONFIG = self.get_agent_config()
+        self.available_commands = Commands(self.AGENT_CONFIG).get_available_commands()
+        self.execute = Commands(self.AGENT_CONFIG).execute_command
         # AI Configuration
         if "settings" in self.AGENT_CONFIG:
             self.PROVIDER_SETTINGS = self.AGENT_CONFIG["settings"]
             if "provider" in self.PROVIDER_SETTINGS:
                 self.AI_PROVIDER = self.PROVIDER_SETTINGS["provider"]
                 self.PROVIDER = Provider(self.AI_PROVIDER, **self.PROVIDER_SETTINGS)
                 self.instruct = self.PROVIDER.instruct
@@ -42,32 +43,48 @@
                 else:
                     self.EMBEDDER = "default"
             if "MAX_TOKENS" in self.PROVIDER_SETTINGS:
                 self.MAX_TOKENS = self.PROVIDER_SETTINGS["MAX_TOKENS"]
             else:
                 self.MAX_TOKENS = 4000
 
-        # Memory Settings
-        self.USE_LONG_TERM_MEMORY_ONLY = os.getenv("USE_LONG_TERM_MEMORY_ONLY", False)
         # Yaml Memory
-        self.memory_file = f"agents/{self.AGENT_NAME}.yaml"
+        self.memory_file = f"agents/{self.agent_name}.yaml"
         self._create_parent_directories(self.memory_file)
         self.memory = self.load_memory()
+        self.memories = Memories(self.agent_name, self)
         self.agent_instances = {}
+        self.agent_config = self.load_agent_config(self.agent_name)
         self.commands = self.load_commands()
 
     def _load_agent_config_keys(self, keys):
         for key in keys:
             if key in self.AGENT_CONFIG:
                 setattr(self, key, self.AGENT_CONFIG[key])
 
     def _create_parent_directories(self, file_path):
         path = Path(file_path)
         path.parent.mkdir(parents=True, exist_ok=True)
 
+    def get_commands_string(self):
+        if len(self.available_commands) == 0:
+            return "No commands."
+
+        enabled_commands = filter(
+            lambda command: command.get("enabled", True), self.available_commands
+        )
+        if not enabled_commands:
+            return "No commands."
+
+        friendly_names = map(
+            lambda command: f"{command['friendly_name']} - {command['name']}({command['args']})",
+            enabled_commands,
+        )
+        return "\n".join(friendly_names)
+
     def get_provider(self):
         config_file = self.get_agent_config()
         if "provider" in config_file:
             return config_file["provider"]
         else:
             return "openai"
 
@@ -98,18 +115,14 @@
             command_class = getattr(module, module_name.lower())()
             if hasattr(command_class, "commands"):
                 for command_name, command_function in command_class.commands.items():
                     params = self.get_command_params(command_function)
                     commands.append((command_name, command_function.__name__, params))
         return commands
 
-    def load_command_files(self):
-        command_files = glob.glob("commands/*.py")
-        return command_files
-
     def create_agent_config_file(self, agent_name, provider_settings, commands):
         agent_dir = os.path.join("agents", agent_name)
         agent_config_file = os.path.join(agent_dir, "config.json")
         if (
             provider_settings is None
             or provider_settings == ""
             or provider_settings == {}
@@ -230,29 +243,29 @@
         if os.path.exists(agent_folder):
             shutil.rmtree(agent_folder)
 
         return {"message": f"Agent {agent_name} deleted."}, 200
 
     def get_agent_config(self):
         while True:
-            agent_file = os.path.abspath(f"agents/{self.AGENT_NAME}/config.json")
+            agent_file = os.path.abspath(f"agents/{self.agent_name}/config.json")
             if os.path.exists(agent_file):
                 with open(agent_file, "r") as f:
                     file_content = f.read().strip()
                     if file_content:
                         agent_config = json.loads(file_content)
                         break
                     else:
-                        self.add_agent(self.AGENT_NAME, {})
+                        self.add_agent(self.agent_name, {})
             else:
-                self.add_agent(self.AGENT_NAME, {})
+                self.add_agent(self.agent_name, {})
         return agent_config
 
     def update_agent_config(self, new_config, config_key):
-        agent_name = self.AGENT_NAME
+        agent_name = self.agent_name
         agent_config_file = os.path.join("agents", agent_name, "config.json")
         if os.path.exists(agent_config_file):
             with open(agent_config_file, "r") as f:
                 current_config = json.load(f)
 
             # Ensure the config_key is present in the current configuration
             if config_key not in current_config:
```

### Comparing `agixt-1.1.51b0/src/agixt/Config/__init__.py` & `agixt-1.1.52b0/src/agixt/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/CustomPrompt.py` & `agixt-1.1.52b0/src/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/Embedding.py` & `agixt-1.1.52b0/src/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/Memories.py` & `agixt-1.1.52b0/src/agixt/Memories.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import chromadb
 from typing import List
 import spacy
 from hashlib import sha256
 from Embedding import Embedding
 from datetime import datetime
 from collections import Counter
+import pandas as pd
+import docx2txt
+import pdfplumber
+from playwright.async_api import async_playwright
+from bs4 import BeautifulSoup
 
 
 class Memories:
-    def __init__(self, AGENT_NAME: str = "AGiXT", AgentConfig=None, nlp=None):
+    def __init__(self, AGENT_NAME: str = "AGiXT", AgentConfig=None):
         self.AGENT_NAME = AGENT_NAME
         self.CFG = AgentConfig
-        self.nlp = nlp if nlp else self.load_spacy_model()
+        self.nlp = self.load_spacy_model()
         self.nlp.max_length = 999999999999999999999999999999999
         embedder = Embedding(CFG=AgentConfig)
         self.embedding_function = embedder.embed
         self.chunk_size = embedder.chunk_size
         self.chroma_persist_dir = f"agents/{self.AGENT_NAME}/memories"
         self.chroma_client = self.initialize_chroma_client()
         self.collection = self.get_or_create_collection()
@@ -153,7 +158,56 @@
         if chunk:
             chunk_text = " ".join(token.text for token in chunk)
             content_chunks.append((self.score_chunk(chunk_text, keywords), chunk_text))
 
         # Sort the chunks by their score in descending order before returning them
         content_chunks.sort(key=lambda x: x[0], reverse=True)
         return [chunk_text for score, chunk_text in content_chunks]
+
+    def read_file(self, file_path: str):
+        try:
+            # If file extension is pdf, convert to text
+            if file_path.endswith(".pdf"):
+                with pdfplumber.open(file_path) as pdf:
+                    content = "\n".join([page.extract_text() for page in pdf.pages])
+            # If file extension is xls, convert to csv
+            elif file_path.endswith(".xls") or file_path.endswith(".xlsx"):
+                content = pd.read_excel(file_path).to_csv()
+            # If file extension is doc, convert to text
+            elif file_path.endswith(".doc") or file_path.endswith(".docx"):
+                content = docx2txt.process(file_path)
+            # TODO: If file is an image, classify it in text.
+            # Otherwise just read the file
+            else:
+                with open(file_path, "r") as f:
+                    content = f.read()
+            self.store_result(task_name=file_path, result=content)
+            return True
+        except:
+            return False
+
+    async def read_website(self, url):
+        try:
+            async with async_playwright() as p:
+                browser = await p.chromium.launch()
+                context = await browser.new_context()
+                page = await context.new_page()
+                await page.goto(url)
+                content = await page.content()
+
+                # Scrape links and their titles
+                links = await page.query_selector_all("a")
+                link_list = []
+                for link in links:
+                    title = await page.evaluate("(link) => link.textContent", link)
+                    href = await page.evaluate("(link) => link.href", link)
+                    link_list.append((title, href))
+
+                await browser.close()
+                soup = BeautifulSoup(content, "html.parser")
+                text_content = soup.get_text()
+                text_content = " ".join(text_content.split())
+                if text_content:
+                    self.store_result(url, text_content)
+                return text_content, link_list
+        except:
+            return None, None
```

### Comparing `agixt-1.1.51b0/src/agixt/app.py` & `agixt-1.1.52b0/src/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/__init__.py` & `agixt-1.1.52b0/src/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/azure.py` & `agixt-1.1.52b0/src/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/bing.py` & `agixt-1.1.52b0/src/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/claude.py` & `agixt-1.1.52b0/src/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/fastchat.py` & `agixt-1.1.52b0/src/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/gpt4all.py` & `agixt-1.1.52b0/src/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/gpt4free.py` & `agixt-1.1.52b0/src/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/gpugpt4all.py` & `agixt-1.1.52b0/src/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/huggingchat.py` & `agixt-1.1.52b0/src/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/kobold.py` & `agixt-1.1.52b0/src/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/llamacpp.py` & `agixt-1.1.52b0/src/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/oobabooga.py` & `agixt-1.1.52b0/src/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/openai.py` & `agixt-1.1.52b0/src/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/palm.py` & `agixt-1.1.52b0/src/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/provider/transformer.py` & `agixt-1.1.52b0/src/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt/requirements.txt` & `agixt-1.1.52b0/src/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.51b0/src/agixt.egg-info/PKG-INFO` & `agixt-1.1.52b0/src/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.51b0
+Version: 1.1.52b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.51b0/src/agixt.egg-info/SOURCES.txt` & `agixt-1.1.52b0/src/agixt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 docs/README.md
 src/agixt/AGiXT.py
 src/agixt/Chain.py
 src/agixt/Commands.py
 src/agixt/CustomPrompt.py
 src/agixt/Embedding.py
 src/agixt/Memories.py
+src/agixt/Tasks.py
 src/agixt/__init__.py
 src/agixt/app.py
-src/agixt/main.py
 src/agixt/requirements.txt
-src/agixt/smartchat.py
-src/agixt/smartinstruct.py
 src/agixt/streamlit.py
 src/agixt/version
 src/agixt.egg-info/PKG-INFO
 src/agixt.egg-info/SOURCES.txt
 src/agixt.egg-info/dependency_links.txt
 src/agixt.egg-info/requires.txt
 src/agixt.egg-info/top_level.txt
```

### Comparing `agixt-1.1.51b0/src/agixt.egg-info/requires.txt` & `agixt-1.1.52b0/src/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

