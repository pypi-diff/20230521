# Comparing `tmp/easyenergy-0.3.0.tar.gz` & `tmp/easyenergy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyenergy-0.3.0.tar", max compression
+gzip compressed data, was "easyenergy-0.3.1.tar", max compression
```

## Comparing `easyenergy-0.3.0.tar` & `easyenergy-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-03-31 13:16:03.604579 easyenergy-0.3.0/LICENSE
--rw-r--r--   0        0        0     7984 2023-03-31 13:16:03.604579 easyenergy-0.3.0/README.md
--rw-r--r--   0        0        0      385 2023-03-31 13:16:03.604579 easyenergy-0.3.0/easyenergy/__init__.py
--rw-r--r--   0        0        0      109 2023-03-31 13:16:03.604579 easyenergy-0.3.0/easyenergy/const.py
--rw-r--r--   0        0        0     8740 2023-03-31 13:16:03.604579 easyenergy-0.3.0/easyenergy/easyenergy.py
--rw-r--r--   0        0        0      296 2023-03-31 13:16:03.604579 easyenergy-0.3.0/easyenergy/exceptions.py
--rw-r--r--   0        0        0    10973 2023-03-31 13:16:03.604579 easyenergy-0.3.0/easyenergy/models.py
--rw-r--r--   0        0        0        0 2023-03-31 13:16:03.604579 easyenergy-0.3.0/easyenergy/py.typed
--rw-r--r--   0        0        0     3921 2023-03-31 13:16:18.116525 easyenergy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9519 1970-01-01 00:00:00.000000 easyenergy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-20 22:18:43.137088 easyenergy-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7984 2023-05-20 22:18:43.137088 easyenergy-0.3.1/README.md
+-rw-r--r--   0        0        0      385 2023-05-20 22:18:43.137088 easyenergy-0.3.1/easyenergy/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-20 22:18:43.137088 easyenergy-0.3.1/easyenergy/const.py
+-rw-r--r--   0        0        0     8740 2023-05-20 22:18:43.137088 easyenergy-0.3.1/easyenergy/easyenergy.py
+-rw-r--r--   0        0        0      296 2023-05-20 22:18:43.137088 easyenergy-0.3.1/easyenergy/exceptions.py
+-rw-r--r--   0        0        0    10973 2023-05-20 22:18:43.137088 easyenergy-0.3.1/easyenergy/models.py
+-rw-r--r--   0        0        0        0 2023-05-20 22:18:43.137088 easyenergy-0.3.1/easyenergy/py.typed
+-rw-r--r--   0        0        0     3832 2023-05-20 22:19:14.941422 easyenergy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     9375 1970-01-01 00:00:00.000000 easyenergy-0.3.1/PKG-INFO
```

### Comparing `easyenergy-0.3.0/LICENSE` & `easyenergy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easyenergy-0.3.0/README.md` & `easyenergy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `easyenergy-0.3.0/easyenergy/easyenergy.py` & `easyenergy-0.3.1/easyenergy/easyenergy.py`

 * *Files identical despite different names*

### Comparing `easyenergy-0.3.0/easyenergy/models.py` & `easyenergy-0.3.1/easyenergy/models.py`

 * *Files identical despite different names*

### Comparing `easyenergy-0.3.0/pyproject.toml` & `easyenergy-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,143 +1,137 @@
 [tool.poetry]
 name = "easyenergy"
-version = "0.3.0"
+version = "0.3.1"
 description = "Asynchronous Python client providing energy/gas prices from easyEnergy"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-easyenergy"
 repository = "https://github.com/klaasnicolaas/python-easyenergy"
 documentation = "https://github.com/klaasnicolaas/python-easyenergy"
 keywords = ["energy", "easyenergy", "gas", "prices", "api", "async", "client"]
 classifiers = [
-    "Framework :: AsyncIO",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+  "Development Status :: 5 - Production/Stable",
+  "Framework :: AsyncIO",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
-    { include = "easyenergy" }
+  { include = "easyenergy" }
 ]
 
 [tool.poetry.dependencies]
+aiodns = "^3.0.0"
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
-aiodns = "^3.0.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-easyenergy/issues"
 Changelog = "https://github.com/klaasnicolaas/python-easyenergy/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.243,<0.0.261"
