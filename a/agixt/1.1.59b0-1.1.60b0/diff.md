# Comparing `tmp/agixt-1.1.59b0.tar.gz` & `tmp/agixt-1.1.60b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.59b0.tar", last modified: Sun May 21 18:14:20 2023, max compression
+gzip compressed data, was "agixt-1.1.60b0.tar", last modified: Sun May 21 19:55:44 2023, max compression
```

## Comparing `agixt-1.1.59b0.tar` & `agixt-1.1.60b0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:14:20.014007 agixt-1.1.59b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 18:14:08.000000 agixt-1.1.59b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 18:14:08.000000 agixt-1.1.59b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 18:14:20.014007 agixt-1.1.59b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:14:20.010007 agixt-1.1.59b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/Commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:14:20.014007 agixt-1.1.59b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 18:14:08.000000 agixt-1.1.59b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:14:20.010007 agixt-1.1.59b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 18:14:20.000000 agixt-1.1.59b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-21 18:14:20.000000 agixt-1.1.59b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:14:20.000000 agixt-1.1.59b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-21 18:14:20.000000 agixt-1.1.59b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 18:14:20.000000 agixt-1.1.59b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:14:20.014007 agixt-1.1.59b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-21 18:14:08.000000 agixt-1.1.59b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 18:14:08.000000 agixt-1.1.59b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:14:20.014007 agixt-1.1.59b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 18:14:08.000000 agixt-1.1.59b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:55:44.442127 agixt-1.1.60b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 19:55:28.000000 agixt-1.1.60b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 19:55:28.000000 agixt-1.1.60b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 19:55:44.442127 agixt-1.1.60b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:55:44.438127 agixt-1.1.60b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:55:44.442127 agixt-1.1.60b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 19:55:28.000000 agixt-1.1.60b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:55:44.438127 agixt-1.1.60b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-05-21 19:55:44.000000 agixt-1.1.60b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-21 19:55:44.000000 agixt-1.1.60b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:55:44.000000 agixt-1.1.60b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-21 19:55:44.000000 agixt-1.1.60b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 19:55:44.000000 agixt-1.1.60b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:55:44.442127 agixt-1.1.60b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-21 19:55:28.000000 agixt-1.1.60b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 19:55:28.000000 agixt-1.1.60b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:55:44.442127 agixt-1.1.60b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 19:55:28.000000 agixt-1.1.60b0/setup.py
```

### Comparing `agixt-1.1.59b0/LICENSE` & `agixt-1.1.60b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/PKG-INFO` & `agixt-1.1.60b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.59b0
+Version: 1.1.60b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.59b0/agixt/AGiXT.py` & `agixt-1.1.60b0/agixt/AGiXT.py`

 * *Files 4% similar despite different names*

```diff
@@ -369,47 +369,48 @@
                             command_args=command_args,
                             command_output=command_output,
                             **kwargs,
                         )
                         return self.execution_agent(
                             execution_response, task, context_results, **kwargs
                         )
-                        return self.revalidation_agent(
-                            task, command_name, command_args, command_output, **kwargs
-                        )
                 else:
                     if command_name == "None.":
                         return "\nNo commands were executed.\n"
                     else:
                         return f"\Command not recognized: {command_name} ."
         except:
             print("\nERROR IN EXECUTION_AGENT, validated_response:\n")
             print(validated_response)
             return "\nNo commands were executed.\n"
 
-    def task_agent(
-        self, result: Dict, task_description: str, task_list: List[str]
-    ) -> List[Dict]:
+    def task_agent(self, result: Dict, task_description: str, task_list) -> List[Dict]:
+        tasks = [task["task_name"] for task in task_list]
+        if len(tasks) == 0:
+            return []
+        task_list = ", ".join(tasks)
+
         response = self.run(
             task=self.primary_objective,
             prompt="task",
             result=result,
             task_description=task_description,
-            tasks=", ".join(task_list),
+            tasks=task_list,
         )
 
         lines = response.split("\n") if "\n" in response else [response]
