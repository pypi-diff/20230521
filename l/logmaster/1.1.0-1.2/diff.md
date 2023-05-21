# Comparing `tmp/logmaster-1.1.0.tar.gz` & `tmp/logmaster-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logmaster-1.1.0.tar", last modified: Sun May 14 15:07:23 2023, max compression
+gzip compressed data, was "logmaster-1.2.tar", last modified: Sun May 21 18:07:36 2023, max compression
```

## Comparing `logmaster-1.1.0.tar` & `logmaster-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 15:07:23.174199 logmaster-1.1.0/
--rw-rw-rw-   0        0        0     1083 2023-05-08 22:14:25.000000 logmaster-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1336 2023-05-14 15:07:23.175197 logmaster-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2023-05-11 15:57:31.000000 logmaster-1.1.0/README.md
--rw-rw-rw-   0        0        0      109 2023-05-09 16:02:47.000000 logmaster-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      432 2023-05-14 15:07:23.179201 logmaster-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 15:07:23.060199 logmaster-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 15:07:23.085201 logmaster-1.1.0/src/logmaster/
--rw-rw-rw-   0        0        0      993 2023-05-14 14:45:28.000000 logmaster-1.1.0/src/logmaster/__init__.py
--rw-rw-rw-   0        0        0       73 2023-05-14 15:04:18.000000 logmaster-1.1.0/src/logmaster/errors.py
--rw-rw-rw-   0        0        0     1901 2023-05-14 15:04:31.000000 logmaster-1.1.0/src/logmaster/logger.py
-drwxrwxrwx   0        0        0        0 2023-05-14 15:07:23.172198 logmaster-1.1.0/src/logmaster.egg-info/
--rw-rw-rw-   0        0        0     1336 2023-05-14 15:07:23.000000 logmaster-1.1.0/src/logmaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-14 15:07:23.000000 logmaster-1.1.0/src/logmaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 15:07:23.000000 logmaster-1.1.0/src/logmaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 15:07:23.000000 logmaster-1.1.0/src/logmaster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 18:07:36.857575 logmaster-1.2/
+-rw-rw-rw-   0        0        0     1083 2023-05-08 22:14:25.000000 logmaster-1.2/LICENSE
+-rw-rw-rw-   0        0        0     1337 2023-05-21 18:07:36.865564 logmaster-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1034 2023-05-21 14:11:16.000000 logmaster-1.2/README.md
+-rw-rw-rw-   0        0        0      109 2023-05-09 16:02:47.000000 logmaster-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      430 2023-05-21 18:07:36.873599 logmaster-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 18:07:36.769567 logmaster-1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 18:07:36.825569 logmaster-1.2/src/logmaster/
+-rw-rw-rw-   0        0        0      993 2023-05-14 14:45:28.000000 logmaster-1.2/src/logmaster/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-05-14 15:04:18.000000 logmaster-1.2/src/logmaster/errors.py
+-rw-rw-rw-   0        0        0     1938 2023-05-21 18:05:34.000000 logmaster-1.2/src/logmaster/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-21 18:07:36.857575 logmaster-1.2/src/logmaster.egg-info/
+-rw-rw-rw-   0        0        0     1337 2023-05-21 18:07:36.000000 logmaster-1.2/src/logmaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-21 18:07:36.000000 logmaster-1.2/src/logmaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 18:07:36.000000 logmaster-1.2/src/logmaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-21 18:07:36.000000 logmaster-1.2/src/logmaster.egg-info/top_level.txt
```

### Comparing `logmaster-1.1.0/LICENSE` & `logmaster-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logmaster-1.1.0/PKG-INFO` & `logmaster-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: logmaster
-Version: 1.1.0
+Version: 1.2
 Summary: A simple logging library for Python
 Home-page: https://github.com/W1L7dev/logmaster
 Author: W1L7dev
 Author-email: w1l7dev@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Logmaster
-## A simple logging package for
-
-
+## A simple logging package for Python
 ---
 
 ### Installation
 ```bash
 pip install logmaster
 ```
 > note: this package is not yet on PyPI, so you will have to install it from source.
```

### Comparing `logmaster-1.1.0/README.md` & `logmaster-1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Logmaster
-## A simple logging package for
-
-
+## A simple logging package for Python
 ---
 
 ### Installation
 ```bash
 pip install logmaster
 ```
 > note: this package is not yet on PyPI, so you will have to install it from source.
```

### Comparing `logmaster-1.1.0/src/logmaster/__init__.py` & `logmaster-1.2/src/logmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `logmaster-1.1.0/src/logmaster.egg-info/PKG-INFO` & `logmaster-1.2/src/logmaster.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: logmaster
-Version: 1.1.0
+Version: 1.2
 Summary: A simple logging library for Python
 Home-page: https://github.com/W1L7dev/logmaster
 Author: W1L7dev
 Author-email: w1l7dev@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Logmaster
-## A simple logging package for
-
-
+## A simple logging package for Python
 ---
 
 ### Installation
 ```bash
 pip install logmaster
 ```
 > note: this package is not yet on PyPI, so you will have to install it from source.
```

