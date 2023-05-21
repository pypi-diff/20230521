# Comparing `tmp/to-pip-2.0.6.tar.gz` & `tmp/to-pip-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-pip-2.0.6.tar", last modified: Sun May 21 00:18:10 2023, max compression
+gzip compressed data, was "to-pip-2.0.7.tar", last modified: Sun May 21 00:19:43 2023, max compression
```

## Comparing `to-pip-2.0.6.tar` & `to-pip-2.0.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 00:18:10.298022 to-pip-2.0.6/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 00:18:10.297923 to-pip-2.0.6/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2121 2023-05-21 00:18:10.000000 to-pip-2.0.6/README.md
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 00:18:10.298054 to-pip-2.0.6/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      488 2023-05-21 00:18:10.000000 to-pip-2.0.6/setup.py
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 00:18:10.297768 to-pip-2.0.6/to_pip.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 00:18:10.000000 to-pip-2.0.6/to_pip.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      210 2023-05-21 00:18:10.000000 to-pip-2.0.6/to_pip.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 00:18:10.000000 to-pip-2.0.6/to_pip.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       40 2023-05-21 00:18:10.000000 to-pip-2.0.6/to_pip.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)      103 2023-05-21 00:18:10.000000 to-pip-2.0.6/to_pip.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        7 2023-05-21 00:18:10.000000 to-pip-2.0.6/to_pip.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     4483 2023-05-21 00:18:10.000000 to-pip-2.0.6/to_pip.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 00:19:43.773320 to-pip-2.0.7/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 00:19:43.773210 to-pip-2.0.7/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2121 2023-05-21 00:19:43.000000 to-pip-2.0.7/README.md
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)       66 2023-05-21 00:19:43.000000 to-pip-2.0.7/hi.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 00:19:43.773353 to-pip-2.0.7/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      508 2023-05-21 00:19:43.000000 to-pip-2.0.7/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 00:19:43.773059 to-pip-2.0.7/to_pip.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      216 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       54 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      103 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       10 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     4483 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.py
```

### Comparing `to-pip-2.0.6/PKG-INFO` & `to-pip-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-pip
-Version: 2.0.6
+Version: 2.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
```

### Comparing `to-pip-2.0.6/README.md` & `to-pip-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `to-pip-2.0.6/to_pip.egg-info/PKG-INFO` & `to-pip-2.0.7/to_pip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-pip
-Version: 2.0.6
+Version: 2.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
```

### Comparing `to-pip-2.0.6/to_pip.py` & `to-pip-2.0.7/to_pip.py`

 * *Files identical despite different names*

