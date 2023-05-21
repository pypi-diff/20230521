# Comparing `tmp/pybash-0.3.0.tar.gz` & `tmp/pybash-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybash-0.3.0.tar", max compression
+gzip compressed data, was "pybash-0.3.1.tar", max compression
```

## Comparing `pybash-0.3.0.tar` & `pybash-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1060 2023-05-14 00:39:18.698108 pybash-0.3.0/LICENSE
--rw-r--r--   0        0        0     3912 2023-05-14 00:39:18.698108 pybash-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-14 00:39:18.698108 pybash-0.3.0/pybash/__init__.py
--rw-r--r--   0        0        0      540 2023-05-14 00:39:18.698108 pybash-0.3.0/pybash/hook.py
--rw-r--r--   0        0        0    15403 2023-05-14 00:39:18.698108 pybash-0.3.0/pybash/transformer.py
--rw-r--r--   0        0        0      791 2023-05-14 00:39:18.698108 pybash-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4454 1970-01-01 00:00:00.000000 pybash-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-05-21 04:39:07.620456 pybash-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4057 2023-05-21 04:39:07.620456 pybash-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 04:39:07.620456 pybash-0.3.1/pybash/__init__.py
+-rw-r--r--   0        0        0      684 2023-05-21 04:39:07.620456 pybash-0.3.1/pybash/__main__.py
+-rw-r--r--   0        0        0      531 2023-05-21 04:39:07.620456 pybash-0.3.1/pybash/hook.py
+-rw-r--r--   0        0        0    15403 2023-05-21 04:39:07.620456 pybash-0.3.1/pybash/transformer.py
+-rw-r--r--   0        0        0      792 2023-05-21 04:39:07.620456 pybash-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4601 1970-01-01 00:00:00.000000 pybash-0.3.1/PKG-INFO
```

### Comparing `pybash-0.3.0/LICENSE` & `pybash-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybash-0.3.0/README.md` & `pybash-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,20 +19,31 @@
 
 ```python
 from pybash.transformer import transform
 
 transform(">echo hello world") # returns the python code for the bash command as string
 ```
 
-## As ideas hook
-`pip install "pybash[ideas]"`
+## As script runner
+`pip install "pybash[script]"`
 
-See [run.py](run.py) for an example.
 
-# Usage
+### Example 
+```py
+#
+text = "HELLO WORLD"
+>echo f{text}
+```
+
+### Run script:
+```bash
+$ python -m pybash hello.py
+```
+
+# Supported transforms
 
 ### 1. Simple execution with output
 ```python
 >python --version
 >echo \\nthis is an echo
 ```
 outputs:
@@ -151,11 +162,12 @@
 
 cp_test()
 ```
 
 # Dev
 
 #### Demo
-`python run.py`
+`python -m pybash examples/hello.py`
+`python -m pybash demo`
 
 #### Debug
 `make debug` to view the transformed source code
```

### Comparing `pybash-0.3.0/pybash/hook.py` & `pybash-0.3.1/pybash/hook.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def source_init():
     """Adds subprocess import"""
     return "import subprocess"
 
 
-def add_hook(**_kwargs):
+def add_hook():
     """Creates and automatically adds the import hook in sys.meta_path"""
     return import_hook.create_hook(
         hook_name=__name__,
         transform_source=transform_source,
         source_init=source_init,
     )
```

### Comparing `pybash-0.3.0/pybash/transformer.py` & `pybash-0.3.1/pybash/transformer.py`

 * *Files identical despite different names*

### Comparing `pybash-0.3.0/pyproject.toml` & `pybash-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "PyBash"
-version = "0.3.0"
+version = "0.3.1"
 description = ">execute bash commands from python easily"
 authors = ["Jay <jay.github0@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pybash"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ideas = { version = "^0.1.5", optional = true }
 token-utils = "^0.1.8"
 
 [tool.poetry.extras]
-ideas = ["ideas"]
+script = ["ideas"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pytest = "^7.2.1"
 isort = "^5.11.4"
 flake8 = "^6.0.0"
 autoflake = "^2.0.0"
```

### Comparing `pybash-0.3.0/PKG-INFO` & `pybash-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pybash
-Version: 0.3.0
+Version: 0.3.1
 Summary: >execute bash commands from python easily
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: ideas
-Requires-Dist: ideas (>=0.1.5,<0.2.0) ; extra == "ideas"
+Provides-Extra: script
+Requires-Dist: ideas (>=0.1.5,<0.2.0) ; extra == "script"
 Requires-Dist: token-utils (>=0.1.8,<0.2.0)
 Description-Content-Type: text/markdown
 
 # PyBash
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jaykv/pybash/python-app.yml?branch=main)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pybash)
@@ -35,20 +35,31 @@
 
 ```python
 from pybash.transformer import transform
 
 transform(">echo hello world") # returns the python code for the bash command as string
 ```
 
-## As ideas hook
-`pip install "pybash[ideas]"`
+## As script runner
+`pip install "pybash[script]"`
 
-See [run.py](run.py) for an example.
 
-# Usage
+### Example 
+```py
+#
+text = "HELLO WORLD"
+>echo f{text}
+```
+
+### Run script:
+```bash
+$ python -m pybash hello.py
+```
+
+# Supported transforms
 
 ### 1. Simple execution with output
 ```python
 >python --version
 >echo \\nthis is an echo
 ```
 outputs:
@@ -167,12 +178,13 @@
 
 cp_test()
 ```
 
 # Dev
 
 #### Demo
-`python run.py`
+`python -m pybash examples/hello.py`
+`python -m pybash demo`
 
 #### Debug
 `make debug` to view the transformed source code
```

