# Comparing `tmp/hstsparser-1.1.5.tar.gz` & `tmp/hstsparser-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstsparser-1.1.5.tar", max compression
+gzip compressed data, was "hstsparser-1.1.6.tar", max compression
```

## Comparing `hstsparser-1.1.5.tar` & `hstsparser-1.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-05-21 01:15:54.056178 hstsparser-1.1.5/LICENSE
--rw-r--r--   0        0        0     2727 2023-05-21 01:15:54.056178 hstsparser-1.1.5/README.md
--rw-r--r--   0        0        0     6257 2023-05-21 01:15:54.056178 hstsparser-1.1.5/hstsparser.py
--rw-r--r--   0        0        0     1351 2023-05-21 01:16:15.856489 hstsparser-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     3642 1970-01-01 00:00:00.000000 hstsparser-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-21 01:24:40.839179 hstsparser-1.1.6/LICENSE
+-rw-r--r--   0        0        0     2727 2023-05-21 01:24:40.839179 hstsparser-1.1.6/README.md
+-rwxr-xr-x   0        0        0     6281 2023-05-21 01:24:40.839179 hstsparser-1.1.6/hstsparser.py
+-rw-r--r--   0        0        0     1356 2023-05-21 01:25:07.231100 hstsparser-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 hstsparser-1.1.6/PKG-INFO
```

### Comparing `hstsparser-1.1.5/LICENSE` & `hstsparser-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hstsparser-1.1.5/README.md` & `hstsparser-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hstsparser-1.1.5/hstsparser.py` & `hstsparser-1.1.6/hstsparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 import csv
 import datetime
 import json
 import os
 import re
 import typing
 from argparse import ArgumentParser, Namespace
```

### Comparing `hstsparser-1.1.5/pyproject.toml` & `hstsparser-1.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstsparser"
-version = "1.1.5"
+version = "1.1.6"
 description = "A tool to parse Firefox and Chrome HSTS databases into forensic artifacts."
 authors = ["Daniel Milnes <daniel@daniel-milnes.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thebeanogamer/hstsparser"
 repository = "https://github.com/thebeanogamer/hstsparser"
 documentation = "https://github.com/thebeanogamer/hstsparser"
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Security",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-PTable = "^0.9.2"
+prettytable = "^3.7.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^6.0.0"
 flake8-bandit = "^4.1.1"
 flake8-bugbear = "^23.5.9"
 flake8-import-order = "^0.18.2"
 flake8-string-format = "^0.3.0"
```

### Comparing `hstsparser-1.1.5/PKG-INFO` & `hstsparser-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstsparser
-Version: 1.1.5
+Version: 1.1.6
 Summary: A tool to parse Firefox and Chrome HSTS databases into forensic artifacts.
 Home-page: https://github.com/thebeanogamer/hstsparser
 License: MIT
 Keywords: chrome,firefox,dfir,forensics,hsts
 Author: Daniel Milnes
 Author-email: daniel@daniel-milnes.uk
 Requires-Python: >=3.9,<3.12
@@ -12,15 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Requires-Dist: PTable (>=0.9.2,<0.10.0)
+Requires-Dist: prettytable (>=3.7.0,<4.0.0)
 Project-URL: Documentation, https://github.com/thebeanogamer/hstsparser
 Project-URL: Repository, https://github.com/thebeanogamer/hstsparser
 Description-Content-Type: text/markdown
 
 # HSTS Parser
 
 [![Lint Codebase](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml) [![Build Releases](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.11.x](https://img.shields.io/badge/python-3.11.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser) [![Downloads](https://pepy.tech/badge/hstsparser)](https://pepy.tech/project/hstsparser)
```

