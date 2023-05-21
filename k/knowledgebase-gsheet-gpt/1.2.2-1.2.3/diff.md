# Comparing `tmp/knowledgebase-gsheet-gpt-1.2.2.tar.gz` & `tmp/knowledgebase-gsheet-gpt-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgebase-gsheet-gpt-1.2.2.tar", last modified: Sun May 14 15:55:31 2023, max compression
+gzip compressed data, was "knowledgebase-gsheet-gpt-1.2.3.tar", last modified: Sun May 21 16:45:31 2023, max compression
```

## Comparing `knowledgebase-gsheet-gpt-1.2.2.tar` & `knowledgebase-gsheet-gpt-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 15:55:31.138957 knowledgebase-gsheet-gpt-1.2.2/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 15:55:31.138844 knowledgebase-gsheet-gpt-1.2.2/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-14 15:55:30.000000 knowledgebase-gsheet-gpt-1.2.2/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 15:55:31.138659 knowledgebase-gsheet-gpt-1.2.2/knowledgebase_gsheet_gpt.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 15:55:31.000000 knowledgebase-gsheet-gpt-1.2.2/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-14 15:55:31.000000 knowledgebase-gsheet-gpt-1.2.2/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-14 15:55:31.000000 knowledgebase-gsheet-gpt-1.2.2/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-14 15:55:31.000000 knowledgebase-gsheet-gpt-1.2.2/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       98 2023-05-14 15:55:31.000000 knowledgebase-gsheet-gpt-1.2.2/knowledgebase_gsheet_gpt.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-14 15:55:31.000000 knowledgebase-gsheet-gpt-1.2.2/knowledgebase_gsheet_gpt.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     5515 2023-05-14 15:55:30.000000 knowledgebase-gsheet-gpt-1.2.2/knowledgebase_gsheet_gpt.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-14 15:55:31.138993 knowledgebase-gsheet-gpt-1.2.2/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-14 15:55:30.000000 knowledgebase-gsheet-gpt-1.2.2/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 16:45:31.603348 knowledgebase-gsheet-gpt-1.2.3/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-21 16:45:31.603237 knowledgebase-gsheet-gpt-1.2.3/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 16:45:31.603060 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       98 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     5515 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 16:45:31.603385 knowledgebase-gsheet-gpt-1.2.3/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-21 16:45:31.000000 knowledgebase-gsheet-gpt-1.2.3/setup.py
```

### Comparing `knowledgebase-gsheet-gpt-1.2.2/PKG-INFO` & `knowledgebase-gsheet-gpt-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.2.2
+Version: 1.2.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.2.2/README.md` & `knowledgebase-gsheet-gpt-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `knowledgebase-gsheet-gpt-1.2.2/knowledgebase_gsheet_gpt.egg-info/PKG-INFO` & `knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.2.2
+Version: 1.2.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.2.2/knowledgebase_gsheet_gpt.py` & `knowledgebase-gsheet-gpt-1.2.3/knowledgebase_gsheet_gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 DEFAULT_BEFORE_KNOWLEDGE_PROMPT = '\n-- reference following knowledge base content to answer the user question (answer as long as possible)\n'
 DEFAULT_MODEL = "gpt-4"
 DEFAULT_TOP_N = 1
 DEFAULT_KEY_FILE = "./keys/google_service_account_key.json"
 
 
 class ChatMemory:
-    def __init__(self, max_n=5):
+    def __init__(self, max_n=3):
         self.max_n = max_n
         self.user_dict = {}
 
     def append_context(self, user, text):
         if user not in self.user_dict:
             self.user_dict[user] = []
         self.user_dict[user].append(text)
```

### Comparing `knowledgebase-gsheet-gpt-1.2.2/setup.py` & `knowledgebase-gsheet-gpt-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="knowledgebase-gsheet-gpt",
-    version="1.2.2",
+    version="1.2.3",
     packages=find_packages(),
     py_modules=['knowledgebase_gsheet_gpt'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'knowledgebase_gsheet_gpt = knowledgebase_gsheet_gpt:main',
         ],
```

