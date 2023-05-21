# Comparing `tmp/agixt-1.1.60b0.tar.gz` & `tmp/agixt-1.1.61b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.60b0.tar", last modified: Sun May 21 19:55:44 2023, max compression
+gzip compressed data, was "agixt-1.1.61b0.tar", last modified: Sun May 21 21:00:55 2023, max compression
```

## Comparing `agixt-1.1.60b0.tar` & `agixt-1.1.61b0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:55:44.442127 agixt-1.1.60b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 19:55:28.000000 agixt-1.1.60b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 19:55:28.000000 agixt-1.1.60b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 19:55:44.442127 agixt-1.1.60b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:55:44.438127 agixt-1.1.60b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:55:44.442127 agixt-1.1.60b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:55:44.438127 agixt-1.1.60b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 19:55:44.000000 agixt-1.1.60b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-21 19:55:44.000000 agixt-1.1.60b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:55:44.000000 agixt-1.1.60b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-21 19:55:44.000000 agixt-1.1.60b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 19:55:44.000000 agixt-1.1.60b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:55:44.442127 agixt-1.1.60b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-21 19:55:28.000000 agixt-1.1.60b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 19:55:28.000000 agixt-1.1.60b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:55:44.442127 agixt-1.1.60b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 19:55:28.000000 agixt-1.1.60b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:00:55.661923 agixt-1.1.61b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 21:00:43.000000 agixt-1.1.61b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 21:00:43.000000 agixt-1.1.61b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 21:00:55.661923 agixt-1.1.61b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:00:55.657923 agixt-1.1.61b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:00:55.661923 agixt-1.1.61b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 21:00:43.000000 agixt-1.1.61b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:00:55.657923 agixt-1.1.61b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 21:00:55.000000 agixt-1.1.61b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-21 21:00:55.000000 agixt-1.1.61b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:00:55.000000 agixt-1.1.61b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-21 21:00:55.000000 agixt-1.1.61b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 21:00:55.000000 agixt-1.1.61b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:00:55.661923 agixt-1.1.61b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-21 21:00:43.000000 agixt-1.1.61b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 21:00:44.000000 agixt-1.1.61b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:00:55.661923 agixt-1.1.61b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 21:00:44.000000 agixt-1.1.61b0/setup.py
```

### Comparing `agixt-1.1.60b0/LICENSE` & `agixt-1.1.61b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/PKG-INFO` & `agixt-1.1.61b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.60b0
+Version: 1.1.61b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.60b0/agixt/AGiXT.py` & `agixt-1.1.61b0/agixt/AGiXT.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 import asyncio
 import regex
 import json
 from datetime import datetime
 from Agent import Agent
 from CustomPrompt import CustomPrompt
-from typing import List, Dict
 from duckduckgo_search import ddg
 from urllib.parse import urlparse
 
 
 class AGiXT:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
@@ -78,17 +77,15 @@
         websearch: bool = False,
         websearch_depth: int = 3,
         async_exec: bool = False,
         learn_file: str = "",
         **kwargs,
     ):
         if learn_file != "":
