# Comparing `tmp/digital-experiments-1.2.1.tar.gz` & `tmp/digital-experiments-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-experiments-1.2.1.tar", last modified: Sat May 20 11:20:12 2023, max compression
+gzip compressed data, was "digital-experiments-1.2.7.tar", last modified: Sun May 21 07:15:59 2023, max compression
```

## Comparing `digital-experiments-1.2.1.tar` & `digital-experiments-1.2.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-20 11:20:12.390848 digital-experiments-1.2.1/
--rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.2.1/LICENSE
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-20 11:20:12.390711 digital-experiments-1.2.1/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.2.1/README.md
--rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-20 11:19:56.000000 digital-experiments-1.2.1/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-05-20 11:20:12.390897 digital-experiments-1.2.1/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-20 11:20:12.383761 digital-experiments-1.2.1/src/
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-20 11:20:12.386469 digital-experiments-1.2.1/src/digital_experiments/
--rw-r--r--   0 john       (504) staff       (20)      138 2023-05-20 11:19:56.000000 digital-experiments-1.2.1/src/digital_experiments/__init__.py
--rw-r--r--   0 john       (504) staff       (20)     1758 2023-05-18 14:04:48.000000 digital-experiments-1.2.1/src/digital_experiments/automate.py
--rw-r--r--   0 john       (504) staff       (20)     6877 2023-05-17 15:48:49.000000 digital-experiments-1.2.1/src/digital_experiments/backends.py
--rw-r--r--   0 john       (504) staff       (20)     2649 2023-05-17 16:01:39.000000 digital-experiments-1.2.1/src/digital_experiments/control_center.py
--rw-r--r--   0 john       (504) staff       (20)     6065 2023-05-19 06:41:38.000000 digital-experiments-1.2.1/src/digital_experiments/data.py
--rw-r--r--   0 john       (504) staff       (20)     4377 2023-05-17 15:50:20.000000 digital-experiments-1.2.1/src/digital_experiments/experiment.py
--rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.2.1/src/digital_experiments/inspection.py
--rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.2.1/src/digital_experiments/observation.py
--rw-r--r--   0 john       (504) staff       (20)      735 2023-05-10 08:20:22.000000 digital-experiments-1.2.1/src/digital_experiments/pretty.py
--rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.2.1/src/digital_experiments/querying.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-20 11:20:12.387863 digital-experiments-1.2.1/src/digital_experiments/search/
--rw-r--r--   0 john       (504) staff       (20)     3354 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/src/digital_experiments/search/distributions.py
--rw-r--r--   0 john       (504) staff       (20)     2896 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/src/digital_experiments/search/skopt_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     2245 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/src/digital_experiments/search/space.py
--rw-r--r--   0 john       (504) staff       (20)     5756 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/src/digital_experiments/search/suggest.py
--rw-r--r--   0 john       (504) staff       (20)     1682 2023-05-17 15:42:42.000000 digital-experiments-1.2.1/src/digital_experiments/timing.py
--rw-r--r--   0 john       (504) staff       (20)     5440 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/src/digital_experiments/util.py
--rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.2.1/src/digital_experiments/version_control.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-20 11:20:12.387261 digital-experiments-1.2.1/src/digital_experiments.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-20 11:20:12.000000 digital-experiments-1.2.1/src/digital_experiments.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1274 2023-05-20 11:20:12.000000 digital-experiments-1.2.1/src/digital_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-05-20 11:20:12.000000 digital-experiments-1.2.1/src/digital_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)      160 2023-05-20 11:20:12.000000 digital-experiments-1.2.1/src/digital_experiments.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)       20 2023-05-20 11:20:12.000000 digital-experiments-1.2.1/src/digital_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-20 11:20:12.390504 digital-experiments-1.2.1/tests/
--rw-r--r--   0 john       (504) staff       (20)      482 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/tests/test_automate.py
--rw-r--r--   0 john       (504) staff       (20)     2135 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/tests/test_backends.py
--rw-r--r--   0 john       (504) staff       (20)     1122 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/tests/test_control_center.py
--rw-r--r--   0 john       (504) staff       (20)     2384 2023-05-19 15:35:33.000000 digital-experiments-1.2.1/tests/test_data.py
--rw-r--r--   0 john       (504) staff       (20)     1395 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/tests/test_distributions.py
--rw-r--r--   0 john       (504) staff       (20)     2099 2023-05-17 11:01:07.000000 digital-experiments-1.2.1/tests/test_experiment.py
--rw-r--r--   0 john       (504) staff       (20)      391 2023-05-17 11:01:07.000000 digital-experiments-1.2.1/tests/test_inspection.py
--rw-r--r--   0 john       (504) staff       (20)      309 2023-05-17 11:01:07.000000 digital-experiments-1.2.1/tests/test_observation.py
--rw-r--r--   0 john       (504) staff       (20)      613 2023-05-10 08:20:22.000000 digital-experiments-1.2.1/tests/test_pretty.py
--rw-r--r--   0 john       (504) staff       (20)     1912 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/tests/test_querying.py
--rw-r--r--   0 john       (504) staff       (20)      712 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/tests/test_space.py
--rw-r--r--   0 john       (504) staff       (20)     3179 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/tests/test_suggest.py
--rw-r--r--   0 john       (504) staff       (20)      682 2023-05-17 15:42:42.000000 digital-experiments-1.2.1/tests/test_timing.py
--rw-r--r--   0 john       (504) staff       (20)     2820 2023-05-17 15:42:42.000000 digital-experiments-1.2.1/tests/test_util.py
--rw-r--r--   0 john       (504) staff       (20)     2830 2023-05-18 14:04:45.000000 digital-experiments-1.2.1/tests/test_version_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:15:59.197177 digital-experiments-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-21 07:15:59.197177 digital-experiments-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 07:15:59.197177 digital-experiments-1.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:15:59.193177 digital-experiments-1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:15:59.193177 digital-experiments-1.2.7/src/digital_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/control_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/querying.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:15:59.193177 digital-experiments-1.2.7/src/digital_experiments/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/search/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/search/skopt_suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/search/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/search/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/src/digital_experiments/version_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:15:59.193177 digital-experiments-1.2.7/src/digital_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-21 07:15:59.000000 digital-experiments-1.2.7/src/digital_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-21 07:15:59.000000 digital-experiments-1.2.7/src/digital_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 07:15:59.000000 digital-experiments-1.2.7/src/digital_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-21 07:15:59.000000 digital-experiments-1.2.7/src/digital_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 07:15:59.000000 digital-experiments-1.2.7/src/digital_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:15:59.197177 digital-experiments-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_control_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_querying.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-21 07:15:16.000000 digital-experiments-1.2.7/tests/test_version_control.py
```

### Comparing `digital-experiments-1.2.1/LICENSE` & `digital-experiments-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/PKG-INFO` & `digital-experiments-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.2.1
+Version: 1.2.7
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -14,14 +14,15 @@
 Keywords: config,experiments,optimisation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: publish
 License-File: LICENSE
 
 <div align="center">
 <img src="docs/source/logo.svg" width="50%">
 </div>
 
 ---
