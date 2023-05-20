# Comparing `tmp/IMDBTraktSyncer-1.2.2.tar.gz` & `tmp/IMDBTraktSyncer-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.2.2.tar", last modified: Sat May 20 20:51:37 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.2.5.tar", last modified: Sat May 20 22:19:45 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.2.2.tar` & `IMDBTraktSyncer-1.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 20:51:37.546074 IMDBTraktSyncer-1.2.2/
-drwxrwxrwx   0        0        0        0 2023-05-20 20:51:37.521037 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    16437 2023-05-20 20:44:52.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1913 2023-05-20 20:45:01.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     5388 2023-05-20 20:44:48.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     4528 2023-05-20 20:47:54.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     5488 2023-05-20 20:44:57.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 20:51:37.543074 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     7755 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     7755 2023-05-20 20:51:37.545074 IMDBTraktSyncer-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     7095 2023-05-20 18:20:58.000000 IMDBTraktSyncer-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 20:51:37.546074 IMDBTraktSyncer-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-05-20 20:51:05.000000 IMDBTraktSyncer-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 22:19:45.664542 IMDBTraktSyncer-1.2.5/
+drwxrwxrwx   0        0        0        0 2023-05-20 22:19:45.642543 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    16437 2023-05-20 20:44:52.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1913 2023-05-20 20:45:01.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     5388 2023-05-20 20:44:48.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     4612 2023-05-20 22:17:55.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     5488 2023-05-20 20:44:57.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 22:19:45.662542 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     7755 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 22:19:45.000000 IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     7755 2023-05-20 22:19:45.664542 IMDBTraktSyncer-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7095 2023-05-20 18:20:58.000000 IMDBTraktSyncer-1.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 22:19:45.665544 IMDBTraktSyncer-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-05-20 22:19:34.000000 IMDBTraktSyncer-1.2.5/setup.py
```

### Comparing `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/traktData.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
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
     print('Processing Trakt Ratings and Comments')
 
     response = EH.make_trakt_request('https://api.trakt.tv/users/me')
     json_data = json.loads(response.text)
-    username = json_data['username']
-
-    # Get Trakt Ratings
-    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{username}/ratings')
+    username_slug = json_data['ids']['slug']
+    encoded_username = urllib.parse.quote(username_slug)
+    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/ratings')
     json_data = json.loads(response.text)
 
     movie_ratings = []
     show_ratings = []
     episode_ratings = []
 
     for item in json_data:
@@ -38,21 +38,21 @@
             episode_id = episode.get('ids', {}).get('imdb')
             episode_title = f'{show_title}: {episode.get("title")}'
             episode_ratings.append({'Title': episode_title, 'Year': episode.get('year'), 'Rating': item.get('rating'), 'ID': episode_id, 'Type': 'episode'})
 
     trakt_ratings = movie_ratings + show_ratings + episode_ratings
 
     # Get Trakt Comments
-    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{username}/comments')
+    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/comments')
     json_data = json.loads(response.text)
     total_pages = response.headers.get('X-Pagination-Page-Count')
     trakt_comments = []
 
     for page in range(1, int(total_pages) + 1):
-        response = EH.make_trakt_request(f'https://api.trakt.tv/users/{username}/comments', params={'page': page})
+        response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/comments', params={'page': page})
         json_data = json.loads(response.text)
 
         for comment in json_data:
             comment_type = comment['type']
             spoiler = comment.get('spoiler', False)
 
             if comment_type == 'movie':
```

### Comparing `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.2
+Version: 1.2.5
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.2.5/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.2/LICENSE` & `IMDBTraktSyncer-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.2/PKG-INFO` & `IMDBTraktSyncer-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.2
+Version: 1.2.5
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDBTraktSyncer-1.2.2/README.md` & `IMDBTraktSyncer-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.2/setup.py` & `IMDBTraktSyncer-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.2.2'
+VERSION = '1.2.5'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

