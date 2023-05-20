# Comparing `tmp/new-component-0.4.3.tar.gz` & `tmp/new-component-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new-component-0.4.3.tar", last modified: Fri May 19 23:23:35 2023, max compression
+gzip compressed data, was "new-component-0.4.4.tar", last modified: Fri May 19 23:58:28 2023, max compression
```

## Comparing `new-component-0.4.3.tar` & `new-component-0.4.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-05-19 23:23:09.543231 new-component-0.4.3/LICENSE
--rw-r--r--   0        0        0     4798 2023-05-19 23:23:09.543231 new-component-0.4.3/README.md
--rw-r--r--   0        0        0     2085 2023-05-19 23:23:09.543231 new-component-0.4.3/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/__init__.py
--rw-r--r--   0        0        0      496 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/__version__.py
--rw-r--r--   0        0        0     1961 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_config.py
--rw-r--r--   0        0        0      708 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_confirms.py
--rw-r--r--   0        0        0      566 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_constants.py
--rw-r--r--   0        0        0     2088 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_echos.py
--rw-r--r--   0        0        0      360 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_jinja.py
--rw-r--r--   0        0        0      249 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_utils.py
--rw-r--r--   0        0        0      206 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/_version.py
--rw-r--r--   0        0        0     4121 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/cli.py
--rw-r--r--   0        0        0      142 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/main.py
--rw-r--r--   0        0        0        0 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/py.typed
--rw-r--r--   0        0        0      269 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/templates/component.js.j2
--rw-r--r--   0        0        0       48 2023-05-19 23:23:09.543231 new-component-0.4.3/src/new_component/templates/index.js.j2
--rw-r--r--   0        0        0        0 2023-05-19 23:23:09.543231 new-component-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0     6177 2023-05-19 23:23:09.543231 new-component-0.4.3/tests/test_new_component.py
--rw-r--r--   0        0        0      285 2023-05-19 23:23:09.543231 new-component-0.4.3/tests/test_version.py
--rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 new-component-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-19 23:58:02.240480 new-component-0.4.4/LICENSE
+-rw-r--r--   0        0        0     4798 2023-05-19 23:58:02.240480 new-component-0.4.4/README.md
+-rw-r--r--   0        0        0     2331 2023-05-19 23:58:02.240480 new-component-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-19 23:58:02.240480 new-component-0.4.4/src/new_component/__init__.py
+-rw-r--r--   0        0        0     1961 2023-05-19 23:58:02.240480 new-component-0.4.4/src/new_component/_config.py
+-rw-r--r--   0        0        0      708 2023-05-19 23:58:02.240480 new-component-0.4.4/src/new_component/_confirms.py
+-rw-r--r--   0        0        0      566 2023-05-19 23:58:02.240480 new-component-0.4.4/src/new_component/_constants.py
+-rw-r--r--   0        0        0     2088 2023-05-19 23:58:02.240480 new-component-0.4.4/src/new_component/_echos.py
+-rw-r--r--   0        0        0      360 2023-05-19 23:58:02.240480 new-component-0.4.4/src/new_component/_jinja.py
+-rw-r--r--   0        0        0      249 2023-05-19 23:58:02.240480 new-component-0.4.4/src/new_component/_utils.py
+-rw-r--r--   0        0        0      663 2023-05-19 23:58:02.240480 new-component-0.4.4/src/new_component/_version.py
+-rw-r--r--   0        0        0     4121 2023-05-19 23:58:02.240480 new-component-0.4.4/src/new_component/cli.py
+-rw-r--r--   0        0        0      142 2023-05-19 23:58:02.244480 new-component-0.4.4/src/new_component/main.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:58:02.244480 new-component-0.4.4/src/new_component/py.typed
+-rw-r--r--   0        0        0      269 2023-05-19 23:58:02.244480 new-component-0.4.4/src/new_component/templates/component.js.j2
+-rw-r--r--   0        0        0       48 2023-05-19 23:58:02.244480 new-component-0.4.4/src/new_component/templates/index.js.j2
+-rw-r--r--   0        0        0        0 2023-05-19 23:58:02.244480 new-component-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     6215 2023-05-19 23:58:02.244480 new-component-0.4.4/tests/test_new_component.py
+-rw-r--r--   0        0        0      326 2023-05-19 23:58:02.244480 new-component-0.4.4/tests/test_version.py
+-rw-r--r--   0        0        0     5401 1970-01-01 00:00:00.000000 new-component-0.4.4/PKG-INFO
```

### Comparing `new-component-0.4.3/LICENSE` & `new-component-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `new-component-0.4.3/README.md` & `new-component-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `new-component-0.4.3/pyproject.toml` & `new-component-0.4.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 [project]
 name = "new_component"
