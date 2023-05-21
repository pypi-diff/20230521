# Comparing `tmp/agixt-1.1.54b0.tar.gz` & `tmp/agixt-1.1.55b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.54b0.tar", last modified: Sun May 21 04:01:23 2023, max compression
+gzip compressed data, was "agixt-1.1.55b0.tar", last modified: Sun May 21 04:12:06 2023, max compression
```

## Comparing `agixt-1.1.54b0.tar` & `agixt-1.1.55b0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.788818 agixt-1.1.54b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 04:01:12.000000 agixt-1.1.54b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 04:01:12.000000 agixt-1.1.54b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-21 04:01:23.788818 agixt-1.1.54b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.784818 agixt-1.1.54b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.784818 agixt-1.1.54b0/agixt/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Config/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.788818 agixt-1.1.54b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.784818 agixt-1.1.54b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-21 04:01:23.000000 agixt-1.1.54b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-21 04:01:23.000000 agixt-1.1.54b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:01:23.000000 agixt-1.1.54b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-21 04:01:23.000000 agixt-1.1.54b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 04:01:23.000000 agixt-1.1.54b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.788818 agixt-1.1.54b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-21 04:01:12.000000 agixt-1.1.54b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 04:01:12.000000 agixt-1.1.54b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:01:23.788818 agixt-1.1.54b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 04:01:12.000000 agixt-1.1.54b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.575996 agixt-1.1.55b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 04:11:49.000000 agixt-1.1.55b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 04:11:49.000000 agixt-1.1.55b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-21 04:12:06.575996 agixt-1.1.55b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.571996 agixt-1.1.55b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.571996 agixt-1.1.55b0/agixt/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Config/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.575996 agixt-1.1.55b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 04:11:49.000000 agixt-1.1.55b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.571996 agixt-1.1.55b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-21 04:12:06.000000 agixt-1.1.55b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-21 04:12:06.000000 agixt-1.1.55b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:12:06.000000 agixt-1.1.55b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-21 04:12:06.000000 agixt-1.1.55b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 04:12:06.000000 agixt-1.1.55b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:12:06.575996 agixt-1.1.55b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-21 04:11:49.000000 agixt-1.1.55b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 04:11:49.000000 agixt-1.1.55b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:12:06.575996 agixt-1.1.55b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 04:11:49.000000 agixt-1.1.55b0/setup.py
```

### Comparing `agixt-1.1.54b0/LICENSE` & `agixt-1.1.55b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/PKG-INFO` & `agixt-1.1.55b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.54b0
+Version: 1.1.55b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.54b0/agixt/AGiXT.py` & `agixt-1.1.55b0/agixt/AGiXT.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/Chain.py` & `agixt-1.1.55b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/Commands.py` & `agixt-1.1.55b0/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/Config/Agent.py` & `agixt-1.1.55b0/agixt/Config/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/Config/__init__.py` & `agixt-1.1.55b0/agixt/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/CustomPrompt.py` & `agixt-1.1.55b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/Embedding.py` & `agixt-1.1.55b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/Memories.py` & `agixt-1.1.55b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/Tasks.py` & `agixt-1.1.55b0/agixt/Tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,18 +75,20 @@
                 result = self.smart_instruct(
                     task=task["task_name"],
                     shots=3,
                     async_exec=async_exec,
                     **kwargs,
                 )
             else:
-                result = self.instruction_agent(task=task["task_name"], **kwargs)
+                result = AGiXT(self.agent_name).instruction_agent(
+                    task=task["task_name"], **kwargs
+                )
             self.update_output_list(f"\nTask Result:\n\n{result}\n")
             task_list = [t["task_name"] for t in self.task_list]
-            new_tasks = self.task_agent(
+            new_tasks = AGiXT(self.agent_name).task_agent(
                 result=result, task_description=task["task_name"], task_list=task_list
             )
             self.update_output_list(f"\nNew Tasks:\n\n{new_tasks}\n")
             for new_task in new_tasks:
                 new_task.update({"task_id": len(self.task_list) + 1})
                 self.task_list.append(new_task)
             task_names = [t["task_name"] for t in self.task_list]
```

### Comparing `agixt-1.1.54b0/agixt/app.py` & `agixt-1.1.55b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/__init__.py` & `agixt-1.1.55b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/azure.py` & `agixt-1.1.55b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/bing.py` & `agixt-1.1.55b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/claude.py` & `agixt-1.1.55b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/fastchat.py` & `agixt-1.1.55b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/gpt4all.py` & `agixt-1.1.55b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/gpt4free.py` & `agixt-1.1.55b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.55b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/huggingchat.py` & `agixt-1.1.55b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/kobold.py` & `agixt-1.1.55b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/llamacpp.py` & `agixt-1.1.55b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/oobabooga.py` & `agixt-1.1.55b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/openai.py` & `agixt-1.1.55b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/palm.py` & `agixt-1.1.55b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/provider/transformer.py` & `agixt-1.1.55b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt/requirements.txt` & `agixt-1.1.55b0/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.55b0/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.54b0
+Version: 1.1.55b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.54b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.55b0/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/agixt.egg-info/requires.txt` & `agixt-1.1.55b0/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/docs/README.md` & `agixt-1.1.55b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.54b0/setup.py` & `agixt-1.1.55b0/setup.py`

 * *Files identical despite different names*