-        new_tasks = [
-            re.sub(r"^.*?(\d)", r"\1", line)
-            for line in lines
-            if line.strip() and re.search(r"\d", line[:10])
-        ] or [response]
-        return [
-            {"task_name": task_name} for task_name in new_tasks if task_name.strip()
-        ]
+        new_tasks = []
+        for line in lines:
+            match = re.match(r"(\d+)\.\s+(.*)", line)
+            if match:
+                task_id, task_name = match.groups()
+                new_tasks.append(
+                    {"task_id": int(task_id), "task_name": task_name.strip()}
+                )
+        return new_tasks
 
     async def websearch_agent(
         self, task: str = "What are the latest breakthroughs in AI?", depth: int = 3
     ):
         async def resursive_browsing(task, links):
             try:
                 words = links.split()
```

### Comparing `agixt-1.1.59b0/agixt/Agent.py` & `agixt-1.1.60b0/agixt/Agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -314,49 +314,7 @@
             yaml.safe_dump(self.memory, file)
 
     def log_interaction(self, role: str, message: str):
         if self.memory is None:
             self.memory = {"interactions": []}
         self.memory["interactions"].append({"role": role, "message": message})
         self.save_memory()
-
-    def get_task_output(self, agent_name, primary_objective=None):
-        if primary_objective is None:
-            return "No primary objective specified."
-
-        # Clean up primary_objective and truncate at 15 characters
-        clean_objective = re.sub(
-            r"\W+", " ", primary_objective
-        )  # Remove non-alphanumeric characters
-        clean_objective = clean_objective.replace(
-            " ", "_"
-        )  # Replace spaces with underscores
-        clean_objective = clean_objective[:15]  # Truncate to 15 characters
-
-        task_output_file = os.path.join(
-            "agents", agent_name, "tasks", f"{clean_objective}.txt"
-        )
-        if os.path.exists(task_output_file):
-            with open(task_output_file, "r") as f:
-                task_output = f.read()
-        else:
-            task_output = ""
-        return task_output
-
-    def save_task_output(self, agent_name, task_output, primary_objective=None):
-        # Check if agents/{agent_name}/tasks/task_name.txt exists
-        # If it does, append to it
-        # If it doesn't, create it
-        if "tasks" not in os.listdir(os.path.join("agents", agent_name)):
-            os.makedirs(os.path.join("agents", agent_name, "tasks"))
-        if primary_objective is None:
-            primary_objective = str(uuid.uuid4())
-        task_output_file = os.path.join(
-            "agents", agent_name, "tasks", f"{primary_objective}.txt"
-        )
-        with open(
-            task_output_file,
-            "a" if os.path.exists(task_output_file) else "w",
-            encoding="utf-8",
-        ) as f:
-            f.write(task_output)
-        return task_output
```

### Comparing `agixt-1.1.59b0/agixt/Chain.py` & `agixt-1.1.60b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/Commands.py` & `agixt-1.1.60b0/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/Config.py` & `agixt-1.1.60b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/CustomPrompt.py` & `agixt-1.1.60b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/Embedding.py` & `agixt-1.1.60b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/Memories.py` & `agixt-1.1.60b0/agixt/Memories.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
     def initialize_chroma_client(self):
         try:
             return chromadb.Client(
                 settings=chromadb.config.Settings(
                     chroma_db_impl="duckdb+parquet",
                     persist_directory=self.chroma_persist_dir,
+                    anonymized_telemetry=False,
                 )
             )
         except Exception as e:
             raise RuntimeError(f"Unable to initialize chroma client: {e}")
 
     def get_or_create_collection(self):
         try:
```

### Comparing `agixt-1.1.59b0/agixt/Tasks.py` & `agixt-1.1.60b0/agixt/Tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from AGiXT import AGiXT
 import re
+import os
 import json
+import uuid
+import yaml
 from pathlib import Path
 from Agent import Agent
 from collections import deque
 
 
 class Tasks:
     def __init__(self, agent_name: str = "AGiXT"):
@@ -28,16 +31,16 @@
         # serialize the task state and save to a file
         task_state = {
             "task_name": task_name,
             "task_list": list(self.task_list),
             "output_list": self.output_list,
             "primary_objective": self.primary_objective,
         }
-        with open(f"agents/{self.agent_name}/{task_name}.json", "w") as f:
-            json.dump(task_state, f)
+        with open(f"agents/{self.agent_name}/{task_name}.yaml", "w") as f:
+            yaml.dump(task_state, f)
 
     def load_task(self, task_name):
         task_name = re.sub(
             r"[^\w\s]", "", task_name
         )  # remove non-alphanumeric & non-space characters
         task_name = task_name[:15]  # truncate to 15 characters
 
