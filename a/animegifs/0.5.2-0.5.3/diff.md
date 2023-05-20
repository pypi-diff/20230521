# Comparing `tmp/animegifs-0.5.2.tar.gz` & `tmp/animegifs-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.5.2.tar", last modified: Wed May 10 14:34:39 2023, max compression
+gzip compressed data, was "animegifs-0.5.3.tar", last modified: Sat May 20 23:53:58 2023, max compression
```

## Comparing `animegifs-0.5.2.tar` & `animegifs-0.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 14:34:39.921667 animegifs-0.5.2/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.5.2/LICENSE
--rw-rw-rw-   0        0        0     1193 2023-05-10 14:34:39.920668 animegifs-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-05-10 01:34:05.000000 animegifs-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 14:34:39.903665 animegifs-0.5.2/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.5.2/animegifs/__init__.py
--rw-rw-rw-   0        0        0     2383 2023-05-10 14:08:03.000000 animegifs-0.5.2/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:34:39.918669 animegifs-0.5.2/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.5.2/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0     1186 2023-05-10 14:18:41.000000 animegifs-0.5.2/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0     1313 2023-04-28 20:51:38.000000 animegifs-0.5.2/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:34:39.913668 animegifs-0.5.2/animegifs.egg-info/
--rw-rw-rw-   0        0        0     1193 2023-05-10 14:34:39.000000 animegifs-0.5.2/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-05-10 14:34:39.000000 animegifs-0.5.2/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 14:34:39.000000 animegifs-0.5.2/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-10 14:34:39.000000 animegifs-0.5.2/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 14:34:39.000000 animegifs-0.5.2/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 14:34:39.921667 animegifs-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-10 14:33:56.000000 animegifs-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:53:58.465564 animegifs-0.5.3/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0     1214 2023-05-20 23:53:58.464563 animegifs-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2023-05-20 23:51:48.000000 animegifs-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 23:53:58.437562 animegifs-0.5.3/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.5.3/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     1064 2023-05-20 23:51:21.000000 animegifs-0.5.3/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:53:58.462563 animegifs-0.5.3/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.5.3/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     1186 2023-05-10 14:18:41.000000 animegifs-0.5.3/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0      705 2023-05-20 23:51:21.000000 animegifs-0.5.3/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:53:58.453564 animegifs-0.5.3/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     1214 2023-05-20 23:53:58.000000 animegifs-0.5.3/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-05-20 23:53:58.000000 animegifs-0.5.3/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 23:53:58.000000 animegifs-0.5.3/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-20 23:53:58.000000 animegifs-0.5.3/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-20 23:53:58.000000 animegifs-0.5.3/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 23:53:58.466565 animegifs-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-20 23:51:21.000000 animegifs-0.5.3/setup.py
```

### Comparing `animegifs-0.5.2/LICENSE` & `animegifs-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.5.2/PKG-INFO` & `animegifs-0.5.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.5.2
+Version: 0.5.3
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # animegifs.py
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
-WIP - updated in time to time. Versions below v0.4.0 aren't expected to work.
+WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all.
 
 `pip install animegifs`
 
 # HOW TO USE
 
 ```py
```

### Comparing `animegifs-0.5.2/README.md` & `animegifs-0.5.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # animegifs.py
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
-WIP - updated in time to time. Versions below v0.4.0 aren't expected to work.
+WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all.
 
 `pip install animegifs`
 
 # HOW TO USE
 
 ```py
```

### Comparing `animegifs-0.5.2/animegifs/distutils/errors.py` & `animegifs-0.5.3/animegifs/distutils/errors.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.5.2/animegifs.egg-info/PKG-INFO` & `animegifs-0.5.3/animegifs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.5.2
+Version: 0.5.3
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # animegifs.py
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
-WIP - updated in time to time. Versions below v0.4.0 aren't expected to work.
+WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all.
 
 `pip install animegifs`
 
 # HOW TO USE
 
 ```py
```

### Comparing `animegifs-0.5.2/setup.py` & `animegifs-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.5.2'
+VERSION = '0.5.3'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
```