-aresponses = "^2.1.6"
-black = "^22.12"
-blacken-docs = "^1.13.0"
-codespell = "^2.2.2"
-coverage = {version = ">=7.2,<8.0", extras = ["toml"]}
-mypy = ">=1.0,<1.2"
-pre-commit = "^3.0.3"
-pre-commit-hooks = "^4.4.0"
-pylint = "^2.16.1"
-pytest = "^7.2.1"
-pytest-asyncio = ">=0.20.3,<0.22.0"
-pytest-cov = "^4.0.0"
-pytest-freezer = "^0.4.6"
-safety = "^2.3.5"
-yamllint = "^1.29.0"
-pytz = ">=2022.6,<2024.0"
-covdefaults = "^2.2.2"
-types-pytz = ">=2022.7.1,<2024.0.0"
-
-[tool.black]
-target-version = ['py39']
-
-[tool.coverage.paths]
-source = ["easyenergy"]
+aresponses = "2.1.6"
+black = "23.3.0"
+blacken-docs = "1.13.0"
+codespell = "2.2.4"
+covdefaults = "2.3.0"
+coverage = {version = "7.2.5", extras = ["toml"]}
+mypy = "1.3.0"
+pre-commit = "3.3.2"
+pre-commit-hooks = "4.4.0"
+pylint = "2.17.4"
+pytest = "7.3.1"
+pytest-asyncio = "0.21.0"
+pytest-cov = "4.0.0"
+pytest-freezer = "0.4.6"
+pytz = "2023.3"
+ruff = "0.0.269"
+types-pytz = "2023.3.0.0"
+yamllint = "1.31.0"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["easyenergy"]
 
+[tool.coverage.report]
+fail_under = 90
+show_missing = true
+
 [tool.mypy]
 # Specify the target platform details in config, so your developers are
 # free to run mypy on Windows, Linux, or macOS and get consistent
 # results.
 platform = "linux"
 python_version = "3.9"
 
+# flake8-mypy expects the two following for sensible formatting
+show_column_numbers = true
+
 # show error messages from unrelated files
 follow_imports = "normal"
 
 # suppress errors about unsatisfied imports
 ignore_missing_imports = true
 
 # be strict
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
-disallow_untyped_defs = true
 disallow_untyped_decorators = true
+disallow_untyped_defs = true
 no_implicit_optional = true
 no_implicit_reexport = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-[tool.pylint.MASTER]
-extension-pkg-whitelist = [
-  "pydantic"
-]
-ignore= [
-  "tests"
-]
-
 [tool.pylint.BASIC]
 good-names = [
-    "_",
-    "ex",
-    "fp",
-    "i",
-    "id",
-    "j",
-    "k",
-    "on",
-    "Run",
-    "T",
+  "_",
+  "ex",
+  "fp",
+  "i",
+  "id",
+  "j",
+  "k",
+  "on",
+  "Run",
+  "T",
+  "wv",
 ]
 
-[tool.pylint.DESIGN]
-max-attributes = 8
-
 [tool.pylint."MESSAGES CONTROL"]
 disable= [
-    "duplicate-code",
-    "format",
-    "unsubscriptable-object",
+  "duplicate-code",
+  "format",
+  "unsubscriptable-object",
 ]
 
 [tool.pylint.SIMILARITIES]
 ignore-imports = true
 
 [tool.pylint.FORMAT]
-max-line-length=88
+max-line-length = 88
+
+[tool.pylint.DESIGN]
+max-attributes = 8
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
 [tool.ruff]
 select = ["ALL"]
@@ -157,9 +151,9 @@
 [tool.ruff.isort]
 known-first-party = ["easyenergy"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `easyenergy-0.3.0/PKG-INFO` & `easyenergy-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: easyenergy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Asynchronous Python client providing energy/gas prices from easyEnergy
 Home-page: https://github.com/klaasnicolaas/python-easyenergy
 License: MIT
 Keywords: energy,easyenergy,gas,prices,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
 Maintainer-email: hello@student-techlife.com
 Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.0.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-easyenergy/issues
 Project-URL: Changelog, https://github.com/klaasnicolaas/python-easyenergy/releases
 Project-URL: Documentation, https://github.com/klaasnicolaas/python-easyenergy
```