-            learning_file = self.agent.memories.read_file(
-                task=task, file_path=learn_file
-            )
+            learning_file = self.agent.memories.read_file(file_path=learn_file)
             if learning_file == False:
                 return "Failed to read file."
         formatted_prompt, unformatted_prompt, tokens = self.format_prompt(
             task=task,
             top_results=context_results,
             prompt=prompt,
             **kwargs,
@@ -379,39 +376,14 @@
                     else:
                         return f"\Command not recognized: {command_name} ."
         except:
             print("\nERROR IN EXECUTION_AGENT, validated_response:\n")
             print(validated_response)
             return "\nNo commands were executed.\n"
 
-    def task_agent(self, result: Dict, task_description: str, task_list) -> List[Dict]:
-        tasks = [task["task_name"] for task in task_list]
-        if len(tasks) == 0:
-            return []
-        task_list = ", ".join(tasks)
-
-        response = self.run(
-            task=self.primary_objective,
-            prompt="task",
-            result=result,
-            task_description=task_description,
-            tasks=task_list,
-        )
-
-        lines = response.split("\n") if "\n" in response else [response]
-        new_tasks = []
-        for line in lines:
-            match = re.match(r"(\d+)\.\s+(.*)", line)
-            if match:
-                task_id, task_name = match.groups()
-                new_tasks.append(
-                    {"task_id": int(task_id), "task_name": task_name.strip()}
-                )
-        return new_tasks
-
     async def websearch_agent(
         self, task: str = "What are the latest breakthroughs in AI?", depth: int = 3
     ):
         async def resursive_browsing(task, links):
             try:
                 words = links.split()
                 links = [
@@ -453,27 +425,7 @@
         results = self.run(task=task, prompt="WebSearch")
         results = results.split("\n")
         for result in results:
             search_string = result.lstrip("0123456789. ")
             links = ddg(search_string, max_results=depth)
             if links is not None:
                 await resursive_browsing(task, links)
-
-    def instruction_agent(self, task, learn_file: str = "", **kwargs):
-        if "task_name" in task:
-            task = task["task_name"]
-        resolver = self.run(
-            task=task,
-            prompt="SmartInstruct-StepByStep",
-            context_results=6,
-            learn_file=learn_file,
-            **kwargs,
-        )
-        execution_response = self.run(
-            task=task,
-            prompt="SmartInstruct-Execution",
-            previous_response=resolver,
-            **kwargs,
-        )
-        return (
-            f"RESPONSE:\n{resolver}\n\nCommand Execution Response{execution_response}"
-        )
```

### Comparing `agixt-1.1.60b0/agixt/Agent.py` & `agixt-1.1.61b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/Chain.py` & `agixt-1.1.61b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/Commands.py` & `agixt-1.1.61b0/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/Config.py` & `agixt-1.1.61b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/CustomPrompt.py` & `agixt-1.1.61b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/Embedding.py` & `agixt-1.1.61b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/Memories.py` & `agixt-1.1.61b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/Tasks.py` & `agixt-1.1.61b0/agixt/Tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 import os
 import json
 import uuid
 import yaml
 from pathlib import Path
 from Agent import Agent
 from collections import deque
+from typing import List, Dict
 
 
 class Tasks:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
         self.agent = Agent(self.agent_name)
         self.primary_objective = None
         self.task_list = deque([])
         self.output_list = []
-        self.stop_running_event = None
+        self.stop_running_event = False
 
     def save_task(self):
         task_name = re.sub(
             r"[^\w\s]", "", self.primary_objective
         )  # remove non-alphanumeric & non-space characters
         task_name = task_name[:15]  # truncate to 15 characters
 
@@ -56,15 +57,15 @@
         except FileNotFoundError:
             print(f"No saved task found with the name '{task_name}'.")
         except Exception as e:
             print(f"An error occurred while loading the task: {e}")
 
     def get_status(self):
         try:
-            return not self.stop_running_event.is_set()
+            return True
         except:
             return False
 
     def get_output_list(self):
         return self.output_list
 
     def save_task_output(self, agent_name, task_output):
@@ -103,21 +104,67 @@
             print(f"No saved task output found with the name '{task_name}'.")
             return None
         except Exception as e:
             print(f"An error occurred while loading the task output: {e}")
             return None
 
     def update_output_list(self, output):
-        print(self.save_task_output(self.agent_name, output, self.primary_objective))
+        print(self.save_task_output(self.agent_name, output))
 
     def stop_tasks(self):
         if self.stop_running_event is not None:
-            self.stop_running_event.set()
+            self.stop_running_event = True
         self.task_list.clear()
 
+    def task_agent(self, result: Dict, task_description: str, task_list) -> List[Dict]:
+        tasks = [task["task_name"] for task in task_list]
+        if len(tasks) == 0:
+            return []
+        task_list = ", ".join(tasks)
+
+        response = AGiXT(self.agent_name).run(
+            task=self.primary_objective,
+            prompt="task",
+            result=result,
+            task_description=task_description,
+            tasks=task_list,
+        )
+
+        lines = response.split("\n") if "\n" in response else [response]
+        new_tasks = []
+        for line in lines:
+            match = re.match(r"(\d+)\.\s+(.*)", line)
+            if match:
+                task_id, task_name = match.groups()
+                new_tasks.append(
+                    {"task_id": int(task_id), "task_name": task_name.strip()}
+                )
+
+        return new_tasks  # This line will return the list of new tasks
+
+    def instruction_agent(self, task, learn_file: str = "", **kwargs):
+        if "task_name" in task:
+            task = task["task_name"]
+        resolver = self.run(
+            task=task,
+            prompt="SmartInstruct-StepByStep",
+            context_results=6,
+            learn_file=learn_file,
+            **kwargs,
+        )
+        execution_response = self.run(
+            task=task,
+            prompt="SmartInstruct-Execution",
+            previous_response=resolver,
+            **kwargs,
+        )
+        return (
+            f"RESPONSE:\n{resolver}\n\nCommand Execution Response{execution_response}"
+        )
+
     def run_task(
         self,
         objective,
         async_exec: bool = False,
         learn_file: str = "",
         smart: bool = False,
         load_task: str = "",
@@ -134,31 +181,29 @@
                             "task_id": 1,
                             "task_name": "Develop a task list to complete the objective if necessary.  The plan is 'None' if not necessary.",
                         }
                     ]
                 )
             self.primary_objective = objective
             if learn_file != "":
