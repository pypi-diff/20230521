# Comparing `tmp/pysast-1.1.0a0.tar.gz` & `tmp/pysast-1.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysast-1.1.0a0.tar", max compression
+gzip compressed data, was "pysast-1.1.2a0.tar", max compression
```

## Comparing `pysast-1.1.0a0.tar` & `pysast-1.1.2a0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35802 2023-05-18 12:47:39.295835 pysast-1.1.0a0/LICENSE
--rw-r--r--   0        0        0     1198 2023-05-21 06:30:17.987945 pysast-1.1.0a0/pyproject.toml
--rw-r--r--   0        0        0    41535 2023-05-21 06:30:18.006373 pysast-1.1.0a0/pysast.py
--rw-r--r--   0        0        0     4458 2023-05-21 06:30:17.957183 pysast-1.1.0a0/README.md
--rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 pysast-1.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0    35802 2023-05-18 12:47:39.295835 pysast-1.1.2a0/LICENSE
+-rw-r--r--   0        0        0     1198 2023-05-21 07:01:09.081563 pysast-1.1.2a0/pyproject.toml
+-rw-r--r--   0        0        0    41389 2023-05-21 07:01:09.111227 pysast-1.1.2a0/pysast.py
+-rw-r--r--   0        0        0     4922 2023-05-21 07:01:09.042706 pysast-1.1.2a0/README.md
+-rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 pysast-1.1.2a0/PKG-INFO
```

### Comparing `pysast-1.1.0a0/LICENSE` & `pysast-1.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysast-1.1.0a0/pyproject.toml` & `pysast-1.1.2a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysast"
-version = "1.1.0-alpha"
+version = "1.1.2-alpha"
 description="SAST Code Scanner in Python"
 authors = ["MatrixEditor"]
 keywords = ["pysast"]
 readme = "README.md"
 license = "GNU GPLv3"
 classifiers = [
      # How mature is this project? Common values are
```

### Comparing `pysast-1.1.0a0/pysast.py` & `pysast-1.1.2a0/pysast.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,29 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __doc__ = """Simple and small python module to perform SAST scans."""
-__version__ = "1.0"
-__sem_version__ = "1.1.0-alpha"
+__version__ = "1.1"
+__sem_version__ = "1.1.2-alpha"
 __authors__ = "MatrixEditor"
 
 import sys
 import os
 import re
 import logging
 import json
 import yaml
 import pathlib
 import subprocess
 import datetime
 import importlib
 
-from multiprocessing import current_process
 from concurrent.futures import ThreadPoolExecutor
 from typing import Generator, Any
 
 RESULT_KEY_META = "meta"
 RESULT_KEY_FILES = "files"
 RESULT_KEY_ABS_PATH = "abs_path"
 RESULT_KEY_LINES = "lines"
@@ -1061,16 +1060,14 @@
         scanner.load_rule_directory(dir_path, True)
 
     if len(scanner.rules) == 0:
         logger.error(
             "No rules loaded - make sure to specify the right file(s) or directory(ies)"
         )
         sys.exit(1)
-    else:
-        print("Using %d rules..." % len(scanner.rules))
 
     excluded = args.exclude_files
 
     def is_excluded(path: str) -> bool:
         for val in excluded:
             if isinstance(val, re.Pattern) and val.match(path) or val == path:
                 return True
@@ -1134,15 +1131,15 @@
         if os.path.isdir(path):
             ppath = pathlib.Path(path)
             # print informational details
             logger.debug(
                 "Scanning %d files...",
                 len(list(ppath.rglob("*") if args.recursive else ppath.iterdir())),
             )
-            if not current_process().daemon and args.threading:
+            if args.threading:
                 # The use threading will lower the amount of time spent for
                 # a scan.
                 with ThreadPoolExecutor() as executor:
                     scan_dir(path, executor)
             else:
                 scan_dir(path)
         else:
```

### Comparing `pysast-1.1.0a0/README.md` & `pysast-1.1.2a0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PySAST
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
 ![Status](https://img.shields.io:/static/v1?label=Status&message=Alpha-Release&color=lightgreen)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=All&color=yellowgreen)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.0-alpha&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.2-alpha&color=lightblue)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
 
 Welcome to `pysast` - a powerful Python package designed for scanning one or multiple files using customizable rules written
 in JSON or YAML. This package allows you to automate the process of code analysis and identify potential issues or violations
 based on your specified criteria.
 
 By utilizing the rule-based system, you can define a set of rules that reflect your desired coding standards, best practices,
@@ -28,32 +28,30 @@
 
 For more detailed information on using pysast, please refer to the [official documentation](https://matrixeditor.github.io/pysast/) on Github.
 
 ## Getting Started
 
 Before you begin using `pysast`, it's recommended to familiarize yourself with the package's functionality and usage. The following steps will guide you through the essential setup and running your first code scan:
 
-1. Rule Definition: Learn how to define rules in JSON or YAML format to specify the analysis criteria for your codebase.
-2. Running Scans: Explore how to execute pysast to scan your files and generate detailed reports.
-3. Advanced Usage: Dive deeper into the advanced features and options offered by pysast to enhance your code analysis capabilities.
+1. [Rule Definition](https://matrixeditor.github.io/pysast/intro/sast_rules.html): Learn how to define rules in JSON or YAML format to specify the analysis criteria for your codebase.
+2. [Running Scans](https://matrixeditor.github.io/pysast/intro/sast_scans.html): Explore how to execute pysast to scan your files and generate detailed reports.
+3. [Advanced Usage](https://matrixeditor.github.io/pysast/api/index.html): Dive deeper into the advanced features and options offered by pysast to enhance your code analysis capabilities.
 
 By following these steps, you'll be equipped with the knowledge and tools to effectively utilize `pysast` in your projects.
 
 ## Optimization
 
 Since version ``1.1.0`` this program introduces an optimization feature that significantly
 improves its performance by leveraging threading. By utilizing the ``--threading`` option
 on the command line, you can enable this optimization to take full advantage of your
 system's resources.
 
 ## CLI Options
 
-    usage: pysast.py [-h] [-r] [-j] [-v] [-s SAST_RULES] [-S SAST_DIRS] \
-                [-rS RECURSIVE_SAST_DIRS] [--disable-prefilter] [--enable-postfilter]
-                [-M MAX_BYTES] [-T] [PATHS ...]
+    usage: pysast.py [-h] [-r] [-j] [-v] [-s SAST_RULES] [-S SAST_DIRS] [-rS RECURSIVE_SAST_DIRS] [--disable-prefilter] [--enable-postfilter] [-M MAX_BYTES] [-T] [-e EXCLUDE_FILES] [--threading] [PATHS ...]
 
     Scan the given file with SAST scanner using all available rules.
 
     positional arguments:
     PATHS                 One or more files or directories to scan.
 
     options:
@@ -67,16 +65,19 @@
                             One or more directories that store SAST rules. (Use -rS for recursive search) The current directory is used if no rules are specified.
     -rS RECURSIVE_SAST_DIRS, --recursive-sast-dir RECURSIVE_SAST_DIRS
                             Load rules from target directories recursively
     --disable-prefilter   Disable prefiltering rules.
     --enable-postfilter   Enable postfiltering.
     -M MAX_BYTES, --max-bytes MAX_BYTES
                             Skip files exteeding a the amount of maximum bytes.
-    -T, --disable-mime        Specifies whether the scanner should use the 'file' utility to retrieve the MIME-type of a file. (enabled as per default)
-
+    -T, --disable-mime, -T, --disable-mime
+                            Specifies whether the scanner should use the 'file' utility to retrieve the MIME-type of a file. (enabled as per default)
+    -e EXCLUDE_FILES, --exclude-file EXCLUDE_FILES
+                            Specifies exclusion files (use re: for regular expressions)
+    --threading           Activates threading for file processing. (Can't be used on daemon processes)
 
 ## Contributing
 
 We welcome contributions from the community! If you'd like to contribute to `pysast`, please refer to the contribution guidelines.
 
 ## Support
```

### Comparing `pysast-1.1.0a0/PKG-INFO` & `pysast-1.1.2a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysast
-Version: 1.1.0a0
+Version: 1.1.2a0
 Summary: SAST Code Scanner in Python
 License: GNU GPLv3
 Keywords: pysast
 Author: MatrixEditor
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 
 # PySAST
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
 ![Status](https://img.shields.io:/static/v1?label=Status&message=Alpha-Release&color=lightgreen)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=All&color=yellowgreen)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.0-alpha&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.2-alpha&color=lightblue)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
 
 Welcome to `pysast` - a powerful Python package designed for scanning one or multiple files using customizable rules written
 in JSON or YAML. This package allows you to automate the process of code analysis and identify potential issues or violations
 based on your specified criteria.
 
 By utilizing the rule-based system, you can define a set of rules that reflect your desired coding standards, best practices,
@@ -50,32 +50,30 @@
 
 For more detailed information on using pysast, please refer to the [official documentation](https://matrixeditor.github.io/pysast/) on Github.
 
 ## Getting Started
 
 Before you begin using `pysast`, it's recommended to familiarize yourself with the package's functionality and usage. The following steps will guide you through the essential setup and running your first code scan:
 
-1. Rule Definition: Learn how to define rules in JSON or YAML format to specify the analysis criteria for your codebase.
-2. Running Scans: Explore how to execute pysast to scan your files and generate detailed reports.
-3. Advanced Usage: Dive deeper into the advanced features and options offered by pysast to enhance your code analysis capabilities.
+1. [Rule Definition](https://matrixeditor.github.io/pysast/intro/sast_rules.html): Learn how to define rules in JSON or YAML format to specify the analysis criteria for your codebase.
+2. [Running Scans](https://matrixeditor.github.io/pysast/intro/sast_scans.html): Explore how to execute pysast to scan your files and generate detailed reports.
+3. [Advanced Usage](https://matrixeditor.github.io/pysast/api/index.html): Dive deeper into the advanced features and options offered by pysast to enhance your code analysis capabilities.
 
 By following these steps, you'll be equipped with the knowledge and tools to effectively utilize `pysast` in your projects.
 
 ## Optimization
 
 Since version ``1.1.0`` this program introduces an optimization feature that significantly
 improves its performance by leveraging threading. By utilizing the ``--threading`` option
 on the command line, you can enable this optimization to take full advantage of your
 system's resources.
 
 ## CLI Options
 
-    usage: pysast.py [-h] [-r] [-j] [-v] [-s SAST_RULES] [-S SAST_DIRS] \
-                [-rS RECURSIVE_SAST_DIRS] [--disable-prefilter] [--enable-postfilter]
-                [-M MAX_BYTES] [-T] [PATHS ...]
+    usage: pysast.py [-h] [-r] [-j] [-v] [-s SAST_RULES] [-S SAST_DIRS] [-rS RECURSIVE_SAST_DIRS] [--disable-prefilter] [--enable-postfilter] [-M MAX_BYTES] [-T] [-e EXCLUDE_FILES] [--threading] [PATHS ...]
 
     Scan the given file with SAST scanner using all available rules.
 
     positional arguments:
     PATHS                 One or more files or directories to scan.
 
     options:
@@ -89,16 +87,19 @@
                             One or more directories that store SAST rules. (Use -rS for recursive search) The current directory is used if no rules are specified.
     -rS RECURSIVE_SAST_DIRS, --recursive-sast-dir RECURSIVE_SAST_DIRS
                             Load rules from target directories recursively
     --disable-prefilter   Disable prefiltering rules.
     --enable-postfilter   Enable postfiltering.
     -M MAX_BYTES, --max-bytes MAX_BYTES
                             Skip files exteeding a the amount of maximum bytes.
-    -T, --disable-mime        Specifies whether the scanner should use the 'file' utility to retrieve the MIME-type of a file. (enabled as per default)
-
+    -T, --disable-mime, -T, --disable-mime
+                            Specifies whether the scanner should use the 'file' utility to retrieve the MIME-type of a file. (enabled as per default)
+    -e EXCLUDE_FILES, --exclude-file EXCLUDE_FILES
+                            Specifies exclusion files (use re: for regular expressions)
+    --threading           Activates threading for file processing. (Can't be used on daemon processes)
 
 ## Contributing
 
 We welcome contributions from the community! If you'd like to contribute to `pysast`, please refer to the contribution guidelines.
 
 ## Support
```