-version = "0.4.3"
 description = "Quickly create opinionated Styled Components for React Projects"
 authors = [
     { name = "Ian Cleary", email = "github@iancleary.me" },
 ]
+dynamic = []
 requires-python = ">=3.11"
-readme = "README.md"
 dependencies = [
     "typer==0.9.0",
     "colorama==0.4.6",
     "shellingham==1.5.0.post1",
     "rich==13.3.5",
     "Jinja2==3.1.2",
 ]
+readme = "README.md"
+keywords = [
+    "script",
+    "javascript",
+    "styled-components",
+]
+classifiers = [
+    "Topic :: Software Development :: Code Generators",
+    "Programming Language :: Python :: 3.11",
+]
+version = "0.4.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://new-component.iancleary.me"
 Repository = "https://github.com/iancleary/new-component"
@@ -31,14 +41,15 @@
 write_to = "new_component/VERSION"
 write_template = "__version__ = '{}'"
 
 [tool.pdm.build]
 package-dir = "src"
 includes = [
     "src/new_component",
+    "src/new_component/templates/**.j2",
 ]
 source-includes = [
     "tests",
     "LICENSE",
     "README.md",
 ]
```

### Comparing `new-component-0.4.3/src/new_component/_config.py` & `new-component-0.4.4/src/new_component/_config.py`

 * *Files identical despite different names*

### Comparing `new-component-0.4.3/src/new_component/_confirms.py` & `new-component-0.4.4/src/new_component/_confirms.py`

 * *Files identical despite different names*

### Comparing `new-component-0.4.3/src/new_component/_constants.py` & `new-component-0.4.4/src/new_component/_constants.py`

 * *Files identical despite different names*

### Comparing `new-component-0.4.3/src/new_component/_echos.py` & `new-component-0.4.4/src/new_component/_echos.py`

 * *Files identical despite different names*

### Comparing `new-component-0.4.3/src/new_component/cli.py` & `new-component-0.4.4/src/new_component/cli.py`

 * *Files identical despite different names*

### Comparing `new-component-0.4.3/tests/test_new_component.py` & `new-component-0.4.4/tests/test_new_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
 import os
 import shutil
 from pathlib import Path
 
 from typer.testing import CliRunner
 
-from new_component import __app_name__, __version__, cli
+from new_component import __app_name__, cli
 from new_component._constants import (
     DEFAULT_COMPONENTS_DIR,
     DEFAULT_FILE_EXTENSION,
     GLOBAL_CONFIG_FILE,
     GLOBAL_CONFIG_PATH,
     LOCAL_CONFIG_FILE,
 )
+from new_component._version import read_version
 
 # ensure component directory is empty
 DEFAULT_COMPONENTS_DIR_PATH = Path(DEFAULT_COMPONENTS_DIR)
 if DEFAULT_COMPONENTS_DIR_PATH.exists():
     shutil.rmtree(path=DEFAULT_COMPONENTS_DIR)
 
 if LOCAL_CONFIG_FILE.exists():
@@ -28,15 +29,15 @@
 # create typer runner for testing
 runner = CliRunner()
 
 
 def test_version() -> None:
     result = runner.invoke(cli.app, ["--version"])
     assert result.exit_code == 0
-    assert f"{__app_name__} v{__version__}\n" in result.stdout
+    assert f"{__app_name__} v{read_version()}\n" in result.stdout
 
 
 def test_prompt_to_create_components_directory() -> None:
     result = runner.invoke(
         cli.app, ["Button"], input="y\n"
     )  # y to create components directory
     assert result.exit_code == 0
```

### Comparing `new-component-0.4.3/PKG-INFO` & `new-component-0.4.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: new_component
-Version: 0.4.3
+Version: 0.4.4
 Summary: Quickly create opinionated Styled Components for React Projects
 License: MIT
+Keywords: script,javascript,styled-components
 Author-email: Ian Cleary <github@iancleary.me>
 Requires-Python: >=3.11
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Code Generators
 Project-URL: Documentation, https://new-component.iancleary.me
 Project-URL: Homepage, https://new-component.iancleary.me
 Project-URL: Repository, https://github.com/iancleary/new-component
 Description-Content-Type: text/markdown
 
 # new-component
```

