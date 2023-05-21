# Comparing `tmp/hotjar-data-wrapper-0.1.0.tar.gz` & `tmp/hotjar-data-wrapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotjar-data-wrapper-0.1.0.tar", max compression
+gzip compressed data, was "hotjar-data-wrapper-0.1.1.tar", last modified: Sun May 21 18:21:33 2023, max compression
```

## Comparing `hotjar-data-wrapper-0.1.0.tar` & `hotjar-data-wrapper-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,17 @@
--rw-r--r--   0        0        0     1062 2022-08-19 12:53:33.913477 hotjar-data-wrapper-0.1.0/LICENSE
--rw-r--r--   0        0        0     1517 2022-08-29 08:01:44.386968 hotjar-data-wrapper-0.1.0/README.md
--rw-r--r--   0        0        0       45 2022-08-19 13:01:48.170562 hotjar-data-wrapper-0.1.0/hotjar_data_wrapper/__init__.py
--rw-r--r--   0        0        0     6077 2022-08-29 07:23:42.945454 hotjar-data-wrapper-0.1.0/hotjar_data_wrapper/hotjar_api.py
--rw-r--r--   0        0        0      683 2022-08-29 08:56:18.194498 hotjar-data-wrapper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2277 2022-08-29 08:57:14.552924 hotjar-data-wrapper-0.1.0/setup.py
--rw-r--r--   0        0        0     2308 2022-08-29 08:57:14.553289 hotjar-data-wrapper-0.1.0/PKG-INFO
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 18:21:33.788039 hotjar-data-wrapper-0.1.1/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       86 2023-05-21 18:20:35.000000 hotjar-data-wrapper-0.1.1/.gitignore
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.1/CODEOWNERS
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.1/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3076 2023-05-21 18:21:33.786965 hotjar-data-wrapper-0.1.1/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1517 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.1/README.md
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      981 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.1/example.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 18:21:33.780109 hotjar-data-wrapper-0.1.1/hotjar_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       45 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.1/hotjar_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     6077 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.1/hotjar_data_wrapper/hotjar_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 18:21:33.785486 hotjar-data-wrapper-0.1.1/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3076 2023-05-21 18:21:33.000000 hotjar-data-wrapper-0.1.1/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      383 2023-05-21 18:21:33.000000 hotjar-data-wrapper-0.1.1/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 18:21:33.000000 hotjar-data-wrapper-0.1.1/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 18:21:33.000000 hotjar-data-wrapper-0.1.1/hotjar_data_wrapper/hotjar_data_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      566 2023-05-21 18:18:54.000000 hotjar-data-wrapper-0.1.1/pyproject.toml
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-05-21 18:21:33.788277 hotjar-data-wrapper-0.1.1/setup.cfg
```

### Comparing `hotjar-data-wrapper-0.1.0/LICENSE` & `hotjar-data-wrapper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hotjar-data-wrapper-0.1.0/README.md` & `hotjar-data-wrapper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hotjar-data-wrapper-0.1.0/hotjar_data_wrapper/hotjar_api.py` & `hotjar-data-wrapper-0.1.1/hotjar_data_wrapper/hotjar_api.py`

 * *Files identical despite different names*

### Comparing `hotjar-data-wrapper-0.1.0/pyproject.toml` & `hotjar-data-wrapper-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-[tool.poetry]
+[project]
 name = "hotjar-data-wrapper"
-version = "0.1.0"
+version = "0.1.1"
 description = "a wrapper for using Hotjar APIs"
-authors = ["Tobias McVey <tobias.mcvey@nav.no>"]
-license = "MIT"
-readme="README.md"
-homepage = "https://github.com/navikt/hotjar-data-wrapper"
-repository = "https://github.com/navikt/hotjar-data-wrapper"
-documentation = "https://github.com/navikt/hotjar-data-wrapper"
+authors = [
+    {name = "Tobias McVey", email = "tobias.mcvey@nav.no"},
+]
+readme = "README.md"
+requires-python = ">=3.10"
+keywords = ["hotjar"]
+license = {file = "LICENSE"}
 
-keywords = ["Hotjar"]
+[project.urls]
+"Homepage" = "https://github.com/navikt/hotjar-data-wrapper"
 
-[tool.poetry.dependencies]
-python = "^3.8"
-requests = "^2.28.1"
-tqdm = "^4.64.0"
-
-[tool.poetry.dev-dependencies]
-ipykernel = "^6.15.1"
-black = "^22.6.0"
-twine = "^4.0.1"
-keyring = "^23.8.2"
+[tool.setuptools.packages.find]
+where = ["hotjar_data_wrapper"]
+exclude = ["tests", "testing", "requirements"]
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
```

### Comparing `hotjar-data-wrapper-0.1.0/PKG-INFO` & `hotjar-data-wrapper-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 Metadata-Version: 2.1
 Name: hotjar-data-wrapper
-Version: 0.1.0
+Version: 0.1.1
 Summary: a wrapper for using Hotjar APIs
-Home-page: https://github.com/navikt/hotjar-data-wrapper
-License: MIT
-Keywords: Hotjar
-Author: Tobias McVey
-Author-email: tobias.mcvey@nav.no
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: tqdm (>=4.64.0,<5.0.0)
-Project-URL: Documentation, https://github.com/navikt/hotjar-data-wrapper
-Project-URL: Repository, https://github.com/navikt/hotjar-data-wrapper
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
+Project-URL: Homepage, https://github.com/navikt/hotjar-data-wrapper
+Keywords: hotjar
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Hotjar Data Wrapper
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is a wrapper for Hotjar APIs to let you login and download survey data and metadata for your account.
```

