# Comparing `tmp/amplitude-data-wrapper-0.4.0.tar.gz` & `tmp/amplitude-data-wrapper-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amplitude-data-wrapper-0.4.0.tar", last modified: Sun May 21 17:33:59 2023, max compression
+gzip compressed data, was "amplitude-data-wrapper-0.4.1.tar", last modified: Sun May 21 20:30:51 2023, max compression
```

## Comparing `amplitude-data-wrapper-0.4.0.tar` & `amplitude-data-wrapper-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 17:33:59.746005 amplitude-data-wrapper-0.4.0/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      111 2023-05-21 17:18:42.000000 amplitude-data-wrapper-0.4.0/.gitignore
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.0/CODEOWNERS
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.0/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5925 2023-05-21 17:33:59.744967 amplitude-data-wrapper-0.4.0/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4322 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.0/README.md
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 17:33:59.737775 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       51 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/__init__.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 17:33:59.743093 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5925 2023-05-21 17:33:59.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      416 2023-05-21 17:33:59.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 17:33:59.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 17:33:59.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/top_level.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)    15281 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/analytics_api.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2295 2023-05-21 17:25:27.000000 amplitude-data-wrapper-0.4.0/example.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      613 2023-05-21 17:33:47.000000 amplitude-data-wrapper-0.4.0/pyproject.toml
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-05-21 17:33:59.746207 amplitude-data-wrapper-0.4.0/setup.cfg
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:30:51.561487 amplitude-data-wrapper-0.4.1/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      130 2023-05-21 17:43:48.000000 amplitude-data-wrapper-0.4.1/.gitignore
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.1/CODEOWNERS
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.1/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      820 2023-05-21 20:22:43.000000 amplitude-data-wrapper-0.4.1/Makefile
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5925 2023-05-21 20:30:51.560445 amplitude-data-wrapper-0.4.1/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4322 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.1/README.md
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:30:51.543777 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       51 2023-05-21 19:02:17.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/__init__.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:30:51.552338 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5925 2023-05-21 20:30:51.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      577 2023-05-21 20:30:51.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 20:30:51.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       99 2023-05-21 20:30:51.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/requires.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 20:30:51.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)    15281 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/analytics_api.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2295 2023-05-21 17:25:27.000000 amplitude-data-wrapper-0.4.1/example.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      773 2023-05-21 20:29:57.000000 amplitude-data-wrapper-0.4.1/pyproject.toml
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:30:51.558812 amplitude-data-wrapper-0.4.1/requirements/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       43 2023-05-21 17:43:48.000000 amplitude-data-wrapper-0.4.1/requirements/dev.in
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2831 2023-05-21 20:20:58.000000 amplitude-data-wrapper-0.4.1/requirements/dev.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       13 2023-05-21 17:43:48.000000 amplitude-data-wrapper-0.4.1/requirements/main.in
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      412 2023-05-21 20:20:52.000000 amplitude-data-wrapper-0.4.1/requirements/main.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-05-21 20:30:51.561678 amplitude-data-wrapper-0.4.1/setup.cfg
```

### Comparing `amplitude-data-wrapper-0.4.0/LICENSE` & `amplitude-data-wrapper-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.0/PKG-INFO` & `amplitude-data-wrapper-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplitude-data-wrapper
-Version: 0.4.0
+Version: 0.4.1
 Summary: python wrapper for using the amplitude analytics and taxonomy APIs
 Author-email: Tobias McVey <tobias.mcvey@nav.no>
 License: MIT License
         
         Copyright (c) 2022 NAV IT
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `amplitude-data-wrapper-0.4.0/README.md` & `amplitude-data-wrapper-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/PKG-INFO` & `amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplitude-data-wrapper
-Version: 0.4.0
+Version: 0.4.1
 Summary: python wrapper for using the amplitude analytics and taxonomy APIs
 Author-email: Tobias McVey <tobias.mcvey@nav.no>
 License: MIT License
         
         Copyright (c) 2022 NAV IT
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/analytics_api.py` & `amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/analytics_api.py`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.0/example.py` & `amplitude-data-wrapper-0.4.1/example.py`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.0/pyproject.toml` & `amplitude-data-wrapper-0.4.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 [project]
 name = "amplitude-data-wrapper"
-version = "0.4.0"
+version = "0.4.1"
 description = "python wrapper for using the amplitude analytics and taxonomy APIs"
 authors = [
     {name = "Tobias McVey", email = "tobias.mcvey@nav.no"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["amplitude"]
 license = {file = "LICENSE"}
 
+dependencies = [
+    "certifi==2023.5.7",
+    "charset-normalizer==3.1.0",
+    "idna==3.4",
+    "requests==2.30.0",
+    "tqdm==4.65.0",
+    "urllib3==2.0.2"
+]
+
 [project.urls]
 "Homepage" = "https://github.com/navikt/amplitude-data-wrapper"
 
 [tool.setuptools.packages.find]
 where = ["amplitude_data_wrapper"]
 exclude = ["tests", "testing", "requirements"]
```

