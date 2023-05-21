# Comparing `tmp/lifx_cli-2.5.2.tar.gz` & `tmp/lifx_cli-2.5.3.tar.gz`

## Comparing `lifx_cli-2.5.2.tar` & `lifx_cli-2.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1519 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/increment_version.sh
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/requirements.txt
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/.github/workflows/python-publish.yml
--rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/auth.py
--rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/colors.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/effects.py
--rwxr-xr-x   0        0        0    12579 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/lifx.py
--rwxr-xr-x   0        0        0     3149 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/lights.py
--rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/scenes.py
--rwxr-xr-x   0        0        0     1262 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/tests/lifx_cli_test.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/tests/requirements.txt
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/LICENSE
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/pyproject.toml
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1519 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/increment_version.sh
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/requirements.txt
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/auth.py
+-rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/colors.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/effects.py
+-rwxr-xr-x   0        0        0    12579 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/lifx.py
+-rwxr-xr-x   0        0        0     3149 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/lights.py
+-rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/scenes.py
+-rwxr-xr-x   0        0        0     1262 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/tests/lifx_cli_test.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/tests/requirements.txt
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/LICENSE
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/README.md
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/PKG-INFO
```

### Comparing `lifx_cli-2.5.2/increment_version.sh` & `lifx_cli-2.5.3/increment_version.sh`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/.github/workflows/pylint.yml` & `lifx_cli-2.5.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/.github/workflows/pytest.yml` & `lifx_cli-2.5.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/.github/workflows/python-publish.yml` & `lifx_cli-2.5.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/src/lifx/auth.py` & `lifx_cli-2.5.3/src/lifx/auth.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/src/lifx/colors.py` & `lifx_cli-2.5.3/src/lifx/colors.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/src/lifx/effects.py` & `lifx_cli-2.5.3/src/lifx/effects.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/src/lifx/lifx.py` & `lifx_cli-2.5.3/src/lifx/lifx.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ██      ██ ███████ ██   ██      ██████ ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ██      ██ █████     ███       ██      ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ███████ ██ ██      ██   ██      ██████ ███████ ██
 
 """
-VERSION = "2.5.2"
+VERSION = "2.5.3"
 
 
 def colors_sub_command(args):
     """Control the actions for the 'colors' sub-command."""
     colors = Colors()
 
     if isinstance(args, list):
```

### Comparing `lifx_cli-2.5.2/src/lifx/lights.py` & `lifx_cli-2.5.3/src/lifx/lights.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/src/lifx/scenes.py` & `lifx_cli-2.5.3/src/lifx/scenes.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/tests/lifx_cli_test.py` & `lifx_cli-2.5.3/tests/lifx_cli_test.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/.gitignore` & `lifx_cli-2.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/LICENSE` & `lifx_cli-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.2/PKG-INFO` & `lifx_cli-2.5.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,10 @@
-Metadata-Version: 2.1
-Name: lifx-cli
-Version: 2.5.2
-Summary: The Unofficial LIFX CLI
-Project-URL: Homepage, https://github.com/necrux/lifx-cli
-Project-URL: Bug Tracker, https://github.com/necrux/lifx-cli/issues
-Author-email: Wes Henderson <info@necrux.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: requests
-Requires-Dist: tabulate
-Description-Content-Type: text/markdown
+# The Unofficial LIFX CLI [![Latest Version](https://img.shields.io/pypi/v/lifx-cli.svg)](https://pypi.org/project/lifx-cli/)
 
-# The Unofficial LIFX CLI
+[![CI/CD](https://github.com/necrux/lifx-cli/actions/workflows/python-publish.yml/badge.svg)](https://github.com/necrux/lifx-cli/actions/workflows/python-publish.yml)[![Linter](https://github.com/necrux/lifx-cli/actions/workflows/pylint.yml/badge.svg)](https://github.com/necrux/lifx-cli/actions/workflows/pylint.yml)[![Tests](https://github.com/necrux/lifx-cli/actions/workflows/pytest.yml/badge.svg)](https://github.com/necrux/lifx-cli/actions/workflows/pytest.yml)[![License](https://img.shields.io/pypi/l/lifx-cli.svg)](https://github.com/necrux/lifx-cli/blob/main/LICENSE)[![Python-Support](https://img.shields.io/pypi/pyversions/lifx-cli.svg)](https://pypi.org/project/lifx-cli/)
 
 This is a work in progress to create a feature-rich LIFX CLI.
 
 **This project is not affiliated with or endorsed by LIFX.**
 
 ## Installation
```

