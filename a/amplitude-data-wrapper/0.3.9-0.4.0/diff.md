# Comparing `tmp/amplitude_data_wrapper-0.3.9.tar.gz` & `tmp/amplitude-data-wrapper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amplitude_data_wrapper-0.3.9.tar", max compression
+gzip compressed data, was "amplitude-data-wrapper-0.4.0.tar", last modified: Sun May 21 17:33:59 2023, max compression
```

## Comparing `amplitude_data_wrapper-0.3.9.tar` & `amplitude-data-wrapper-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,17 @@
--rw-r--r--   0        0        0     1062 2022-08-16 12:59:05.385355 amplitude_data_wrapper-0.3.9/LICENSE
--rw-r--r--   0        0        0     4322 2022-08-16 12:31:25.379733 amplitude_data_wrapper-0.3.9/README.md
--rw-r--r--   0        0        0       51 2022-08-16 12:31:25.380519 amplitude_data_wrapper-0.3.9/amplitude_data_wrapper/__init__.py
--rw-r--r--   0        0        0    15281 2022-08-16 18:48:41.479058 amplitude_data_wrapper-0.3.9/amplitude_data_wrapper/analytics_api.py
--rw-r--r--   0        0        0      842 2023-05-09 10:05:32.345651 amplitude_data_wrapper-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     5214 1970-01-01 00:00:00.000000 amplitude_data_wrapper-0.3.9/PKG-INFO
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 17:33:59.746005 amplitude-data-wrapper-0.4.0/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      111 2023-05-21 17:18:42.000000 amplitude-data-wrapper-0.4.0/.gitignore
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.0/CODEOWNERS
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.0/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5925 2023-05-21 17:33:59.744967 amplitude-data-wrapper-0.4.0/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4322 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.0/README.md
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 17:33:59.737775 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       51 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/__init__.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 17:33:59.743093 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5925 2023-05-21 17:33:59.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      416 2023-05-21 17:33:59.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 17:33:59.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 17:33:59.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)    15281 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/analytics_api.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2295 2023-05-21 17:25:27.000000 amplitude-data-wrapper-0.4.0/example.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      613 2023-05-21 17:33:47.000000 amplitude-data-wrapper-0.4.0/pyproject.toml
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-05-21 17:33:59.746207 amplitude-data-wrapper-0.4.0/setup.cfg
```

### Comparing `amplitude_data_wrapper-0.3.9/LICENSE` & `amplitude-data-wrapper-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amplitude_data_wrapper-0.3.9/README.md` & `amplitude-data-wrapper-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `amplitude_data_wrapper-0.3.9/amplitude_data_wrapper/analytics_api.py` & `amplitude-data-wrapper-0.4.0/amplitude_data_wrapper/analytics_api.py`

 * *Files identical despite different names*

### Comparing `amplitude_data_wrapper-0.3.9/PKG-INFO` & `amplitude-data-wrapper-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 Metadata-Version: 2.1
 Name: amplitude-data-wrapper
-Version: 0.3.9
+Version: 0.4.0
 Summary: python wrapper for using the amplitude analytics and taxonomy APIs
-Home-page: https://github.com/navikt/amplitude-data-wrapper
-License: MIT
+Author-email: Tobias McVey <tobias.mcvey@nav.no>
+License: MIT License
+        
+        Copyright (c) 2022 NAV IT
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/navikt/amplitude-data-wrapper
 Keywords: amplitude
-Author: Tobias McVey
-Author-email: tobias.mcvey@nav.no
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: tqdm (>=4.62.3,<5.0.0)
-Project-URL: Documentation, https://github.com/navikt/amplitude-data-wrapper
-Project-URL: Repository, https://github.com/navikt/amplitude-data-wrapper
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Amplitude data wrapper
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is a wrapper for [Amplitude](https://amplitude.com/) APIs. You can use it to query and export data from your account and use the taxonomy API.
```

