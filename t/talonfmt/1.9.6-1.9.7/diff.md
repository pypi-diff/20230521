# Comparing `tmp/talonfmt-1.9.6.tar.gz` & `tmp/talonfmt-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talonfmt-1.9.6.tar", last modified: Thu May 18 12:11:12 2023, max compression
+gzip compressed data, was "talonfmt-1.9.7.tar", last modified: Thu May 18 12:12:48 2023, max compression
```

## Comparing `talonfmt-1.9.6.tar` & `talonfmt-1.9.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:12.725077 talonfmt-1.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 12:10:53.000000 talonfmt-1.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-18 12:11:12.725077 talonfmt-1.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-18 12:10:53.000000 talonfmt-1.9.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-18 12:10:53.000000 talonfmt-1.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:11:12.725077 talonfmt-1.9.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:12.725077 talonfmt-1.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:12.725077 talonfmt-1.9.6/src/talonfmt/
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-18 12:10:53.000000 talonfmt-1.9.6/src/talonfmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 12:10:53.000000 talonfmt-1.9.6/src/talonfmt/assert_equivalent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-18 12:10:53.000000 talonfmt-1.9.6/src/talonfmt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-18 12:10:53.000000 talonfmt-1.9.6/src/talonfmt/editorconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-05-18 12:10:53.000000 talonfmt-1.9.6/src/talonfmt/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:12.725077 talonfmt-1.9.6/src/talonfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:12.725077 talonfmt-1.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-18 12:10:53.000000 talonfmt-1.9.6/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-18 12:10:53.000000 talonfmt-1.9.6/tests/test_smart1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-18 12:10:53.000000 talonfmt-1.9.6/tests/test_smart80.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:12:48.278617 talonfmt-1.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 12:12:28.000000 talonfmt-1.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-18 12:12:48.278617 talonfmt-1.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-18 12:12:28.000000 talonfmt-1.9.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-18 12:12:28.000000 talonfmt-1.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:12:48.278617 talonfmt-1.9.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:12:48.278617 talonfmt-1.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:12:48.278617 talonfmt-1.9.7/src/talonfmt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-18 12:12:28.000000 talonfmt-1.9.7/src/talonfmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 12:12:28.000000 talonfmt-1.9.7/src/talonfmt/assert_equivalent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-18 12:12:28.000000 talonfmt-1.9.7/src/talonfmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-18 12:12:28.000000 talonfmt-1.9.7/src/talonfmt/editorconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-05-18 12:12:28.000000 talonfmt-1.9.7/src/talonfmt/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:12:48.278617 talonfmt-1.9.7/src/talonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-18 12:12:48.000000 talonfmt-1.9.7/src/talonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-18 12:12:48.000000 talonfmt-1.9.7/src/talonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:12:48.000000 talonfmt-1.9.7/src/talonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 12:12:48.000000 talonfmt-1.9.7/src/talonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-18 12:12:48.000000 talonfmt-1.9.7/src/talonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 12:12:48.000000 talonfmt-1.9.7/src/talonfmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:12:48.278617 talonfmt-1.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-18 12:12:28.000000 talonfmt-1.9.7/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-18 12:12:28.000000 talonfmt-1.9.7/tests/test_smart1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-18 12:12:28.000000 talonfmt-1.9.7/tests/test_smart80.py
```

### Comparing `talonfmt-1.9.6/LICENSE` & `talonfmt-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.6/PKG-INFO` & `talonfmt-1.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talonfmt
-Version: 1.9.6
+Version: 1.9.7
 Summary: A code formatter for Talon files
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2022 Wen Kokke
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,13 +36,13 @@
 Description-Content-Type: text/markdown
 Provides-Extra: mypy
 Provides-Extra: test
 License-File: LICENSE
 
 ![PyPI](https://img.shields.io/pypi/v/talonfmt)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/wenkokke/talonfmt)
-![GitHub Workflow Status](https://github.com/wenkokke/talonfmt/actions/workflows/build.yml/badge.svg)
+![GitHub Workflow Status](https://github.com/wenkokke/talonfmt/actions/workflows/ci.yml/badge.svg)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/wenkokke/talonfmt/dev.svg)](https://results.pre-commit.ci/latest/github/wenkokke/talonfmt/dev)
 
 # talonfmt
 
 Code formatter for Talon files.
```

### Comparing `talonfmt-1.9.6/pyproject.toml` & `talonfmt-1.9.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talonfmt"
-version = "1.9.6"
+version = "1.9.7"
 description = "A code formatter for Talon files"
 license = { file = 'LICENSE' }
 authors = [{ name = "Wen Kokke", email = "wenkokke@users.noreply.github.com" }]
 readme = "README.md"
 keywords = ["talon", "formatter"]
 classifiers = [
   "License :: OSI Approved :: MIT License",
@@ -37,15 +37,15 @@
   "pytest_benchmark >=3.4.1,<5.0.0"
 ]
 
 [project.scripts]
 talondoc = "talonfmt.cli:cli"
 
 [tool.bumpver]
-current_version = "1.9.6"
+current_version = "1.9.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `talonfmt-1.9.6/src/talonfmt/__init__.py` & `talonfmt-1.9.7/src/talonfmt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from doc_printer import DocRenderer, SimpleDocRenderer, SimpleLayout, SmartDocRenderer
 from tree_sitter_talon import Node, parse
 
 from .editorconfig import get_indent_size, get_max_line_length
 from .formatter import EmptyMatchContext, TalonFormatter
 
-__version__: str = "1.9.6"
+__version__: str = "1.9.7"
 
 
 def talonfmt(
     contents: Union[str, bytes, Node],
     *,
     filename: Optional[str] = None,
     encoding: str = "utf-8",
```

### Comparing `talonfmt-1.9.6/src/talonfmt/assert_equivalent.py` & `talonfmt-1.9.7/src/talonfmt/assert_equivalent.py`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.6/src/talonfmt/cli.py` & `talonfmt-1.9.7/src/talonfmt/cli.py`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.6/src/talonfmt/editorconfig.py` & `talonfmt-1.9.7/src/talonfmt/editorconfig.py`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.6/src/talonfmt/formatter.py` & `talonfmt-1.9.7/src/talonfmt/formatter.py`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.6/src/talonfmt.egg-info/PKG-INFO` & `talonfmt-1.9.7/src/talonfmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talonfmt
-Version: 1.9.6
+Version: 1.9.7
 Summary: A code formatter for Talon files
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2022 Wen Kokke
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,13 +36,13 @@
 Description-Content-Type: text/markdown
 Provides-Extra: mypy
 Provides-Extra: test
 License-File: LICENSE
 
 ![PyPI](https://img.shields.io/pypi/v/talonfmt)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/wenkokke/talonfmt)
-![GitHub Workflow Status](https://github.com/wenkokke/talonfmt/actions/workflows/build.yml/badge.svg)
+![GitHub Workflow Status](https://github.com/wenkokke/talonfmt/actions/workflows/ci.yml/badge.svg)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/wenkokke/talonfmt/dev.svg)](https://results.pre-commit.ci/latest/github/wenkokke/talonfmt/dev)
 
 # talonfmt
 
 Code formatter for Talon files.
```

### Comparing `talonfmt-1.9.6/tests/test_simple.py` & `talonfmt-1.9.7/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.6/tests/test_smart1k.py` & `talonfmt-1.9.7/tests/test_smart1k.py`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.6/tests/test_smart80.py` & `talonfmt-1.9.7/tests/test_smart80.py`

 * *Files identical despite different names*