@@ -60,35 +63,70 @@
             return not self.stop_running_event.is_set()
         except:
             return False
 
     def get_output_list(self):
         return self.output_list
 
-    def update_output_list(self, output):
-        print(
-            self.agent.save_task_output(self.agent_name, output, self.primary_objective)
+    def save_task_output(self, agent_name, task_output):
+        # Check if agents/{agent_name}/tasks/task_name.txt exists
+        # If it does, append to it
+        # If it doesn't, create it
+        if "tasks" not in os.listdir(os.path.join("agents", agent_name)):
+            os.makedirs(os.path.join("agents", agent_name, "tasks"))
+        if self.primary_objective is None:
+            self.primary_objective = str(uuid.uuid4())
+        task_output_file = os.path.join(
+            "agents", agent_name, "tasks", f"{self.primary_objective}.yaml"
         )
+        with open(
+            task_output_file,
+            "a" if os.path.exists(task_output_file) else "w",
+            encoding="utf-8",
+        ) as f:
+            yaml.dump(task_output, f)
+        return task_output
+
+    def get_task_output(self):
+        task_name = re.sub(
+            r"[^\w\s]", "", self.primary_objective
+        )  # remove non-alphanumeric & non-space characters
+        task_name = task_name[:15]  # truncate to 15 characters
+
+        try:
+            with open(f"agents/{self.agent_name}/tasks/{task_name}.yaml", "r") as f:
+                task_output = yaml.safe_load(f)
+
+            print(f"Successfully loaded task output for '{task_name}'.")
+            return task_output
+
+        except FileNotFoundError:
+            print(f"No saved task output found with the name '{task_name}'.")
+            return None
+        except Exception as e:
+            print(f"An error occurred while loading the task output: {e}")
+            return None
+
+    def update_output_list(self, output):
+        print(self.save_task_output(self.agent_name, output, self.primary_objective))
 
     def stop_tasks(self):
         if self.stop_running_event is not None:
             self.stop_running_event.set()
         self.task_list.clear()
 
     def run_task(
         self,
-        stop_event,
         objective,
         async_exec: bool = False,
         learn_file: str = "",
         smart: bool = False,
         load_task: str = "",
         **kwargs,
     ):
-        self.stop_running_event = stop_event
         if load_task != "":
             self.load_task(load_task)
             self.update_output_list(f"Loaded task '{load_task}'.\n\n")
         else:
             if self.task_list == deque([]) or self.task_list == []:
                 self.task_list = deque(
                     [
@@ -137,19 +175,20 @@
             else:
                 result = AGiXT(self.agent_name).instruction_agent(
                     task=task["task_name"], **kwargs
                 )
 
             self.update_output_list(f"\nTask Result:\n\n{result}\n")
 
-            new_tasks = AGiXT(self.agent_name).task_agent(
+            task_agent = AGiXT(self.agent_name).task_agent(
                 result=result,
                 task_description=task["task_name"],
-                task_list=list(self.task_list),
+                task_list=self.task_list,
             )
+            new_tasks = deque(task_agent)
             self.update_output_list(f"\nNew Tasks:\n\n{new_tasks}\n")
 
             for new_task in new_tasks:
                 new_task_id = len(self.task_list) + 1
                 new_task.update({"task_id": new_task_id})
                 self.task_list.append(new_task)
```

### Comparing `agixt-1.1.59b0/agixt/app.py` & `agixt-1.1.60b0/agixt/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from fastapi.middleware.cors import CORSMiddleware
 from pydantic import BaseModel
 from Config import Config
 from AGiXT import AGiXT
 from Agent import Agent
 from Commands import Commands
 from Chain import Chain
+from Tasks import Tasks
 from CustomPrompt import CustomPrompt
-import threading
 from typing import Optional, Dict, List, Any
 from provider import get_provider_options
 from Embedding import get_embedding_providers
 import os
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "version"), encoding="utf-8") as f:
@@ -251,58 +251,42 @@
             detail=f"Error enabling all commands for agent '{agent_name}': {str(e)}",
         )
 
 
 @app.post("/api/agent/{agent_name}/task", tags=["Agent"])
 async def start_task_agent(agent_name: str, objective: Objective) -> ResponseMessage:
     # If it's running stop it.
-    CFG = Agent(agent_name)
-    if (
-        agent_name in CFG.agent_instances
-        and CFG.agent_instances[agent_name].get_status()
-    ):
-        agent_stop_events[agent_name].set()
-        del agent_threads[agent_name]
-        del agent_stop_events[agent_name]
+    task_status = Tasks(agent_name).get_status()
+    if task_status != False:
+        Tasks(agent_name).stop_tasks()
         return ResponseMessage(message="Task agent stopped")
-    # Otherwise start it.
-    # If it doesn't exist, create it.
-    if agent_name not in CFG.agent_instances:
-        CFG.agent_instances[agent_name] = AGiXT(agent_name)
-    stop_event = threading.Event()
-    agent_stop_events[agent_name] = stop_event
-    agent_thread = threading.Thread(
-        target=CFG.agent_instances[agent_name].run_task,
-        args=(stop_event, objective.objective),
-    )
-    agent_threads[agent_name] = agent_thread
-    agent_thread.start()
+    # If it's not running start it.
+    Tasks(agent_name).run_task(objective=objective.objective)
     return ResponseMessage(message="Task agent started")
 
 
 @app.get("/api/agent/{agent_name}/task", tags=["Agent"])
 async def get_task_output(agent_name: str) -> TaskOutput:
-    CFG = Agent(agent_name)
-    if agent_name not in CFG.agent_instances:
-        return TaskOutput(output="", message="")
-    return TaskOutput(
-        output=CFG.get_task_output(
-            agent_name, CFG.agent_instances[agent_name].primary_objective
-        ),
-        message="Task agent is still running",
-    )
+    task_output = Tasks(agent_name).get_task_output()
+    if task_output != False:
+        return TaskOutput(
+            output=task_output,
+            message="Task agent is not running",
+        )
+    else:
+        return TaskOutput(
+            output="",
+            message="Task agent is not running",
+        )
 
 
 @app.get("/api/agent/{agent_name}/task/status", tags=["Agent"])
 async def get_task_status(agent_name: str):
-    CFG = Agent(agent_name)
-    if agent_name not in CFG.agent_instances:
-        return {"status": False}
-    status = CFG.agent_instances[agent_name].get_status()
-    return {"status": status}
+    task_status = Tasks(agent_name).get_status()
+    return {"status": task_status}
 
 
 @app.get("/api/chain", tags=["Chain"])
 async def get_chains():
     chains = Chain().get_chains()
     return chains
 
@@ -337,15 +321,15 @@
 async def delete_chain(chain_name: str) -> ResponseMessage:
     Chain().delete_chain(chain_name)
     return ResponseMessage(message=f"Chain '{chain_name}' deleted.")
 
 
 @app.post("/api/chain/{chain_name}/step", tags=["Chain"])
 async def add_step(chain_name: str, step_info: StepInfo) -> ResponseMessage:
-    Chain().add_step(
+    Chain().add_chain_step(
         chain_name,
         step_info.step_number,
         step_info.prompt_type,
         step_info.prompt,
         step_info.agent_name,
     )
     return {"message": f"Step {step_info.step_number} added to chain '{chain_name}'."}
```

### Comparing `agixt-1.1.59b0/agixt/provider/__init__.py` & `agixt-1.1.60b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/azure.py` & `agixt-1.1.60b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/bing.py` & `agixt-1.1.60b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/chatgpt.py` & `agixt-1.1.60b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/claude.py` & `agixt-1.1.60b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/fastchat.py` & `agixt-1.1.60b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/gpt4all.py` & `agixt-1.1.60b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/gpt4free.py` & `agixt-1.1.60b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.60b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/huggingchat.py` & `agixt-1.1.60b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/kobold.py` & `agixt-1.1.60b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/llamacpp.py` & `agixt-1.1.60b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/oobabooga.py` & `agixt-1.1.60b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/openai.py` & `agixt-1.1.60b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/palm.py` & `agixt-1.1.60b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/provider/transformer.py` & `agixt-1.1.60b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt/requirements.txt` & `agixt-1.1.60b0/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.60b0/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.59b0
+Version: 1.1.60b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.59b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.60b0/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/agixt.egg-info/requires.txt` & `agixt-1.1.60b0/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/docs/README.md` & `agixt-1.1.60b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.59b0/setup.py` & `agixt-1.1.60b0/setup.py`

 * *Files identical despite different names*

