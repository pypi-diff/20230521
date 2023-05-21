# Comparing `tmp/utilki-0.2.1.tar.gz` & `tmp/utilki-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.2.1.tar", max compression
+gzip compressed data, was "utilki-0.3.0.tar", max compression
```

## Comparing `utilki-0.2.1.tar` & `utilki-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.2.1/README.md
--rw-r--r--   0        0        0      532 2023-05-19 16:45:21.125911 utilki-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.2.1/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.2.1/utilki/cli.py
--rw-r--r--   0        0        0     4982 2023-05-19 16:44:45.084982 utilki-0.2.1/utilki/task_mixin.py
--rw-r--r--   0        0        0     1848 2023-05-19 16:45:27.512269 utilki-0.2.1/setup.py
--rw-r--r--   0        0        0     1510 2023-05-19 16:45:27.512461 utilki-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.0/README.md
+-rw-r--r--   0        0        0      525 2023-05-21 16:08:41.934991 utilki-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.3.0/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.0/utilki/cli.py
+-rw-r--r--   0        0        0     4982 2023-05-19 16:44:45.084982 utilki-0.3.0/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1846 2023-05-21 16:09:07.748099 utilki-0.3.0/setup.py
+-rw-r--r--   0        0        0     1608 2023-05-21 16:09:07.748276 utilki-0.3.0/PKG-INFO
```

### Comparing `utilki-0.2.1/README.md` & `utilki-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.2.1/pyproject.toml` & `utilki-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "utilki"
-version = "0.2.1"
+version = "0.3.0"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1"
+python = ">=3.7"
 click = "^8.1.3"
 pydantic = "^1.10.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 black = "^23.3.0"
-flake8 = "^6.0.0"
+flake8 = "*"
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `utilki-0.2.1/utilki/cli.py` & `utilki-0.3.0/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.2.1/utilki/task_mixin.py` & `utilki-0.3.0/utilki/task_mixin.py`

 * *Files identical despite different names*

### Comparing `utilki-0.2.1/setup.py` & `utilki-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 ['click>=8.1.3,<9.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utilki = utilki.cli:cli']}
 
 setup_kwargs = {
     'name': 'utilki',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'A collection of useful utilities',
     'long_description': '# utilki\n\n[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)\n\nutils that are frequently used by me and might be useful for others\n\n## installation\n\n```bash\npip install utilki\n```\n\n## TaskMixin\n\nMixin class that adds `create()` classmethod to dataclass you define as your task params. Useful when you have a lot of container based tasks executed on remote clusters (e.g. Kubernetes, Hashicorp Nomad, etc.). It reads task params from environment variables, parses, and validates them. \n\n```python\nfrom utilki import TaskMixin\n\n@dataclass\nclass Task(TaskMixin):\n    ayy: float = 69.69\n    lmao: str = "420"\n\nos.environ["ayy"] = "42.42"\nos.environ["lmao"] = "69"\n\nt = Task.create()\nprint(f"ayy: {t.ayy}, type: {type(t.ayy)}")\n# ayy: 42.42, type: <class \'float\'>\nprint(f"lmao: {t.lmao}, type: {type(t.lmao)}")\n# lmao: 69, type: <class \'str\'>\n```\n\n## Cli\n\n### Venv\n\n```bash\n$ utilki venv 3.8.10\n$ Enter venv name: new_venv\n$ Created venv `new_venv` with Python version 3.8.10\n```',
     'author': 'Khaidar Bikmaev',
     'author_email': 'khaidar@bikmaev.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8.1',
+    'python_requires': '>=3.7',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `utilki-0.2.1/PKG-INFO` & `utilki-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.2.1
+Version: 0.3.0
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
-Requires-Python: >=3.8.1
+Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown
 
 # utilki
```

