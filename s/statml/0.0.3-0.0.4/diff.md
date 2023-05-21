# Comparing `tmp/statml-0.0.3.tar.gz` & `tmp/statml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statml-0.0.3.tar", last modified: Sat May 20 14:12:24 2023, max compression
+gzip compressed data, was "statml-0.0.4.tar", last modified: Sun May 21 11:30:57 2023, max compression
```

## Comparing `statml-0.0.3.tar` & `statml-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:12:24.807168 statml-0.0.3/
--rw-rw-rw-   0        0        0      381 2023-05-20 14:12:24.807168 statml-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-05-20 12:40:16.000000 statml-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 14:12:24.807168 statml-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      608 2023-05-20 14:12:10.000000 statml-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:12:24.791544 statml-0.0.3/statml/
--rw-rw-rw-   0        0        0       21 2023-05-20 14:11:59.000000 statml-0.0.3/statml/__init__.py
--rw-rw-rw-   0        0        0     3538 2023-05-20 14:05:21.000000 statml-0.0.3/statml/playchat.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:12:24.807168 statml-0.0.3/statml.egg-info/
--rw-rw-rw-   0        0        0      381 2023-05-20 14:12:24.000000 statml-0.0.3/statml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-05-20 14:12:24.000000 statml-0.0.3/statml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:12:24.000000 statml-0.0.3/statml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-20 14:12:24.000000 statml-0.0.3/statml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 11:30:57.800472 statml-0.0.4/
+-rw-rw-rw-   0        0        0      381 2023-05-21 11:30:57.800472 statml-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-05-20 12:40:16.000000 statml-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 11:30:57.800472 statml-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-05-21 11:28:05.000000 statml-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 11:30:57.784854 statml-0.0.4/statml/
+-rw-rw-rw-   0        0        0       21 2023-05-21 11:28:28.000000 statml-0.0.4/statml/__init__.py
+-rw-rw-rw-   0        0        0     3538 2023-05-20 14:05:21.000000 statml-0.0.4/statml/playchat.py
+-rw-rw-rw-   0        0        0     5209 2023-05-21 11:26:39.000000 statml-0.0.4/statml/stepwise.py
+drwxrwxrwx   0        0        0        0 2023-05-21 11:30:57.800472 statml-0.0.4/statml.egg-info/
+-rw-rw-rw-   0        0        0      381 2023-05-21 11:30:57.000000 statml-0.0.4/statml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-05-21 11:30:57.000000 statml-0.0.4/statml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 11:30:57.000000 statml-0.0.4/statml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 11:30:57.000000 statml-0.0.4/statml.egg-info/top_level.txt
```

### Comparing `statml-0.0.3/setup.py` & `statml-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="statml",
-    version="0.0.3",
+    version="0.0.4",
     author="HaeWoon",
     author_email="likesea7@gmail.com",
     description="stat and ml example",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `statml-0.0.3/statml/playchat.py` & `statml-0.0.4/statml/playchat.py`

 * *Files identical despite different names*

