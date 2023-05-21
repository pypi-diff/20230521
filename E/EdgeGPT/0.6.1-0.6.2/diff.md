# Comparing `tmp/EdgeGPT-0.6.1.tar.gz` & `tmp/EdgeGPT-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.6.1.tar", last modified: Sun May 21 12:03:56 2023, max compression
+gzip compressed data, was "EdgeGPT-0.6.2.tar", last modified: Sun May 21 14:19:13 2023, max compression
```

## Comparing `EdgeGPT-0.6.1.tar` & `EdgeGPT-0.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:03:56.927191 EdgeGPT-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-21 12:03:28.000000 EdgeGPT-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 12:03:56.927191 EdgeGPT-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-21 12:03:56.000000 EdgeGPT-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 12:03:56.927191 EdgeGPT-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-21 12:03:28.000000 EdgeGPT-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:03:56.927191 EdgeGPT-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:03:56.927191 EdgeGPT-0.6.1/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 12:03:56.000000 EdgeGPT-0.6.1/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 12:03:56.000000 EdgeGPT-0.6.1/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:03:56.000000 EdgeGPT-0.6.1/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 12:03:56.000000 EdgeGPT-0.6.1/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 12:03:56.000000 EdgeGPT-0.6.1/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-21 12:03:56.000000 EdgeGPT-0.6.1/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    37881 2023-05-21 12:03:28.000000 EdgeGPT-0.6.1/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-21 12:03:28.000000 EdgeGPT-0.6.1/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:13.103952 EdgeGPT-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-21 14:18:43.000000 EdgeGPT-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 14:19:13.103952 EdgeGPT-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-21 14:19:12.000000 EdgeGPT-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 14:19:13.103952 EdgeGPT-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-21 14:18:43.000000 EdgeGPT-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:13.103952 EdgeGPT-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:19:13.103952 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-21 14:19:13.000000 EdgeGPT-0.6.2/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-05-21 14:18:43.000000 EdgeGPT-0.6.2/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-21 14:18:43.000000 EdgeGPT-0.6.2/src/ImageGen.py
```

### Comparing `EdgeGPT-0.6.1/LICENSE` & `EdgeGPT-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.1/PKG-INFO` & `EdgeGPT-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.1
+Version: 0.6.2
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `EdgeGPT-0.6.1/README.md` & `EdgeGPT-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.1/setup.py` & `EdgeGPT-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.6.1",
+    version="0.6.2",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.6.1/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.6.2/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.1
+Version: 0.6.2
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `EdgeGPT-0.6.1/src/EdgeGPT.py` & `EdgeGPT-0.6.2/src/EdgeGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -691,14 +691,15 @@
         """
         Reset the conversation
         """
         await self.close()
         self.chat_hub = _ChatHub(
             await _Conversation.create(self.proxy),
             proxy=self.proxy,
+            cookies=self.chat_hub.cookies,
         )
 
 
 async def _get_input_async(
     session: PromptSession = None,
     completer: WordCompleter = None,
 ) -> str:
```

