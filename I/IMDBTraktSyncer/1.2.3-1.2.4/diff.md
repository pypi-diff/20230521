# Comparing `tmp/IMDBTraktSyncer-1.2.3.tar.gz` & `tmp/IMDBTraktSyncer-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.2.3.tar", last modified: Sat May 20 21:59:37 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.2.4.tar", last modified: Sat May 20 22:10:14 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.2.3.tar` & `IMDBTraktSyncer-1.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 21:59:37.570212 IMDBTraktSyncer-1.2.3/
-drwxrwxrwx   0        0        0        0 2023-05-20 21:59:37.550198 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    16437 2023-05-20 20:44:52.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1913 2023-05-20 20:45:01.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     5388 2023-05-20 20:44:48.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     4575 2023-05-20 21:58:18.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     5488 2023-05-20 20:44:57.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 21:59:37.567196 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     7755 2023-05-20 21:59:37.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-20 21:59:37.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 21:59:37.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 21:59:37.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-20 21:59:37.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 21:59:37.000000 IMDBTraktSyncer-1.2.3/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     7755 2023-05-20 21:59:37.569196 IMDBTraktSyncer-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     7095 2023-05-20 18:20:58.000000 IMDBTraktSyncer-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 21:59:37.570212 IMDBTraktSyncer-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-05-20 21:59:26.000000 IMDBTraktSyncer-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 22:10:14.349085 IMDBTraktSyncer-1.2.4/
+drwxrwxrwx   0        0        0        0 2023-05-20 22:10:14.329085 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    16437 2023-05-20 20:44:52.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1913 2023-05-20 20:45:01.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     5388 2023-05-20 20:44:48.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     4596 2023-05-20 22:09:24.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     5488 2023-05-20 20:44:57.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 22:10:14.347086 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     7755 2023-05-20 22:10:14.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-20 22:10:14.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 22:10:14.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 22:10:14.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-20 22:10:14.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 22:10:14.000000 IMDBTraktSyncer-1.2.4/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     7755 2023-05-20 22:10:14.349085 IMDBTraktSyncer-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7095 2023-05-20 18:20:58.000000 IMDBTraktSyncer-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 22:10:14.349085 IMDBTraktSyncer-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-05-20 22:09:49.000000 IMDBTraktSyncer-1.2.4/setup.py
```

### Comparing `IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/traktData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import requests
 import time
+import urllib.parse
 try:
     from IMDBTraktSyncer import errorHandling as EH
 except ImportError:
     import errorHandling as EH
 
 def getTraktData():
     # Process Trakt Ratings and Comments
```

### Comparing `IMDBTraktSyncer-1.2.3/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.2.4/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.3/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.2.4/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.3
+Version: 1.2.4
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDBTraktSyncer-1.2.3/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.2.4/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.3/LICENSE` & `IMDBTraktSyncer-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.3/PKG-INFO` & `IMDBTraktSyncer-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.3
+Version: 1.2.4
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDBTraktSyncer-1.2.3/README.md` & `IMDBTraktSyncer-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.3/setup.py` & `IMDBTraktSyncer-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.2.3'
+VERSION = '1.2.4'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

