# Comparing `tmp/aij-1.0.8.tar.gz` & `tmp/aij-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.0.8.tar", last modified: Sun May 21 19:36:43 2023, max compression
+gzip compressed data, was "aij-1.0.9.tar", last modified: Sun May 21 20:06:42 2023, max compression
```

## Comparing `aij-1.0.8.tar` & `aij-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.760583 aij-1.0.8/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-21 19:36:43.759586 aij-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.0.8/README.md
--rw-rw-rw-   0        0        0     6363 2023-05-21 19:36:29.000000 aij-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 19:36:43.761593 aij-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.701261 aij-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.741925 aij-1.0.8/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      213 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0       46 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.742929 aij-1.0.8/src/chat/
--rw-rw-rw-   0        0        0      563 2023-05-21 19:33:03.000000 aij-1.0.8/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.744445 aij-1.0.8/src/intro/
--rw-rw-rw-   0        0        0     4607 2023-05-21 19:15:32.000000 aij-1.0.8/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.747473 aij-1.0.8/src/messaging/
--rw-rw-rw-   0        0        0     4444 2023-05-21 19:19:30.000000 aij-1.0.8/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.750012 aij-1.0.8/src/news/
--rw-rw-rw-   0        0        0     9588 2023-05-21 19:19:41.000000 aij-1.0.8/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.752014 aij-1.0.8/src/setup/
--rw-rw-rw-   0        0        0     3080 2023-05-21 19:19:56.000000 aij-1.0.8/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.754534 aij-1.0.8/src/speech/
--rw-rw-rw-   0        0        0     1289 2023-05-21 19:35:54.000000 aij-1.0.8/src/speech/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.756581 aij-1.0.8/src/webcam/
--rw-rw-rw-   0        0        0    17592 2023-05-21 19:07:03.000000 aij-1.0.8/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.797595 aij-1.0.9/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-21 20:06:42.795586 aij-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.0.9/README.md
+-rw-rw-rw-   0        0        0     6423 2023-05-21 20:06:32.000000 aij-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 20:06:42.797595 aij-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.729812 aij-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.777360 aij-1.0.9/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      252 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       46 2023-05-21 20:06:42.000000 aij-1.0.9/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.778997 aij-1.0.9/src/chat/
+-rw-rw-rw-   0        0        0      561 2023-05-21 19:57:44.000000 aij-1.0.9/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.781183 aij-1.0.9/src/intro/
+-rw-rw-rw-   0        0        0     4607 2023-05-21 19:15:32.000000 aij-1.0.9/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.784075 aij-1.0.9/src/messaging/
+-rw-rw-rw-   0        0        0     4444 2023-05-21 19:19:30.000000 aij-1.0.9/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.786822 aij-1.0.9/src/news/
+-rw-rw-rw-   0        0        0     9588 2023-05-21 19:19:41.000000 aij-1.0.9/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.788524 aij-1.0.9/src/setup/
+-rw-rw-rw-   0        0        0     3080 2023-05-21 19:19:56.000000 aij-1.0.9/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.791048 aij-1.0.9/src/speech/
+-rw-rw-rw-   0        0        0     1289 2023-05-21 19:35:54.000000 aij-1.0.9/src/speech/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:06:42.793600 aij-1.0.9/src/webcam/
+-rw-rw-rw-   0        0        0    17592 2023-05-21 19:07:03.000000 aij-1.0.9/src/webcam/__init__.py
```

### Comparing `aij-1.0.8/LICENSE.txt` & `aij-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.0.8/PKG-INFO` & `aij-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.0.8
+Version: 1.0.9
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.0.8/README.md` & `aij-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.0.8/pyproject.toml` & `aij-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.8"
+version = "1.0.9"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -111,16 +111,19 @@
     "pandas",
     "gtts",
     "pygame",
     "cairosvg",
     "pika",
     "newsapi-python",
     "openai",
+    "openai-whisper",
     "langchain",
-    "plyer"
+    "plyer",
+    "python-dotenv",
+    "kivy[dev]"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
```

### Comparing `aij-1.0.8/src/aij.egg-info/PKG-INFO` & `aij-1.0.9/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.0.8
+Version: 1.0.9
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.0.8/src/chat/__init__.py` & `aij-1.0.9/src/chat/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import openai
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
 
 response = openai.Completion.create(
     model="text-davinci-003",
-    prompt="The following is a conversation with an AI journalist. The assistant is helpful, creative, clever, and very friendly.\n\nHuman: Hello, who are you?\nAI: I am an AI created by OpenAI. How can I help you today?\nHuman: I'd like to cancel my subscription.\nAI:",
+    prompt="The following is a conversation with an AI journalist. The assistant is helpful, creative, clever, and very friendly.\n\nHuman: Hello, who are you?\nAI: I am an AI created by OpenAI. How can I help you today?\nHuman: I'd like to read the latest news.\nAI:",
     temperature=0.9,
     max_tokens=150,
     top_p=1,
     frequency_penalty=0.0,
     presence_penalty=0.6,
     stop=[" Human:", " AI:"]
 )
```

### Comparing `aij-1.0.8/src/intro/__init__.py` & `aij-1.0.9/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.8/src/messaging/__init__.py` & `aij-1.0.9/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.8/src/news/__init__.py` & `aij-1.0.9/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.8/src/setup/__init__.py` & `aij-1.0.9/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.8/src/speech/__init__.py` & `aij-1.0.9/src/speech/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.8/src/webcam/__init__.py` & `aij-1.0.9/src/webcam/__init__.py`

 * *Files identical despite different names*

