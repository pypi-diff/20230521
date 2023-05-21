# Comparing `tmp/python-llm-0.1.6.tar.gz` & `tmp/python-llm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-llm-0.1.6.tar", last modified: Sat May 20 20:04:05 2023, max compression
+gzip compressed data, was "python-llm-0.1.7.tar", last modified: Sun May 21 11:55:51 2023, max compression
```

## Comparing `python-llm-0.1.6.tar` & `python-llm-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 20:04:05.084755 python-llm-0.1.6/
--rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.6/LICENSE
--rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-20 20:04:05.084598 python-llm-0.1.6/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)     2342 2023-05-20 19:12:04.000000 python-llm-0.1.6/README.md
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 20:04:05.082815 python-llm-0.1.6/llm/
--rw-r--r--   0 danielgross   (501) staff       (20)       81 2023-05-20 15:11:39.000000 python-llm-0.1.6/llm/__init__.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 20:04:05.083111 python-llm-0.1.6/llm/api/
--rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.6/llm/api/__init__.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2387 2023-05-20 16:23:02.000000 python-llm-0.1.6/llm/api/anthropicapi.py
--rw-r--r--   0 danielgross   (501) staff       (20)     1651 2023-05-20 16:32:24.000000 python-llm-0.1.6/llm/api/openaiapi.py
--rw-r--r--   0 danielgross   (501) staff       (20)     4401 2023-05-20 19:51:36.000000 python-llm-0.1.6/llm/main.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 20:04:05.083408 python-llm-0.1.6/llm/utils/
--rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-05-20 11:50:33.000000 python-llm-0.1.6/llm/utils/__init__.py
--rw-r--r--   0 danielgross   (501) staff       (20)     3200 2023-05-20 11:56:01.000000 python-llm-0.1.6/llm/utils/apikeys.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2441 2023-05-20 19:38:17.000000 python-llm-0.1.6/llm/utils/parsing.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 20:04:05.083966 python-llm-0.1.6/python_llm.egg-info/
--rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-20 20:04:05.000000 python-llm-0.1.6/python_llm.egg-info/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)      424 2023-05-20 20:04:05.000000 python-llm-0.1.6/python_llm.egg-info/SOURCES.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-20 20:04:05.000000 python-llm-0.1.6/python_llm.egg-info/dependency_links.txt
--rw-r--r--   0 danielgross   (501) staff       (20)      167 2023-05-20 20:04:05.000000 python-llm-0.1.6/python_llm.egg-info/requires.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-20 20:04:05.000000 python-llm-0.1.6/python_llm.egg-info/top_level.txt
--rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-20 20:04:05.084805 python-llm-0.1.6/setup.cfg
--rw-r--r--   0 danielgross   (501) staff       (20)      650 2023-05-20 20:03:58.000000 python-llm-0.1.6/setup.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 20:04:05.084364 python-llm-0.1.6/tests/
--rw-r--r--   0 danielgross   (501) staff       (20)     3407 2023-05-20 19:49:17.000000 python-llm-0.1.6/tests/test_anthropic.py
--rw-r--r--   0 danielgross   (501) staff       (20)      945 2023-05-20 19:51:00.000000 python-llm-0.1.6/tests/test_multi_stream.py
--rw-r--r--   0 danielgross   (501) staff       (20)     3651 2023-05-20 19:32:25.000000 python-llm-0.1.6/tests/test_openai.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.165750 python-llm-0.1.7/
+-rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.7/LICENSE
+-rw-r--r--   0 danielgross   (501) staff       (20)       24 2023-05-21 11:54:44.000000 python-llm-0.1.7/MANIFEST.in
+-rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-21 11:55:51.165633 python-llm-0.1.7/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)     2342 2023-05-20 19:12:04.000000 python-llm-0.1.7/README.md
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.163796 python-llm-0.1.7/llm/
+-rw-r--r--   0 danielgross   (501) staff       (20)       81 2023-05-20 15:11:39.000000 python-llm-0.1.7/llm/__init__.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.164121 python-llm-0.1.7/llm/api/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.7/llm/api/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2387 2023-05-20 16:23:02.000000 python-llm-0.1.7/llm/api/anthropicapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     1651 2023-05-20 16:32:24.000000 python-llm-0.1.7/llm/api/openaiapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     4401 2023-05-20 19:51:36.000000 python-llm-0.1.7/llm/main.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.164428 python-llm-0.1.7/llm/utils/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-05-20 11:50:33.000000 python-llm-0.1.7/llm/utils/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     3200 2023-05-20 11:56:01.000000 python-llm-0.1.7/llm/utils/apikeys.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2441 2023-05-20 19:38:17.000000 python-llm-0.1.7/llm/utils/parsing.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.165020 python-llm-0.1.7/python_llm.egg-info/
+-rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-21 11:55:51.000000 python-llm-0.1.7/python_llm.egg-info/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)      453 2023-05-21 11:55:51.000000 python-llm-0.1.7/python_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-21 11:55:51.000000 python-llm-0.1.7/python_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)      167 2023-05-21 11:55:51.000000 python-llm-0.1.7/python_llm.egg-info/requires.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-21 11:55:51.000000 python-llm-0.1.7/python_llm.egg-info/top_level.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)      166 2023-05-20 11:50:33.000000 python-llm-0.1.7/requirements.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-21 11:55:51.165787 python-llm-0.1.7/setup.cfg
+-rw-r--r--   0 danielgross   (501) staff       (20)      650 2023-05-21 11:54:56.000000 python-llm-0.1.7/setup.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 11:55:51.165436 python-llm-0.1.7/tests/
+-rw-r--r--   0 danielgross   (501) staff       (20)     3407 2023-05-20 19:49:17.000000 python-llm-0.1.7/tests/test_anthropic.py
+-rw-r--r--   0 danielgross   (501) staff       (20)      945 2023-05-20 19:51:00.000000 python-llm-0.1.7/tests/test_multi_stream.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     3651 2023-05-20 19:32:25.000000 python-llm-0.1.7/tests/test_openai.py
```

### Comparing `python-llm-0.1.6/LICENSE` & `python-llm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.6/PKG-INFO` & `python-llm-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-llm
-Version: 0.1.6
+Version: 0.1.7
 Summary: An LLM wrapper for Humans
 Home-page: https://github.com/danielgross/python-llm
 Author: Daniel Gross
 Author-email: d@dcgross.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-llm-0.1.6/README.md` & `python-llm-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.6/llm/api/anthropicapi.py` & `python-llm-0.1.7/llm/api/anthropicapi.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.6/llm/api/openaiapi.py` & `python-llm-0.1.7/llm/api/openaiapi.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.6/llm/main.py` & `python-llm-0.1.7/llm/main.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.6/llm/utils/apikeys.py` & `python-llm-0.1.7/llm/utils/apikeys.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.6/llm/utils/parsing.py` & `python-llm-0.1.7/llm/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.6/python_llm.egg-info/PKG-INFO` & `python-llm-0.1.7/python_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-llm
-Version: 0.1.6
+Version: 0.1.7
 Summary: An LLM wrapper for Humans
 Home-page: https://github.com/danielgross/python-llm
 Author: Daniel Gross
 Author-email: d@dcgross.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-llm-0.1.6/setup.py` & `python-llm-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='python-llm',
-    version='0.1.6',
+    version='0.1.7',
     author='Daniel Gross',
     author_email='d@dcgross.com',
     description='An LLM wrapper for Humans',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(include=['llm', 'llm.*']),
     url="https://github.com/danielgross/python-llm",
```

### Comparing `python-llm-0.1.6/tests/test_anthropic.py` & `python-llm-0.1.7/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.6/tests/test_multi_stream.py` & `python-llm-0.1.7/tests/test_multi_stream.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.6/tests/test_openai.py` & `python-llm-0.1.7/tests/test_openai.py`

 * *Files identical despite different names*

