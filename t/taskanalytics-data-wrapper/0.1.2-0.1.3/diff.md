# Comparing `tmp/taskanalytics-data-wrapper-0.1.2.tar.gz` & `tmp/taskanalytics-data-wrapper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskanalytics-data-wrapper-0.1.2.tar", last modified: Sun May 21 18:11:59 2023, max compression
+gzip compressed data, was "taskanalytics-data-wrapper-0.1.3.tar", last modified: Sun May 21 20:37:56 2023, max compression
```

## Comparing `taskanalytics-data-wrapper-0.1.2.tar` & `taskanalytics-data-wrapper-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 18:11:59.299399 taskanalytics-data-wrapper-0.1.2/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       88 2023-05-21 18:04:35.000000 taskanalytics-data-wrapper-0.1.2/.gitignore
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.2/CODEOWNERS
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.2/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4994 2023-05-21 18:11:59.298776 taskanalytics-data-wrapper-0.1.2/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3362 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.2/README.md
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2321 2023-05-21 18:11:27.000000 taskanalytics-data-wrapper-0.1.2/example.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      649 2023-05-21 18:03:53.000000 taskanalytics-data-wrapper-0.1.2/pyproject.toml
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-05-21 18:11:59.299525 taskanalytics-data-wrapper-0.1.2/setup.cfg
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 18:11:59.293180 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       59 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/__init__.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5217 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_api.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 18:11:59.297828 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4994 2023-05-21 18:11:59.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      460 2023-05-21 18:11:59.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 18:11:59.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 18:11:59.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:37:56.172299 taskanalytics-data-wrapper-0.1.3/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       85 2023-05-21 18:14:07.000000 taskanalytics-data-wrapper-0.1.3/.gitignore
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.3/CODEOWNERS
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.3/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      820 2023-05-21 20:33:58.000000 taskanalytics-data-wrapper-0.1.3/Makefile
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4994 2023-05-21 20:37:56.171248 taskanalytics-data-wrapper-0.1.3/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3362 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.3/README.md
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2321 2023-05-21 18:11:27.000000 taskanalytics-data-wrapper-0.1.3/example.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      969 2023-05-21 20:37:36.000000 taskanalytics-data-wrapper-0.1.3/pyproject.toml
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:37:56.148591 taskanalytics-data-wrapper-0.1.3/requirements/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       43 2023-05-21 18:03:20.000000 taskanalytics-data-wrapper-0.1.3/requirements/dev.in
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2831 2023-05-21 20:34:36.000000 taskanalytics-data-wrapper-0.1.3/requirements/dev.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       13 2023-05-21 18:03:07.000000 taskanalytics-data-wrapper-0.1.3/requirements/main.in
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      412 2023-05-21 20:34:30.000000 taskanalytics-data-wrapper-0.1.3/requirements/main.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-05-21 20:37:56.172554 taskanalytics-data-wrapper-0.1.3/setup.cfg
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:37:56.162451 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       59 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5217 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:37:56.169201 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4994 2023-05-21 20:37:56.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      629 2023-05-21 20:37:56.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 20:37:56.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       99 2023-05-21 20:37:56.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/requires.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 20:37:56.000000 taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/top_level.txt
```

### Comparing `taskanalytics-data-wrapper-0.1.2/LICENSE` & `taskanalytics-data-wrapper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taskanalytics-data-wrapper-0.1.2/PKG-INFO` & `taskanalytics-data-wrapper-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskanalytics-data-wrapper
-Version: 0.1.2
+Version: 0.1.3
 Summary: a wrapper for using Task Analytics APIs and downloading survey responses
 Author-email: Tobias McVey <tobias.mcvey@nav.no>
 License: MIT License
         
         Copyright (c) 2022 NAV IT
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `taskanalytics-data-wrapper-0.1.2/README.md` & `taskanalytics-data-wrapper-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `taskanalytics-data-wrapper-0.1.2/example.py` & `taskanalytics-data-wrapper-0.1.3/example.py`

 * *Files identical despite different names*

### Comparing `taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_api.py` & `taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_api.py`

 * *Files identical despite different names*

### Comparing `taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/PKG-INFO` & `taskanalytics-data-wrapper-0.1.3/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskanalytics-data-wrapper
-Version: 0.1.2
+Version: 0.1.3
 Summary: a wrapper for using Task Analytics APIs and downloading survey responses
 Author-email: Tobias McVey <tobias.mcvey@nav.no>
 License: MIT License
         
         Copyright (c) 2022 NAV IT
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

