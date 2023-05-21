# Comparing `tmp/python-llm-0.1.7.tar.gz` & `tmp/python-llm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-llm-0.1.7.tar", last modified: Sun May 21 11:55:51 2023, max compression
+gzip compressed data, was "python-llm-0.1.8.tar", last modified: Sun May 21 12:22:25 2023, max compression
```

## Comparing `python-llm-0.1.7.tar` & `python-llm-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.165750 python-llm-0.1.7/
--rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.7/LICENSE
--rw-r--r--   0 danielgross   (501) staff       (20)       24 2023-05-21 11:54:44.000000 python-llm-0.1.7/MANIFEST.in
--rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-21 11:55:51.165633 python-llm-0.1.7/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)     2342 2023-05-20 19:12:04.000000 python-llm-0.1.7/README.md
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.163796 python-llm-0.1.7/llm/
--rw-r--r--   0 danielgross   (501) staff       (20)       81 2023-05-20 15:11:39.000000 python-llm-0.1.7/llm/__init__.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.164121 python-llm-0.1.7/llm/api/
--rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.7/llm/api/__init__.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2387 2023-05-20 16:23:02.000000 python-llm-0.1.7/llm/api/anthropicapi.py
--rw-r--r--   0 danielgross   (501) staff       (20)     1651 2023-05-20 16:32:24.000000 python-llm-0.1.7/llm/api/openaiapi.py
--rw-r--r--   0 danielgross   (501) staff       (20)     4401 2023-05-20 19:51:36.000000 python-llm-0.1.7/llm/main.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.164428 python-llm-0.1.7/llm/utils/
--rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-05-20 11:50:33.000000 python-llm-0.1.7/llm/utils/__init__.py
--rw-r--r--   0 danielgross   (501) staff       (20)     3200 2023-05-20 11:56:01.000000 python-llm-0.1.7/llm/utils/apikeys.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2441 2023-05-20 19:38:17.000000 python-llm-0.1.7/llm/utils/parsing.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.165020 python-llm-0.1.7/python_llm.egg-info/
--rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-21 11:55:51.000000 python-llm-0.1.7/python_llm.egg-info/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)      453 2023-05-21 11:55:51.000000 python-llm-0.1.7/python_llm.egg-info/SOURCES.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-21 11:55:51.000000 python-llm-0.1.7/python_llm.egg-info/dependency_links.txt
--rw-r--r--   0 danielgross   (501) staff       (20)      167 2023-05-21 11:55:51.000000 python-llm-0.1.7/python_llm.egg-info/requires.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-21 11:55:51.000000 python-llm-0.1.7/python_llm.egg-info/top_level.txt
--rw-r--r--   0 danielgross   (501) staff       (20)      166 2023-05-20 11:50:33.000000 python-llm-0.1.7/requirements.txt
--rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-21 11:55:51.165787 python-llm-0.1.7/setup.cfg
--rw-r--r--   0 danielgross   (501) staff       (20)      650 2023-05-21 11:54:56.000000 python-llm-0.1.7/setup.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.165436 python-llm-0.1.7/tests/
--rw-r--r--   0 danielgross   (501) staff       (20)     3407 2023-05-20 19:49:17.000000 python-llm-0.1.7/tests/test_anthropic.py
--rw-r--r--   0 danielgross   (501) staff       (20)      945 2023-05-20 19:51:00.000000 python-llm-0.1.7/tests/test_multi_stream.py
--rw-r--r--   0 danielgross   (501) staff       (20)     3651 2023-05-20 19:32:25.000000 python-llm-0.1.7/tests/test_openai.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 12:22:25.272877 python-llm-0.1.8/
+-rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.8/LICENSE
+-rw-r--r--   0 danielgross   (501) staff       (20)       24 2023-05-21 11:54:44.000000 python-llm-0.1.8/MANIFEST.in
+-rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-21 12:22:25.272750 python-llm-0.1.8/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)     2342 2023-05-20 19:12:04.000000 python-llm-0.1.8/README.md
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 12:22:25.271168 python-llm-0.1.8/llm/
+-rw-r--r--   0 danielgross   (501) staff       (20)       81 2023-05-20 15:11:39.000000 python-llm-0.1.8/llm/__init__.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 12:22:25.271467 python-llm-0.1.8/llm/api/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.8/llm/api/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2387 2023-05-20 16:23:02.000000 python-llm-0.1.8/llm/api/anthropicapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     1651 2023-05-20 16:32:24.000000 python-llm-0.1.8/llm/api/openaiapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     4713 2023-05-21 12:10:19.000000 python-llm-0.1.8/llm/main.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 12:22:25.271747 python-llm-0.1.8/llm/utils/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-05-20 11:50:33.000000 python-llm-0.1.8/llm/utils/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     3200 2023-05-20 11:56:01.000000 python-llm-0.1.8/llm/utils/apikeys.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2441 2023-05-20 19:38:17.000000 python-llm-0.1.8/llm/utils/parsing.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 12:22:25.272281 python-llm-0.1.8/python_llm.egg-info/
+-rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-21 12:22:25.000000 python-llm-0.1.8/python_llm.egg-info/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)      453 2023-05-21 12:22:25.000000 python-llm-0.1.8/python_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-21 12:22:25.000000 python-llm-0.1.8/python_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)      167 2023-05-21 12:22:25.000000 python-llm-0.1.8/python_llm.egg-info/requires.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-21 12:22:25.000000 python-llm-0.1.8/python_llm.egg-info/top_level.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)      166 2023-05-20 11:50:33.000000 python-llm-0.1.8/requirements.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-21 12:22:25.272927 python-llm-0.1.8/setup.cfg
+-rw-r--r--   0 danielgross   (501) staff       (20)      650 2023-05-21 12:22:22.000000 python-llm-0.1.8/setup.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 12:22:25.272607 python-llm-0.1.8/tests/
+-rw-r--r--   0 danielgross   (501) staff       (20)     3407 2023-05-20 19:49:17.000000 python-llm-0.1.8/tests/test_anthropic.py
+-rw-r--r--   0 danielgross   (501) staff       (20)      945 2023-05-20 19:51:00.000000 python-llm-0.1.8/tests/test_multi_stream.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     3651 2023-05-20 19:32:25.000000 python-llm-0.1.8/tests/test_openai.py
```

### Comparing `python-llm-0.1.7/LICENSE` & `python-llm-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.7/PKG-INFO` & `python-llm-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-llm
-Version: 0.1.7
+Version: 0.1.8
 Summary: An LLM wrapper for Humans
 Home-page: https://github.com/danielgross/python-llm
 Author: Daniel Gross
 Author-email: d@dcgross.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-llm-0.1.7/README.md` & `python-llm-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.7/llm/api/anthropicapi.py` & `python-llm-0.1.8/llm/api/anthropicapi.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.7/llm/api/openaiapi.py` & `python-llm-0.1.8/llm/api/openaiapi.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.7/llm/main.py` & `python-llm-0.1.8/llm/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,28 +19,32 @@
 
 def complete(prompt, engine="openai:text-davinci-003", **kwargs):
     args = parse_args(engine, **kwargs)
     if args.service == "openai":
         result = openaiapi.complete(prompt, args.engine, **args.kwargs)
     elif args.service == "anthropic":
         result = anthropicapi.complete(prompt, args.engine, **args.kwargs)
