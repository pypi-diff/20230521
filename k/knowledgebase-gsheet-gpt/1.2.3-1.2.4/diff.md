# Comparing `tmp/knowledgebase-gsheet-gpt-1.2.3.tar.gz` & `tmp/knowledgebase-gsheet-gpt-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgebase-gsheet-gpt-1.2.3.tar", last modified: Sun May 21 16:45:31 2023, max compression
+gzip compressed data, was "knowledgebase-gsheet-gpt-1.2.4.tar", last modified: Sun May 21 17:04:15 2023, max compression
```

## Comparing `knowledgebase-gsheet-gpt-1.2.3.tar` & `knowledgebase-gsheet-gpt-1.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 16:45:31.603348 knowledgebase-gsheet-gpt-1.2.3/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-21 16:45:31.603237 knowledgebase-gsheet-gpt-1.2.3/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 16:45:31.603060 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       98 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     5515 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 16:45:31.603385 knowledgebase-gsheet-gpt-1.2.3/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 17:04:15.587326 knowledgebase-gsheet-gpt-1.2.4/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-21 17:04:15.587181 knowledgebase-gsheet-gpt-1.2.4/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-21 17:04:15.000000 knowledgebase-gsheet-gpt-1.2.4/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 17:04:15.586897 knowledgebase-gsheet-gpt-1.2.4/knowledgebase_gsheet_gpt.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-21 17:04:15.000000 knowledgebase-gsheet-gpt-1.2.4/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-21 17:04:15.000000 knowledgebase-gsheet-gpt-1.2.4/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 17:04:15.000000 knowledgebase-gsheet-gpt-1.2.4/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-21 17:04:15.000000 knowledgebase-gsheet-gpt-1.2.4/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       98 2023-05-21 17:04:15.000000 knowledgebase-gsheet-gpt-1.2.4/knowledgebase_gsheet_gpt.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-21 17:04:15.000000 knowledgebase-gsheet-gpt-1.2.4/knowledgebase_gsheet_gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     5625 2023-05-21 17:04:15.000000 knowledgebase-gsheet-gpt-1.2.4/knowledgebase_gsheet_gpt.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 17:04:15.587368 knowledgebase-gsheet-gpt-1.2.4/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-21 17:04:15.000000 knowledgebase-gsheet-gpt-1.2.4/setup.py
```

### Comparing `knowledgebase-gsheet-gpt-1.2.3/PKG-INFO` & `knowledgebase-gsheet-gpt-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.2.3
+Version: 1.2.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.2.3/README.md` & `knowledgebase-gsheet-gpt-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/PKG-INFO` & `knowledgebase-gsheet-gpt-1.2.4/knowledgebase_gsheet_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.2.3
+Version: 1.2.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.py` & `knowledgebase-gsheet-gpt-1.2.4/knowledgebase_gsheet_gpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,17 +107,20 @@
         knowledge_prompt += f"{ranked_result['ranking'][i]['content']}"
         knowledge_prompt += '\n\n'
 
     knowledge_prompt += before_question_prompt
     knowledge_prompt += f"{prompt}\n"
 
     # print('knowledgebase_gsheet_gpt.py, knowledge_prompt:\n', knowledge_prompt)
-    chat_memory.append_context(user, knowledge_prompt)
+    # chat_memory.append_context(user, knowledge_prompt)
+
     print("knowledgebase_gsheet_gpt.py chat_memory.get_context(user):\n", chat_memory.get_context(user))
-    response_queue = openai_chat_thread.openai_chat_thread_taiwan(prompt=chat_memory.get_context(user), model=model)
+    # response_queue = openai_chat_thread.openai_chat_thread_taiwan(prompt=chat_memory.get_context(user), model=model)
+
+    response_queue = openai_chat_thread.openai_chat_thread_taiwan(prompt=knowledge_prompt, model=model)
     return response_queue
 
 
 def main():
     arg = parse_arguments()
     response_stream = knowledgebase_gsheet_gpt(arg.user,
                                                arg.prompt,
```

### Comparing `knowledgebase-gsheet-gpt-1.2.3/setup.py` & `knowledgebase-gsheet-gpt-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="knowledgebase-gsheet-gpt",
-    version="1.2.3",
+    version="1.2.4",
     packages=find_packages(),
     py_modules=['knowledgebase_gsheet_gpt'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'knowledgebase_gsheet_gpt = knowledgebase_gsheet_gpt:main',
         ],
```

