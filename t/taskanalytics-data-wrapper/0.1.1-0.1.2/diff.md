# Comparing `tmp/taskanalytics_data_wrapper-0.1.1.tar.gz` & `tmp/taskanalytics-data-wrapper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskanalytics_data_wrapper-0.1.1.tar", max compression
+gzip compressed data, was "taskanalytics-data-wrapper-0.1.2.tar", last modified: Sun May 21 18:11:59 2023, max compression
```

## Comparing `taskanalytics_data_wrapper-0.1.1.tar` & `taskanalytics-data-wrapper-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,17 @@
--rw-r--r--   0        0        0     1062 2022-08-17 13:26:47.338552 taskanalytics_data_wrapper-0.1.1/LICENSE
--rw-r--r--   0        0        0     1594 2022-08-17 13:36:54.278695 taskanalytics_data_wrapper-0.1.1/README.md
--rw-r--r--   0        0        0      858 2023-03-06 15:46:51.329067 taskanalytics_data_wrapper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       59 2022-08-17 13:50:59.794277 taskanalytics_data_wrapper-0.1.1/taskanalytics_data_wrapper/__init__.py
--rw-r--r--   0        0        0     5217 2023-03-06 15:41:43.287220 taskanalytics_data_wrapper-0.1.1/taskanalytics_data_wrapper/taskanalytics_api.py
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 taskanalytics_data_wrapper-0.1.1/setup.py
--rw-r--r--   0        0        0     2523 1970-01-01 00:00:00.000000 taskanalytics_data_wrapper-0.1.1/PKG-INFO
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 18:11:59.299399 taskanalytics-data-wrapper-0.1.2/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       88 2023-05-21 18:04:35.000000 taskanalytics-data-wrapper-0.1.2/.gitignore
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.2/CODEOWNERS
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.2/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4994 2023-05-21 18:11:59.298776 taskanalytics-data-wrapper-0.1.2/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3362 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.2/README.md
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2321 2023-05-21 18:11:27.000000 taskanalytics-data-wrapper-0.1.2/example.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      649 2023-05-21 18:03:53.000000 taskanalytics-data-wrapper-0.1.2/pyproject.toml
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-05-21 18:11:59.299525 taskanalytics-data-wrapper-0.1.2/setup.cfg
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 18:11:59.293180 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       59 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5217 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 18:11:59.297828 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4994 2023-05-21 18:11:59.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      460 2023-05-21 18:11:59.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 18:11:59.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 18:11:59.000000 taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_data_wrapper.egg-info/top_level.txt
```

### Comparing `taskanalytics_data_wrapper-0.1.1/LICENSE` & `taskanalytics-data-wrapper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskanalytics_data_wrapper-0.1.1/taskanalytics_data_wrapper/taskanalytics_api.py` & `taskanalytics-data-wrapper-0.1.2/taskanalytics_data_wrapper/taskanalytics_api.py`

 * *Files identical despite different names*

