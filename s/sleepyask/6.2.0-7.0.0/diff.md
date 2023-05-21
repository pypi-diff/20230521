# Comparing `tmp/sleepyask-6.2.0.tar.gz` & `tmp/sleepyask-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyask-6.2.0.tar", last modified: Sun May 21 08:27:51 2023, max compression
+gzip compressed data, was "sleepyask-7.0.0.tar", last modified: Sun May 21 10:08:26 2023, max compression
```

## Comparing `sleepyask-6.2.0.tar` & `sleepyask-7.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:27:51.102526 sleepyask-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 08:27:36.000000 sleepyask-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 08:27:51.102526 sleepyask-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-21 08:27:36.000000 sleepyask-6.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-21 08:27:36.000000 sleepyask-6.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 08:27:51.102526 sleepyask-6.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:27:51.098526 sleepyask-6.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:27:51.102526 sleepyask-6.2.0/src/sleepyask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:27:36.000000 sleepyask-6.2.0/src/sleepyask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-21 08:27:36.000000 sleepyask-6.2.0/src/sleepyask/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:27:51.102526 sleepyask-6.2.0/src/sleepyask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 08:27:51.000000 sleepyask-6.2.0/src/sleepyask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-21 08:27:51.000000 sleepyask-6.2.0/src/sleepyask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 08:27:51.000000 sleepyask-6.2.0/src/sleepyask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 08:27:51.000000 sleepyask-6.2.0/src/sleepyask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 08:27:51.000000 sleepyask-6.2.0/src/sleepyask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:08:26.071340 sleepyask-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 10:08:14.000000 sleepyask-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 10:08:26.071340 sleepyask-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-21 10:08:14.000000 sleepyask-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-21 10:08:14.000000 sleepyask-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 10:08:26.071340 sleepyask-7.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:08:26.067340 sleepyask-7.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:08:26.071340 sleepyask-7.0.0/src/sleepyask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:08:14.000000 sleepyask-7.0.0/src/sleepyask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-21 10:08:14.000000 sleepyask-7.0.0/src/sleepyask/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:08:26.071340 sleepyask-7.0.0/src/sleepyask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-21 10:08:26.000000 sleepyask-7.0.0/src/sleepyask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-21 10:08:26.000000 sleepyask-7.0.0/src/sleepyask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 10:08:26.000000 sleepyask-7.0.0/src/sleepyask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 10:08:26.000000 sleepyask-7.0.0/src/sleepyask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 10:08:26.000000 sleepyask-7.0.0/src/sleepyask.egg-info/top_level.txt
```

### Comparing `sleepyask-6.2.0/LICENSE` & `sleepyask-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepyask-6.2.0/PKG-INFO` & `sleepyask-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 6.2.0
+Version: 7.0.0
 Summary: A small tool for automating collecting data from ChatGPT
 Author-email: hwelsters <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/hwelsters/sleepyask
 Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sleepyask Version: 6.2.0 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 7.0.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
```

### Comparing `sleepyask-6.2.0/README.md` & `sleepyask-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sleepyask-6.2.0/pyproject.toml` & `sleepyask-7.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sleepyask"
-version = "6.2.0"
+version = "7.0.0"
 authors = [
   { name="hwelsters", email="redacted@redacted.redacted" },
 ]
 description = "A small tool for automating collecting data from ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = []
```

### Comparing `sleepyask-6.2.0/src/sleepyask.egg-info/PKG-INFO` & `sleepyask-7.0.0/src/sleepyask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 6.2.0
+Version: 7.0.0
 Summary: A small tool for automating collecting data from ChatGPT
 Author-email: hwelsters <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/hwelsters/sleepyask
 Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sleepyask Version: 6.2.0 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 7.0.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
```

