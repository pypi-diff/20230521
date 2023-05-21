# Comparing `tmp/to-pip-2.0.3.tar.gz` & `tmp/to-pip-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-pip-2.0.3.tar", last modified: Sun May 21 00:07:15 2023, max compression
+gzip compressed data, was "to-pip-2.0.4.tar", last modified: Sun May 21 00:09:07 2023, max compression
```

## Comparing `to-pip-2.0.3.tar` & `to-pip-2.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 00:07:15.770584 to-pip-2.0.3/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 00:07:15.770478 to-pip-2.0.3/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2121 2023-05-21 00:07:15.000000 to-pip-2.0.3/README.md
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 00:07:15.770617 to-pip-2.0.3/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      493 2023-05-21 00:07:15.000000 to-pip-2.0.3/setup.py
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 00:07:15.770330 to-pip-2.0.3/to_pip.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 00:07:15.000000 to-pip-2.0.3/to_pip.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      200 2023-05-21 00:07:15.000000 to-pip-2.0.3/to_pip.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 00:07:15.000000 to-pip-2.0.3/to_pip.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       40 2023-05-21 00:07:15.000000 to-pip-2.0.3/to_pip.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)      103 2023-05-21 00:07:15.000000 to-pip-2.0.3/to_pip.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 00:07:15.000000 to-pip-2.0.3/to_pip.egg-info/top_level.txt
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 00:09:07.489047 to-pip-2.0.4/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 00:09:07.488947 to-pip-2.0.4/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2121 2023-05-21 00:09:07.000000 to-pip-2.0.4/README.md
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 00:09:07.489078 to-pip-2.0.4/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      493 2023-05-21 00:09:07.000000 to-pip-2.0.4/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 00:09:07.488798 to-pip-2.0.4/to_pip.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 00:09:07.000000 to-pip-2.0.4/to_pip.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      200 2023-05-21 00:09:07.000000 to-pip-2.0.4/to_pip.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 00:09:07.000000 to-pip-2.0.4/to_pip.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       40 2023-05-21 00:09:07.000000 to-pip-2.0.4/to_pip.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      103 2023-05-21 00:09:07.000000 to-pip-2.0.4/to_pip.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 00:09:07.000000 to-pip-2.0.4/to_pip.egg-info/top_level.txt
```

### Comparing `to-pip-2.0.3/PKG-INFO` & `to-pip-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-pip
-Version: 2.0.3
+Version: 2.0.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
```

### Comparing `to-pip-2.0.3/README.md` & `to-pip-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `to-pip-2.0.3/to_pip.egg-info/PKG-INFO` & `to-pip-2.0.4/to_pip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-pip
-Version: 2.0.3
+Version: 2.0.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
```