-                learned_file = self.agent.memories.read_file(
-                    task=objective, file_path=learn_file
-                )
+                learned_file = self.agent.memories.read_file(file_path=learn_file)
                 if learned_file:
                     self.update_output_list(
                         f"Read file {learn_file} into memory for task {objective}.\n\n"
                     )
                 else:
                     self.update_output_list(
                         f"Failed to read file {learn_file} into memory.\n\n"
                     )
 
             self.update_output_list(
                 f"Starting task with objective: {self.primary_objective}.\n\n"
             )
 
-        while not self.stop_running_event.is_set() and self.task_list:
+        while not self.stop_running_event and self.task_list:
             task = self.task_list.popleft()
 
             if task["task_name"] in ["None", "None.", ""]:
                 self.stop_tasks()
                 continue
 
             self.update_output_list(
@@ -169,31 +214,31 @@
                 result = AGiXT(self.agent_name).smart_instruct(
                     task=task["task_name"],
                     shots=3,
                     async_exec=async_exec,
                     **kwargs,
                 )
             else:
-                result = AGiXT(self.agent_name).instruction_agent(
-                    task=task["task_name"], **kwargs
-                )
+                result = self.instruction_agent(task=task["task_name"], **kwargs)
 
             self.update_output_list(f"\nTask Result:\n\n{result}\n")
 
-            task_agent = AGiXT(self.agent_name).task_agent(
+            new_tasks = self.task_agent(
                 result=result,
                 task_description=task["task_name"],
                 task_list=self.task_list,
             )
-            new_tasks = deque(task_agent)
+
+            self.task_list = deque(new_tasks)
+
             self.update_output_list(f"\nNew Tasks:\n\n{new_tasks}\n")
 
             for new_task in new_tasks:
                 new_task_id = len(self.task_list) + 1
                 new_task.update({"task_id": new_task_id})
                 self.task_list.append(new_task)
 
         if not self.task_list:
             self.stop_tasks()
-        if self.stop_running_event.is_set():
+        if self.stop_running_event:
             self.save_task()
         self.update_output_list("All tasks completed or stopped.")
```

### Comparing `agixt-1.1.60b0/agixt/app.py` & `agixt-1.1.61b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/__init__.py` & `agixt-1.1.61b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/azure.py` & `agixt-1.1.61b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/bing.py` & `agixt-1.1.61b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/chatgpt.py` & `agixt-1.1.61b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/claude.py` & `agixt-1.1.61b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/fastchat.py` & `agixt-1.1.61b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/gpt4all.py` & `agixt-1.1.61b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/gpt4free.py` & `agixt-1.1.61b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.61b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/huggingchat.py` & `agixt-1.1.61b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/kobold.py` & `agixt-1.1.61b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/llamacpp.py` & `agixt-1.1.61b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/oobabooga.py` & `agixt-1.1.61b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/openai.py` & `agixt-1.1.61b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/palm.py` & `agixt-1.1.61b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/provider/transformer.py` & `agixt-1.1.61b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt/requirements.txt` & `agixt-1.1.61b0/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.61b0/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.60b0
+Version: 1.1.61b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.60b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.61b0/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/agixt.egg-info/requires.txt` & `agixt-1.1.61b0/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/docs/README.md` & `agixt-1.1.61b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.60b0/setup.py` & `agixt-1.1.61b0/setup.py`

 * *Files identical despite different names*

