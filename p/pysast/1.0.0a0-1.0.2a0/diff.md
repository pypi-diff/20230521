# Comparing `tmp/pysast-1.0.0a0.tar.gz` & `tmp/pysast-1.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysast-1.0.0a0.tar", max compression
+gzip compressed data, was "pysast-1.0.2a0.tar", max compression
```

## Comparing `pysast-1.0.0a0.tar` & `pysast-1.0.2a0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35802 2023-05-18 12:47:39.295835 pysast-1.0.0a0/LICENSE
--rw-r--r--   0        0        0     1198 2023-05-19 17:30:42.867606 pysast-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0    37926 2023-05-19 16:59:05.963357 pysast-1.0.0a0/pysast.py
--rw-r--r--   0        0        0     3855 2023-05-19 17:17:49.575399 pysast-1.0.0a0/README.md
--rw-r--r--   0        0        0     4591 1970-01-01 00:00:00.000000 pysast-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0    35802 2023-05-18 12:47:39.295835 pysast-1.0.2a0/LICENSE
+-rw-r--r--   0        0        0     1198 2023-05-21 04:48:47.757113 pysast-1.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0    39896 2023-05-21 04:48:47.133849 pysast-1.0.2a0/pysast.py
+-rw-r--r--   0        0        0     4147 2023-05-21 04:48:46.895373 pysast-1.0.2a0/README.md
+-rw-r--r--   0        0        0     4881 1970-01-01 00:00:00.000000 pysast-1.0.2a0/PKG-INFO
```

### Comparing `pysast-1.0.0a0/LICENSE` & `pysast-1.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysast-1.0.0a0/pyproject.toml` & `pysast-1.0.2a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysast"
-version = "1.0.0-alpha"
+version = "1.0.2-alpha"
 description="SAST Code Scanner in Python"
 authors = ["MatrixEditor"]
 keywords = ["pysast"]
 readme = "README.md"
 license = "GNU GPLv3"
 classifiers = [
      # How mature is this project? Common values are
```

### Comparing `pysast-1.0.0a0/pysast.py` & `pysast-1.0.2a0/pysast.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __doc__ = """Simple and small python module to perform SAST scans."""
-__version__ = "0.0.1"
+__version__ = "1.0"
+__sem_version__ = "1.0.2-alpha"
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
+import sarif_om
 
 from typing import Generator, Any
 
 RESULT_KEY_META = "meta"
 RESULT_KEY_FILES = "files"
 RESULT_KEY_ABS_PATH = "abs_path"
 RESULT_KEY_LINES = "lines"
@@ -163,15 +165,15 @@
         self._inverted = not self._inverted
         return self
 
     def with_re(self) -> None:
         """Enable regular expression matching.
 
         This method enables regular expression matching when applying the filter. After
-        calling this method, the :ref:`pysast.FileFilter.apply` method will use regular expressions
+        calling this method, the ``apply(...)`` method will use regular expressions
         to match files against the filter criteria.
         """
         self._use_re = True
 
     def apply(self, value: str, target: str) -> bool:
         """Apply the filter to a target value.
 
@@ -670,33 +672,37 @@
     :type disable_prefilter: bool
     :param disable_postfilter: Optional. Specifies whether to disable post-filtering
                                of scan results. Default is True.
     :type disable_postfilter: bool
     :param max_bytes: Optional. Maximum number of bytes to read from a file during
                       scanning. Default is ``DEFAULT_MAX_BYTES``.
     :type max_bytes: int
+    :patam use_mime_type: Specifies whether the MIME-type should be loaded
+    :type use_mime_type: bool
     """
 
     def __init__(
         self,
         rules_dir: str = None,
         rules_path: str = None,
         rules: list[SastRule] = None,
         recursive_dir: bool = False,
         disable_prefilter: bool = False,
         disable_postfilter: bool = True,
         max_bytes=DEFAULT_MAX_BYTES,
+        use_mime_type: bool = True,
     ) -> None:
         super().__init__()
         self._scan_results = []
         self._rules = []
 
         self.max_bytes = max_bytes
         self.disable_prefilter = disable_prefilter
         self.disable_postfilter = disable_postfilter
+        self.use_mime_type = use_mime_type
 
         if rules_dir is not None:
             self.load_rule_directory(rules_dir, recursive_dir)
         if rules_path is not None:
             self.load_rule_file(rules_path)
         if rules is not None:
             self.rules.extend(rules)
@@ -787,16 +793,18 @@
         """Perform the scanning process on the specified file.
 
         :param file_path: the file to be scanned
         :type file_path: str
         :return: whether there are any scan results
         :rtype: bool
         """
-        mime_type = get_mime_type(file_path)
-        logger.debug(f"Got mime-type {mime_type} for {file_path}")
+        mime_type = None
+        if self.use_mime_type:
+            mime_type = get_mime_type(file_path)
+            logger.debug(f"Got mime-type {mime_type} for {file_path}")
 
         if os.path.getsize(file_path) > self.max_bytes:
             logger.warning("File too large - skipping '%s'", file_path)
             return self.has_matches
 
         context = self.get_context(file_path, mime_type)
         start = datetime.datetime.now()
@@ -843,14 +851,16 @@
 def load_sast_rules(file_path: str) -> list[SastRule]:
     """Loads SAST (Static Application Security Testing) rules from a file.
 
     The method takes a file path as input and returns a list of :class:`SastRule`
     objects. The file can be in either JSON or YAML format.
 
     Example:
+    ~~~~~~~~
+
     >>> rules = load_sast_rules("sast_rules.json")
     >>> for rule in rules:
     ...     print(rule.rule_id, rule.meta["severity"])
     example-rule INFO
 
     :param file_path: The path to the file containing the SAST rules.
     :type file_path: str
@@ -930,23 +940,26 @@
     parser.add_argument(
         "-S",
         "--sast-dir",
         required=False,
         default=[],
         action="append",
         dest="sast_dirs",
-        help="One or more directories that store SAST rules. (Use -rS for recursive search)",
+        help=(
+            "One or more directories that store SAST rules. (Use -rS for recursive search) "
+            "The current directory is used if no rules are specified."
+        ),
     )
     parser.add_argument(
         "-rS",
         "--recursive-sast-dir",
         required=False,
-        default=False,
-        action="store_true",
-        dest="recursive_sast_dir",
+        default=[],
+        action="append",
+        dest="recursive_sast_dirs",
         help="Load rules from target directories recursively",
     )
     parser.add_argument(
         "--disable-prefilter",
         dest="disable_prefilter",
         action="store_true",
         default=False,
@@ -962,78 +975,132 @@
     parser.add_argument(
         "-M",
         "--max-bytes",
         default=DEFAULT_MAX_BYTES,
         type=int,
         help="Skip files exteeding a the amount of maximum bytes.",
     )
+    parser.add_argument(
+        "-T",
+        "--disable-mime",
+        required=False,
+        default=False,
+        action="store_true",
+        help=(
+            "Specifies whether the scanner should use the 'file' utility "
+            "to retrieve the MIME-type of a file. (enabled as per default)"
+        ),
+    )
+    parser.add_argument(
+        "-e",
+        "--exclude-file",
+        required=False,
+        default=[],
+        action="append",
+        dest="exclude_files",
+        help="Specifies exclusion files (use re: for regular expressions)",
+    )
 
     args = parser.parse_args(cmd)
 
     # Setup logging
     log_levels = {
         0: logging.ERROR,
         1: logging.WARNING,
         2: logging.INFO,
         3: logging.DEBUG,
     }
     log_level = min(3, max(args.verbose, 0))
     logging.basicConfig(level=log_levels[log_level])
 
     if len(args.sast_rules) == 0 and len(args.sast_dirs) == 0:
-        logger.error("Please specify at least one rule file or rule directory!")
-        sys.exit(1)
+        logger.warning("No rules specified, using current directory...")
+        args.sast_dirs.append(os.path.abspath("."))
+
+    for i, val in enumerate(args.exclude_files):
+        if val.startswith("re:"):
+            args.exclude_files[i] = re.compile(val[3:])
 
     scanner = SastScanner(
         max_bytes=args.max_bytes,
         disable_postfilter=not args.enable_postfilter,
         disable_prefilter=args.disable_prefilter,
+        use_mime_type=not args.use_mime,
+        exclude_files=args.exclude_files,
+        exclude_dirs=args.exclude_dirs,
     )
 
     for file_path in args.sast_rules:
         scanner.load_rule_file(file_path)
 
     for dir_path in args.sast_dirs:
-        scanner.load_rule_directory(dir_path, args.recursive_sast_dir)
+        scanner.load_rule_directory(dir_path, False)
+
+    for dir_path in args.recursive_sast_dirs:
+        scanner.load_rule_directory(dir_path, True)
+
+    if len(scanner.rules) == 0:
+        logger.error(
+            "No rules loaded - make sure to specify the right file(s) or directory(ies)"
+        )
+        sys.exit(1)
+
+    excluded = args.excluded_files
+
+    def is_excluded(path: str) -> bool:
+        for val in excluded:
+            if isinstance(val, re.Pattern) and val.match(path) or val == path:
+                return True
 
     def pprint_match(match: dict, intent: str):
-        print(intent, "+ match:%s (%s)"
+        print(
+            intent,
+            "+ match:%s (%s)"
             % (
                 match[RESULT_KEY_RULE_ID],
                 match[RESULT_KEY_META].get("severity", "None"),
-            )
-        )
+            ),
+        )  # noqa
         print(intent * 3, "Title:", match[RESULT_KEY_META].get("title", "No Title"))
-        print(intent * 3, "Description", match[RESULT_KEY_META].get("description", "<>"))
-        print(intent * 3, "Lines:", pprint.pformat(match[RESULT_KEY_LINES], compact=True))
-        print(intent * 3,"Offsets:",pprint.pformat(match[RESULT_KEY_POSITIONS], compact=True))
+        print(
+            intent * 3, "Description", match[RESULT_KEY_META].get("description", "<>")
+        )
+        print(
+            intent * 3, "Lines:", pprint.pformat(match[RESULT_KEY_LINES], compact=True)
+        )
+        print(
+            intent * 3,
+            "Offsets:",
+            pprint.pformat(match[RESULT_KEY_POSITIONS], compact=True),
+        )
         print(intent * 3, "Meta:", pprint.pformat(match[RESULT_KEY_META]), "\n")
 
     def scan_file(file_path: str) -> bool:
         try:
             if scanner.scan(file_path):
                 if args.dump_json:
                     json.dump(
-                        scanner.scan_results, sys.stdout, sort_keys=True, indent=4
+                        obj=scanner.scan_results,
+                        fp=sys.stdout,
+                        sort_keys=True,
+                        indent=4,
                     )
                 else:
                     print("+ file:", file_path)
                     for match in scanner.scan_results:
                         pprint_match(match, " ")
                 return True
 
         except Exception as err:
             logger.exception("(%s) Scan failed for %s:", type(err).__name__, file_path)
             return False
 
     def scan_dir(dir_path: str) -> bool:
-        for file_path in pathlib.Path(dir_path).iterdir():
-            if file_path.is_dir() and args.recursive:
-                scan_dir(str(file_path))
-            else:
+        for file_path in pathlib.Path(dir_path).glob("**/*" if args.recursive else "*"):
+            if file_path.is_file() and not is_excluded(str(file_path)):
                 scan_file(str(file_path))
 
     for path in args.paths:
         if os.path.isdir(path):
             scan_dir(path)
         else:
             if not scan_file(path):
```

### Comparing `pysast-1.0.0a0/README.md` & `pysast-1.0.2a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PySAST
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
 ![Status](https://img.shields.io:/static/v1?label=Status&message=Alpha-Release&color=lightgreen)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=All&color=yellowgreen)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.0.0-alpha&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.0.2-alpha&color=lightblue)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
 
 Welcome to `pysast` - a powerful Python package designed for scanning one or multiple files using customizable rules written
 in JSON or YAML. This package allows you to automate the process of code analysis and identify potential issues or violations
 based on your specified criteria.
 
 By utilizing the rule-based system, you can define a set of rules that reflect your desired coding standards, best practices,
@@ -32,37 +32,39 @@
 2. Running Scans: Explore how to execute pysast to scan your files and generate detailed reports.
 3. Advanced Usage: Dive deeper into the advanced features and options offered by pysast to enhance your code analysis capabilities.
 
 By following these steps, you'll be equipped with the knowledge and tools to effectively utilize `pysast` in your projects.
 
 ## CLI Options
 
-    usage: pysast.py [-h] [-r] [-j] [-v] [-s SAST_RULES] [-S SAST_DIRS] [-rS] \
-                [--disable-prefilter] [--enable-postfilter] [-M MAX_BYTES] [PATHS ...]
+    usage: pysast.py [-h] [-r] [-j] [-v] [-s SAST_RULES] [-S SAST_DIRS] \
+                [-rS RECURSIVE_SAST_DIRS] [--disable-prefilter] [--enable-postfilter]
+                [-M MAX_BYTES] [-T] [PATHS ...]
 
     Scan the given file with SAST scanner using all available rules.
 
     positional arguments:
     PATHS                 One or more files or directories to scan.
 
     options:
     -h, --help            show this help message and exit
     -r, --recursive       Scan target directories recursively
     -j, --json            Dump JSON output instead of pprint.
     -v, --verbose         Specifies the verbosity for the next scan. Use -vvv for more verbose output.
     -s SAST_RULES, --sast-rule SAST_RULES
                             File path(s) to SAST rules to import. (Use -S for directories)
     -S SAST_DIRS, --sast-dir SAST_DIRS
-                            One or more directories that store SAST rules. (Use -rS for recursive search)
-    -rS, --recursive-sast-dir
+                            One or more directories that store SAST rules. (Use -rS for recursive search) The current directory is used if no rules are specified.
+    -rS RECURSIVE_SAST_DIRS, --recursive-sast-dir RECURSIVE_SAST_DIRS
                             Load rules from target directories recursively
     --disable-prefilter   Disable prefiltering rules.
     --enable-postfilter   Enable postfiltering.
     -M MAX_BYTES, --max-bytes MAX_BYTES
                             Skip files exteeding a the amount of maximum bytes.
+    -T, --disable-mime        Specifies whether the scanner should use the 'file' utility to retrieve the MIME-type of a file. (enabled as per default)
 
 
 ## Documentation
 
 For more detailed information on using pysast, please refer to the [official documentation](https://matrixeditor.github.io/pysast/) on Github.
 
 ## Contributing
```

### Comparing `pysast-1.0.0a0/PKG-INFO` & `pysast-1.0.2a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysast
-Version: 1.0.0a0
+Version: 1.0.2a0
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
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.0.0-alpha&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.0.2-alpha&color=lightblue)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
 
 Welcome to `pysast` - a powerful Python package designed for scanning one or multiple files using customizable rules written
 in JSON or YAML. This package allows you to automate the process of code analysis and identify potential issues or violations
 based on your specified criteria.
 
 By utilizing the rule-based system, you can define a set of rules that reflect your desired coding standards, best practices,
@@ -54,37 +54,39 @@
 2. Running Scans: Explore how to execute pysast to scan your files and generate detailed reports.
 3. Advanced Usage: Dive deeper into the advanced features and options offered by pysast to enhance your code analysis capabilities.
 
 By following these steps, you'll be equipped with the knowledge and tools to effectively utilize `pysast` in your projects.
 
 ## CLI Options
 
-    usage: pysast.py [-h] [-r] [-j] [-v] [-s SAST_RULES] [-S SAST_DIRS] [-rS] \
-                [--disable-prefilter] [--enable-postfilter] [-M MAX_BYTES] [PATHS ...]
+    usage: pysast.py [-h] [-r] [-j] [-v] [-s SAST_RULES] [-S SAST_DIRS] \
+                [-rS RECURSIVE_SAST_DIRS] [--disable-prefilter] [--enable-postfilter]
+                [-M MAX_BYTES] [-T] [PATHS ...]
 
     Scan the given file with SAST scanner using all available rules.
 
     positional arguments:
     PATHS                 One or more files or directories to scan.
 
     options:
     -h, --help            show this help message and exit
     -r, --recursive       Scan target directories recursively
     -j, --json            Dump JSON output instead of pprint.
     -v, --verbose         Specifies the verbosity for the next scan. Use -vvv for more verbose output.
     -s SAST_RULES, --sast-rule SAST_RULES
                             File path(s) to SAST rules to import. (Use -S for directories)
     -S SAST_DIRS, --sast-dir SAST_DIRS
-                            One or more directories that store SAST rules. (Use -rS for recursive search)
-    -rS, --recursive-sast-dir
+                            One or more directories that store SAST rules. (Use -rS for recursive search) The current directory is used if no rules are specified.
+    -rS RECURSIVE_SAST_DIRS, --recursive-sast-dir RECURSIVE_SAST_DIRS
                             Load rules from target directories recursively
     --disable-prefilter   Disable prefiltering rules.
     --enable-postfilter   Enable postfiltering.
     -M MAX_BYTES, --max-bytes MAX_BYTES
                             Skip files exteeding a the amount of maximum bytes.
+    -T, --disable-mime        Specifies whether the scanner should use the 'file' utility to retrieve the MIME-type of a file. (enabled as per default)
 
 
 ## Documentation
 
 For more detailed information on using pysast, please refer to the [official documentation](https://matrixeditor.github.io/pysast/) on Github.
 
 ## Contributing
```

