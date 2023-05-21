# Comparing `tmp/scorecardpipeline-0.1.3.tar.gz` & `tmp/scorecardpipeline-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecardpipeline-0.1.3.tar", last modified: Thu May  4 16:31:43 2023, max compression
+gzip compressed data, was "scorecardpipeline-0.1.4.tar", last modified: Sun May 21 06:43:12 2023, max compression
```

## Comparing `scorecardpipeline-0.1.3.tar` & `scorecardpipeline-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxr-x   0 itlubber  (1000) itlubber  (1000)        0 2023-05-04 16:31:43.240709 scorecardpipeline-0.1.3/
--rw-rw-r--   0 itlubber  (1000) itlubber  (1000)     1065 2023-05-04 16:28:26.000000 scorecardpipeline-0.1.3/LICENSE
--rw-rw-r--   0 itlubber  (1000) itlubber  (1000)     1069 2023-05-04 16:31:43.240709 scorecardpipeline-0.1.3/PKG-INFO
--rw-rw-r--   0 itlubber  (1000) itlubber  (1000)      187 2023-05-04 16:28:26.000000 scorecardpipeline-0.1.3/README.md
-drwxrwxr-x   0 itlubber  (1000) itlubber  (1000)        0 2023-05-04 16:31:43.240709 scorecardpipeline-0.1.3/scorecardpipeline/
--rw-rw-r--   0 itlubber  (1000) itlubber  (1000)      125 2023-05-04 16:28:58.000000 scorecardpipeline-0.1.3/scorecardpipeline/__init__.py
-drwxrwxr-x   0 itlubber  (1000) itlubber  (1000)        0 2023-05-04 16:31:43.240709 scorecardpipeline-0.1.3/scorecardpipeline.egg-info/
--rw-rw-r--   0 itlubber  (1000) itlubber  (1000)     1069 2023-05-04 16:31:43.000000 scorecardpipeline-0.1.3/scorecardpipeline.egg-info/PKG-INFO
--rw-rw-r--   0 itlubber  (1000) itlubber  (1000)      220 2023-05-04 16:31:43.000000 scorecardpipeline-0.1.3/scorecardpipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 itlubber  (1000) itlubber  (1000)        1 2023-05-04 16:31:43.000000 scorecardpipeline-0.1.3/scorecardpipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 itlubber  (1000) itlubber  (1000)       18 2023-05-04 16:31:43.000000 scorecardpipeline-0.1.3/scorecardpipeline.egg-info/top_level.txt
--rw-rw-r--   0 itlubber  (1000) itlubber  (1000)       38 2023-05-04 16:31:43.240709 scorecardpipeline-0.1.3/setup.cfg
--rw-rw-r--   0 itlubber  (1000) itlubber  (1000)     1788 2023-05-04 16:28:52.000000 scorecardpipeline-0.1.3/setup.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 06:43:12.531588 scorecardpipeline-0.1.4/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-04 06:14:30.000000 scorecardpipeline-0.1.4/LICENSE
+-rw-r--r--   0 lubberit   (501) staff       (20)    33207 2023-05-21 06:43:12.531265 scorecardpipeline-0.1.4/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)    32325 2023-05-21 06:41:54.000000 scorecardpipeline-0.1.4/README.md
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 06:43:12.529021 scorecardpipeline-0.1.4/scorecardpipeline/
+-rw-r--r--   0 lubberit   (501) staff       (20)      318 2023-05-21 06:04:58.000000 scorecardpipeline-0.1.4/scorecardpipeline/__init__.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    20443 2023-05-21 06:04:42.000000 scorecardpipeline-0.1.4/scorecardpipeline/excel_writer.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    19272 2023-05-21 06:42:22.000000 scorecardpipeline-0.1.4/scorecardpipeline/model.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    21517 2023-05-21 06:04:50.000000 scorecardpipeline-0.1.4/scorecardpipeline/processing.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    19966 2023-05-21 06:04:53.000000 scorecardpipeline-0.1.4/scorecardpipeline/utils.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 06:43:12.530791 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/
+-rw-r--r--   0 lubberit   (501) staff       (20)    33207 2023-05-21 06:43:12.000000 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)      380 2023-05-21 06:43:12.000000 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-21 06:43:12.000000 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)      214 2023-05-21 06:43:12.000000 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/requires.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       18 2023-05-21 06:43:12.000000 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/top_level.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-21 06:43:12.531686 scorecardpipeline-0.1.4/setup.cfg
+-rw-r--r--   0 lubberit   (501) staff       (20)     1788 2023-05-21 06:05:12.000000 scorecardpipeline-0.1.4/setup.py
```

### Comparing `scorecardpipeline-0.1.3/LICENSE` & `scorecardpipeline-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.3/setup.py` & `scorecardpipeline-0.1.4/setup.py`

 * *Files identical despite different names*

