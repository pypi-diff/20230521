# Comparing `tmp/tomte-0.2.6.tar.gz` & `tmp/tomte-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomte-0.2.6.tar", max compression
+gzip compressed data, was "tomte-0.2.7.tar", max compression
```

## Comparing `tomte-0.2.6.tar` & `tomte-0.2.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1063 2022-10-01 14:11:14.626018 tomte-0.2.6/LICENSE
--rw-r--r--   0        0        0     2856 2023-05-21 15:38:36.444320 tomte-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-21 15:38:41.437413 tomte-0.2.6/tomte/__init__.py
--rw-r--r--   0        0        0     2829 2023-05-21 15:29:39.235525 tomte-0.2.6/tomte/cli.py
--rw-r--r--   0        0        0      876 2022-09-11 16:56:11.417175 tomte-0.2.6/tomte/tools/__init__.py
--rwxr-xr-x   0        0        0    11371 2023-05-21 15:29:26.911765 tomte-0.2.6/tomte/tools/check_copyright.py
--rwxr-xr-x   0        0        0     6967 2023-05-21 15:29:39.322671 tomte-0.2.6/tomte/tools/check_doc_links.py
--rwxr-xr-x   0        0        0     1678 2023-05-21 10:59:04.565876 tomte-0.2.6/tomte/tools/check_readme.py
--rwxr-xr-x   0        0        0     1348 2023-05-21 15:29:26.914379 tomte-0.2.6/tomte/tools/freeze_dependencies.py
--rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 tomte-0.2.6/setup.py
--rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 tomte-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-10-01 14:11:14.626018 tomte-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2856 2023-05-21 16:11:41.976598 tomte-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-21 16:11:47.592865 tomte-0.2.7/tomte/__init__.py
+-rw-r--r--   0        0        0     2865 2023-05-21 16:08:38.259096 tomte-0.2.7/tomte/cli.py
+-rw-r--r--   0        0        0      876 2022-09-11 16:56:11.417175 tomte-0.2.7/tomte/tools/__init__.py
+-rwxr-xr-x   0        0        0    11139 2023-05-21 16:09:32.802247 tomte-0.2.7/tomte/tools/check_copyright.py
+-rwxr-xr-x   0        0        0     6964 2023-05-21 16:10:52.628522 tomte-0.2.7/tomte/tools/check_doc_links.py
+-rwxr-xr-x   0        0        0     1678 2023-05-21 10:59:04.565876 tomte-0.2.7/tomte/tools/check_readme.py
+-rwxr-xr-x   0        0        0     1348 2023-05-21 15:29:26.914379 tomte-0.2.7/tomte/tools/freeze_dependencies.py
+-rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 tomte-0.2.7/setup.py
+-rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 tomte-0.2.7/PKG-INFO
```

### Comparing `tomte-0.2.6/LICENSE` & `tomte-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tomte-0.2.6/pyproject.toml` & `tomte-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomte"
-version = "0.2.6"
+version = "0.2.7"
 description = "A library that wraps many useful tools (linters, analysers, etc) to keep Python code clean, secure, well-documented and optimised."
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 tox = {version = "==3.28.0", optional = true}
```

### Comparing `tomte-0.2.6/tomte/cli.py` & `tomte-0.2.7/tomte/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 def format_code() -> None:
     """Run code formatters sequentially: isort and black."""
     sys.argv = ["tox", "-e", "isort", "-e", "black"]
     tox_cmdline()
 
 
 @click.command()
-def format_copyright() -> None:
+@click.option("--author", type=str, required=True)
+def format_copyright(author) -> None:
     """Run copyright formatter."""
-    sys.argv = ["tox", "-e", "fix-copyright"]
-    tox_cmdline()
+    check_copyright_main(author, fix=True)
 
 
 @click.command()
 def check_code() -> None:
     """Run code checks in parallel: black, isort, flake8, mypy, pylint, and darglint."""
     sys.argv = [
         "tox",
```

### Comparing `tomte-0.2.6/tomte/tools/__init__.py` & `tomte-0.2.7/tomte/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.6/tomte/tools/check_copyright.py` & `tomte-0.2.7/tomte/tools/check_copyright.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 - (optional) the Python shebang
 - the encoding header;
 - the copyright and license notices;
 
 It is assumed the script is run from the repository root.
 """
 
-import argparse
 import itertools
 import re
 import shutil
 import subprocess  # nosec
 import sys
 from datetime import datetime
 from pathlib import Path
@@ -287,27 +286,17 @@
         )
         sys.exit(1)
     else:
         print("OK")
         sys.exit(0)
 
 
-def get_args() -> argparse.Namespace:
-    """Get CLI arguments."""
-
-    argparser = argparse.ArgumentParser()
-    argparser.add_argument("--check", action="store_true")
-    return argparser.parse_args()
-
-
-def main(author: str) -> None:
+def main(author: str, fix: bool = False) -> None:
     """Main function."""
 
-    args = get_args()
-
     exclude_files = {Path("scripts", "whitelist.py")}
     python_files = filter(
         lambda x: x not in exclude_files,
         itertools.chain(
             Path("packages", author).glob("**/*.py"),
             Path("tests").glob("**/*.py"),
             Path("scripts").glob("**/*.py"),
@@ -329,11 +318,11 @@
                     and "t_protocol_no_ct" not in file.parts
                     and "build" not in file.parts
                 )
             )
         )
 
     python_files_filtered = filter(_file_filter, python_files)
-    if args.check:
-        run_check(python_files_filtered)
-    else:
+    if fix:
         update_headers(python_files_filtered)
+    else:
+        run_check(python_files_filtered)
```

### Comparing `tomte-0.2.6/tomte/tools/check_doc_links.py` & `tomte-0.2.7/tomte/tools/check_doc_links.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,16 @@
 from itertools import chain
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import requests
 import urllib3  # type: ignore
 from requests.adapters import HTTPAdapter  # type: ignore
-from requests.packages.urllib3.util.retry import (
-    Retry,
-)  # type: ignore # pylint: disable=import-error
+from requests.packages.urllib3.util.retry import \
+    Retry  # type: ignore # pylint: disable=import-error
 
 # Disable insecure request warning (expired SSL certificates)
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 MAX_WORKERS = 10
 URL_REGEX = r'(https?:\/\/(?:www\.|(?!www))[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]\.[^\s)"]{2,}|www\.[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]\.[^\s)"]{2,}|https?:\/\/(?:www\.|(?!www))[a-zA-Z0-9]+\.[^\s)"]{2,}|www\.[a-zA-Z0-9]+\.[^\s)"]{2,})'
```

### Comparing `tomte-0.2.6/tomte/tools/check_readme.py` & `tomte-0.2.7/tomte/tools/check_readme.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.6/tomte/tools/freeze_dependencies.py` & `tomte-0.2.7/tomte/tools/freeze_dependencies.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.6/setup.py` & `tomte-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  'vulture': ['vulture==2.7']}
 
 entry_points = \
 {'console_scripts': ['tomte = tomte.cli:cli']}
 
 setup_kwargs = {
     'name': 'tomte',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': 'A library that wraps many useful tools (linters, analysers, etc) to keep Python code clean, secure, well-documented and optimised.',
     'long_description': 'None',
     'author': 'David Minarsch',
     'author_email': 'david.minarsch@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tomte-0.2.6/PKG-INFO` & `tomte-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomte
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library that wraps many useful tools (linters, analysers, etc) to keep Python code clean, secure, well-documented and optimised.
 License: MIT
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

