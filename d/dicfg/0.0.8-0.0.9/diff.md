# Comparing `tmp/dicfg-0.0.8.tar.gz` & `tmp/dicfg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicfg-0.0.8.tar", last modified: Fri Mar 31 19:14:03 2023, max compression
+gzip compressed data, was "dicfg-0.0.9.tar", last modified: Sat Apr  1 11:07:09 2023, max compression
```

## Comparing `dicfg-0.0.8.tar` & `dicfg-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:14:03.686510 dicfg-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 19:13:45.000000 dicfg-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-31 19:14:03.686510 dicfg-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-31 19:13:45.000000 dicfg-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:14:03.686510 dicfg-0.0.8/dicfg/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-31 19:13:45.000000 dicfg-0.0.8/dicfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 19:13:45.000000 dicfg-0.0.8/dicfg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-03-31 19:13:45.000000 dicfg-0.0.8/dicfg/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-03-31 19:13:45.000000 dicfg-0.0.8/dicfg/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-31 19:13:45.000000 dicfg-0.0.8/dicfg/magics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-03-31 19:13:45.000000 dicfg-0.0.8/dicfg/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:14:03.686510 dicfg-0.0.8/dicfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-31 19:14:03.000000 dicfg-0.0.8/dicfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-31 19:14:03.000000 dicfg-0.0.8/dicfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:14:03.000000 dicfg-0.0.8/dicfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-31 19:14:03.000000 dicfg-0.0.8/dicfg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 19:14:03.000000 dicfg-0.0.8/dicfg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-31 19:13:45.000000 dicfg-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 19:14:03.686510 dicfg-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:07:09.725642 dicfg-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-01 11:06:55.000000 dicfg-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-04-01 11:07:09.725642 dicfg-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-01 11:06:55.000000 dicfg-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:07:09.725642 dicfg-0.0.9/dicfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-01 11:06:55.000000 dicfg-0.0.9/dicfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-01 11:06:55.000000 dicfg-0.0.9/dicfg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-01 11:06:55.000000 dicfg-0.0.9/dicfg/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-01 11:06:55.000000 dicfg-0.0.9/dicfg/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-01 11:06:55.000000 dicfg-0.0.9/dicfg/magics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-01 11:06:55.000000 dicfg-0.0.9/dicfg/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:07:09.725642 dicfg-0.0.9/dicfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-04-01 11:07:09.000000 dicfg-0.0.9/dicfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-01 11:07:09.000000 dicfg-0.0.9/dicfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 11:07:09.000000 dicfg-0.0.9/dicfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-01 11:07:09.000000 dicfg-0.0.9/dicfg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-01 11:07:09.000000 dicfg-0.0.9/dicfg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-01 11:06:55.000000 dicfg-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 11:07:09.725642 dicfg-0.0.9/setup.cfg
```

### Comparing `dicfg-0.0.8/LICENSE` & `dicfg-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dicfg-0.0.8/PKG-INFO` & `dicfg-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicfg
-Version: 0.0.8
+Version: 0.0.9
 Author-email: Mart van Rijthoven <mart.vanrijthoven@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 martvanrijthoven
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,15 +40,15 @@
 
 <img src="https://raw.githubusercontent.com/martvanrijthoven/dicfg/f6639bb5788b6426133967b1929e8f4374eab78a/docs/source/_static/logo.svg" width="50%" height="50%">
 
 
 [![PyPI](https://img.shields.io/pypi/v/dicfg?color=0&label=pypi%20package)](https://pypi.org/project/dicfg/)
 [![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/dicfg)](https://anaconda.org/conda-forge/dicfg)
 [![docs](https://github.com/martvanrijthoven/dicfg/actions/workflows/docs.yml/badge.svg)](https://github.com/martvanrijthoven/dicfg/actions/workflows/docs.yml)
-[![tests](https://github.com/martvanrijthoven/dicfg/actions/workflows/tests.yml/badge.svg)](https://github.com/martvanrijthoven/dicfg/actions/workflows/tests.yml)
+[![CI Tests](https://github.com/martvanrijthoven/dicfg/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/martvanrijthoven/dicfg/actions/workflows/ci_tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/martvanrijthoven/dicfg/badge.svg?branch=main)](https://coveralls.io/github/martvanrijthoven/dicfg?branch=main)
 [![codeinspector](https://api.codiga.io/project/34959/score/svg)](https://app.codiga.io/public/project/34959/dicfg/dashboard)
 [![GitHub](https://img.shields.io/github/license/martvanrijthoven/dicfg)](https://github.com/martvanrijthoven/dicfg/blob/main/LICENSE)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dicfg)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7320310.svg)](https://doi.org/10.5281/zenodo.7320310)
 
 Dicfg is a **configuration system** that supports **dependency injection** via **object interpolation** in config files.
```

### Comparing `dicfg-0.0.8/README.md` & `dicfg-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <img src="https://raw.githubusercontent.com/martvanrijthoven/dicfg/f6639bb5788b6426133967b1929e8f4374eab78a/docs/source/_static/logo.svg" width="50%" height="50%">
 
 
 [![PyPI](https://img.shields.io/pypi/v/dicfg?color=0&label=pypi%20package)](https://pypi.org/project/dicfg/)
 [![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/dicfg)](https://anaconda.org/conda-forge/dicfg)
 [![docs](https://github.com/martvanrijthoven/dicfg/actions/workflows/docs.yml/badge.svg)](https://github.com/martvanrijthoven/dicfg/actions/workflows/docs.yml)
-[![tests](https://github.com/martvanrijthoven/dicfg/actions/workflows/tests.yml/badge.svg)](https://github.com/martvanrijthoven/dicfg/actions/workflows/tests.yml)
+[![CI Tests](https://github.com/martvanrijthoven/dicfg/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/martvanrijthoven/dicfg/actions/workflows/ci_tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/martvanrijthoven/dicfg/badge.svg?branch=main)](https://coveralls.io/github/martvanrijthoven/dicfg?branch=main)
 [![codeinspector](https://api.codiga.io/project/34959/score/svg)](https://app.codiga.io/public/project/34959/dicfg/dashboard)
 [![GitHub](https://img.shields.io/github/license/martvanrijthoven/dicfg)](https://github.com/martvanrijthoven/dicfg/blob/main/LICENSE)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dicfg)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7320310.svg)](https://doi.org/10.5281/zenodo.7320310)
 
 Dicfg is a **configuration system** that supports **dependency injection** via **object interpolation** in config files.
```

### Comparing `dicfg-0.0.8/dicfg/config.py` & `dicfg-0.0.9/dicfg/config.py`

 * *Files identical despite different names*

### Comparing `dicfg-0.0.8/dicfg/factory.py` & `dicfg-0.0.9/dicfg/factory.py`

 * *Files identical despite different names*

### Comparing `dicfg-0.0.8/dicfg/magics.py` & `dicfg-0.0.9/dicfg/magics.py`

 * *Files identical despite different names*

### Comparing `dicfg-0.0.8/dicfg/reader.py` & `dicfg-0.0.9/dicfg/reader.py`

 * *Files identical despite different names*

### Comparing `dicfg-0.0.8/dicfg.egg-info/PKG-INFO` & `dicfg-0.0.9/dicfg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicfg
-Version: 0.0.8
+Version: 0.0.9
 Author-email: Mart van Rijthoven <mart.vanrijthoven@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 martvanrijthoven
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,15 +40,15 @@
 
 <img src="https://raw.githubusercontent.com/martvanrijthoven/dicfg/f6639bb5788b6426133967b1929e8f4374eab78a/docs/source/_static/logo.svg" width="50%" height="50%">
 
 
 [![PyPI](https://img.shields.io/pypi/v/dicfg?color=0&label=pypi%20package)](https://pypi.org/project/dicfg/)
 [![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/dicfg)](https://anaconda.org/conda-forge/dicfg)
 [![docs](https://github.com/martvanrijthoven/dicfg/actions/workflows/docs.yml/badge.svg)](https://github.com/martvanrijthoven/dicfg/actions/workflows/docs.yml)
-[![tests](https://github.com/martvanrijthoven/dicfg/actions/workflows/tests.yml/badge.svg)](https://github.com/martvanrijthoven/dicfg/actions/workflows/tests.yml)
+[![CI Tests](https://github.com/martvanrijthoven/dicfg/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/martvanrijthoven/dicfg/actions/workflows/ci_tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/martvanrijthoven/dicfg/badge.svg?branch=main)](https://coveralls.io/github/martvanrijthoven/dicfg?branch=main)
 [![codeinspector](https://api.codiga.io/project/34959/score/svg)](https://app.codiga.io/public/project/34959/dicfg/dashboard)
 [![GitHub](https://img.shields.io/github/license/martvanrijthoven/dicfg)](https://github.com/martvanrijthoven/dicfg/blob/main/LICENSE)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dicfg)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7320310.svg)](https://doi.org/10.5281/zenodo.7320310)
 
 Dicfg is a **configuration system** that supports **dependency injection** via **object interpolation** in config files.
```

### Comparing `dicfg-0.0.8/pyproject.toml` & `dicfg-0.0.9/pyproject.toml`

 * *Files identical despite different names*