```

### Comparing `digital-experiments-1.2.1/README.md` & `digital-experiments-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/pyproject.toml` & `digital-experiments-1.2.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digital-experiments"
-version = "1.2.1"
+version = "1.2.7"
 description = "Keep track of digital experiments."
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -36,20 +36,21 @@
     "sphinx",
     "furo",
     "nbsphinx",
     "seedir",
     "emoji",
     "pytest-cov",
 ]
+publish = ["build", "twine"]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/digital-experiments"
 
 [tool.bumpver]
-current_version = "1.2.1"
+current_version = "1.2.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digital-experiments-1.2.1/src/digital_experiments/automate.py` & `digital-experiments-1.2.7/src/digital_experiments/automate.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/backends.py` & `digital-experiments-1.2.7/src/digital_experiments/backends.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/control_center.py` & `digital-experiments-1.2.7/src/digital_experiments/control_center.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/data.py` & `digital-experiments-1.2.7/src/digital_experiments/data.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/experiment.py` & `digital-experiments-1.2.7/src/digital_experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/observation.py` & `digital-experiments-1.2.7/src/digital_experiments/observation.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/pretty.py` & `digital-experiments-1.2.7/src/digital_experiments/pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/querying.py` & `digital-experiments-1.2.7/src/digital_experiments/querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/search/distributions.py` & `digital-experiments-1.2.7/src/digital_experiments/search/distributions.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/search/skopt_suggest.py` & `digital-experiments-1.2.7/src/digital_experiments/search/skopt_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/search/space.py` & `digital-experiments-1.2.7/src/digital_experiments/search/space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/search/suggest.py` & `digital-experiments-1.2.7/src/digital_experiments/search/suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/timing.py` & `digital-experiments-1.2.7/src/digital_experiments/timing.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/util.py` & `digital-experiments-1.2.7/src/digital_experiments/util.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments/version_control.py` & `digital-experiments-1.2.7/src/digital_experiments/version_control.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/src/digital_experiments.egg-info/PKG-INFO` & `digital-experiments-1.2.7/src/digital_experiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.2.1
+Version: 1.2.7
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -14,14 +14,15 @@
 Keywords: config,experiments,optimisation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: publish
 License-File: LICENSE
 
 <div align="center">
 <img src="docs/source/logo.svg" width="50%">
 </div>
 
 ---
```

### Comparing `digital-experiments-1.2.1/src/digital_experiments.egg-info/SOURCES.txt` & `digital-experiments-1.2.7/src/digital_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_backends.py` & `digital-experiments-1.2.7/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_control_center.py` & `digital-experiments-1.2.7/tests/test_control_center.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_data.py` & `digital-experiments-1.2.7/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_distributions.py` & `digital-experiments-1.2.7/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_experiment.py` & `digital-experiments-1.2.7/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_pretty.py` & `digital-experiments-1.2.7/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_querying.py` & `digital-experiments-1.2.7/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_space.py` & `digital-experiments-1.2.7/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_suggest.py` & `digital-experiments-1.2.7/tests/test_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_timing.py` & `digital-experiments-1.2.7/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_util.py` & `digital-experiments-1.2.7/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.2.1/tests/test_version_control.py` & `digital-experiments-1.2.7/tests/test_version_control.py`

 * *Files identical despite different names*

