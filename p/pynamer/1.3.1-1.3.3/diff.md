# Comparing `tmp/pynamer-1.3.1.tar.gz` & `tmp/pynamer-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-1.3.1.tar", last modified: Wed May 17 16:09:52 2023, max compression
+gzip compressed data, was "pynamer-1.3.3.tar", last modified: Sun May 21 16:33:50 2023, max compression
```

## Comparing `pynamer-1.3.1.tar` & `pynamer-1.3.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.338316 pynamer-1.3.1/
--rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-1.3.1/AUTHORS.md
--rw-rw-rw-   0        0        0     8219 2023-05-17 16:09:37.000000 pynamer-1.3.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0    18474 2023-05-17 16:09:52.338316 pynamer-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    16952 2023-05-16 18:56:04.000000 pynamer-1.3.1/README.md
--rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     1840 2023-05-17 16:09:52.338316 pynamer-1.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.215853 pynamer-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.253662 pynamer-1.3.1/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-13 20:08:21.000000 pynamer-1.3.1/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1895 2023-05-17 16:09:37.000000 pynamer-1.3.1/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0      754 2023-05-15 18:15:27.000000 pynamer-1.3.1/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.269311 pynamer-1.3.1/src/pynamer/project_name/
--rw-rw-rw-   0        0        0       37 2023-05-13 20:08:54.000000 pynamer-1.3.1/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0    34592 2023-05-17 11:05:22.000000 pynamer-1.3.1/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      401 2023-05-17 16:00:31.000000 pynamer-1.3.1/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-15 18:15:27.000000 pynamer-1.3.1/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0     1594 2023-05-16 19:07:11.000000 pynamer-1.3.1/src/pynamer/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.269311 pynamer-1.3.1/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    18474 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 16:09:52.000000 pynamer-1.3.1/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 16:09:52.338316 pynamer-1.3.1/tests/
--rw-rw-rw-   0        0        0     1869 2023-05-15 11:23:19.000000 pynamer-1.3.1/tests/test_args.py
--rw-rw-rw-   0        0        0     1923 2023-05-12 17:32:19.000000 pynamer-1.3.1/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1080 2023-05-12 17:31:19.000000 pynamer-1.3.1/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1018 2023-05-17 16:03:17.000000 pynamer-1.3.1/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1587 2023-05-15 18:15:27.000000 pynamer-1.3.1/tests/test_defaults.py
--rw-rw-rw-   0        0        0      538 2023-05-12 17:32:19.000000 pynamer-1.3.1/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-15 11:23:19.000000 pynamer-1.3.1/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2698 2023-05-09 14:10:02.000000 pynamer-1.3.1/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-12 17:32:19.000000 pynamer-1.3.1/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1259 2023-05-12 17:31:19.000000 pynamer-1.3.1/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0      282 2023-05-12 16:17:19.000000 pynamer-1.3.1/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     1664 2023-05-11 09:16:33.000000 pynamer-1.3.1/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1496 2023-05-11 08:50:00.000000 pynamer-1.3.1/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-12 17:31:19.000000 pynamer-1.3.1/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1117 2023-05-12 17:31:19.000000 pynamer-1.3.1/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      405 2023-05-12 17:32:19.000000 pynamer-1.3.1/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      737 2023-05-08 13:03:26.000000 pynamer-1.3.1/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      882 2023-05-12 17:32:19.000000 pynamer-1.3.1/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1617 2023-05-15 13:42:17.000000 pynamer-1.3.1/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-12 17:31:19.000000 pynamer-1.3.1/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-05-21 16:33:50.136540 pynamer-1.3.3/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-1.3.3/AUTHORS.md
+-rw-rw-rw-   0        0        0     9132 2023-05-21 16:33:33.000000 pynamer-1.3.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    18662 2023-05-21 16:33:50.136540 pynamer-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    17536 2023-05-21 12:10:39.000000 pynamer-1.3.3/README.md
+-rw-rw-rw-   0        0        0     2071 2023-05-21 12:45:00.000000 pynamer-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1893 2023-05-21 16:33:50.136540 pynamer-1.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 16:33:49.762366 pynamer-1.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 16:33:49.855265 pynamer-1.3.3/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-1.3.3/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1807 2023-05-21 16:33:34.000000 pynamer-1.3.3/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0      754 2023-05-21 12:10:39.000000 pynamer-1.3.3/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-05-21 16:33:49.870903 pynamer-1.3.3/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-1.3.3/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0    35223 2023-05-21 12:10:39.000000 pynamer-1.3.3/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      401 2023-05-21 16:30:10.000000 pynamer-1.3.3/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-1.3.3/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0     1641 2023-05-21 12:10:39.000000 pynamer-1.3.3/src/pynamer/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-21 16:33:49.870903 pynamer-1.3.3/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    18662 2023-05-21 16:33:49.000000 pynamer-1.3.3/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1053 2023-05-21 16:33:49.000000 pynamer-1.3.3/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 16:33:49.000000 pynamer-1.3.3/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-21 16:33:49.000000 pynamer-1.3.3/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2023-05-21 16:33:49.000000 pynamer-1.3.3/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 16:33:49.000000 pynamer-1.3.3/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 16:33:50.136540 pynamer-1.3.3/tests/
+-rw-rw-rw-   0        0        0     1869 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_args.py
+-rw-rw-rw-   0        0        0     1923 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1080 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0      978 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1587 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      538 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1450 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     1721 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      517 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      764 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      882 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1671 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-1.3.3/tests/test_write_output_file.py
```

### Comparing `pynamer-1.3.1/CHANGELOG.md` & `pynamer-1.3.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.3 (2023-05-21)
+
+
+## v1.3.2 (2023-05-21)
+### Fix
+* Add .pre-commit-config.yaml to mypy config ([`514c74f`](https://github.com/Stephen-RA-King/pynamer/commit/514c74f06091f4e28d82f4bd937aa44f4c552753))
+* Remove function in minimalist __init__ ([`1d74fbb`](https://github.com/Stephen-RA-King/pynamer/commit/1d74fbb18265b13ee25d7c49a03705e6284985c2))
+* Type hint annotations for importlib traversible ([`a579dca`](https://github.com/Stephen-RA-King/pynamer/commit/a579dcab34862fc72e21726316ca9e685cd84938))
+
+### Documentation
+* Update help text ([`c763420`](https://github.com/Stephen-RA-King/pynamer/commit/c763420d2a24b5fb682a4d61288e873a8019d8c6))
+* Minor updates ([`145ddcd`](https://github.com/Stephen-RA-King/pynamer/commit/145ddcde8fd1e8680180689cff6c9f644a52204b))
+* Update badges ([`b6eec6c`](https://github.com/Stephen-RA-King/pynamer/commit/b6eec6c88896c50d1e81eb3c9e5bd24208cab1fc))
+
 ## v1.3.1 (2023-05-17)
 ### Fix
 * Restore text in setup ([`087d094`](https://github.com/Stephen-RA-King/pynamer/commit/087d094a554a9c70738fefe57e4f469e08252b48))
 
 ### Documentation
 * Update readme images ([`392ec09`](https://github.com/Stephen-RA-King/pynamer/commit/392ec09379268bca7f85b40d0319a4fec8a5a1c4))
```

### Comparing `pynamer-1.3.1/LICENSE` & `pynamer-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/PKG-INFO` & `pynamer-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 1.3.1
+Version: 1.3.3
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
 Keywords: utility
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -28,22 +29,21 @@
 
 _**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
-[![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
+[![CodeQl][codeql-image]][codeql-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
+[![readthedocs][readthedocs-image]][readthedocs-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
-[![CodeQl][codeql-image]][codeql-url]
-[![readthedocs][readthedocs-image]][readthedocs-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
@@ -149,15 +149,14 @@
 ---
 
 ### Prerequisites
 
 ---
 
 -   [x] Python >= 3.9.
--   [x] [**pipx**](https://pypa.github.io/pipx/)
 
 The following are optional but required for 'registering' a project name on PyPI
 
 -   [x] An account on PyPI (and generate a PyPI API token).
 -   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API key
 
     or
@@ -175,14 +174,22 @@
 repository = https://upload.pypi.org/legacy/
 username = __token__
 password = your_API_token_here
 ```
 
 ### Installation
 
+Pynamer can be installed into any python environment using pip:
+
+```bash
+~ $ pip install pynamer
+```
+
+However, optimal installation can be archived using [**pipx**][pipx-url]:
+
 ```bash
 ~ $ pipx install pynamer
 ```
 
 ### Basic Usage
 
 #### A package name that is not available
@@ -227,15 +234,15 @@
 positional arguments:
   projects              Optional - one or more project names
 
 optional arguments:
   -h, --help            show this help message and exit
   -r, --register        register the name on PyPi if the name is available
   -v, --verbose         display information about similar projects
-  -g, --generate        generate a new PyPI simple index
+  -g, --generate        generate a new PyPI index file
   -m, --meta            input new meta data when registering (Author and email address)
   -w, --webbrowser      open the project on PyPI in a webbrowser
   --version             display version number
   -f FILE, --file FILE  file containing a list of projects to analyze
   -o OUTPUT, --output OUTPUT
                         file to store the test results
 ```
@@ -444,27 +451,28 @@
 [codeql-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynamer/?ref=repository-badge
-[downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
+[downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynamer
 [format-image]: https://img.shields.io/pypi/format/pynamer
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/context:python
 [license-image]: https://img.shields.io/pypi/l/pynamer
 [license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
 [pypi-url]: https://pypi.org/project/pynamer/
 [pypi-image]: https://img.shields.io/pypi/v/pynamer.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynamer
```

### Comparing `pynamer-1.3.1/README.md` & `pynamer-1.3.3/src/pynamer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,448 +1,484 @@
-_**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
-
-[![PyPI][pypi-image]][pypi-url]
-[![Downloads][downloads-image]][downloads-url]
-[![Status][status-image]][pypi-url]
-[![Python Version][python-version-image]][pypi-url]
-[![Format][format-image]][pypi-url]
-[![tests][tests-image]][tests-url]
-[![Codecov][codecov-image]][codecov-url]
-[![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
-[![CodeFactor][codefactor-image]][codefactor-url]
-[![Codeclimate][codeclimate-image]][codeclimate-url]
-[![CodeQl][codeql-image]][codeql-url]
-[![readthedocs][readthedocs-image]][readthedocs-url]
-[![Imports: isort][isort-image]][isort-url]
-[![Code style: black][black-image]][black-url]
-[![Checked with mypy][mypy-image]][mypy-url]
-[![security: bandit][bandit-image]][bandit-url]
-[![Commitizen friendly][commitizen-image]][commitizen-url]
-[![Conventional Commits][conventional-commits-image]][conventional-commits-url]
-[![DeepSource][deepsource-image]][deepsource-url]
-[![license][license-image]][license-url]
-
-As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' on PyPI.
-
-![](assets/pynamer.png)
-
-# Contents
-
--   [tl;dr](#TLDR)
--   [Introduction](#Introduction)
--   [Quick Start](#Quick-Start)
-    -   [Prerequisites](#Prerequisites)
-    -   [Installation](#Installation)
-    -   [Basic Usage](#Basic-Usage)
--   [Usage](#Usage)
-    -   [Specifying multiple names](#Specifying-multiple-names)
-    -   [Using an input file](#Using-an-input-file)
-    -   [Saving the results to a file](#Saving-the-results-to-a-file)
-    -   [Register the name with PyPI](#Register-the-name-with-PyPI)
-    -   [Verbose output](#Verbose-output)
-    -   [Regenerate the PyPI simple Repository Index](#Regenerate-the-PyPI-simple-Repository-Index)
--   [The oddities](#The-Oddities)
--   [Limitations](#Limitations)
--   [Documentation](#Documentation)
-    -   [Read the Docs](https://pynamer.readthedocs.io/en/latest/)
-    -   [API](https://pynamer.readthedocs.io/en/latest/autoapi/pynamer/pynamer/index.html)
-    -   [Wiki](https://github.com/Stephen-RA-King/pynamer/wiki)
--   [Planned Future improvements](#Planned-Future-improvements)
-
-## Introduction
-
-### Project Rationale
-
-Some of you may have reached the point where you want to publish a package on the PyPI python repository.
-The first step of which is to choose a unique name. Here lies the problem.
-
-A recent look at the PyPI repository revealed there were over 453,769 projects, so many names have already been taken.
-
-pip leaps to the rescue with its search utility... or does it?
-
-```python
-pip search zaphod
-```
-
-```bash
-ERROR: XMLRPC request failed [code: -32500]
-RuntimeError: PyPI no longer supports 'pip search' (or XML-RPC search).
-Please use https://pypi.org/search (via a browser) instead.
-See https://warehouse.pypa.io/api-reference/xml-rpc.html#deprecated-methods for more information.
-```
-
-A quick search will show the internet replete with articles explaining the situation:
-
--   [The Register: Why Python's pip search isn't working](https://www.theregister.com/2021/05/25/pypi_search_error/)
--   [Python.org discussion: Pip search is still broken](https://discuss.python.org/t/pip-search-is-still-broken/18680)
-
-OK so I go to the PyPI website and do a search for 'zaphod' as suggested by pip and 7 results are displayed none of which have the package name 'zaphod'
-
-![](assets/pypi_zaphod.png)
-
-Fantastic! I now think unbelievably that I have a unique name for a project that I can use.
-So, I go ahead and code my new project, along with all the test files, documentation and meta data.
-I diligently debug and commit and push to git and github so I have a history.
-
-Finally the project is good enough to release and publish as an installable package on PyPI.
-
-Here goes....
-
-```bash
-~ $ python -m twine upload --config-file .pypirc dist/*
-Uploading distributions to https://upload.pypi.org/legacy/
-Uploading zaphod-0.0.0-py3-none-any.whl
-100% ---------------------------------------- 3.8/3.8 kB • 00:00 • ?
-WARNING  Error during upload. Retry with the --verbose option for more details.
-ERROR    HTTPError: 403 Forbidden from https://upload.pypi.org/legacy/
-         The user 'stephenking' isn't allowed to upload to project 'zaphod'. See https://pypi.org/help/#project-name for more information.
-```
-
-AARGH!
-
-What just happened?
-
-Yes unbelievably the project already exists and yes unbelievably PyPI's own search
-did not find the project.
-
-Enter Pynamer. Pynamer does not rely on a single method of finding a PyPI package:
-
-#### TLDR
-
-Pynamer uses the following methods to ascertain whether a package already exists on PyPI:
-
--   A simple request to the project url on PyPI.
--   Uses the PyPI "simple" repository - a text-based listing of all the packages available on PyPI.
--   Uses PyPI's own search 'API' and scrapes the results.
-
-Pynamer provides a way to optionally 'register' a name on PyPI by building a minimalistic package and uploading
-
-## Quick Start
-
----
-
-### Prerequisites
-
----
-
--   [x] Python >= 3.9.
--   [x] [**pipx**](https://pypa.github.io/pipx/)
-
-The following are optional but required for 'registering' a project name on PyPI
-
--   [x] An account on PyPI (and generate a PyPI API token).
--   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API key
-
-    or
-
--   [x] [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
-
-Your .pypirc file should contain the following and be on your PATH:
-
-```file
-[distutils]
-index-servers =
-    pypi
-
-[pypi]
-repository = https://upload.pypi.org/legacy/
-username = __token__
-password = your_API_token_here
-```
-
-### Installation
-
-```bash
-~ $ pipx install pynamer
-```
-
-### Basic Usage
-
-#### A package name that is not available
-
-```bash
-~ $ pynamer pynball
-```
-
-![](assets/usage_pynball.png)
-
-#### A package name that is available
-
-```bash
-~ $ pynamer allitnil
-```
-
-![](assets/usage_available.png)
-
-Holy smoke batman! You've managed to identify a unique name.
-
-Yes, even though the odds were against you (given there are over 450,000+ registered projects), you did it!
-
-Even though the name has nothing in common with your project, or may not even be a real word... you did it!
-
-Congratulations!
-
-# Usage
-
----
-
-Display the help menu with the -h argument
-
-```bash
-~ $ pynamer -h
-```
-
-```bash
-usage: pynamer [-h] [-r] [-v] [-g] [-m] [-w] [--version] [-f FILE] [-o OUTPUT] [projects ...]
-
-Determine if project name is available on pypi with the option to 'register' it for future use if available
-
-positional arguments:
-  projects              Optional - one or more project names
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -r, --register        register the name on PyPi if the name is available
-  -v, --verbose         display information about similar projects
-  -g, --generate        generate a new PyPI simple index
-  -m, --meta            input new meta data when registering (Author and email address)
-  -w, --webbrowser      open the project on PyPI in a webbrowser
-  --version             display version number
-  -f FILE, --file FILE  file containing a list of projects to analyze
-  -o OUTPUT, --output OUTPUT
-                        file to store the test results
-```
-
-## Specifying multiple names
-
-You can specify as many names as you like from the command line e.g.
-
-```bash
-~ $ pynamer ganymede europa callisto
-```
-
-## Using an input file
-
-You can use the -f argument to specify a file containing the a names of projects to analyze.
-You specify a space separated sequence of as many names as you like on as many lines as you like. e.g.
-
-'projects' file
-
-```file
-ganymede europa
-IO callisto
-```
-
-Then specify the -f argument
-
-```bash
-~ $ pynamer -f projects
-```
-
-You can use the input file with names from the command line. The names will be aggregated. e.g.
-
-```bash
-~ $ pynamer ersa pandia leda metis -f projects
-```
-
-## Saving the results to a file
-
-You can specify a file to write the result to by using the -o argument. e.g.
-
-```bash
-~ $ pynamer ersa pandia leda -o results
-```
-
-This will write a file e.g.
-
-results
-
-```file
-Result from pynamer PyPI utility 2023-05-02
--------------------------------------------
-test 1 - Basic url lookup on PyPI
-test 2 - Search of PyPIs simple index
-test 3 - Search using an request to PyPIs search 'API'.
-
-Project name    Test1      Test2        Test 3          Conclusion
--------------------------------------------------------------------
-ersa            Found       Found       Found           Not Available
-pandia          Not Found   Not Found   Found           Not Available
-leda            Not Found   Not Found   Not Found       Available
-```
-
-Again you can use a combination of names from the command line and input file.
-
-## Register the package name with PyPI
-
-You can optionally 'register' the name on PyPI by using the -r argument.
-If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
-to PyPI.
-
-The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
-You can also optionally choose to change the version and description.
-
-![](assets/usage_register_first.png)
-
-This information will be retained and you will not be prompted to enter this information again. However, you can regenerate
-this meta data by using the -m argument along with the -r argument. You can just enter on the options you dont want to change.
-
-![](assets/usage_register_meta.png)
-
-```bash
-~ $ pynamer agrajag -r
-```
-
-![](assets/usage_register.png)
-
-## Verbose output
-
-ith the -v argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
-The algorithm that PyPI uses to select these in unknown but seems to be a mixture of names and other
-projects written by the same author.
-
-```bash
-~ $ pynamer pynamer -v
-```
-
-![](assets/usage_verbose.png)
-
-## Regenerate the PyPI simple Repository Index
-
-As one of its tests Pynamer makes use of a list of package names scraped from its simple index site.
-
-The PyPI Simple Index is a plain text file that lists the names of all the packages available on PyPI.
-
-It is a simplified version of the PyPI index that makes it easier for users to browse and download packages.
-
-The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
-The Index is updated every few hours.
-
-Using the -g argument can be used to regenerate the local file contents.
-
-```bash
-~ $ pynamer -g
-```
-
-![](assets/usage_generate.png)
-
-See planned future improvements
-
-## The Oddities
-
-The reason I wrote this application in the first place...
-
-```bash
-~ $ pynamer zaphod
-```
-
-![](assets/usage_zaphod.png)
-
-Even worse ...
-
-```bash
-~ $ pynamer zem
-```
-
-![](assets/usage_zem.png)
-
-## Limitations
-
-There will be occasions where all the tests pass, the name appears to be available but the upload to PyPI still fails.
-This can be several reasons for this:
-
--   You are trying to use an internally "reserved" keyword for PyPI.
--   The name you are using is too similar to an existing project name and you get the following error message:
-
-```bash
-...
-Error during upload. Retry with the --verbose option for more details.
-HTTPError: 400 Bad Request from https://test.pypi.org/legacy/
-The name 'yourpackage' is too similar to an existing project. See https://test.pypi.org/help/#project-name for more information-
-```
-
-Using a name similar to to an existing package name is a security issue.
-
-Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
-e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found at GitHub: [warehouse](https://github.com/pypi/warehouse).
-
-## Documentation
-
----
-
-[**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
-
--   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
--   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
--   [**Changelog**](https://pynamer.readthedocs.io/en/latest/changelog.html)
--   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
-
-[**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
-
-## Planned Future improvements
-
--   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
-
-## Meta
-
----
-
-[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
-[![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/pynamer)
-[![](assets/www.png)](https://www.justpython.tech)
-[![](assets/email.png)](mailto:sking.github@gmail.com)
-
-Stephen R A King : [sking.github@gmail.com](sking.github@gmail.com)
-
-Distributed under the MIT license. See [![][license-image]][license-url] for more information.
-
-Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
-
-<!-- Markdown link & img dfn's -->
-
-[bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
-[bandit-url]: https://github.com/PyCQA/bandit
-[black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-url]: https://github.com/psf/black
-[pydough-url]: https://github.com/Stephen-RA-King/pydough
-[codeclimate-image]: https://api.codeclimate.com/v1/badges/b95fb617fbcd469ccfc3/maintainability
-[codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynamer/maintainability
-[codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynamer/maintainability
-[codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynamer/branch/main/graph/badge.svg
-[codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynamer
-[codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer/badge
-[codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer
-[codeql-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql/badge.svg
-[codeql-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql
-[commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
-[commitizen-url]: http://commitizen.github.io/cz-cli/
-[conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
-[conventional-commits-url]: https://conventionalcommits.org
-[deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
-[deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynamer/?ref=repository-badge
-[downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
-[downloads-url]: https://pepy.tech/project/pynamer
-[format-image]: https://img.shields.io/pypi/format/pynamer
-[isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
-[isort-url]: https://github.com/pycqa/isort/
-[lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
-[lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
-[lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
-[lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/context:python
-[license-image]: https://img.shields.io/pypi/l/pynamer
-[license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/LICENSE
-[mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
-[mypy-url]: http://mypy-lang.org/
-[pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
-[pre-commit-url]: https://github.com/pre-commit/pre-commit
-[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
-[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
-[pypi-url]: https://pypi.org/project/pynamer/
-[pypi-image]: https://img.shields.io/pypi/v/pynamer.svg
-[python-version-image]: https://img.shields.io/pypi/pyversions/pynamer
-[readthedocs-image]: https://readthedocs.org/projects/pynamer/badge/?version=latest
-[readthedocs-url]: https://pynamer.readthedocs.io/en/latest/?badge=latest
-[status-image]: https://img.shields.io/pypi/status/pynamer.svg
-[tests-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/tests.yml/badge.svg
-[tests-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/tests.yml
-[wiki]: https://github.com/Stephen-RA-King/pynamer/wiki
+Metadata-Version: 2.1
+Name: pynamer
+Version: 1.3.3
+Summary: Utility to find an available package name on the PyPI repository and register it
+Home-page: https://github.com/Stephen-RA-King/pynamer
+Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
+Author: Stephen R A King
+Author-email: sking.github@gmail.com
+Maintainer: Stephen R A King
+Maintainer-email: sking.github@gmail.com
+License: MIT
+Keywords: utility
+Platform: Any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
+_**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
+
+[![PyPI][pypi-image]][pypi-url]
+[![Downloads][downloads-image]][downloads-url]
+[![Status][status-image]][pypi-url]
+[![Python Version][python-version-image]][pypi-url]
+[![tests][tests-image]][tests-url]
+[![Codecov][codecov-image]][codecov-url]
+[![CodeQl][codeql-image]][codeql-url]
+[![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
+[![readthedocs][readthedocs-image]][readthedocs-url]
+[![CodeFactor][codefactor-image]][codefactor-url]
+[![Codeclimate][codeclimate-image]][codeclimate-url]
+[![Imports: isort][isort-image]][isort-url]
+[![Code style: black][black-image]][black-url]
+[![Checked with mypy][mypy-image]][mypy-url]
+[![security: bandit][bandit-image]][bandit-url]
+[![Commitizen friendly][commitizen-image]][commitizen-url]
+[![Conventional Commits][conventional-commits-image]][conventional-commits-url]
+[![DeepSource][deepsource-image]][deepsource-url]
+[![license][license-image]][license-url]
+
+As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' on PyPI.
+
+![](assets/pynamer.png)
+
+# Contents
+
+-   [tl;dr](#TLDR)
+-   [Introduction](#Introduction)
+-   [Quick Start](#Quick-Start)
+    -   [Prerequisites](#Prerequisites)
+    -   [Installation](#Installation)
+    -   [Basic Usage](#Basic-Usage)
+-   [Usage](#Usage)
+    -   [Specifying multiple names](#Specifying-multiple-names)
+    -   [Using an input file](#Using-an-input-file)
+    -   [Saving the results to a file](#Saving-the-results-to-a-file)
+    -   [Register the name with PyPI](#Register-the-name-with-PyPI)
+    -   [Verbose output](#Verbose-output)
+    -   [Regenerate the PyPI simple Repository Index](#Regenerate-the-PyPI-simple-Repository-Index)
+-   [The oddities](#The-Oddities)
+-   [Limitations](#Limitations)
+-   [Documentation](#Documentation)
+    -   [Read the Docs](https://pynamer.readthedocs.io/en/latest/)
+    -   [API](https://pynamer.readthedocs.io/en/latest/autoapi/pynamer/pynamer/index.html)
+    -   [Wiki](https://github.com/Stephen-RA-King/pynamer/wiki)
+-   [Planned Future improvements](#Planned-Future-improvements)
+
+## Introduction
+
+### Project Rationale
+
+Some of you may have reached the point where you want to publish a package on the PyPI python repository.
+The first step of which is to choose a unique name. Here lies the problem.
+
+A recent look at the PyPI repository revealed there were over 453,769 projects, so many names have already been taken.
+
+pip leaps to the rescue with its search utility... or does it?
+
+```python
+pip search zaphod
+```
+
+```bash
+ERROR: XMLRPC request failed [code: -32500]
+RuntimeError: PyPI no longer supports 'pip search' (or XML-RPC search).
+Please use https://pypi.org/search (via a browser) instead.
+See https://warehouse.pypa.io/api-reference/xml-rpc.html#deprecated-methods for more information.
+```
+
+A quick search will show the internet replete with articles explaining the situation:
+
+-   [The Register: Why Python's pip search isn't working](https://www.theregister.com/2021/05/25/pypi_search_error/)
+-   [Python.org discussion: Pip search is still broken](https://discuss.python.org/t/pip-search-is-still-broken/18680)
+
+OK so I go to the PyPI website and do a search for 'zaphod' as suggested by pip and 7 results are displayed none of which have the package name 'zaphod'
+
+![](assets/pypi_zaphod.png)
+
+Fantastic! I now think unbelievably that I have a unique name for a project that I can use.
+So, I go ahead and code my new project, along with all the test files, documentation and meta data.
+I diligently debug and commit and push to git and github so I have a history.
+
+Finally the project is good enough to release and publish as an installable package on PyPI.
+
+Here goes....
+
+```bash
+~ $ python -m twine upload --config-file .pypirc dist/*
+Uploading distributions to https://upload.pypi.org/legacy/
+Uploading zaphod-0.0.0-py3-none-any.whl
+100% ---------------------------------------- 3.8/3.8 kB • 00:00 • ?
+WARNING  Error during upload. Retry with the --verbose option for more details.
+ERROR    HTTPError: 403 Forbidden from https://upload.pypi.org/legacy/
+         The user 'stephenking' isn't allowed to upload to project 'zaphod'. See https://pypi.org/help/#project-name for more information.
+```
+
+AARGH!
+
+What just happened?
+
+Yes unbelievably the project already exists and yes unbelievably PyPI's own search
+did not find the project.
+
+Enter Pynamer. Pynamer does not rely on a single method of finding a PyPI package:
+
+#### TLDR
+
+Pynamer uses the following methods to ascertain whether a package already exists on PyPI:
+
+-   A simple request to the project url on PyPI.
+-   Uses the PyPI "simple" repository - a text-based listing of all the packages available on PyPI.
+-   Uses PyPI's own search 'API' and scrapes the results.
+
+Pynamer provides a way to optionally 'register' a name on PyPI by building a minimalistic package and uploading
+
+## Quick Start
+
+---
+
+### Prerequisites
+
+---
+
+-   [x] Python >= 3.9.
+
+The following are optional but required for 'registering' a project name on PyPI
+
+-   [x] An account on PyPI (and generate a PyPI API token).
+-   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API key
+
+    or
+
+-   [x] [Twine environment variables](https://twine.readthedocs.io/en/latest/#environment-variables)
+
+Your .pypirc file should contain the following and be on your PATH:
+
+```file
+[distutils]
+index-servers =
+    pypi
+
+[pypi]
+repository = https://upload.pypi.org/legacy/
+username = __token__
+password = your_API_token_here
+```
+
+### Installation
+
+Pynamer can be installed into any python environment using pip:
+
+```bash
+~ $ pip install pynamer
+```
+
+However, optimal installation can be archived using [**pipx**][pipx-url]:
+
+```bash
+~ $ pipx install pynamer
+```
+
+### Basic Usage
+
+#### A package name that is not available
+
+```bash
+~ $ pynamer pynball
+```
+
+![](assets/usage_pynball.png)
+
+#### A package name that is available
+
+```bash
+~ $ pynamer allitnil
+```
+
+![](assets/usage_available.png)
+
+Holy smoke batman! You've managed to identify a unique name.
+
+Yes, even though the odds were against you (given there are over 450,000+ registered projects), you did it!
+
+Even though the name has nothing in common with your project, or may not even be a real word... you did it!
+
+Congratulations!
+
+# Usage
+
+---
+
+Display the help menu with the -h argument
+
+```bash
+~ $ pynamer -h
+```
+
+```bash
+usage: pynamer [-h] [-r] [-v] [-g] [-m] [-w] [--version] [-f FILE] [-o OUTPUT] [projects ...]
+
+Determine if project name is available on pypi with the option to 'register' it for future use if available
+
+positional arguments:
+  projects              Optional - one or more project names
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -r, --register        register the name on PyPi if the name is available
+  -v, --verbose         display information about similar projects
+  -g, --generate        generate a new PyPI index file
+  -m, --meta            input new meta data when registering (Author and email address)
+  -w, --webbrowser      open the project on PyPI in a webbrowser
+  --version             display version number
+  -f FILE, --file FILE  file containing a list of projects to analyze
+  -o OUTPUT, --output OUTPUT
+                        file to store the test results
+```
+
+## Specifying multiple names
+
+You can specify as many names as you like from the command line e.g.
+
+```bash
+~ $ pynamer ganymede europa callisto
+```
+
+## Using an input file
+
+You can use the -f argument to specify a file containing the a names of projects to analyze.
+You specify a space separated sequence of as many names as you like on as many lines as you like. e.g.
+
+'projects' file
+
+```file
+ganymede europa
+IO callisto
+```
+
+Then specify the -f argument
+
+```bash
+~ $ pynamer -f projects
+```
+
+You can use the input file with names from the command line. The names will be aggregated. e.g.
+
+```bash
+~ $ pynamer ersa pandia leda metis -f projects
+```
+
+## Saving the results to a file
+
+You can specify a file to write the result to by using the -o argument. e.g.
+
+```bash
+~ $ pynamer ersa pandia leda -o results
+```
+
+This will write a file e.g.
+
+results
+
+```file
+Result from pynamer PyPI utility 2023-05-02
+-------------------------------------------
+test 1 - Basic url lookup on PyPI
+test 2 - Search of PyPIs simple index
+test 3 - Search using an request to PyPIs search 'API'.
+
+Project name    Test1      Test2        Test 3          Conclusion
+-------------------------------------------------------------------
+ersa            Found       Found       Found           Not Available
+pandia          Not Found   Not Found   Found           Not Available
+leda            Not Found   Not Found   Not Found       Available
+```
+
+Again you can use a combination of names from the command line and input file.
+
+## Register the package name with PyPI
+
+You can optionally 'register' the name on PyPI by using the -r argument.
+If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
+to PyPI.
+
+The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
+You can also optionally choose to change the version and description.
+
+![](assets/usage_register_first.png)
+
+This information will be retained and you will not be prompted to enter this information again. However, you can regenerate
+this meta data by using the -m argument along with the -r argument. You can just enter on the options you dont want to change.
+
+![](assets/usage_register_meta.png)
+
+```bash
+~ $ pynamer agrajag -r
+```
+
+![](assets/usage_register.png)
+
+## Verbose output
+
+ith the -v argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
+The algorithm that PyPI uses to select these in unknown but seems to be a mixture of names and other
+projects written by the same author.
+
+```bash
+~ $ pynamer pynamer -v
+```
+
+![](assets/usage_verbose.png)
+
+## Regenerate the PyPI simple Repository Index
+
+As one of its tests Pynamer makes use of a list of package names scraped from its simple index site.
+
+The PyPI Simple Index is a plain text file that lists the names of all the packages available on PyPI.
+
+It is a simplified version of the PyPI index that makes it easier for users to browse and download packages.
+
+The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
+The Index is updated every few hours.
+
+Using the -g argument can be used to regenerate the local file contents.
+
+```bash
+~ $ pynamer -g
+```
+
+![](assets/usage_generate.png)
+
+See planned future improvements
+
+## The Oddities
+
+The reason I wrote this application in the first place...
+
+```bash
+~ $ pynamer zaphod
+```
+
+![](assets/usage_zaphod.png)
+
+Even worse ...
+
+```bash
+~ $ pynamer zem
+```
+
+![](assets/usage_zem.png)
+
+## Limitations
+
+There will be occasions where all the tests pass, the name appears to be available but the upload to PyPI still fails.
+This can be several reasons for this:
+
+-   You are trying to use an internally "reserved" keyword for PyPI.
+-   The name you are using is too similar to an existing project name and you get the following error message:
+
+```bash
+...
+Error during upload. Retry with the --verbose option for more details.
+HTTPError: 400 Bad Request from https://test.pypi.org/legacy/
+The name 'yourpackage' is too similar to an existing project. See https://test.pypi.org/help/#project-name for more information-
+```
+
+Using a name similar to to an existing package name is a security issue.
+
+Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
+e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found at GitHub: [warehouse](https://github.com/pypi/warehouse).
+
+## Documentation
+
+---
+
+[**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
+
+-   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
+-   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
+-   [**Changelog**](https://pynamer.readthedocs.io/en/latest/changelog.html)
+-   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
+
+## Planned Future improvements
+
+-   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
+
+## Meta
+
+---
+
+[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
+[![](assets/github.png)](https://github.com/Stephen-RA-King)
+[![](assets/pypi.png)](https://pypi.org/project/pynamer)
+[![](assets/www.png)](https://www.justpython.tech)
+[![](assets/email.png)](mailto:sking.github@gmail.com)
+
+Stephen R A King : [sking.github@gmail.com](sking.github@gmail.com)
+
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
+
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
+
+<!-- Markdown link & img dfn's -->
+
+[bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
+[bandit-url]: https://github.com/PyCQA/bandit
+[black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
+[black-url]: https://github.com/psf/black
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
+[codeclimate-image]: https://api.codeclimate.com/v1/badges/b95fb617fbcd469ccfc3/maintainability
+[codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynamer/maintainability
+[codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynamer/maintainability
+[codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynamer/branch/main/graph/badge.svg
+[codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynamer
+[codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer/badge
+[codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer
+[codeql-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql/badge.svg
+[codeql-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql
+[commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
+[commitizen-url]: http://commitizen.github.io/cz-cli/
+[conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
+[conventional-commits-url]: https://conventionalcommits.org
+[deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
+[deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynamer/?ref=repository-badge
+[downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
+[downloads-url]: https://pepy.tech/project/pynamer
+[format-image]: https://img.shields.io/pypi/format/pynamer
+[isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+[isort-url]: https://github.com/pycqa/isort/
+[lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
+[lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
+[lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
+[lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/context:python
+[license-image]: https://img.shields.io/pypi/l/pynamer
+[license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/LICENSE
+[mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
+[mypy-url]: http://mypy-lang.org/
+[pipx-url]: https://pypa.github.io/pipx/
+[pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+[pre-commit-url]: https://github.com/pre-commit/pre-commit
+[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
+[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
+[pypi-url]: https://pypi.org/project/pynamer/
+[pypi-image]: https://img.shields.io/pypi/v/pynamer.svg
+[python-version-image]: https://img.shields.io/pypi/pyversions/pynamer
+[readthedocs-image]: https://readthedocs.org/projects/pynamer/badge/?version=latest
+[readthedocs-url]: https://pynamer.readthedocs.io/en/latest/?badge=latest
+[status-image]: https://img.shields.io/pypi/status/pynamer.svg
+[tests-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/tests.yml/badge.svg
+[tests-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/tests.yml
+[wiki]: https://github.com/Stephen-RA-King/pynamer/wiki
```

### Comparing `pynamer-1.3.1/pyproject.toml` & `pynamer-1.3.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,98 @@
-[build-system]
-requires = [
-    "setuptools",
-    "wheel"
-]
-build-backend = "setuptools.build_meta"
-
-[tool]
-[tool.black]
-line-length = 88
-
-[tool.cruft]
-skip = [
-    "tests/",
-    "src/",
-    "*/header.png",
-    ".pypirc",
-    "CHANGELOG.md",
-    "setup.cfg"
-]
-
-[tool.pytest.ini_options]
-# https://docs.pytest.org/en/6.2.x/reference.html?highlight=minversion#configuration-options
-minversion = "6.0"
-testpaths = [
-    "tests",
-]
-
-[tool.isort]
-import_heading_stdlib = "Core Library modules"
-import_heading_thirdparty = "Third party modules"
-import_heading_firstparty = "First party modules"
-import_heading_localfolder = "Local modules"
-include_trailing_comma = true
-indent = '    '
-known_third_party = [
-    "click",
-    "pytest",
-    "setuptools",
-    "pip-tools",
-    "pre-commit"
-]
-known_first_party = [
-    "pathmagic"
-]
-line_length = 80
-multi_line_output = 3
-force_grid_wrap = 0
-use_parentheses = true
-ensure_newline_before_comments = true
-balanced_wrapping = true
-combine_as_imports = true
-
-[tool.mypy]
-ignore_missing_imports = true
-check_untyped_defs = true
-disallow_untyped_defs = false
-warn_unused_ignores = true
-strict_optional = true
-warn_redundant_casts = true
-warn_unused_configs = true
-disallow_untyped_calls = false
-disallow_incomplete_defs = true
-follow_imports = "skip"
-html_report = "mypy-report"
-mypy_path = "typeshed/pyi:typeshed/imports"
-
-[tool.semantic_release]
-version_variable = [
-    "src/pynamer/__init__.py:__version__",
-    "docs/conf.py:version",
-]
-branch = "main"
-changelog_file = "CHANGELOG.md"
-build_command = "python -m build"
-dist_path = "dist/"
-upload_to_pypi = true
-upload_to_repository = true
-remove_dist = true
-version_source = "tag"
-commit_message = "chore: generate by PSR"
-
-[tool.flakeheaven]
-# base = "https://raw.githubusercontent.com/flakeheaven/flakeheaven/main/pyproject.toml"
-exclude = ["example.py"]
-format = "grouped"
-max_line_length = 80
-show_source = true
-
-[tool.flakeheaven.plugins]
-pyflakes = ["+*", "-F401"]
-"flake8-*" = ["+*"]
-mccabe = ["+*"]
-pep8-naming = ["+*"]
-pycodestyle = ["+*"]
-pylint = ["+F*", "+E*", "-E0611", "-E1101", "-E0401", "-E1102", "-E1123"]
-
-[tool.coverage.run]
-branch = true
-parallel = true
-
-[tool.coverage.report]
-show_missing = true
-precision = 2
-skip_empty = true
+[build-system]
+requires = [
+    "setuptools",
+    "wheel"
+]
+build-backend = "setuptools.build_meta"
+
+[tool]
+[tool.black]
+line-length = 88
+
+[tool.cruft]
+skip = [
+    "tests/",
+    "src/",
+    "*/header.png",
+    ".pypirc",
+    "CHANGELOG.md",
+    "setup.cfg"
+]
+
+[tool.isort]
+import_heading_stdlib = "Core Library modules"
+import_heading_thirdparty = "Third party modules"
+import_heading_firstparty = "First party modules"
+import_heading_localfolder = "Local modules"
+include_trailing_comma = true
+indent = '    '
+known_third_party = [
+    "click",
+    "pytest",
+    "setuptools",
+    "pip-tools",
+    "pre-commit"
+]
+known_first_party = [
+    "pathmagic"
+]
+line_length = 80
+multi_line_output = 3
+force_grid_wrap = 0
+use_parentheses = true
+ensure_newline_before_comments = true
+balanced_wrapping = true
+combine_as_imports = true
+
+[tool.mypy]
+ignore_missing_imports = true
+check_untyped_defs = true
+disallow_untyped_defs = false
+warn_unused_ignores = true
+strict_optional = true
+warn_redundant_casts = true
+warn_unused_configs = true
+disallow_untyped_calls = false
+disallow_incomplete_defs = true
+follow_imports = "skip"
+html_report = "mypy-report"
+mypy_path = "typeshed/pyi:typeshed/imports"
+
+[tool.semantic_release]
+version_variable = [
+    "src/pynamer/__init__.py:__version__",
+    "docs/conf.py:version",
+]
+branch = "main"
+changelog_file = "CHANGELOG.md"
+build_command = "python -m build"
+dist_path = "dist/"
+upload_to_pypi = true
+upload_to_repository = true
+remove_dist = true
+version_source = "tag"
+commit_message = "chore: generate by PSR"
+
+[tool.flakeheaven]
+# base = "https://raw.githubusercontent.com/flakeheaven/flakeheaven/main/pyproject.toml"
+exclude = ["example.py"]
+format = "grouped"
+max_line_length = 80
+show_source = true
+
+[tool.flakeheaven.plugins]
+pyflakes = ["+*", "-F401"]
+"flake8-*" = ["+*"]
+mccabe = ["+*"]
+pep8-naming = ["+*"]
+pycodestyle = ["+*"]
+pylint = ["+F*", "+E*", "-E0611", "-E1101", "-E0401", "-E1102", "-E1123"]
+
+[tool.coverage.run]
+branch = true
+parallel = true
+
+[tool.coverage.report]
+show_missing = true
+precision = 2
+skip_empty = true
```

### Comparing `pynamer-1.3.1/setup.cfg` & `pynamer-1.3.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -37,79 +37,83 @@
 00000240: 6173 7369 6669 6572 7320 3d20 0d0a 0944  assifiers = ...D
 00000250: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
 00000260: 7320 3a3a 2035 202d 2050 726f 6475 6374  s :: 5 - Product
 00000270: 696f 6e2f 5374 6162 6c65 0d0a 0945 6e76  ion/Stable...Env
 00000280: 6972 6f6e 6d65 6e74 203a 3a20 436f 6e73  ironment :: Cons
 00000290: 6f6c 650d 0a09 496e 7465 6e64 6564 2041  ole...Intended A
 000002a0: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-000002b0: 6f70 6572 730d 0a09 4f70 6572 6174 696e  opers...Operatin
-000002c0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-000002d0: 6e64 6570 656e 6465 6e74 0d0a 094e 6174  ndependent...Nat
-000002e0: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
-000002f0: 2045 6e67 6c69 7368 0d0a 0950 726f 6772   English...Progr
-00000300: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000310: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-00000320: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000330: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000340: 3a3a 2033 203a 3a20 4f6e 6c79 0d0a 0950  :: 3 :: Only...P
-00000350: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000360: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000370: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
-00000380: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000390: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
+000002b0: 6f70 6572 730d 0a09 4c69 6365 6e73 6520  opers...License 
+000002c0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000002d0: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+000002e0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+000002f0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000300: 656e 740d 0a09 4e61 7475 7261 6c20 4c61  ent...Natural La
+00000310: 6e67 7561 6765 203a 3a20 456e 676c 6973  nguage :: Englis
+00000320: 680d 0a09 5072 6f67 7261 6d6d 696e 6720  h...Programming 
+00000330: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000340: 6f6e 203a 3a20 330d 0a09 5072 6f67 7261  on :: 3...Progra
+00000350: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000360: 3a20 5079 7468 6f6e 203a 3a20 3320 3a3a  : Python :: 3 ::
+00000370: 204f 6e6c 790d 0a09 5072 6f67 7261 6d6d   Only...Programm
+00000380: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000390: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
 000003a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 000003b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000003c0: 3a20 332e 3131 0d0a 0d0a 5b6f 7074 696f  : 3.11....[optio
-000003d0: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
-000003e0: 203d 200d 0a09 3d73 7263 0d0a 7061 636b   = ...=src..pack
-000003f0: 6167 6573 203d 2066 696e 643a 0d0a 7072  ages = find:..pr
-00000400: 6f6a 6563 745f 7572 6c73 203d 200d 0a69  oject_urls = ..i
-00000410: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-00000420: 6174 6120 3d20 5472 7565 0d0a 7079 7468  ata = True..pyth
-00000430: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000440: 332e 390d 0a69 6e73 7461 6c6c 5f72 6571  3.9..install_req
-00000450: 7569 7265 7320 3d20 0d0a 096a 696e 6a61  uires = ...jinja
-00000460: 320d 0a09 6273 340d 0a09 6275 696c 640d  2...bs4...build.
-00000470: 0a09 636f 6c6f 7261 6d61 0d0a 0970 7979  ..colorama...pyy
-00000480: 616d 6c0d 0a09 7265 7175 6573 7473 0d0a  aml...requests..
-00000490: 0972 6963 680d 0a09 7477 696e 650d 0a09  .rich...twine...
-000004a0: 7471 646d 0d0a 0977 6865 656c 0d0a 0d0a  tqdm...wheel....
-000004b0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-000004c0: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-000004d0: 2073 7263 0d0a 0d0a 5b6f 7074 696f 6e73   src....[options
-000004e0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
-000004f0: 7079 6e61 6d65 7220 3d20 0d0a 0952 4541  pynamer = ...REA
-00000500: 444d 452e 6d64 0d0a 0963 6f6e 6669 672e  DME.md...config.
-00000510: 7079 0d0a 0970 726f 6a65 6374 5f63 6f75  py...project_cou
-00000520: 6e74 2e70 6963 6b6c 650d 0a09 7072 6f6a  nt.pickle...proj
-00000530: 6563 745f 6e61 6d65 0d0a 0970 726f 6a65  ect_name...proje
-00000540: 6374 5f6e 616d 652f 5f5f 696e 6974 5f5f  ct_name/__init__
-00000550: 2e70 790d 0a09 7365 7475 702e 7478 740d  .py...setup.txt.
-00000560: 0a09 7365 7475 705f 6261 7365 2e74 7874  ..setup_base.txt
-00000570: 0d0a 0975 7469 6c73 2e70 790d 0a0d 0a5b  ...utils.py....[
-00000580: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-00000590: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
-000005a0: 6372 6970 7473 203d 200d 0a09 7079 6e61  cripts = ...pyna
-000005b0: 6d65 7220 3d20 7079 6e61 6d65 722e 7079  mer = pynamer.py
-000005c0: 6e61 6d65 723a 6d61 696e 0d0a 0d0a 5b66  namer:main....[f
-000005d0: 6c61 6b65 385d 0d0a 646f 6373 7472 696e  lake8]..docstrin
-000005e0: 672d 636f 6e76 656e 7469 6f6e 203d 206e  g-convention = n
-000005f0: 756d 7079 0d0a 6d61 782d 636f 6d70 6c65  umpy..max-comple
-00000600: 7869 7479 203d 2031 380d 0a6d 6178 2d6c  xity = 18..max-l
-00000610: 696e 652d 6c65 6e67 7468 203d 2038 380d  ine-length = 88.
-00000620: 0a73 656c 6563 7420 3d20 422c 2042 392c  .select = B, B9,
-00000630: 2043 2c20 442c 2045 2c20 462c 204e 2c20   C, D, E, F, N, 
-00000640: 570d 0a65 7863 6c75 6465 203d 2074 6573  W..exclude = tes
-00000650: 7473 2f2a 2c2e 746f 782f 2a2c 2e6e 6f78  ts/*,.tox/*,.nox
-00000660: 2f2a 2c64 6f63 732f 2a2c 2e67 6974 2f2a  /*,docs/*,.git/*
-00000670: 2c2e 6769 7468 7562 2f2a 0d0a 6967 6e6f  ,.github/*..igno
-00000680: 7265 203d 200d 0a09 4532 3033 2c0d 0a09  re = ...E203,...
-00000690: 5735 3033 2c0d 0a09 4634 3031 2c0d 0a70  W503,...F401,..p
-000006a0: 6572 2d66 696c 652d 6967 6e6f 7265 7320  er-file-ignores 
-000006b0: 3d20 0d0a 095f 5f69 6e69 745f 5f2e 7079  = ...__init__.py
-000006c0: 3a46 3430 310d 0a09 7061 7468 6d61 6769  :F401...pathmagi
-000006d0: 632e 7079 3a46 3430 310d 0a09 7465 7374  c.py:F401...test
-000006e0: 5f70 796e 616d 6572 2e70 793a 4634 3031  _pynamer.py:F401
-000006f0: 0d0a 0970 796e 616d 6572 2e70 793a 4634  ...pynamer.py:F4
-00000700: 3031 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  01....[egg_info]
-00000710: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000720: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+000003c0: 3a20 332e 3130 0d0a 0950 726f 6772 616d  : 3.10...Program
+000003d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000003e0: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
+000003f0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
+00000400: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
+00000410: 7372 630d 0a70 6163 6b61 6765 7320 3d20  src..packages = 
+00000420: 6669 6e64 3a0d 0a70 726f 6a65 6374 5f75  find:..project_u
+00000430: 726c 7320 3d20 0d0a 696e 636c 7564 655f  rls = ..include_
+00000440: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
+00000450: 7275 650d 0a70 7974 686f 6e5f 7265 7175  rue..python_requ
+00000460: 6972 6573 203d 203e 3d33 2e39 0d0a 696e  ires = >=3.9..in
+00000470: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000480: 200d 0a09 6273 340d 0a09 6275 696c 640d   ...bs4...build.
+00000490: 0a09 636f 6c6f 7261 6d61 0d0a 096a 696e  ..colorama...jin
+000004a0: 6a61 320d 0a09 7061 636b 6167 696e 670d  ja2...packaging.
+000004b0: 0a09 7079 7961 6d6c 0d0a 0972 6571 7565  ..pyyaml...reque
+000004c0: 7374 730d 0a09 7269 6368 0d0a 0974 7164  sts...rich...tqd
+000004d0: 6d0d 0a09 7477 696e 650d 0a09 7768 6565  m...twine...whee
+000004e0: 6c0d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  l....[options.pa
+000004f0: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+00000500: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
+00000510: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+00000520: 7461 5d0d 0a70 796e 616d 6572 203d 200d  ta]..pynamer = .
+00000530: 0a09 5245 4144 4d45 2e6d 640d 0a09 636f  ..README.md...co
+00000540: 6e66 6967 2e70 790d 0a09 7072 6f6a 6563  nfig.py...projec
+00000550: 745f 636f 756e 742e 7069 636b 6c65 0d0a  t_count.pickle..
+00000560: 0970 726f 6a65 6374 5f6e 616d 650d 0a09  .project_name...
+00000570: 7072 6f6a 6563 745f 6e61 6d65 2f5f 5f69  project_name/__i
+00000580: 6e69 745f 5f2e 7079 0d0a 0973 6574 7570  nit__.py...setup
+00000590: 2e74 7874 0d0a 0973 6574 7570 5f62 6173  .txt...setup_bas
+000005a0: 652e 7478 740d 0a09 7574 696c 732e 7079  e.txt...utils.py
+000005b0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
+000005c0: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
+000005d0: 6f6c 655f 7363 7269 7074 7320 3d20 0d0a  ole_scripts = ..
+000005e0: 0970 796e 616d 6572 203d 2070 796e 616d  .pynamer = pynam
+000005f0: 6572 2e70 796e 616d 6572 3a6d 6169 6e0d  er.pynamer:main.
+00000600: 0a0d 0a5b 666c 616b 6538 5d0d 0a64 6f63  ...[flake8]..doc
+00000610: 7374 7269 6e67 2d63 6f6e 7665 6e74 696f  string-conventio
+00000620: 6e20 3d20 6e75 6d70 790d 0a6d 6178 2d63  n = numpy..max-c
+00000630: 6f6d 706c 6578 6974 7920 3d20 3138 0d0a  omplexity = 18..
+00000640: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
+00000650: 3d20 3838 0d0a 7365 6c65 6374 203d 2042  = 88..select = B
+00000660: 2c20 4239 2c20 432c 2044 2c20 452c 2046  , B9, C, D, E, F
+00000670: 2c20 4e2c 2057 0d0a 6578 636c 7564 6520  , N, W..exclude 
+00000680: 3d20 7465 7374 732f 2a2c 2e74 6f78 2f2a  = tests/*,.tox/*
+00000690: 2c2e 6e6f 782f 2a2c 646f 6373 2f2a 2c2e  ,.nox/*,docs/*,.
+000006a0: 6769 742f 2a2c 2e67 6974 6875 622f 2a0d  git/*,.github/*.
+000006b0: 0a69 676e 6f72 6520 3d20 0d0a 0945 3230  .ignore = ...E20
+000006c0: 332c 0d0a 0957 3530 332c 0d0a 0946 3430  3,...W503,...F40
+000006d0: 312c 0d0a 7065 722d 6669 6c65 2d69 676e  1,..per-file-ign
+000006e0: 6f72 6573 203d 200d 0a09 5f5f 696e 6974  ores = ...__init
+000006f0: 5f5f 2e70 793a 4634 3031 0d0a 0970 6174  __.py:F401...pat
+00000700: 686d 6167 6963 2e70 793a 4634 3031 0d0a  hmagic.py:F401..
+00000710: 0974 6573 745f 7079 6e61 6d65 722e 7079  .test_pynamer.py
+00000720: 3a46 3430 310d 0a09 7079 6e61 6d65 722e  :F401...pynamer.
+00000730: 7079 3a46 3430 310d 0a0d 0a5b 6567 675f  py:F401....[egg_
+00000740: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000750: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000760: 300d 0a0d 0a                             0....
```

### Comparing `pynamer-1.3.1/src/pynamer/config.py` & `pynamer-1.3.3/src/pynamer/config.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/src/pynamer/pynamer.py` & `pynamer-1.3.3/src/pynamer/pynamer.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,34 +9,44 @@
 import re
 import shutil
 import string
 import subprocess
 import sys
 import webbrowser
 from datetime import datetime
+from importlib.resources import as_file, files
 from pathlib import Path
 from typing import Any, Union
 
 # Third party modules
 import build
 import requests
 from bs4 import BeautifulSoup
 from colorama import Back, Fore, Style
 from jinja2 import Template
 from rich.console import Console
 from rich.table import Table
 from tqdm import tqdm
 
 # Local modules
-from . import meta, project_count, project_path, setup_text
+from . import (
+    meta,
+    meta_file_trv,
+    project_count,
+    project_count_file_trv,
+    project_path,
+    pypi_index_file_trv,
+    setup_base_file_trv,
+    setup_file_trv,
+    setup_text,
+)
 from .config import config
 from .utils import _check_version
 
 logger = logging.getLogger()
-project_path = Path(str(project_path))
 
 
 def _feedback(message: str, feedback_type: str) -> None:
     """Generates a formatted messages appropriate to the message type.
 
     Args:
         message:        Text to be echoed.
@@ -117,18 +127,15 @@
 
     The object being to create a setup.py file from a 'template' file for the purpose of
     creating a minimalist package for upload to PyPI.
 
     Args:
         new_project_name:       name used to render the template.
     """
-    meta_file = Path(project_path / "meta.pickle")
-    setup_file = Path(project_path / "setup.txt")
-    setup_base_file = Path(project_path / "setup_base.txt")
-    setup_file_py = Path(project_path / "setup.py")
+    setup_file_py_trv = project_path / "setup.py"
 
     author = meta["author"] if meta else ""
     email = meta["email"] if meta else ""
     description = meta["description"] if meta else config.description
     version = meta["version"] if meta else config.package_version
 
     _email_pattern = (
@@ -147,15 +154,15 @@
                         + f"please enter your author name ({author}): "
                         + Style.RESET_ALL
                     )
                     or author
                 )
                 if author != "":
                     break
-        except KeyboardInterrupt:
+        except KeyboardInterrupt:  # pragma: no cover
             _feedback("...bye!", "warning")
             raise SystemExit()
 
         try:
             while True:
                 email = (
                     input(
@@ -172,16 +179,16 @@
                 else:
                     print(
                         Fore.YELLOW
                         + Back.BLACK
                         + Style.BRIGHT
                         + "does not appear to be a valid email address"
                         + Style.RESET_ALL
-                    )
-        except KeyboardInterrupt:
+                    )  # pragma: no cover
+        except KeyboardInterrupt:  # pragma: no cover
             _feedback("...bye!", "warning")
             raise SystemExit()
 
         try:
             while True:
                 version = (
                     input(
@@ -191,15 +198,15 @@
                         + f"version number: ({version}): "
                         + Style.RESET_ALL
                     )
                     or version
                 )
                 if version != "":
                     break
-        except KeyboardInterrupt:
+        except KeyboardInterrupt:  # pragma: no cover
             raise SystemExit("Bye!")
 
         try:
             while True:
                 description = (
                     input(
                         Fore.YELLOW
@@ -208,54 +215,52 @@
                         + f"description: ({description}): "
                         + Style.RESET_ALL
                     )
                     or description
                 )
                 if description != "":
                     break
-        except KeyboardInterrupt:
+        except KeyboardInterrupt:  # pragma: no cover
             raise SystemExit("Bye!")
 
-        setup_file.unlink()
-
-        with open(setup_base_file, encoding="utf-8") as f:
-            setup_text_base = f.read()
+        with as_file(setup_file_trv) as setup_file:
+            if setup_file.exists():
+                setup_file.unlink(missing_ok=True)
 
+        setup_text_base = setup_base_file_trv.read_text(encoding="utf-8")
         template = Template(setup_text_base)
         content = template.render(
             PROJECT_NAME="{{ PROJECT_NAME }}",
             PACKAGE_VERSION=version,
             DESCRIPTION=description,
             AUTHOR=author,
             EMAIL=email,
         )
-        with open(setup_file, mode="w", encoding="utf-8") as f:
+        with setup_file_trv.open("w", encoding="utf-8") as f:
             f.write(content)
 
     meta_save = {
         "author": author,
         "email": email,
         "description": description,
         "version": version,
     }
-    with open(meta_file, "wb") as f:
+    with meta_file_trv.open("wb") as f:
         pickle.dump(meta_save, f)
 
-    with open(setup_file) as f:
-        setup_text_file = f.read()
-        template = Template(setup_text_file)
-        content = template.render(
-            PROJECT_NAME=new_project_name,
-        )
-    with open(setup_file_py, mode="w", encoding="utf-8") as message:
+    setup_text_file = setup_file_trv.read_text(encoding="utf-8")
+    template = Template(setup_text_file)
+    content = template.render(PROJECT_NAME=new_project_name)
+
+    with setup_file_py_trv.open("w", encoding="utf-8") as message:
         logger.debug("creating new setup.py with the following: \n %s", content)
         message.write(content)
 
 
-def _delete_director(items_to_delete: list[Path]) -> None:
+def _delete_director(items_to_delete: Any) -> None:
     """Utility function to delete files and directories.
 
     Args:
         items_to_delete:    A list of Path like objects to delete.
     """
     for item in items_to_delete:
         if not item.exists():
@@ -317,16 +322,14 @@
 
     Args:
         project_name:   the name of the project to test.
 
     Returns:
         True:           If the name passes the basic check
         False:          If the name fails the basic check
-
-
     """
     pattern = r"^[a-z][_\-a-z0-9]*$"
     if re.match(pattern, project_name) is not None:
         return True
     else:
         return False
 
@@ -406,16 +409,18 @@
     Args:
         project_name:   the name of the project currently under test.
 
     Notes:
         twine expects a filesystem path not Path object so use os.fspath()
     """
     logger.debug("Uploading the distribution... ")
-    dir_path = os.fspath(project_path / "dist" / "*")
-    pypirc_path = os.fspath(config.pypirc)
+
+    project_build = str(project_path / "dist" / "*")
+    dir_path = os.fspath(project_build)
+    pypirc_path = os.fspath(str(config.pypirc))
     _run_command(
         sys.executable,
         "-m",
         "twine",
         "upload",
         "--config-file",
         pypirc_path,
@@ -426,19 +431,19 @@
 
 def _cleanup(project_name: str) -> None:
     """Builds a manifest of artifacts to delete into a list of Path objects.
 
     Args:
         project_name:   the name of the project currently under test.
     """
-    if config.no_cleanup is True:
+    if config.no_cleanup is True:  # pragma: no cover
         return
     _rename_project_dir(
-        project_path.joinpath(project_name),
-        project_path.joinpath(config.original_project_name),
+        str(project_path.joinpath(project_name)),
+        str(project_path.joinpath(config.original_project_name)),
     )
     build_artifacts = [
         project_path / "build",
         project_path / "dist",
         project_path / "".join([project_name, ".egg-info"]),
         project_path / "setup.py",
     ]
@@ -456,58 +461,71 @@
         A potentially expensive operation as there are almost 500,000 projects to
         process. Can take 2-3 seconds. Look to improve performance at a later date:
         look at asyncio, asyncio.http etc.
         An improvement is to automatically periodically run this in the background.
     """
     new_count = 0
     pattern = re.compile(r">([\w\W]*?)<")
+    with as_file(pypi_index_file_trv) as pypi_index_file:
+        if pypi_index_file.exists():
+            pypi_index_file.unlink(missing_ok=True)
+
     progress_bar = tqdm(total=config.project_count)
-    pypi_index = project_path / "pypi_index"
-    pypi_count = project_path / "project_count.pickle"
-    if pypi_index.exists():
-        Path.unlink(pypi_index, missing_ok=True)
+
     try:
         index_object_raw = requests.get(config.pypi_simple_index_url, timeout=10)
     except requests.RequestException as e:
         logger.error("An error occurred: %s", e)
         raise SystemExit("An error occurred with an HTTP request")
-    with pypi_index.open(mode="a") as file:
+    with pypi_index_file_trv.open("a") as file:
         for line in index_object_raw.iter_lines():
             line = str(line)
             project_text = re.search(pattern, line)
             if project_text is not None:
                 new_count += 1
                 progress_bar.update(1)
                 project = "".join([project_text.group(1), " \n"])
                 file.write(project)
     progress_bar.close()
-    with open(pypi_count, "wb") as f:
+    with project_count_file_trv.open("wb") as f:
         pickle.dump(new_count, f)
 
+    if config.project_count > 0:
+        diff = new_count - config.project_count
+        if diff > 0:  # pragma: no cover
+            _feedback(
+                f"Project count has increased by {diff} since last index generation",
+                "warning",
+            )
+        elif diff < 0:  # pragma: no cover
+            _feedback(
+                f"Project count has decreased by {diff} since last index generation",
+                "warning",
+            )
+
 
 def _pypi_search_index(project_name: str) -> bool:
     """Open the generated index file and search for the project name.
 
     Args:
         project_name:   the name of the project currently under test.
 
     Returns:
         True:           A match was found.
         False:          A match was not found.
     """
-    pypi_index = project_path / "pypi_index"
-    if not pypi_index.exists():
+    if not pypi_index_file_trv.is_file():
         _generate_pypi_index()
-    with pypi_index.open(mode="r") as file:
-        projects = file.read()
-        if project_name in projects:
-            logger.debug("%s FOUND in the PyPI simple index", project_name)
-            return True
-        logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
-        return False
+
+    projects = pypi_index_file_trv.read_text(encoding="utf-8")
+    if project_name in projects:
+        logger.debug("%s FOUND in the PyPI simple index", project_name)
+        return True
+    logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
+    return False
 
 
 def _pypi_search(
     search_project: str,
 ) -> tuple[list[list[Union[str, Any]]], list[list[Union[str, Any]]], str]:
     """Performs a get request to PyPI's search API for the project name.
 
@@ -583,29 +601,29 @@
     """
     file_path = Path(file)
     try:
         with file_path.open(mode="r") as f:
             file_contents = f.read()
             projects = file_contents.split()
             return list(set(projects))
-    except FileNotFoundError:
+    except FileNotFoundError:  # pragma: no cover
         _feedback(f"The file {file} does not exist", "warning")
-        raise SystemExit()  # pragma: no cover
-    except PermissionError:
+        raise SystemExit()
+    except PermissionError:  # pragma: no cover
         _feedback(f"Permission denied to file: {file}", "warning")
-        raise SystemExit()  # pragma: no cover
-    except IsADirectoryError:
+        raise SystemExit()
+    except IsADirectoryError:  # pragma: no cover
         _feedback(f"{file} is a directory not a file", "warning")
-        raise SystemExit()  # pragma: no cover
-    except OSError:
+        raise SystemExit()
+    except OSError:  # pragma: no cover
         _feedback(f"A general IO error has occurred opening file: {file}", "warning")
-        raise SystemExit()  # pragma: no cover
-    except Exception as e:
+        raise SystemExit()
+    except Exception as e:  # pragma: no cover
         _feedback(f"An error occurred:, {str(e)}", "warning")
-        raise SystemExit()  # pragma: no cover
+        raise SystemExit()
 
 
 def _write_output_file(file_name: str, results: dict) -> None:
     """Write the results to a file
 
     Args:
         file_name:      Name of file to save as a simple string.
@@ -643,29 +661,29 @@
         projects_results = "".join([projects_results, "\n", "-" * header_width, "\n"])
 
     final_output_text = "".join([title, header, projects_results])
 
     try:  # pragma: no cover
         with file_path.open(mode="w") as f:
             f.write(final_output_text)
-    except PermissionError:
+    except PermissionError:  # pragma: no cover
         _feedback(f"Permission denied to file: {file_path.open}", "warning")
-        raise SystemExit()  # pragma: no cover
-    except FileExistsError:
+        raise SystemExit()
+    except FileExistsError:  # pragma: no cover
         _feedback(f"File {file_path.open} already exists", "warning")
-        raise SystemExit()  # pragma: no cover
-    except IsADirectoryError:
+        raise SystemExit()
+    except IsADirectoryError:  # pragma: no cover
         _feedback(f"{file_path.open} is a directory not a file", "warning")
-        raise SystemExit()  # pragma: no cover
-    except OSError:
+        raise SystemExit()
+    except OSError:  # pragma: no cover
         _feedback("General IO error has occurred", "warning")
-        raise SystemExit()  # pragma: no cover
-    except Exception as e:
+        raise SystemExit()
+    except Exception as e:  # pragma: no cover
         _feedback(f"An error occurred:, {str(e)}", "warning")
-        raise SystemExit()  # pragma: no cover
+        raise SystemExit()
 
 
 def _final_analysis(pattern: list[int]) -> None:
     """Displays a rich console table displaying the conclusion of the test results
 
     Args:
         pattern:    A list of the test results:
@@ -745,15 +763,15 @@
         action="store_true",
         help="display information about similar projects",
     )
     parser.add_argument(
         "-g",
         "--generate",
         action="store_true",
-        help="generate a new PyPI simple index",
+        help="generate a new PyPI index file",
     )
     parser.add_argument(
         "-m",
         "--meta",
         action="store_true",
         help="input new meta data when registering (Author and email address)",
     )
@@ -791,15 +809,15 @@
     args, parser = _parse_args(sys.argv[1:])
     logger.debug(" args: %s", args)
 
     if args.generate:
         _generate_pypi_index()
 
     if args.version:
-        version, message, result = _check_version()
+        version, message, result = _check_version()  # type: ignore
         if result:
             _feedback(f"{version} : {message}", "nominal")
         else:
             _feedback(f"{version} : {message}", "warning")
 
     if args.projects == "None" and args.file == "None" and args.register:
         _feedback("You need to specify a project name to register it", "error")
@@ -936,16 +954,16 @@
             test_results == [0, 0, 0]
             and args.register is True
             and config.pypirc is not None
             and len(project_list) == 1
         ):
             _create_setup(new_project, new_meta=args.meta)
             _rename_project_dir(
-                project_path.joinpath(config.original_project_name),
-                project_path.joinpath(new_project),
+                str(project_path.joinpath(config.original_project_name)),
+                str(project_path.joinpath(new_project)),
             )
             _build_dist()
             if args.dryrun is False:
                 _upload_dist(new_project)
             else:
                 _feedback("Dryrun .... bypassing upload to PyPI..", "warning")
             _cleanup(new_project)
```

### Comparing `pynamer-1.3.1/src/pynamer/utils.py` & `pynamer-1.3.3/src/pynamer/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-#!/usr/bin/env python3
-
-# Core Library modules
-import json
-from typing import Union
-
-# Third party modules
-import requests
-from packaging import version
-
-# First party modules
-import pynamer
-
-# Local modules
-from .config import config
-
-
-def _check_integrity() -> None:
-    pass
-
-
-def _reset() -> None:
-    pass
-
-
-def _check_version() -> Union[tuple[version, str, bool], None]:
-    """Utility function to compare package version against latest version on PyPI.
-
-    Returns:
-        current_version:    version of the installed package.
-        str:                Message concerning the result of the comparison.
-        bool:               True: if the installed package is up to date.
-                            False: if there is a newer version on PyPI.
-    """
-    url_json = "".join([config.pypi_json_url, "pynamer", "/json"])
-    current_version = version.parse(pynamer.__version__)
-    try:
-        project_json_raw = requests.get(url_json, timeout=10)
-    except requests.RequestException as e:
-        raise SystemExit("An error occurred with an HTTP request")
-    if project_json_raw.status_code == 200:
-        project_json = json.loads(project_json_raw.content)
-        pypi_version = version.parse(project_json["info"]["version"])
-        if pypi_version > current_version:
-            return (
-                current_version,
-                f"(There is a newer version available: {pypi_version})",
-                False,
-            )
-        elif pypi_version == current_version:
-            return current_version, "(You have the most recent version)", True
-    return None
+#!/usr/bin/env python3
+
+# Core Library modules
+import json
+from typing import Union
+
+# Third party modules
+import requests
+from packaging import version
+
+# First party modules
+import pynamer
+
+# Local modules
+from .config import config
+
+
+def _check_integrity() -> None:
+    pass
+
+
+def _reset() -> None:
+    pass
+
+
+def _check_version() -> Union[tuple[version, str, bool], None]:
+    """Utility function to compare package version against latest version on PyPI.
+
+    Returns:
+        current_version:    version of the installed package.
+        str:                Message concerning the result of the comparison.
+        bool:               True: if the installed package is up to date.
+                            False: if there is a newer version on PyPI.
+    """
+    url_json = "".join([config.pypi_json_url, "pynamer", "/json"])
+    current_version = version.parse(pynamer.__version__)
+    try:
+        project_json_raw = requests.get(url_json, timeout=10)
+    except requests.RequestException:
+        raise SystemExit("An error occurred with an HTTP request")
+    if project_json_raw.status_code == 200:
+        project_json = json.loads(project_json_raw.content)
+        pypi_version = version.parse(project_json["info"]["version"])
+        if pypi_version > current_version:
+            return (
+                current_version,
+                f"(There is a newer version available: {pypi_version})",
+                False,
+            )
+        elif pypi_version == current_version:
+            return current_version, "(You have the most recent version)", True
+    return None
```

### Comparing `pynamer-1.3.1/src/pynamer.egg-info/PKG-INFO` & `pynamer-1.3.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,20 @@
-Metadata-Version: 2.1
-Name: pynamer
-Version: 1.3.1
-Summary: Utility to find an available package name on the PyPI repository and register it
-Home-page: https://github.com/Stephen-RA-King/pynamer
-Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
-Author: Stephen R A King
-Author-email: sking.github@gmail.com
-Maintainer: Stephen R A King
-Maintainer-email: sking.github@gmail.com
-License: MIT
-Keywords: utility
-Platform: Any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-
 _**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
-[![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
+[![CodeQl][codeql-image]][codeql-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
+[![readthedocs][readthedocs-image]][readthedocs-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
-[![CodeQl][codeql-image]][codeql-url]
-[![readthedocs][readthedocs-image]][readthedocs-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
@@ -149,15 +120,14 @@
 ---
 
 ### Prerequisites
 
 ---
 
 -   [x] Python >= 3.9.
--   [x] [**pipx**](https://pypa.github.io/pipx/)
 
 The following are optional but required for 'registering' a project name on PyPI
 
 -   [x] An account on PyPI (and generate a PyPI API token).
 -   [x] A [**.pypirc**](https://packaging.python.org/en/latest/specifications/pypirc/) file containing your PyPI API key
 
     or
@@ -175,14 +145,22 @@
 repository = https://upload.pypi.org/legacy/
 username = __token__
 password = your_API_token_here
 ```
 
 ### Installation
 
+Pynamer can be installed into any python environment using pip:
+
+```bash
+~ $ pip install pynamer
+```
+
+However, optimal installation can be archived using [**pipx**][pipx-url]:
+
 ```bash
 ~ $ pipx install pynamer
 ```
 
 ### Basic Usage
 
 #### A package name that is not available
@@ -227,15 +205,15 @@
 positional arguments:
   projects              Optional - one or more project names
 
 optional arguments:
   -h, --help            show this help message and exit
   -r, --register        register the name on PyPi if the name is available
   -v, --verbose         display information about similar projects
-  -g, --generate        generate a new PyPI simple index
+  -g, --generate        generate a new PyPI index file
   -m, --meta            input new meta data when registering (Author and email address)
   -w, --webbrowser      open the project on PyPI in a webbrowser
   --version             display version number
   -f FILE, --file FILE  file containing a list of projects to analyze
   -o OUTPUT, --output OUTPUT
                         file to store the test results
 ```
@@ -444,27 +422,28 @@
 [codeql-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynamer/?ref=repository-badge
-[downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
+[downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynamer
 [format-image]: https://img.shields.io/pypi/format/pynamer
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/context:python
 [license-image]: https://img.shields.io/pypi/l/pynamer
 [license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
 [pypi-url]: https://pypi.org/project/pynamer/
 [pypi-image]: https://img.shields.io/pypi/v/pynamer.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynamer
```

### Comparing `pynamer-1.3.1/src/pynamer.egg-info/SOURCES.txt` & `pynamer-1.3.3/src/pynamer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_args.py` & `pynamer-1.3.3/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_build_dist.py` & `pynamer-1.3.3/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_cleanup.py` & `pynamer-1.3.3/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_create_setup_file.py` & `pynamer-1.3.3/tests/test_create_setup_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 #!/usr/bin/env python3
 # Core Library modules
 from pathlib import Path
 
-# Third party modules
-import pytest
-
 # First party modules
 from pynamer import pynamer
 
 BASE_DIR = Path(__file__).parents[0]
 expected_content = """#!/usr/bin/env python3
```

### Comparing `pynamer-1.3.1/tests/test_defaults.py` & `pynamer-1.3.3/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_delete_director.py` & `pynamer-1.3.3/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_feedback.py` & `pynamer-1.3.3/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_final_analysis.py` & `pynamer-1.3.3/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_find_pypirc_file.py` & `pynamer-1.3.3/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_generate_pypi_index.py` & `pynamer-1.3.3/tests/test_generate_pypi_index.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,24 +17,28 @@
 def my_custom_get(url, **kwargs):
     _pickle_file = BASE_DIR / "resources" / "simple_index.pickle"
     _pickle_bytes = _pickle_file.read_bytes()
     pickle_content = pickle.loads(_pickle_bytes)
     return pickle_content
 
 
-def test_ping_json(monkeypatch, project_path_mock):
+def test_generate_pypi_index(monkeypatch):
     monkeypatch.setattr(requests, "get", my_custom_get)
+    monkeypatch.setattr(pynamer, "pypi_index_file_trv", BASE_DIR / "pypi_index")
+    monkeypatch.setattr(
+        pynamer, "project_count_file_trv", BASE_DIR / "project_count.pickle"
+    )
     pynamer._generate_pypi_index()
     assert (BASE_DIR / "pypi_index").exists()
     assert (BASE_DIR / "project_count.pickle").exists()
     (BASE_DIR / "pypi_index").unlink()
     (BASE_DIR / "project_count.pickle").unlink()
 
 
-def test_ping_project_error(monkeypatch, project_path_mock):
+def test_generate_pypi_index_error(monkeypatch, project_path_mock):
     def mock_requests_error(*args, **kwargs):
         raise ConnectTimeout("Connection timed out")
 
     monkeypatch.setattr(requests, "get", mock_requests_error)
 
     with pytest.raises(SystemExit) as excinfo:
         pynamer._generate_pypi_index()
```

### Comparing `pynamer-1.3.1/tests/test_ping_json.py` & `pynamer-1.3.3/tests/test_ping_json.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#!/usr/bin/env python3
-# Core Library modules
-import pickle
-from pathlib import Path
-
-# Third party modules
-import pytest
-import requests
-from requests.exceptions import ConnectTimeout
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-expected_response_found = """Stephen R A King
-sking.github@gmail.com
-1.5.5
-Utility command line tool to manage python versions"""
-
-
-def my_custom_get_found(url, **kwargs):
-    # Implement your custom logic here
-    _pickle_file = BASE_DIR / "resources" / "requests_get_json_pynball.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def my_custom_get_not_found(url, **kwargs):
-    _pickle_file = BASE_DIR / "resources" / "requests_get_json_zeedonk.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def test_ping_json_found(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_found)
-    result = pynamer._ping_json("pynball")
-    assert result == expected_response_found
-
-
-def test_ping_json_not_found(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_not_found)
-    result = pynamer._ping_json("zeedonk")
-    assert result == ""
-
-
-def test_ping_json_error(monkeypatch):
-    def mock_requests_error(*args, **kwargs):
-        raise ConnectTimeout("Connection timed out")
-
-    monkeypatch.setattr(requests, "get", mock_requests_error)
-
-    with pytest.raises(SystemExit) as excinfo:
-        pynamer._ping_json("pynball")
-    assert str(excinfo.value) == "An error occurred with an HTTP request"
+#!/usr/bin/env python3
+# Core Library modules
+import pickle
+from pathlib import Path
+
+# Third party modules
+import pytest
+import requests
+from requests.exceptions import ConnectTimeout
+
+# First party modules
+from pynamer import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+expected_response_found = """Stephen R A King
+sking.github@gmail.com
+1.5.5
+Utility command line tool to manage python versions"""
+
+
+def my_custom_get_found(url, **kwargs):
+    # Implement your custom logic here
+    _pickle_file = BASE_DIR / "resources" / "requests_get_json_pynball.pickle"
+    _pickle_bytes = _pickle_file.read_bytes()
+    pickle_content = pickle.loads(_pickle_bytes)
+    return pickle_content
+
+
+def my_custom_get_not_found(url, **kwargs):
+    _pickle_file = BASE_DIR / "resources" / "requests_get_json_zeedonk.pickle"
+    _pickle_bytes = _pickle_file.read_bytes()
+    pickle_content = pickle.loads(_pickle_bytes)
+    return pickle_content
+
+
+def test_ping_json_found(monkeypatch):
+    monkeypatch.setattr(requests, "get", my_custom_get_found)
+    result = pynamer._ping_json("pynball")
+    assert result == expected_response_found
+
+
+def test_ping_json_not_found(monkeypatch):
+    monkeypatch.setattr(requests, "get", my_custom_get_not_found)
+    result = pynamer._ping_json("zeedonk")
+    assert result == ""
+
+
+def test_ping_json_error(monkeypatch):
+    def mock_requests_error(*args, **kwargs):
+        raise ConnectTimeout("Connection timed out")
+
+    monkeypatch.setattr(requests, "get", mock_requests_error)
+
+    with pytest.raises(SystemExit) as excinfo:
+        pynamer._ping_json("pynball")
+    assert str(excinfo.value) == "An error occurred with an HTTP request"
```

### Comparing `pynamer-1.3.1/tests/test_ping_project.py` & `pynamer-1.3.3/tests/test_ping_project.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-#!/usr/bin/env python3
-# Core Library modules
-import pickle
-from pathlib import Path
-
-# Third party modules
-import pytest
-import requests
-from requests.exceptions import ConnectTimeout
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-def my_custom_get_found(url, **kwargs):
-    _pickle_file = BASE_DIR / "resources" / "requests_get_ping_pynball.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def my_custom_get_not_found(url, **kwargs):
-    _pickle_file = BASE_DIR / "resources" / "requests_get_ping_zeedonk.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def test_ping_project_found(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_found)
-    result = pynamer._ping_project("pynball")
-    assert result is True
-
-
-def test_ping_project_not_found(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_not_found)
-    result = pynamer._ping_project("zeedonk")
-    assert result is False
-
-
-def test_ping_project_error(monkeypatch):
-    def mock_requests_error(*args, **kwargs):
-        raise ConnectTimeout("Connection timed out")
-
-    monkeypatch.setattr(requests, "get", mock_requests_error)
-
-    with pytest.raises(SystemExit) as excinfo:
-        pynamer._ping_project("pynball")
-    assert str(excinfo.value) == "An error occurred with an HTTP request"
+#!/usr/bin/env python3
+# Core Library modules
+import pickle
+from pathlib import Path
+
+# Third party modules
+import pytest
+import requests
+from requests.exceptions import ConnectTimeout
+
+# First party modules
+from pynamer import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+def my_custom_get_found(url, **kwargs):
+    _pickle_file = BASE_DIR / "resources" / "requests_get_ping_pynball.pickle"
+    _pickle_bytes = _pickle_file.read_bytes()
+    pickle_content = pickle.loads(_pickle_bytes)
+    return pickle_content
+
+
+def my_custom_get_not_found(url, **kwargs):
+    _pickle_file = BASE_DIR / "resources" / "requests_get_ping_zeedonk.pickle"
+    _pickle_bytes = _pickle_file.read_bytes()
+    pickle_content = pickle.loads(_pickle_bytes)
+    return pickle_content
+
+
+def test_ping_project_found(monkeypatch):
+    monkeypatch.setattr(requests, "get", my_custom_get_found)
+    result = pynamer._ping_project("pynball")
+    assert result is True
+
+
+def test_ping_project_not_found(monkeypatch):
+    monkeypatch.setattr(requests, "get", my_custom_get_not_found)
+    result = pynamer._ping_project("zeedonk")
+    assert result is False
+
+
+def test_ping_project_error(monkeypatch):
+    def mock_requests_error(*args, **kwargs):
+        raise ConnectTimeout("Connection timed out")
+
+    monkeypatch.setattr(requests, "get", mock_requests_error)
+
+    with pytest.raises(SystemExit) as excinfo:
+        pynamer._ping_project("pynball")
+    assert str(excinfo.value) == "An error occurred with an HTTP request"
```

### Comparing `pynamer-1.3.1/tests/test_process_input_file.py` & `pynamer-1.3.3/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_pypi_search.py` & `pynamer-1.3.3/tests/test_pypi_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 ]
 
 others_expected = [
     [
         "pynamer",
         "0.5.5",
         "2023-05-03",
-        "Utility to find an available package name on the PyPI repository and register it",
+        "Utility to find an available package name on the PyPI repository "
+        "and register it",
     ],
 ]
 
 
 def my_custom_get(url, *args, **kwargs):
     _pickle_file = BASE_DIR / "resources" / "requests_get_search_pynball.pickle"
     _pickle_bytes = _pickle_file.read_bytes()
```

### Comparing `pynamer-1.3.1/tests/test_rename_project_dir.py` & `pynamer-1.3.3/tests/test_rename_project_dir.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-#!/usr/bin/env python3
-# Core Library modules
-from pathlib import Path
-
-# Third party modules
-import pytest
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-def test_rename_directory(create_env):
-    old_name = BASE_DIR / "project_name"
-    new_name = BASE_DIR / "pynamer"
-    assert old_name.exists()
-    pynamer._rename_project_dir(str(old_name), str(new_name))
-    assert new_name.exists()
-    pynamer._rename_project_dir(str(new_name), str(old_name))
-
-
-def test_rename_directory_dir_missing(create_env):
-    old_name = BASE_DIR / "project_name1"
-    new_name = BASE_DIR / "pynamer"
-    with pytest.raises(FileNotFoundError):
-        pynamer._rename_project_dir(str(old_name), str(new_name))
+#!/usr/bin/env python3
+# Core Library modules
+from pathlib import Path
+
+# Third party modules
+import pytest
+
+# First party modules
+from pynamer import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+def test_rename_directory(create_env):
+    old_name = BASE_DIR / "project_name"
+    new_name = BASE_DIR / "pynamer"
+    assert old_name.exists()
+    pynamer._rename_project_dir(str(old_name), str(new_name))
+    assert new_name.exists()
+    pynamer._rename_project_dir(str(new_name), str(old_name))
+
+
+def test_rename_directory_dir_missing(create_env):
+    old_name = BASE_DIR / "project_name1"
+    new_name = BASE_DIR / "pynamer"
+    with pytest.raises(FileNotFoundError):
+        pynamer._rename_project_dir(str(old_name), str(new_name))
```

### Comparing `pynamer-1.3.1/tests/test_upload_dist.py` & `pynamer-1.3.3/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-1.3.1/tests/test_write_output_file.py` & `pynamer-1.3.3/tests/test_write_output_file.py`

 * *Files identical despite different names*

