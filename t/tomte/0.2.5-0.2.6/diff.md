# Comparing `tmp/tomte-0.2.5.tar.gz` & `tmp/tomte-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomte-0.2.5.tar", max compression
+gzip compressed data, was "tomte-0.2.6.tar", max compression
```

## Comparing `tomte-0.2.5.tar` & `tomte-0.2.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1063 2022-10-01 14:11:14.626018 tomte-0.2.5/LICENSE
--rw-r--r--   0        0        0     2855 2023-05-21 15:30:21.552974 tomte-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-21 15:30:38.331472 tomte-0.2.5/tomte/__init__.py
--rw-r--r--   0        0        0     2829 2023-05-21 15:29:39.235525 tomte-0.2.5/tomte/cli.py
--rw-r--r--   0        0        0      876 2022-09-11 16:56:11.417175 tomte-0.2.5/tomte/tools/__init__.py
--rwxr-xr-x   0        0        0    11371 2023-05-21 15:29:26.911765 tomte-0.2.5/tomte/tools/check_copyright.py
--rwxr-xr-x   0        0        0     6967 2023-05-21 15:29:39.322671 tomte-0.2.5/tomte/tools/check_doc_links.py
--rwxr-xr-x   0        0        0     1678 2023-05-21 10:59:04.565876 tomte-0.2.5/tomte/tools/check_readme.py
--rwxr-xr-x   0        0        0     1348 2023-05-21 15:29:26.914379 tomte-0.2.5/tomte/tools/freeze_dependencies.py
--rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 tomte-0.2.5/setup.py
--rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 tomte-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-10-01 14:11:14.626018 tomte-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2856 2023-05-21 15:38:36.444320 tomte-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-21 15:38:41.437413 tomte-0.2.6/tomte/__init__.py
+-rw-r--r--   0        0        0     2829 2023-05-21 15:29:39.235525 tomte-0.2.6/tomte/cli.py
+-rw-r--r--   0        0        0      876 2022-09-11 16:56:11.417175 tomte-0.2.6/tomte/tools/__init__.py
+-rwxr-xr-x   0        0        0    11371 2023-05-21 15:29:26.911765 tomte-0.2.6/tomte/tools/check_copyright.py
+-rwxr-xr-x   0        0        0     6967 2023-05-21 15:29:39.322671 tomte-0.2.6/tomte/tools/check_doc_links.py
+-rwxr-xr-x   0        0        0     1678 2023-05-21 10:59:04.565876 tomte-0.2.6/tomte/tools/check_readme.py
+-rwxr-xr-x   0        0        0     1348 2023-05-21 15:29:26.914379 tomte-0.2.6/tomte/tools/freeze_dependencies.py
+-rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 tomte-0.2.6/setup.py
+-rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 tomte-0.2.6/PKG-INFO
```

### Comparing `tomte-0.2.5/LICENSE` & `tomte-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tomte-0.2.5/pyproject.toml` & `tomte-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomte"
-version = "0.2.5"
+version = "0.2.6"
 description = "A library that wraps many useful tools (linters, analysers, etc) to keep Python code clean, secure, well-documented and optimised."
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 tox = {version = "==3.28.0", optional = true}
@@ -36,15 +36,15 @@
 pytest-rerunfailures = {version = "==11.0", optional = true}
 bs4 = {version = "==0.0.1", optional = true}
 Pygments = {version = "==2.14.0", optional = true}
 liccheck = {version = "==0.8.3", optional = true}
 
 # don't change unless changed on open-aea
 click = {version = "==8.0.2", optional = true}
-requests = {version = "^2.30.0", optional = true}
+requests = {version = "==2.28.2", optional = true}
 
 [tool.poetry.extras]
 black = ["black", "click"]
 bandit = ["bandit"]
 cli = ["click", "requests", "tox"]
 isort = ["isort"]
 flake8 = ["flake8", "flake8-bugbear", "flake8-docstrings", "flake8-eradicate", "flake8-isort", "pydocstyle"]
```

### Comparing `tomte-0.2.5/tomte/cli.py` & `tomte-0.2.6/tomte/cli.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.5/tomte/tools/__init__.py` & `tomte-0.2.6/tomte/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.5/tomte/tools/check_copyright.py` & `tomte-0.2.6/tomte/tools/check_copyright.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.5/tomte/tools/check_doc_links.py` & `tomte-0.2.6/tomte/tools/check_doc_links.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.5/tomte/tools/check_readme.py` & `tomte-0.2.6/tomte/tools/check_readme.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.5/tomte/tools/freeze_dependencies.py` & `tomte-0.2.6/tomte/tools/freeze_dependencies.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.5/setup.py` & `tomte-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 package_data = \
 {'': ['*']}
 
 extras_require = \
 {'bandit': ['bandit==1.7.4'],
  'black': ['black==22.12.0', 'click==8.0.2'],
- 'cli': ['tox==3.28.0', 'click==8.0.2', 'requests>=2.30.0,<3.0.0'],
+ 'cli': ['tox==3.28.0', 'click==8.0.2', 'requests==2.28.2'],
  'darglint': ['darglint==1.8.1'],
  'docs': ['mkdocs==1.4.2',
           'mkdocs-material==9.0.4',
           'mkdocs-macros-plugin==0.7.0',
           'Markdown==3.3.7',
           'markdown-include==0.8.0',
           'pydoc-markdown==4.6.4',
@@ -43,15 +43,15 @@
  'vulture': ['vulture==2.7']}
 
 entry_points = \
 {'console_scripts': ['tomte = tomte.cli:cli']}
 
 setup_kwargs = {
     'name': 'tomte',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'A library that wraps many useful tools (linters, analysers, etc) to keep Python code clean, secure, well-documented and optimised.',
     'long_description': 'None',
     'author': 'David Minarsch',
     'author_email': 'david.minarsch@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tomte-0.2.5/PKG-INFO` & `tomte-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomte
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library that wraps many useful tools (linters, analysers, etc) to keep Python code clean, secure, well-documented and optimised.
 License: MIT
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -51,11 +51,11 @@
 Requires-Dist: pylint (==2.13.9) ; extra == "pylint"
 Requires-Dist: pymdown-extensions (==9.9.1) ; extra == "docs"
 Requires-Dist: pytest (==7.2.1) ; extra == "tests"
 Requires-Dist: pytest-asyncio (==0.20.3) ; extra == "tests"
 Requires-Dist: pytest-cov (==4.0.0) ; extra == "tests"
 Requires-Dist: pytest-randomly (==3.12.0) ; extra == "tests"
 Requires-Dist: pytest-rerunfailures (==11.0) ; extra == "tests"
-Requires-Dist: requests (>=2.30.0,<3.0.0) ; extra == "cli"
+Requires-Dist: requests (==2.28.2) ; extra == "cli"
 Requires-Dist: safety (==2.3.5) ; extra == "safety"
 Requires-Dist: tox (==3.28.0) ; extra == "cli" or extra == "tox"
 Requires-Dist: vulture (==2.7) ; extra == "vulture"
```

