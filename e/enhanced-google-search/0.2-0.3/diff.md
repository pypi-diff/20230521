# Comparing `tmp/enhanced_google_search-0.2.tar.gz` & `tmp/enhanced_google_search-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhanced_google_search-0.2.tar", last modified: Fri May 19 13:19:20 2023, max compression
+gzip compressed data, was "enhanced_google_search-0.3.tar", last modified: Sun May 21 13:50:20 2023, max compression
```

## Comparing `enhanced_google_search-0.2.tar` & `enhanced_google_search-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 13:19:20.982349 enhanced_google_search-0.2/
--rw-rw-rw-   0        0        0     1044 2023-05-19 13:19:20.981354 enhanced_google_search-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      717 2023-05-19 13:18:29.000000 enhanced_google_search-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 13:19:20.982349 enhanced_google_search-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1447 2023-05-19 13:18:11.000000 enhanced_google_search-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:19:20.951432 enhanced_google_search-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 13:19:20.979356 enhanced_google_search-0.2/src/enhanced_google_search.egg-info/
--rw-rw-rw-   0        0        0     1044 2023-05-19 13:19:20.000000 enhanced_google_search-0.2/src/enhanced_google_search.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-19 13:19:20.000000 enhanced_google_search-0.2/src/enhanced_google_search.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 13:19:20.000000 enhanced_google_search-0.2/src/enhanced_google_search.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-19 13:19:20.000000 enhanced_google_search-0.2/src/enhanced_google_search.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-19 13:19:20.000000 enhanced_google_search-0.2/src/enhanced_google_search.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1159 2023-05-19 13:17:04.000000 enhanced_google_search-0.2/src/enhanced_google_search.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:50:20.579959 enhanced_google_search-0.3/
+-rw-rw-rw-   0        0        0     1170 2023-05-21 13:50:20.578961 enhanced_google_search-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      843 2023-05-21 13:48:48.000000 enhanced_google_search-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 13:50:20.579959 enhanced_google_search-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      528 2023-05-21 13:49:17.000000 enhanced_google_search-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:50:20.541860 enhanced_google_search-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 13:50:20.574973 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/
+-rw-rw-rw-   0        0        0     1170 2023-05-21 13:50:19.000000 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-21 13:50:20.000000 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 13:50:19.000000 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-21 13:50:19.000000 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-21 13:50:19.000000 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1159 2023-05-19 13:17:04.000000 enhanced_google_search-0.3/src/enhanced_google_search.py
```

### Comparing `enhanced_google_search-0.2/PKG-INFO` & `enhanced_google_search-0.3/src/enhanced_google_search.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
-Name: enhanced_google_search
-Version: 0.2
+Name: enhanced-google-search
+Version: 0.3
 Summary: An enhanced google search library
 Home-page: https://github.com/K-K-L-L/google_search_py
 Author: KKLL
 Keywords: googlesearch.py,enhanced_google_search,python google search,google search pypi,google api
 Description-Content-Type: text/markdown
 
 # enhanced_google_search
 An enhanced google search library
 
+**The New PyPi Project: https://pypi.org/project/enhanced-google-search/**
+
 Fixed the language issue in the original repo: https://github.com/cj-praveen/googlesearch.py so you can search with any language google.com support
 
+```py
+pip install enhanced-google-search
+```
 
 Examples:
 ```py
 from enhanced_google_search import search
 
 results = search("بايثون", lang = "ar")
 print(results)
```

### Comparing `enhanced_google_search-0.2/src/enhanced_google_search.egg-info/PKG-INFO` & `enhanced_google_search-0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
-Name: enhanced-google-search
-Version: 0.2
+Name: enhanced_google_search
+Version: 0.3
 Summary: An enhanced google search library
 Home-page: https://github.com/K-K-L-L/google_search_py
 Author: KKLL
 Keywords: googlesearch.py,enhanced_google_search,python google search,google search pypi,google api
 Description-Content-Type: text/markdown
 
 # enhanced_google_search
 An enhanced google search library
 
+**The New PyPi Project: https://pypi.org/project/enhanced-google-search/**
+
 Fixed the language issue in the original repo: https://github.com/cj-praveen/googlesearch.py so you can search with any language google.com support
 
+```py
+pip install enhanced-google-search
+```
 
 Examples:
 ```py
 from enhanced_google_search import search
 
 results = search("بايثون", lang = "ar")
 print(results)
```

### Comparing `enhanced_google_search-0.2/src/enhanced_google_search.py` & `enhanced_google_search-0.3/src/enhanced_google_search.py`

 * *Files identical despite different names*