+    elif args.service == "test":
+        result = testapi.complete(prompt, args.engine, **args.kwargs)
     else:
         raise ValueError(f"Engine {engine} is not supported.")
     return result.strip()
 
 
 # Can also pass in system="Behave like a bunny rabbit" for system message.
 def chat(messages, engine="openai:gpt-3.5-turbo", **kwargs):
     """Chat with the LLM API."""
     args = parse_args(engine, **kwargs)
     messages = structure_chat(messages)
     if args.service == "openai":
         result = openaiapi.chat(messages, args.engine, **args.kwargs)
     elif args.service == "anthropic":
         result = anthropicapi.chat(messages, args.engine, **args.kwargs)
+    elif args.service == "test":
+        result = testapi.chat(messages, args.engine, **args.kwargs)
     else:
         raise ValueError(f"Engine {engine} is not supported.")
     return result.strip()
 
 
 async def stream_chat(messages, engine="openai:gpt-3.5-turbo", stream_method="default", **kwargs):
     """Chat with the LLM API.
@@ -50,14 +54,16 @@
     """
     args = parse_args(engine, **kwargs)
     messages = structure_chat(messages)
     if args.service == "openai":
         result = openaiapi.stream_chat(messages, args.engine, **args.kwargs)
     elif args.service == "anthropic":
         result = anthropicapi.stream_chat(messages, args.engine, **args.kwargs)
+    elif args.service == "test":
+        result = testapi.stream_chat(messages, args.engine, **args.kwargs)
     else:
         raise ValueError(f"Engine {engine} is not supported.")
 
     output_cache = []
     initial_response_done = False
     async for raw_token in result:
         token, output_cache = format_streaming_output(
```

### Comparing `python-llm-0.1.7/llm/utils/apikeys.py` & `python-llm-0.1.8/llm/utils/apikeys.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.7/llm/utils/parsing.py` & `python-llm-0.1.8/llm/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.7/python_llm.egg-info/PKG-INFO` & `python-llm-0.1.8/python_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-llm
-Version: 0.1.7
+Version: 0.1.8
 Summary: An LLM wrapper for Humans
 Home-page: https://github.com/danielgross/python-llm
 Author: Daniel Gross
 Author-email: d@dcgross.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-llm-0.1.7/setup.py` & `python-llm-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='python-llm',
-    version='0.1.7',
+    version='0.1.8',
     author='Daniel Gross',
     author_email='d@dcgross.com',
     description='An LLM wrapper for Humans',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(include=['llm', 'llm.*']),
     url="https://github.com/danielgross/python-llm",
```

### Comparing `python-llm-0.1.7/tests/test_anthropic.py` & `python-llm-0.1.8/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.7/tests/test_multi_stream.py` & `python-llm-0.1.8/tests/test_multi_stream.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.7/tests/test_openai.py` & `python-llm-0.1.8/tests/test_openai.py`

 * *Files identical despite different names*

