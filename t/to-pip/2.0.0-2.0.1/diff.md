# Comparing `tmp/to-pip-2.0.0.tar.gz` & `tmp/to-pip-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-pip-2.0.0.tar", last modified: Sat May 20 23:51:31 2023, max compression
+gzip compressed data, was "to-pip-2.0.1.tar", last modified: Sat May 20 23:57:26 2023, max compression
```

## Comparing `to-pip-2.0.0.tar` & `to-pip-2.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-20 23:51:31.864720 to-pip-2.0.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-20 23:51:31.864611 to-pip-2.0.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2121 2023-05-20 23:51:31.000000 to-pip-2.0.0/README.md
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-20 23:51:31.864753 to-pip-2.0.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      507 2023-05-20 23:51:31.000000 to-pip-2.0.0/setup.py
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-20 23:51:31.864454 to-pip-2.0.0/to_pip.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-20 23:51:31.000000 to-pip-2.0.0/to_pip.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      200 2023-05-20 23:51:31.000000 to-pip-2.0.0/to_pip.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-20 23:51:31.000000 to-pip-2.0.0/to_pip.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       54 2023-05-20 23:51:31.000000 to-pip-2.0.0/to_pip.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)      103 2023-05-20 23:51:31.000000 to-pip-2.0.0/to_pip.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-20 23:51:31.000000 to-pip-2.0.0/to_pip.egg-info/top_level.txt
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-20 23:57:26.230730 to-pip-2.0.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-20 23:57:26.230630 to-pip-2.0.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2121 2023-05-20 23:57:26.000000 to-pip-2.0.1/README.md
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-20 23:57:26.230766 to-pip-2.0.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      493 2023-05-20 23:57:26.000000 to-pip-2.0.1/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-20 23:57:26.230481 to-pip-2.0.1/to_pip.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-20 23:57:26.000000 to-pip-2.0.1/to_pip.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      200 2023-05-20 23:57:26.000000 to-pip-2.0.1/to_pip.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-20 23:57:26.000000 to-pip-2.0.1/to_pip.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       40 2023-05-20 23:57:26.000000 to-pip-2.0.1/to_pip.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      103 2023-05-20 23:57:26.000000 to-pip-2.0.1/to_pip.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-20 23:57:26.000000 to-pip-2.0.1/to_pip.egg-info/top_level.txt
```

### Comparing `to-pip-2.0.0/PKG-INFO` & `to-pip-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-pip
-Version: 2.0.0
+Version: 2.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
```

### Comparing `to-pip-2.0.0/README.md` & `to-pip-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `to-pip-2.0.0/to_pip.egg-info/PKG-INFO` & `to-pip-2.0.1/to_pip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-pip
-Version: 2.0.0
+Version: 2.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
```

