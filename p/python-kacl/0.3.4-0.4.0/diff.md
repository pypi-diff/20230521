# Comparing `tmp/python-kacl-0.3.4.tar.gz` & `tmp/python-kacl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-kacl-0.3.4.tar", last modified: Tue Jan 24 14:04:53 2023, max compression
+gzip compressed data, was "python-kacl-0.4.0.tar", last modified: Sun May 21 18:15:03 2023, max compression
```

## Comparing `python-kacl-0.3.4.tar` & `python-kacl-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-24 14:04:53.533718 python-kacl-0.3.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2023-01-24 14:04:27.000000 python-kacl-0.3.4/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2023-01-24 14:04:27.000000 python-kacl-0.3.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    17532 2023-01-24 14:04:53.533718 python-kacl-0.3.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    16896 2023-01-24 14:04:27.000000 python-kacl-0.3.4/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-24 14:04:53.529720 python-kacl-0.3.4/kacl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      599 2023-01-24 14:04:36.000000 python-kacl-0.3.4/kacl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      742 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/changes.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-24 14:04:53.529720 python-kacl-0.3.4/kacl/config/
--rw-rw-r--   0 travis    (2000) travis    (2000)      991 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/config/kacl-default.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2647 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22020 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/document.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      415 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/element.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/exception.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    13293 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/kacl_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1575 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/link_provider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2221 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2195 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/serializer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2029 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/validation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2974 2023-01-24 14:04:27.000000 python-kacl-0.3.4/kacl/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-24 14:04:53.533718 python-kacl-0.3.4/python_kacl.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17532 2023-01-24 14:04:53.000000 python-kacl-0.3.4/python_kacl.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      603 2023-01-24 14:04:53.000000 python-kacl-0.3.4/python_kacl.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-01-24 14:04:53.000000 python-kacl-0.3.4/python_kacl.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2023-01-24 14:04:53.000000 python-kacl-0.3.4/python_kacl.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-01-24 14:04:32.000000 python-kacl-0.3.4/python_kacl.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-01-24 14:04:53.000000 python-kacl-0.3.4/python_kacl.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-01-24 14:04:53.000000 python-kacl-0.3.4/python_kacl.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-01-24 14:04:53.533718 python-kacl-0.3.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1503 2023-01-24 14:04:27.000000 python-kacl-0.3.4/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-24 14:04:53.533718 python-kacl-0.3.4/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-01-24 14:04:27.000000 python-kacl-0.3.4/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1241 2023-01-24 14:04:27.000000 python-kacl-0.3.4/tests/snapshot_directory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5286 2023-01-24 14:04:27.000000 python-kacl-0.3.4/tests/test_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11337 2023-01-24 14:04:27.000000 python-kacl-0.3.4/tests/test_kacl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:15:03.269774 python-kacl-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-21 18:14:53.000000 python-kacl-0.4.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-21 18:14:53.000000 python-kacl-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17898 2023-05-21 18:15:03.269774 python-kacl-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    17249 2023-05-21 18:14:53.000000 python-kacl-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:15:03.267774 python-kacl-0.4.0/kacl/
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/changes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:15:03.267774 python-kacl-0.4.0/kacl/config/
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/config/kacl-default.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    23133 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/document.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/element.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)    14244 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/kacl_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/link_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-05-21 18:14:53.000000 python-kacl-0.4.0/kacl/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:15:03.268774 python-kacl-0.4.0/python_kacl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17898 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-21 18:15:03.000000 python-kacl-0.4.0/python_kacl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 18:15:03.269774 python-kacl-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-21 18:14:53.000000 python-kacl-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:15:03.269774 python-kacl-0.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-21 18:14:53.000000 python-kacl-0.4.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-05-21 18:14:53.000000 python-kacl-0.4.0/tests/snapshot_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-05-21 18:14:53.000000 python-kacl-0.4.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    11806 2023-05-21 18:14:53.000000 python-kacl-0.4.0/tests/test_kacl.py
```

### Comparing `python-kacl-0.3.4/LICENSE` & `python-kacl-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-kacl-0.3.4/PKG-INFO` & `python-kacl-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.3.4
+Version: 0.4.0
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
-Home-page: http://github.com/mschmieder/python-kacl
+Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-kacl
 
-[![Build Status](https://travis-ci.org/mschmieder/python-kacl.svg?branch=master)](https://travis-ci.org/mschmieder/python-kacl)
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=mschmieder_python-kacl&metric=coverage)](https://sonarcloud.io/dashboard?id=mschmieder_python-kacl)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=mschmieder_python-kacl&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=mschmieder_python-kacl)
+[![Build Status](https://gitlab.com/schmieder.matthias/python-kacl/badges/main/pipeline.svg?ignore_skipped=true](https://gitlab.com/schmieder.matthias/python-kacl)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=coverage)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
+[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
 
 A tool for verifying and modifying changelog in the [**K**eep-**A-C**hange-**L**og](https://keepachangelog.com/en/1.0.0/) format.
 
 - [python-kacl](#python-kacl)
   - [Installation](#installation)
     - [From Source](#from-source)
     - [Pip Package](#pip-package)
@@ -51,15 +52,15 @@
 - docker
 
 All approaches are described in detail within this section.
 
 ### From Source
 
 ```bash
-git clone https://github.com/mschmieder/python-kacl
+git clone https://gitlab.com/schmieder.matthias/python-kacl
 cd python-kacl
 ```
 
 **Global Install**
 
 ```bash
 pip3 install .
@@ -92,15 +93,15 @@
 ```
 
 ### pre-commit
 
 The package can also be used as a pre-commit hook. Just add the following to your `.pre-commit-config.yaml`
 
 ```yaml
-- repo: https://github.com/mschmieder/python-kacl
+- repo: https://gitlab.com/schmieder.matthias/python-kacl
   rev: 'v0.3.0'
   hooks:
     - id: kacl-verify
 ```
 
 ## CLI
 
@@ -316,16 +317,16 @@
 ### Added
 - `release` command will make sure changelog is valid before doing any changes.
 
 ## 0.2.16 - 2020-01-07
 ### Fixed
 - fixed issue #3 that did not detect linked versions with missing links
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/tree/v1.0.0...HEAD
-[1.0.0]: https://github.com/mschmieder/python-kacl/compare/v0.2.16...v1.0.0
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/tree/v1.0.0...HEAD
+[1.0.0]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v0.2.16...v1.0.0
 ```
 
 **Usage with fixed version**
 
 ```bash
 kacl-cli release 1.0.0
 ```
@@ -345,15 +346,15 @@
 - implemented basic cli with `new`, `get`, `release`, `verify`
 - added `--json` option to `verify` command
 
 ## 0.1.0 - 2019-12-12
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v1.0.0...HEAD
 ```
 
 Example CHANGELOG.md (after):
 
 ```markdown
 # Changelog
 All notable changes to this project will be documented in this file.
@@ -369,15 +370,15 @@
 - implemented basic cli with `new`, `get`, `release`, `verify`
 - added `--json` option to `verify` command
 
 ## 0.1.0 - 2019-12-12
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v1.0.0...HEAD
 ```
 
 **Usage with version increment**
 
 ```bash
 kacl-cli release patch
 ```
@@ -399,30 +400,30 @@
 - implemented basic cli with `new`, `get`, `release`, `verify`
 - added `--json` option to `verify` command
 
 ## 0.1.0 - 2019-12-12
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v1.0.0...HEAD
 ```
 
 ## Link Generation
 
 `kacl-cli` let's you easily generate links to your versions. You can automatically generate all links following the desired patterns using `kacl-cli link generate`.
 The link generation can also be easily included into the `release` command and will take care of updating the `unreleased` and `latest_version` section.
 
 ```bash
 Usage: kacl-cli link generate [OPTIONS]
 
 Options:
   -m, --modify                    This option will add the changes directly
                                   into changelog file.
   --host-url TEXT                 Host url to the git service. (i.e
-                                  https://github.com/mschmieder/python-kacl)
+                                  https://gitlab.com/schmieder.matthias/python-kacl)
   --compare-versions-template TEXT
                                   Template string for version comparison link.
   --unreleased-changes-template TEXT
                                   Template string for unreleased changes link.
   --initial-version-template TEXT
                                   Template string for initial version link.
   --help                          Show this message and exit.
@@ -527,15 +528,15 @@
 
 ## Development
 
 With these instructions you can easily setup a development environment
 
 ```bash
 # clone the project
-git clone https://github.com/mschmieder/python-kacl
+git clone https://gitlab.com/schmieder.matthias/python-kacl
 cd python-kacl
 
 # create a virtual env
 python3 -m venv .venv
 source ./venv/bin/activate
 
 # install in development mode
```

### Comparing `python-kacl-0.3.4/README.md` & `python-kacl-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # python-kacl
 
-[![Build Status](https://travis-ci.org/mschmieder/python-kacl.svg?branch=master)](https://travis-ci.org/mschmieder/python-kacl)
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=mschmieder_python-kacl&metric=coverage)](https://sonarcloud.io/dashboard?id=mschmieder_python-kacl)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=mschmieder_python-kacl&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=mschmieder_python-kacl)
+[![Build Status](https://gitlab.com/schmieder.matthias/python-kacl/badges/main/pipeline.svg?ignore_skipped=true](https://gitlab.com/schmieder.matthias/python-kacl)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=coverage)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
+[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
 
 A tool for verifying and modifying changelog in the [**K**eep-**A-C**hange-**L**og](https://keepachangelog.com/en/1.0.0/) format.
 
 - [python-kacl](#python-kacl)
   - [Installation](#installation)
     - [From Source](#from-source)
     - [Pip Package](#pip-package)
@@ -34,15 +35,15 @@
 - docker
 
 All approaches are described in detail within this section.
 
 ### From Source
 
 ```bash
-git clone https://github.com/mschmieder/python-kacl
+git clone https://gitlab.com/schmieder.matthias/python-kacl
 cd python-kacl
 ```
 
 **Global Install**
 
 ```bash
 pip3 install .
@@ -75,15 +76,15 @@
 ```
 
 ### pre-commit
 
 The package can also be used as a pre-commit hook. Just add the following to your `.pre-commit-config.yaml`
 
 ```yaml
-- repo: https://github.com/mschmieder/python-kacl
+- repo: https://gitlab.com/schmieder.matthias/python-kacl
   rev: 'v0.3.0'
   hooks:
     - id: kacl-verify
 ```
 
 ## CLI
 
@@ -299,16 +300,16 @@
 ### Added
 - `release` command will make sure changelog is valid before doing any changes.
 
 ## 0.2.16 - 2020-01-07
 ### Fixed
 - fixed issue #3 that did not detect linked versions with missing links
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/tree/v1.0.0...HEAD
-[1.0.0]: https://github.com/mschmieder/python-kacl/compare/v0.2.16...v1.0.0
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/tree/v1.0.0...HEAD
+[1.0.0]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v0.2.16...v1.0.0
 ```
 
 **Usage with fixed version**
 
 ```bash
 kacl-cli release 1.0.0
 ```
@@ -328,15 +329,15 @@
 - implemented basic cli with `new`, `get`, `release`, `verify`
 - added `--json` option to `verify` command
 
 ## 0.1.0 - 2019-12-12
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v1.0.0...HEAD
 ```
 
 Example CHANGELOG.md (after):
 
 ```markdown
 # Changelog
 All notable changes to this project will be documented in this file.
@@ -352,15 +353,15 @@
 - implemented basic cli with `new`, `get`, `release`, `verify`
 - added `--json` option to `verify` command
 
 ## 0.1.0 - 2019-12-12
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v1.0.0...HEAD
 ```
 
 **Usage with version increment**
 
 ```bash
 kacl-cli release patch
 ```
@@ -382,30 +383,30 @@
 - implemented basic cli with `new`, `get`, `release`, `verify`
 - added `--json` option to `verify` command
 
 ## 0.1.0 - 2019-12-12
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v1.0.0...HEAD
 ```
 
 ## Link Generation
 
 `kacl-cli` let's you easily generate links to your versions. You can automatically generate all links following the desired patterns using `kacl-cli link generate`.
 The link generation can also be easily included into the `release` command and will take care of updating the `unreleased` and `latest_version` section.
 
 ```bash
 Usage: kacl-cli link generate [OPTIONS]
 
 Options:
   -m, --modify                    This option will add the changes directly
                                   into changelog file.
   --host-url TEXT                 Host url to the git service. (i.e
-                                  https://github.com/mschmieder/python-kacl)
+                                  https://gitlab.com/schmieder.matthias/python-kacl)
   --compare-versions-template TEXT
                                   Template string for version comparison link.
   --unreleased-changes-template TEXT
                                   Template string for unreleased changes link.
   --initial-version-template TEXT
                                   Template string for initial version link.
   --help                          Show this message and exit.
@@ -510,15 +511,15 @@
 
 ## Development
 
 With these instructions you can easily setup a development environment
 
 ```bash
 # clone the project
-git clone https://github.com/mschmieder/python-kacl
+git clone https://gitlab.com/schmieder.matthias/python-kacl
 cd python-kacl
 
 # create a virtual env
 python3 -m venv .venv
 source ./venv/bin/activate
 
 # install in development mode
```

### Comparing `python-kacl-0.3.4/kacl/changes.py` & `python-kacl-0.4.0/kacl/changes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from .parser import KACLParser
-from .element import KACLElement
-import re
+from kacl.element import KACLElement
 
 
 class KACLChanges(KACLElement):
     def __init__(self, element):
-        KACLElement.__init__(self, 
-                             raw=element.raw(),
-                             title=element.title(),
-                             body=element.body(),
-                             line_number=element.line_number())
+        KACLElement.__init__(
+            self,
+            raw=element.raw(),
+            title=element.title(),
+            body=element.body(),
+            line_number=element.line_number(),
+        )
         self.__items = []
 
     def items(self):
         if not len(self.__items) and len(self.body().strip()):
             body = self.body()
-            items = ("\n"+body).split('\n-')
+            items = ("\n" + body).split("\n-")
             self.__items = [x.strip() for x in items if len(x.strip()) > 0]
         return self.__items
 
     def add(self, item):
         self.items().append(item)
```

### Comparing `python-kacl-0.3.4/kacl/config/kacl-default.yml` & `python-kacl-0.4.0/kacl/config/kacl-default.yml`

 * *Files identical despite different names*

### Comparing `python-kacl-0.3.4/kacl/config.py` & `python-kacl-0.4.0/kacl/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 import os
+
 import yaml
 
+
 class KACLConfig:
     def __init__(self, config_file=None):
-        default_config_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'config', 'kacl-default.yml')
+        default_config_file = os.path.join(
+            os.path.dirname(os.path.abspath(__file__)), "config", "kacl-default.yml"
+        )
         self.__config = {}
-        with open(default_config_file, 'r') as df:
+        with open(default_config_file, "r") as df:
             self.__config = yaml.safe_load(df)
         if config_file:
-            with open(os.path.expanduser(config_file), 'r') as f:
+            with open(os.path.expanduser(config_file), "r") as f:
                 KACLConfig.merge(self.__config, yaml.safe_load(f))
 
-        self.__config = self.__config.get('kacl',{})
-
-        self.allowed_header_titles = self.__config.get('allowed_header_titles')
-        self.allowed_version_sections = self.__config.get('allowed_version_sections')
-        self.default_content = self.__config.get('default_content')
-        self.git_tag_name = self.__config.get('git',{}).get('tag_name')
-        self.git_tag_description = self.__config.get('git',{}).get('tag_description')
-        self.changelog_file_path = self.__config.get('file')
-        self.git_create_tag = self.__config.get('git',{}).get('tag')
-        self.git_create_commit = self.__config.get('git',{}).get('commit')
-        self.git_commit_message = self.__config.get('git',{}).get('commit_message')
-        self.git_commit_additional_files = self.__config.get('git',{}).get('commit_additional_files')
-        self.link_auto_generate = self.__config.get('links',{}).get('auto_generate')
-        self.link_host_url = self.__config.get('links',{}).get('host_url')
-        self.links_compare_versions_template = self.__config.get('links',{}).get('compare_versions_template')
-        self.links_unreleased_changes_template = self.__config.get('links',{}).get('unreleased_changes_template')
-        self.links_initial_version_template = self.__config.get('links',{}).get('initial_version_template')
-        self.post_release_version_prefix = self.__config.get('extension', {}).get('post_release_version_prefix')
+        self.__config = self.__config.get("kacl", {})
 
+        self.allowed_header_titles = self.__config.get("allowed_header_titles")
+        self.allowed_version_sections = self.__config.get("allowed_version_sections")
+        self.default_content = self.__config.get("default_content")
+        self.git_tag_name = self.__config.get("git", {}).get("tag_name")
+        self.git_tag_description = self.__config.get("git", {}).get("tag_description")
+        self.changelog_file_path = self.__config.get("file")
+        self.git_create_tag = self.__config.get("git", {}).get("tag")
+        self.git_create_commit = self.__config.get("git", {}).get("commit")
+        self.git_commit_message = self.__config.get("git", {}).get("commit_message")
+        self.git_commit_additional_files = self.__config.get("git", {}).get(
+            "commit_additional_files"
+        )
+        self.link_auto_generate = self.__config.get("links", {}).get("auto_generate")
+        self.link_host_url = self.__config.get("links", {}).get("host_url")
+        self.links_compare_versions_template = self.__config.get("links", {}).get(
+            "compare_versions_template"
+        )
+        self.links_unreleased_changes_template = self.__config.get("links", {}).get(
+            "unreleased_changes_template"
+        )
+        self.links_initial_version_template = self.__config.get("links", {}).get(
+            "initial_version_template"
+        )
+        self.post_release_version_prefix = self.__config.get("extension", {}).get(
+            "post_release_version_prefix"
+        )
 
     @staticmethod
     def merge(a, b, path=None):
-        """ merge two dictionaries
+        """merge two dictionaries
         :param a: dictionary the values will be merged into
         :param b: dictionary the values will be used when overwriting values
         :param path:
         :return:
         """
         if path is None:
             path = []
@@ -48,8 +61,8 @@
                 elif a[key] == b[key]:
                     pass  # same leaf value
                 else:
                     a[key] = b[key]
 
             else:
                 a[key] = b[key]
-        return a
+        return a
```

### Comparing `python-kacl-0.3.4/kacl/document.py` & `python-kacl-0.4.0/kacl/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import datetime
-import re
-import semver
 import os
+import re
+
 import git
+import semver
 
-from .element import KACLElement
-from .version import KACLVersion
-from .parser import KACLParser
-from .config import KACLConfig
-from .link_provider import LinkProvider
-from .validation import KACLValidation
-from .exception import KACLException
+from kacl.config import KACLConfig
+from kacl.element import KACLElement
+from kacl.exception import KACLException
+from kacl.link_provider import LinkProvider
+from kacl.parser import KACLParser
+from kacl.validation import KACLValidation
+from kacl.version import KACLVersion
+
+WINDOWS_LINE_ENDING = r"\r\n"
+UNIX_LINE_ENDING = r"\n"
 
-WINDOWS_LINE_ENDING = r'\r\n'
-UNIX_LINE_ENDING = r'\n'
 
 class KACLDocument:
-    def __init__(self, data="", headers=[], versions=[], link_references=None, config=KACLConfig()):
+    def __init__(
+        self,
+        data="",
+        headers=None,
+        versions=None,
+        link_references=None,
+        config=KACLConfig(),
+    ):
         self.__data = data
-        self.__headers = headers
-        self.__versions = versions
+        self.__headers = headers if headers else []
+        self.__versions = versions if versions else []
         self.__link_references = link_references
         if not self.__link_references:
             self.__link_references = dict()
         self.config = config
 
     def validate(self):
         """Validates the current changelog and returns KACLValidation object containing all information
@@ -33,60 +42,62 @@
         """
         validation = KACLValidation()
         # 1. assert only one header and starts on first line
         if len(self.__headers) == 0:
             validation.add_error(
                 line=None,
                 line_number=None,
-                error_message="No 'Changelog' header found.")
+                error_message="No 'Changelog' header found.",
+            )
 
             # we can stop here already
             return validation
         else:
             if self.header().raw() != self.header().raw().lstrip():
                 validation.add_error(
                     line=None,
                     line_number=None,
-                    error_message="Changelog header not placed on first line.")
+                    error_message="Changelog header not placed on first line.",
+                )
 
         if len(self.__headers) > 1:
             for header in self.__headers[1:]:
                 validation.add_error(
                     line=header.raw(),
                     line_number=header.line_number(),
                     error_message="Unexpected additional top-level heading found.",
                     start_character_pos=0,
-                    end_character_pos=len(header.raw())
+                    end_character_pos=len(header.raw()),
                 )
 
         # 1.1 assert header title is in allowed list of header titles
         if self.header().title() not in self.config.allowed_header_titles:
             header = self.header()
             start_pos = header.raw().find(header.title())
-            end_pos = start_pos+len(header.title())
+            end_pos = start_pos + len(header.title())
             validation.add_error(
                 line=header.raw(),
                 line_number=header.line_number(),
                 error_message=f"Header title not valid. Options are [{','.join(self.config.allowed_header_titles)}]",
                 start_character_pos=start_pos,
-                end_character_pos=end_pos
+                end_character_pos=end_pos,
             )
 
         # 1.2 assert default content is in the header section
         for default_line in self.config.default_content:
-            if default_line not in self.header().body().replace('\n', ' '):
+            if default_line not in self.header().body().replace("\n", " "):
                 header = self.header()
                 start_pos = header.raw().find(header.title())
-                end_pos = start_pos+len(header.title())
+                end_pos = start_pos + len(header.title())
                 validation.add_error(
                     line=header.raw(),
                     line_number=header.line_number(),
                     error_message=f"Missing default content '{default_line}'",
                     start_character_pos=start_pos,
-                    end_character_pos=end_pos
+                    end_character_pos=end_pos,
                 )
 
         # 2. assert 'unreleased' version is available
         # if self.get('Unreleased') == None:
         #     validation.add_error(
         #         line=None,
         #         line_number=None,
@@ -95,140 +106,143 @@
 
         # 3. assert versions in valid format
         versions = self.versions()
         for v in versions:
             if "Unreleased" != v.version():
                 raw = v.raw()
                 regex = KACLParser.semver_regex
-                regex_error = r'#\s+(.*)\s+'
+                regex_error = r"#\s+(.*)\s+"
                 if v.link():
-                    regex = f'#\\s+\\[{KACLParser.semver_regex}\\]'
-                    regex_error = r'#\s+\[(.*)\]'
+                    regex = f"#\\s+\\[{KACLParser.semver_regex}\\]"
+                    regex_error = r"#\s+\[(.*)\]"
                 if not KACLParser.parse_sem_ver(raw, regex):
                     start_pos = 0
                     end_pos = 0
                     m = re.match(regex_error, raw)
                     if m:
                         start_pos = raw.find(m.group(1))
-                        end_pos = start_pos+len(m.group(1))
+                        end_pos = start_pos + len(m.group(1))
                     validation.add_error(
                         line=raw,
                         line_number=v.line_number(),
-                        error_message=f"Version is not a valid semantic version.",
+                        error_message="Version is not a valid semantic version.",
                         start_character_pos=start_pos,
-                        end_character_pos=end_pos
+                        end_character_pos=end_pos,
                     )
 
         # 3.1 assert versions in descending order
-        for i in range(len(versions)-1):
+        for i in range(len(versions) - 1):
             try:
                 v0 = versions[i]
-                v1 = versions[i+1]
+                v1 = versions[i + 1]
                 if semver.VersionInfo.compare(v0.version(), v1.version()) < 1:
                     validation.add_error(
                         line=v1.raw(),
                         line_number=v1.line_number(),
                         error_message="Versions are not in descending order.",
                         start_character_pos=0,
-                        end_character_pos=len(v1.raw())
+                        end_character_pos=len(v1.raw()),
                     )
-            except:
+            except Exception:
                 pass
 
         # 3.2 assert versions have a valid date
         for v in versions:
             if "Unreleased" != v.version():
                 if not v.date() or len(v.date()) < 1:
                     validation.add_error(
                         line=v.raw(),
                         line_number=v.line_number(),
                         error_message="Versions need to be decorated with a release date in the following format 'YYYY-MM-DD'",
                         start_character_pos=0,
-                        end_character_pos=len(v.raw())
+                        end_character_pos=len(v.raw()),
                     )
-                if v.date() and not re.match(r'\d\d\d\d-[0-1][0-9]-[0-3][0-9]', v.date()):
+                if v.date() and not re.match(r"\d\d\d\d-[0-1][\d]-[0-3][\d]", v.date()):
                     start_pos = v.raw().find(v.date())
-                    end_pos = start_pos+len(v.date())
+                    end_pos = start_pos + len(v.date())
                     validation.add_error(
                         line=v.raw(),
                         line_number=v.line_number(),
                         error_message="Date does not match format 'YYYY-MM-DD'",
                         start_character_pos=start_pos,
-                        end_character_pos=end_pos
+                        end_character_pos=end_pos,
                     )
 
-        # 3.3 check that only allowed sections are in the version
+            # 3.3 check that only allowed sections are in the version
             sections = v.sections()
             for title, element in sections.items():
                 if title not in self.config.allowed_version_sections:
                     start_pos = element.raw().find(title)
-                    end_pos = start_pos+len(title)
+                    end_pos = start_pos + len(title)
                     validation.add_error(
                         line=element.raw(),
                         line_number=element.line_number(),
                         error_message=f'"{title}" is not a valid section for a version. Options are [{",".join( self.config.allowed_version_sections)}]',
                         start_character_pos=start_pos,
-                        end_character_pos=end_pos
+                        end_character_pos=end_pos,
                     )
-        # 3.4 check that only list elements are in the sections
+                # 3.4 check that only list elements are in the sections
                 # 3.4.1 bring everything into a single line
                 body = element.body()
-                body_clean = re.sub(r'\n\s+', '', body)
-                lines = body_clean.split('\n\n')
-                non_list_lines = [x for x in lines if not x.strip(
-                ).startswith('-') and len(x.strip()) > 0]
+                body_clean = re.sub(r"\n\s+", "", body)
+                lines = body_clean.split("\n\n")
+                non_list_lines = [
+                    x
+                    for x in lines
+                    if not x.strip().startswith("-") and len(x.strip()) > 0
+                ]
                 if len(non_list_lines) > 0:
                     validation.add_error(
                         line=body.strip(),
                         line_number=element.line_number(),
-                        error_message='Section does contain more than only listings.'
+                        error_message="Section does contain more than only listings.",
                     )
-        # 3.5 make sure that every version that has content has it's content in a section
+            # 3.5 make sure that every version that has content has it's content in a section
             if len(v.sections()) == 0 and len(v.body().strip()) != 0:
                 validation.add_error(
                     line=v.raw(),
                     line_number=v.line_number(),
-                    error_message=f'Version "{v.version()}" has change elements outside of a change section.'
+                    error_message=f'Version "{v.version()}" has change elements outside of a change section.',
                 )
 
-        # 3.6 Check that a link exists for linked versions
-            if '[' in v.raw() and ']' in v.raw() and not v.has_link_reference():
+            # 3.6 Check that a link exists for linked versions
+            if "[" in v.raw() and "]" in v.raw() and not v.has_link_reference():
                 validation.add_error(
                     line=v.raw(),
                     line_number=v.line_number(),
                     error_message=f'Version "{v.version()}" is linked, but no link reference found in changelog file.',
-                    start_character_pos=v.raw().find('['),
-                    end_character_pos=v.raw().find(']')
+                    start_character_pos=v.raw().find("["),
+                    end_character_pos=v.raw().find("]"),
                 )
 
         # 4 link references
         # 4.1 check that there are only linked references
         version_strings = [v.version() for v in versions]
         for v, link in self.__link_references.items():
             if v not in version_strings:
                 validation.add_error(
                     line=link.raw(),
                     line_number=link.line_number(),
-                    error_message=f"Link not referenced anywhere in the document",
+                    error_message="Link not referenced anywhere in the document",
                     start_character_pos=0,
-                    end_character_pos=len(link.raw())
+                    end_character_pos=len(link.raw()),
                 )
 
         return validation
 
     def is_valid(self):
         """Checks if the current changelog is valid
         Returns:
             [bool] -- true if valid false if not
         """
         validation_results = self.validate()
         return validation_results.is_valid()
 
     def has_changes(self):
-        unreleased_version = self.get('Unreleased')
+        unreleased_version = self.get("Unreleased")
         if not unreleased_version:
             return False
 
         sections = unreleased_version.sections()
         if not sections or len(sections) == 0:
             return False
 
@@ -241,16 +255,16 @@
     def add(self, section, data):
         """adds a new change to a given section in the 'unreleased' version
 
         Arguments:
             section {[str]} -- section to add data to
             data {[str]} -- change information
         """
-        unreleased_version = self.get('Unreleased')
-        if unreleased_version == None:
+        unreleased_version = self.get("Unreleased")
+        if unreleased_version is None:
             unreleased_version = KACLVersion(version="Unreleased")
             self.__versions.insert(0, unreleased_version)
         unreleased_version.add(section.capitalize(), data)
 
     def release(self, version=None, link=None, auto_link=False, increment=None):
         """Creates a new release version by copying the 'unreleased' changes into the
         new version
@@ -260,164 +274,210 @@
             version {[str]} -- semantic versioning string
             increment {[str]} -- use either 'patch', 'minor', or 'major' to automatically increment the last version
         """
         if increment:
             v = self.current_version()
             if v:
                 sv = semver.VersionInfo.parse(v)
-                if 'post' == increment:
-                    sv = sv.bump_prerelease(token='post')
-                elif 'patch' == increment:
+                if "post" == increment:
+                    sv = sv.bump_prerelease(token="post")
+                elif "patch" == increment:
                     sv = sv.bump_patch()
-                elif 'minor' == increment:
+                elif "minor" == increment:
                     sv = sv.bump_minor()
-                elif 'major' == increment:
+                elif "major" == increment:
                     sv = sv.bump_major()
                 version = str(sv)
             else:
-                raise KACLException("No previously released version found. Incrementing not possible")
+                raise KACLException(
+                    "No previously released version found. Incrementing not possible"
+                )
 
         # check that version is a valid semantic version
-        future_version = semver.VersionInfo.parse(version) # --> will throw a ValueError if version is not a valid semver
+        future_version = semver.VersionInfo.parse(
+            version
+        )  # --> will throw a ValueError if version is not a valid semver
 
         # check if there are changes to release
         if self.has_changes() is False:
-            raise KACLException("The current changelog has no changes. You can only release if changes are available.")
+            raise KACLException(
+                "The current changelog has no changes. You can only release if changes are available."
+            )
 
         # check if the version already exists
-        if self.get(version) != None:
-            raise KACLException(f"The version '{version}' already exists in the changelog. You cannot release the same version twice.")
+        if self.get(version) is not None:
+            raise KACLException(
+                f"The version '{version}' already exists in the changelog. You cannot release the same version twice."
+            )
 
         # check if new version is greater than the last one
         #   1. there has to be an 'unreleased' section
         #   2. All other versions are in descending order
         version_list = self.versions()
-        if len(version_list) > 1: # versions[0] --> unreleased
+        if len(version_list) > 1:  # versions[0] --> unreleased
             last_version = semver.VersionInfo.parse(version_list[1].version())
 
-            last_version_base = semver.VersionInfo(major=last_version.major, minor=last_version.minor, patch=last_version.patch)
-            future_version_base = semver.VersionInfo(major=future_version.major, minor=future_version.minor, patch=future_version.patch)
+            last_version_base = semver.VersionInfo(
+                major=last_version.major,
+                minor=last_version.minor,
+                patch=last_version.patch,
+            )
+            future_version_base = semver.VersionInfo(
+                major=future_version.major,
+                minor=future_version.minor,
+                patch=future_version.patch,
+            )
 
             # check if 'post_release_version_prefix' is set
             post_release_version_prefix = self.config.post_release_version_prefix
             comp_result = 0
             if post_release_version_prefix:
                 #   2.1 Check if 'future version' is a 'post version'
-                if future_version.prerelease and post_release_version_prefix in future_version.prerelease:
-                #   2.2 if 'last version' was a 'post version' continue
-                    if last_version.prerelease and post_release_version_prefix in last_version.prerelease:
+                if (
+                    future_version.prerelease
+                    and post_release_version_prefix in future_version.prerelease
+                ):
+                    #   2.2 if 'last version' was a 'post version' continue
+                    if (
+                        last_version.prerelease
+                        and post_release_version_prefix in last_version.prerelease
+                    ):
                         comp_result = future_version.compare(last_version)
-                #   2.3 if 'last version' was NOT a 'post version' ensure 'post version' has same 'base version'
+                    #   2.3 if 'last version' was NOT a 'post version' ensure 'post version' has same 'base version'
                     elif future_version_base != last_version_base:
-                        comp_result = -1 # indicate error
+                        comp_result = -1  # indicate error
                     else:
                         comp_result = 1
                 else:
                     comp_result = future_version.compare(last_version)
             else:
                 comp_result = future_version.compare(last_version)
 
             if comp_result < 1:
-                raise KACLException(f"The version '{version}' cannot be released since it is smaller than the preceding version '{last_version}'.")
+                raise KACLException(
+                    f"The version '{version}' cannot be released since it is smaller than the preceding version '{last_version}'."
+                )
 
         # get current unreleased changes
-        unreleased_version = self.get('Unreleased')
+        unreleased_version = self.get("Unreleased")
 
         # remove current unrelease version from list
         self.__versions.pop(0)
 
-        self.__versions.insert(0, KACLVersion(version="Unreleased", link=unreleased_version.link()))
+        self.__versions.insert(
+            0, KACLVersion(version="Unreleased", link=unreleased_version.link())
+        )
 
         # convert unreleased version to version
-        self.__versions.insert(1, KACLVersion(version=version,
-                                              link=KACLElement(
-                                                  title=version, body=link),
-                                              date=datetime.datetime.now().strftime("%Y-%m-%d"),
-                                              sections=unreleased_version.sections()))
+        self.__versions.insert(
+            1,
+            KACLVersion(
+                version=version,
+                link=KACLElement(title=version, body=link),
+                date=datetime.datetime.now().strftime("%Y-%m-%d"),
+                sections=unreleased_version.sections(),
+            ),
+        )
 
         if auto_link:
             link_provider = self.__get_link_provider()
             for i in range(2):
                 fargs = {
                     "version": self.__versions[i].version(),
                     "previous_version": None,
-                    "latest_version": version
+                    "latest_version": version,
                 }
 
-                if len(self.__versions) > i+1:
-                    fargs["previous_version"] = self.__versions[i+1].version()
+                if len(self.__versions) > i + 1:
+                    fargs["previous_version"] = self.__versions[i + 1].version()
 
-                if 'unreleased' in self.__versions[i].version().lower():
-                    self.__versions[i].set_link( link_provider.unreleased_changes(**fargs) )
+                if "unreleased" in self.__versions[i].version().lower():
+                    self.__versions[i].set_link(
+                        link_provider.unreleased_changes(**fargs)
+                    )
                 else:
                     if fargs["previous_version"]:
-                        self.__versions[i].set_link( link_provider.compare_versions(**fargs) )
+                        self.__versions[i].set_link(
+                            link_provider.compare_versions(**fargs)
+                        )
                     else:
-                        self.__versions[i].set_link( link_provider.initial_version(**fargs) )
+                        self.__versions[i].set_link(
+                            link_provider.initial_version(**fargs)
+                        )
 
     def get(self, version):
         """Returns the selected version
 
         Arguments:
             version {[str]} -- semantic versioning string
 
         Returns:
             [KACLVersion] -- version object with all information
         """
-        res = [x for x in self.__versions if x.version()
-               and version.capitalize() == x.version()]
+        res = [
+            x
+            for x in self.__versions
+            if x.version() and version.capitalize() == x.version()
+        ]
         if res and len(res):
             return res[0]
 
     def current_version(self):
         """returns the current version (last released)
 
         Returns:
             [str] -- latest released version, None if none is available
         """
         version_list = self.versions()
         for v in version_list:
-            if v.version().lower() != 'unreleased':
+            if v.version().lower() != "unreleased":
                 return v.version()
 
-    def generate_links(self, host_url=None, compare_versions_template=None, unreleased_changes_template=None, initial_version_template=None):
+    def generate_links(
+        self,
+        host_url=None,
+        compare_versions_template=None,
+        unreleased_changes_template=None,
+        initial_version_template=None,
+    ):
         """automatically generates links for all versions
 
         Returns: None
         """
-        link_provider = self.__get_link_provider(host_url=host_url,
-                                                 compare_versions_template=compare_versions_template,
-                                                 unreleased_changes_template=unreleased_changes_template,
-                                                 initial_version_template=initial_version_template)
+        link_provider = self.__get_link_provider(
+            host_url=host_url,
+            compare_versions_template=compare_versions_template,
+            unreleased_changes_template=unreleased_changes_template,
+            initial_version_template=initial_version_template,
+        )
 
         versions = self.versions()
         if len(versions) > 1:
-            for i in range(len(versions)-1):
+            for i in range(len(versions) - 1):
                 fargs = {
                     "version": versions[i].version(),
-                    "previous_version": versions[i+1].version(),
-                    "latest_version": self.current_version()
+                    "previous_version": versions[i + 1].version(),
+                    "latest_version": self.current_version(),
                 }
 
-                if 'unreleased' in versions[i].version().lower():
-                    versions[i].set_link( link_provider.unreleased_changes(**fargs) )
+                if "unreleased" in versions[i].version().lower():
+                    versions[i].set_link(link_provider.unreleased_changes(**fargs))
                 else:
-                    versions[i].set_link( link_provider.compare_versions(**fargs) )
-            versions[-1].set_link( link_provider.initial_version(**fargs) )
+                    versions[i].set_link(link_provider.compare_versions(**fargs))
+            versions[-1].set_link(link_provider.initial_version(**fargs))
         elif len(versions) == 1:
             fargs = {
                 "version": versions[0].version(),
-                "latest_version": self.current_version()
+                "latest_version": self.current_version(),
             }
 
-            if 'unreleased' in versions[0].version().lower():
-                versions[0].set_link( link_provider.initial_version(version="master") )
+            if "unreleased" in versions[0].version().lower():
+                versions[0].set_link(link_provider.initial_version(version="master"))
             else:
-                versions[0].set_link( link_provider.initial_version(**fargs) )
-
+                versions[0].set_link(link_provider.initial_version(**fargs))
 
     def header(self):
         """Gives access to the top level heading element
 
         Returns:
             [KACLElement] -- object holding all information of the top level heading
         """
@@ -440,21 +500,23 @@
         Returns:
             [list] -- list of KACLVersions
         """
         return self.__versions
 
     @staticmethod
     def init():
-        return KACLDocument.parse("""# Changelog
+        return KACLDocument.parse(
+            """# Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
-        """)
+        """
+        )
 
     @staticmethod
     def parse(data):
         """Parses a given text object and returns the KACLDocument
 
         Arguments:
             data {[str]} -- markdown text holding the changelog
@@ -462,15 +524,17 @@
         Returns:
             [KACLDocument] -- object holding all information
         """
 
         data_lf = data.replace(WINDOWS_LINE_ENDING, UNIX_LINE_ENDING)
 
         # First check if there are link references and split the document where they begin
-        link_reference_begin, link_references = KACLParser.parse_link_references(data_lf)
+        link_reference_begin, link_references = KACLParser.parse_link_references(
+            data_lf
+        )
 
         changelog_body = data_lf
         if link_reference_begin:
             changelog_body = data_lf[:link_reference_begin]
 
         # read header
         headers = KACLParser.parse_header(changelog_body, 1, 2)
@@ -479,33 +543,59 @@
         versions = KACLParser.parse_header(changelog_body, 2, 2)
         versions = [KACLVersion(element=x) for x in versions]
 
         # set link references into versions if available
         for v in versions:
             v.set_link(link_references.get(v.version(), None))
 
-        return KACLDocument(data=data, headers=headers, versions=versions, link_references=link_references)
-
-
-    def __get_link_provider(self, host_url=None, compare_versions_template=None, unreleased_changes_template=None, initial_version_template=None):
+        return KACLDocument(
+            data=data,
+            headers=headers,
+            versions=versions,
+            link_references=link_references,
+        )
+
+    def __get_link_provider(
+        self,
+        host_url=None,
+        compare_versions_template=None,
+        unreleased_changes_template=None,
+        initial_version_template=None,
+    ):
         host_url = host_url if host_url else self.config.link_host_url
-        compare_versions_template = compare_versions_template if compare_versions_template else self.config.links_compare_versions_template
-        unreleased_changes_template = unreleased_changes_template if unreleased_changes_template else self.config.links_unreleased_changes_template
-        initial_version_template = initial_version_template if initial_version_template else self.config.links_initial_version_template
+        compare_versions_template = (
+            compare_versions_template
+            if compare_versions_template
+            else self.config.links_compare_versions_template
+        )
+        unreleased_changes_template = (
+            unreleased_changes_template
+            if unreleased_changes_template
+            else self.config.links_unreleased_changes_template
+        )
+        initial_version_template = (
+            initial_version_template
+            if initial_version_template
+            else self.config.links_initial_version_template
+        )
 
         if host_url is None:
-            if 'CI_PROJECT_URL' in os.environ:
-                host_url = os.environ['CI_PROJECT_URL']
+            if "CI_PROJECT_URL" in os.environ:
+                host_url = os.environ["CI_PROJECT_URL"]
             else:
                 try:
                     repo = git.Repo(os.getcwd())
                     remote = repo.remote()
                     for url in remote.urls:
                         host_url = url
                         break
-                except:
-                    raise KACLException("ERROR: Could not determine project url. Update your config or run within a valid git repository")
+                except Exception:
+                    raise KACLException(
+                        "ERROR: Could not determine project url. Update your config or run within a valid git repository"
+                    )
 
-        return LinkProvider(host_url=host_url,
-                            compare_versions_template=compare_versions_template,
-                            unreleased_changes_template=unreleased_changes_template,
-                            initial_version_template=initial_version_template)
+        return LinkProvider(
+            host_url=host_url,
+            compare_versions_template=compare_versions_template,
+            unreleased_changes_template=unreleased_changes_template,
+            initial_version_template=initial_version_template,
+        )
```

### Comparing `python-kacl-0.3.4/kacl/kacl_cli.py` & `python-kacl-0.4.0/kacl/kacl_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,333 +1,516 @@
 # -*- coding: utf-8 -*-
-
 """kacl.kacl-cli: provides entry point main()."""
-
-import sys
-import os
-import kacl
-import click
 import json
-import semver
+import os
+import sys
 import traceback
-import git
 from datetime import datetime
 
+import click
+import git
+import semver
+
+import kacl
+from kacl.config import KACLConfig
 from kacl.exception import KACLException
 
+
 def load_changelog(ctx):
-    config_file_path = ctx.obj['config']
-    file = ctx.obj['file']
+    config_file_path = ctx.obj["config"]
+    input_file = ctx.obj["file"]
 
-    default_config_path = os.path.join(os.getcwd(), '.kacl.yml')
+    default_config_path = os.path.join(os.getcwd(), ".kacl.yml")
     if not config_file_path and os.path.exists(default_config_path):
-        kacl_config = kacl.KACLConfig(default_config_path)
+        kacl_config = KACLConfig(default_config_path)
     elif config_file_path:
-        kacl_config = kacl.KACLConfig(config_file_path)
+        kacl_config = KACLConfig(config_file_path)
     else:
-        kacl_config = kacl.KACLConfig()
+        kacl_config = KACLConfig()
 
-    if file:
-        kacl_config.changelog_file_path = file
+    if input_file:
+        kacl_config.changelog_file_path = input_file
 
     if not os.path.exists(kacl_config.changelog_file_path):
-        click.echo(click.style("Error: ", fg='red') +
-                    f"{kacl_config.changelog_file_path} not found")
+        click.echo(
+            click.style("Error: ", fg="red")
+            + f"{kacl_config.changelog_file_path} not found"
+        )
         sys.exit(1)
 
     # read the changelog
     kacl_changelog = kacl.load(kacl_config.changelog_file_path)
     kacl_changelog.config = kacl_config
 
     # share the objects
     return kacl_changelog
 
+
 def prefixed_environ():
     return dict((("${}".format(key), value) for key, value in os.environ.items()))
 
+
 @click.group(invoke_without_command=True)
-@click.option('-v', '--version', is_flag=True, required=False, help='Prints the current version of the CLI.')
-@click.option('-c', '--config', required=False, default=None, type=click.Path(exists=False, dir_okay=False, file_okay=True), help='Path to kacl config file.', show_default=True)
-@click.option('-f', '--file', required=False, default=None, type=click.Path(exists=True, dir_okay=False, file_okay=True), help='Path to changelog file.', show_default=True)
+@click.option(
+    "-v",
+    "--version",
+    is_flag=True,
+    required=False,
+    help="Prints the current version of the CLI.",
+)
+@click.option(
+    "-c",
+    "--config",
+    required=False,
+    default=None,
+    type=click.Path(exists=False, dir_okay=False, file_okay=True),
+    help="Path to kacl config file.",
+    show_default=True,
+)
+@click.option(
+    "-f",
+    "--file",
+    required=False,
+    default=None,
+    type=click.Path(exists=True, dir_okay=False, file_okay=True),
+    help="Path to changelog file.",
+    show_default=True,
+)
 @click.pass_context
 def cli(ctx, version=None, config=None, file=None):
     if ctx.obj is None:
         ctx.obj = dict()
 
-    ctx.obj['config'] = config
-    ctx.obj['file'] = file
+    ctx.obj["config"] = config
+    ctx.obj["file"] = file
 
     # if --version was given, print version and exit directly
     if version:
         click.echo(kacl.__version__)
         sys.exit(0)
 
 
 @cli.command()
 @click.pass_context
-@click.argument('section', type=str)
-@click.argument('message', type=str)
-@click.option('-m', '--modify', is_flag=True, help='This option will add the changes directly into changelog file.')
+@click.argument("section", type=str)
+@click.argument("message", type=str)
+@click.option(
+    "-m",
+    "--modify",
+    is_flag=True,
+    help="This option will add the changes directly into changelog file.",
+)
 def add(ctx, section, message, modify):
-    """Adds a given message to a specified unreleased section. Use '--modify' to directly modify the changelog file.
-    """
+    """Adds a given message to a specified unreleased section. Use '--modify' to directly modify the changelog file."""
     kacl_changelog = load_changelog(ctx)
 
     # add changes to changelog
     kacl_changelog.add(section=section, data=message)
     kacl_changelog_content = kacl.dump(kacl_changelog)
     if modify:
-        with open(kacl_changelog.config.changelog_file_path, 'w') as f:
+        with open(kacl_changelog.config.changelog_file_path, "w") as f:
             f.write(kacl_changelog_content)
         f.close()
     else:
         click.echo(kacl_changelog_content)
 
 
 @cli.command()
 @click.pass_context
 def current(ctx):
-    """Returns the current version from the Changelog.
-    """
+    """Returns the current version from the Changelog."""
     kacl_changelog = load_changelog(ctx)
 
     current_version = kacl_changelog.current_version()
     click.echo(current_version)
 
 
 @cli.command()
 @click.pass_context
-@click.argument('version', type=str)
+@click.argument("version", type=str)
 def get(ctx, version):
-    """Returns a given version from the Changelog.
-    """
+    """Returns a given version from the Changelog."""
     kacl_changelog = load_changelog(ctx)
 
     # add changes to changelog
     kacl_version = kacl_changelog.get(version)
 
     if kacl_version:
         kacl_changelog_content = kacl.dump(kacl_version)
         click.echo(kacl_changelog_content)
     else:
-        click.echo(click.style("Error: ", fg='red') +
-                   f'"{version}" could not be found in changelog.')
+        click.echo(
+            click.style("Error: ", fg="red")
+            + f'"{version}" could not be found in changelog.'
+        )
         sys.exit(1)
 
 
 @cli.group(invoke_without_command=True)
 @click.pass_context
 def link(ctx):
-    """Lets you modify version links
-    """
+    """Lets you modify version links"""
     pass
 
+
 @link.command()
 @click.pass_context
-@click.option('-m', '--modify', is_flag=True, help='This option will add the changes directly into changelog file.')
-@click.option('--host-url', required=False, default=None, type=str, help='Host url to the git service. (i.e https://github.com/mschmieder/python-kacl)', show_default=True)
-@click.option('--compare-versions-template', required=False, default=None, type=str, help='Template string for version comparison link.', show_default=True)
-@click.option('--unreleased-changes-template', required=False, default=None, type=str, help='Template string for unreleased changes link.', show_default=True)
-@click.option('--initial-version-template', required=False, default=None, type=str, help='Template string for initial version link.', show_default=True)
-def generate(ctx, modify, host_url, compare_versions_template, unreleased_changes_template, initial_version_template):
+@click.option(
+    "-m",
+    "--modify",
+    is_flag=True,
+    help="This option will add the changes directly into changelog file.",
+)
+@click.option(
+    "--host-url",
+    required=False,
+    default=None,
+    type=str,
+    help="Host url to the git service. (i.e https://github.com/mschmieder/python-kacl)",
+    show_default=True,
+)
+@click.option(
+    "--compare-versions-template",
+    required=False,
+    default=None,
+    type=str,
+    help="Template string for version comparison link.",
+    show_default=True,
+)
+@click.option(
+    "--unreleased-changes-template",
+    required=False,
+    default=None,
+    type=str,
+    help="Template string for unreleased changes link.",
+    show_default=True,
+)
+@click.option(
+    "--initial-version-template",
+    required=False,
+    default=None,
+    type=str,
+    help="Template string for initial version link.",
+    show_default=True,
+)
+def generate(
+    ctx,
+    modify,
+    host_url,
+    compare_versions_template,
+    unreleased_changes_template,
+    initial_version_template,
+):
     kacl_changelog = load_changelog(ctx)
 
-    kacl_changelog.generate_links(host_url=host_url,
-                                  compare_versions_template=compare_versions_template,
-                                  unreleased_changes_template=unreleased_changes_template,
-                                  initial_version_template=initial_version_template)
+    kacl_changelog.generate_links(
+        host_url=host_url,
+        compare_versions_template=compare_versions_template,
+        unreleased_changes_template=unreleased_changes_template,
+        initial_version_template=initial_version_template,
+    )
 
     kacl_changelog_content = kacl.dump(kacl_changelog)
     if modify:
-        with open(kacl_changelog.config.changelog_file_path, 'w') as f:
+        with open(kacl_changelog.config.changelog_file_path, "w") as f:
             f.write(kacl_changelog_content)
         f.close()
     else:
         click.echo(kacl_changelog_content)
 
 
 @cli.command()
 @click.pass_context
-@click.option('--json', 'as_json', is_flag=True, help='Print validation output as json.')
+@click.option(
+    "--json", "as_json", is_flag=True, help="Print validation output as json."
+)
 def verify(ctx, as_json):
     """Verifies if the changelog is in "keep-a-changelog" format.
     Use '--json' get JSON formatted output that can be easier integrated into CI workflows.
     Exit code is the number of identified errors.
     """
     kacl_changelog = load_changelog(ctx)
-    kacl_changelog_filepath = os.path.basename(kacl_changelog.config.changelog_file_path)
+    kacl_changelog_filepath = os.path.basename(
+        kacl_changelog.config.changelog_file_path
+    )
 
     valid = kacl_changelog.is_valid()
     validation = kacl_changelog.validate()
     if as_json:
         validation_map = validation.convert_to_dict()
         click.echo(json.dumps(validation_map, sort_keys=True, indent=4))
     else:
         for error in validation.errors():
             start_char_pos, end_char_pos = error.position()
 
             char_indicator = start_char_pos
-            if start_char_pos == None:
+            if start_char_pos is None:
                 char_indicator = 0
 
-            click.echo(click.style(
-                kacl_changelog_filepath + ':' +
-                f'{error.line_number()}:{char_indicator}: ' +
-                click.style('error: ', fg='red') +
-                error.error_message(), bold=True))
+            click.echo(
+                click.style(
+                    kacl_changelog_filepath
+                    + ":"
+                    + f"{error.line_number()}:{char_indicator}: "
+                    + click.style("error: ", fg="red")
+                    + error.error_message(),
+                    bold=True,
+                )
+            )
 
             if error.line():
                 click.echo(error.line())
-                if start_char_pos != None and end_char_pos != None:
-                    mark_length = end_char_pos-start_char_pos-1
-                    click.echo(' '*start_char_pos + click.style('^' + '~'*(mark_length), fg="green"))
+                if start_char_pos is not None and end_char_pos is not None:
+                    mark_length = end_char_pos - start_char_pos - 1
+                    click.echo(
+                        " " * start_char_pos
+                        + click.style("^" + "~" * (mark_length), fg="green")
+                    )
         if not valid:
-            click.echo(f'{len(validation.errors())} error(s) generated.')
+            click.echo(f"{len(validation.errors())} error(s) generated.")
         else:
-            click.secho('Success', fg='green')
+            click.secho("Success", fg="green")
 
     if not valid:
         sys.exit(len(validation.errors()))
 
 
 @cli.command()
 @click.pass_context
-@click.argument('version', type=str)
-@click.option('-m', '--modify', is_flag=True, help='This option will add the changes directly into changelog file.')
-@click.option('-l', '--link', required=False, default=None, type=str, help='A url that the version will be linked with.', show_default=True)
-@click.option('-g', '--auto-link', is_flag=True, help='Will automatically create and update necessary links.')
-@click.option('-c', '--commit', is_flag=True, help='If passed this will create a git commit with the changed Changelog.')
-@click.option('--no-commit', is_flag=True, help='This will disabled the commit option even if it is set in the config.')
-@click.option('--commit-message', required=False, default=None, type=str, help='The commit message to use when using --commit flag')
-@click.option('-t', '--tag', is_flag=True, help='If passed this will create a git tag for the newly released version.')
-@click.option('--tag-name', required=False, default=None, type=str, help='The tag name to use when using --tag flag')
-@click.option('--tag-description', required=False, default=None, type=str, help='The tag description text to use when using --tag flag')
-@click.option('-d', '--allow-dirty', is_flag=True, help='If passed this will allow to commit/tag even on a "dirty".')
-def release(ctx, version, modify, link, auto_link, commit, no_commit, commit_message, tag, tag_name, tag_description, allow_dirty):
+@click.argument("version", type=str)
+@click.option(
+    "-m",
+    "--modify",
+    is_flag=True,
+    help="This option will add the changes directly into changelog file.",
+)
+@click.option(
+    "-l",
+    "--link",
+    required=False,
+    default=None,
+    type=str,
+    help="A url that the version will be linked with.",
+    show_default=True,
+)
+@click.option(
+    "-g",
+    "--auto-link",
+    is_flag=True,
+    help="Will automatically create and update necessary links.",
+)
+@click.option(
+    "-c",
+    "--commit",
+    is_flag=True,
+    help="If passed this will create a git commit with the changed Changelog.",
+)
+@click.option(
+    "--no-commit",
+    is_flag=True,
+    help="This will disabled the commit option even if it is set in the config.",
+)
+@click.option(
+    "--commit-message",
+    required=False,
+    default=None,
+    type=str,
+    help="The commit message to use when using --commit flag",
+)
+@click.option(
+    "-t",
+    "--tag",
+    is_flag=True,
+    help="If passed this will create a git tag for the newly released version.",
+)
+@click.option(
+    "--tag-name",
+    required=False,
+    default=None,
+    type=str,
+    help="The tag name to use when using --tag flag",
+)
+@click.option(
+    "--tag-description",
+    required=False,
+    default=None,
+    type=str,
+    help="The tag description text to use when using --tag flag",
+)
+@click.option(
+    "-d",
+    "--allow-dirty",
+    is_flag=True,
+    help='If passed this will allow to commit/tag even on a "dirty".',
+)
+def release(
+    ctx,
+    version,
+    modify,
+    link,
+    auto_link,
+    commit,
+    no_commit,
+    commit_message,
+    tag,
+    tag_name,
+    tag_description,
+    allow_dirty,
+):
     """Creates a release for the latest 'unreleased' changes. Use '--modify' to directly modify the changelog file.
     You can automatically use the latest version by using the version keywords 'major', 'minor', 'patch', 'post'
 
     Example:
 
         kacl-cli release 1.0.0
 
         kacl-cli release major|minor|patch|post
     """
     kacl_changelog = load_changelog(ctx)
     kacl_config = kacl_changelog.config
 
     if not kacl_changelog.is_valid():
-        click.echo(click.style("Error: ", fg='red') +
-                       f"Changelog is not valid. Run 'kacl-cli verify' for more information.")
+        click.echo(
+            click.style("Error: ", fg="red")
+            + "Changelog is not valid. Run 'kacl-cli verify' for more information."
+        )
         sys.exit(1)
 
     # check if the version string indicates automatic increment
     increment = None
-    if version in ['major', 'minor', 'patch', 'post']:
+    if version in ["major", "minor", "patch", "post"]:
         increment = version
         version = None  # reset
     else:
         # check if version is a valid semantic version
         try:
             semver.VersionInfo.parse(version)
-        except:
-            click.echo(click.style("Error: ", fg='red') +
-                       f'"{version}" not a valid semantic version.')
+        except Exception:
+            click.echo(
+                click.style("Error: ", fg="red")
+                + f'"{version}" not a valid semantic version.'
+            )
             sys.exit(1)
 
     if not kacl_changelog.has_changes():
-        click.echo(click.style("Error: ", fg='red') +
-                   'The current changelog has no changes. You can only release if changes are available.')
+        click.echo(
+            click.style("Error: ", fg="red")
+            + "The current changelog has no changes. You can only release if changes are available."
+        )
         sys.exit(1)
 
     # get the latest_version before the release
     latest_version = kacl_changelog.current_version()
 
     # check config to see if we need to autogenerate changes
     if auto_link is False and kacl_config.link_auto_generate:
         auto_link = True
 
-    kacl_changelog.release(version=version, link=link, auto_link=auto_link, increment=increment)
+    kacl_changelog.release(
+        version=version, link=link, auto_link=auto_link, increment=increment
+    )
 
     # get the new version
     new_version = kacl_changelog.current_version()
 
     # dump the content
     kacl_changelog_content = kacl.dump(kacl_changelog)
 
     # check if we should modify the file
     if modify:
-        with open(kacl_changelog.config.changelog_file_path, 'w') as f:
+        with open(kacl_changelog.config.changelog_file_path, "w") as f:
             f.write(kacl_changelog_content)
         f.close()
 
         if not no_commit:
-            if commit or tag or kacl_config.git_create_commit or kacl_config.git_create_tag:
-                vcs_context = {
-                    "latest_version": latest_version,
-                    "new_version": new_version,
-                }
-                time_context = {
-                    'now': datetime.now(),
-                    'utcnow': datetime.utcnow(),
-                }
-                vcs_context.update(time_context)
-                vcs_context.update(prefixed_environ())
-
-                commit_message  = commit_message if commit_message != None else kacl_config.git_commit_message
-                tag_name        = tag_name if tag_name != None else kacl_config.git_tag_name
-                tag_description = tag_description if tag_description != None else kacl_config.git_tag_description
-
-                repo = None
-                try:
-                    repo = git.Repo(os.getcwd())
-                except git.InvalidGitRepositoryError:
-                    click.echo(click.style("Error: ", fg='red') +
-                            f'"{os.getcwd()}" is no valid git repository.')
-
-                if repo:
-                    if not repo.is_dirty() and not allow_dirty:
-                        click.echo(click.style("Error: ", fg='red') +
-                                f"Repository is marked 'dirty'. Use --allow-dirty if you want to commit/tag on a dirty repository")
-
-                    if commit or kacl_config.git_create_commit:
-                        repo.git.add(kacl_config.changelog_file_path)
-                        for f in kacl_config.git_commit_additional_files:
-                            repo.git.add(f)
-                        repo.git.commit('-m', commit_message.format(**vcs_context))
-
-                    if tag or kacl_config.git_create_tag:
-                        repo.create_tag(tag_name.format(**vcs_context),
-                                        message=tag_description.format(**vcs_context))
+            return
+
+        if commit or tag or kacl_config.git_create_commit or kacl_config.git_create_tag:
+            vcs_context = {
+                "latest_version": latest_version,
+                "new_version": new_version,
+            }
+            time_context = {
+                "now": datetime.now(),
+                "utcnow": datetime.utcnow(),
+            }
+            vcs_context.update(time_context)
+            vcs_context.update(prefixed_environ())
+
+            commit_message = (
+                commit_message
+                if commit_message is not None
+                else kacl_config.git_commit_message
+            )
+            tag_name = tag_name if tag_name is not None else kacl_config.git_tag_name
+            tag_description = (
+                tag_description
+                if tag_description is not None
+                else kacl_config.git_tag_description
+            )
+
+            repo = None
+            try:
+                repo = git.Repo(os.getcwd())
+            except git.InvalidGitRepositoryError:
+                click.echo(
+                    click.style("Error: ", fg="red")
+                    + f'"{os.getcwd()}" is no valid git repository.'
+                )
+
+            if repo:
+                if not repo.is_dirty() and not allow_dirty:
+                    click.echo(
+                        click.style("Error: ", fg="red")
+                        + "Repository is marked 'dirty'. Use --allow-dirty if you want to commit/tag on a dirty repository"
+                    )
+
+                if commit or kacl_config.git_create_commit:
+                    repo.git.add(kacl_config.changelog_file_path)
+                    for f in kacl_config.git_commit_additional_files:
+                        repo.git.add(f)
+                    repo.git.commit("-m", commit_message.format(**vcs_context))
+
+                if tag or kacl_config.git_create_tag:
+                    repo.create_tag(
+                        tag_name.format(**vcs_context),
+                        message=tag_description.format(**vcs_context),
+                    )
     else:
         click.echo(kacl_changelog_content)
 
 
 @cli.command()
-@click.option('-o', '--output-file', required=False, type=click.Path(exists=False), help='File to write the created changelog to.')
+@click.option(
+    "-o",
+    "--output-file",
+    required=False,
+    type=click.Path(exists=False),
+    help="File to write the created changelog to.",
+)
 def new(output_file):
-    """Creates a new changelog.
-    """
+    """Creates a new changelog."""
     kacl_changelog = kacl.new()
     kacl_changelog_content = kacl.dump(kacl_changelog)
     if output_file:
-        with open(output_file, 'w') as f:
+        with open(output_file, "w") as f:
             f.write(kacl_changelog_content)
         f.close()
     else:
         click.echo(kacl_changelog_content)
 
 
 def start():
     try:
         cli(obj={})
     except SystemExit as e:
         sys.exit(e.code)
     except KACLException as e:
-        click.secho(str(e), fg='red')
+        click.secho(str(e), fg="red")
         sys.exit(1)
-    except:
+    except Exception:
         click.echo(traceback.format_exc())
         sys.exit(1)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     start()
```

### Comparing `python-kacl-0.3.4/kacl/link_provider.py` & `python-kacl-0.4.0/kacl/link_provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 import re
 
+
 class LinkProvider:
-    def __init__(self, host_url=None, compare_versions_template=None, unreleased_changes_template=None, initial_version_template=None):
-        self.host_url = self.__sanatize_url(host_url)
+    def __init__(
+        self,
+        host_url=None,
+        compare_versions_template=None,
+        unreleased_changes_template=None,
+        initial_version_template=None,
+    ):
+        self.host_url = self.__sanitize_url(host_url)
         self.compare_versions_template = compare_versions_template
         self.unreleased_changes_template = unreleased_changes_template
         self.initial_version_template = initial_version_template
 
-    def __sanatize_url(self, url):
+    def __sanitize_url(self, url):
         if url:
-            regExpr = r'git@(.*):(.*).git'
-            m = re.search(regExpr, url)
+            reg_expr = r"git@(.*):(.*).git"
+            m = re.search(reg_expr, url)
             if m:
-                return f'https://{m.group(1)}/{m.group(2)}'
+                return f"https://{m.group(1)}/{m.group(2)}"
         return url
 
-    def compare_versions(self, version=None, previous_version=None, latest_version=None):
+    def compare_versions(
+        self, version=None, previous_version=None, latest_version=None
+    ):
         return self.compare_versions_template.format(
             host=self.host_url,
             version=version,
             previous_version=previous_version,
             latest_version=latest_version,
         )
 
@@ -27,14 +36,16 @@
         return self.initial_version_template.format(
             host=self.host_url,
             version=version,
             previous_version=previous_version,
             latest_version=latest_version,
         )
 
-    def unreleased_changes(self, version=None, previous_version=None, latest_version=None):
+    def unreleased_changes(
+        self, version=None, previous_version=None, latest_version=None
+    ):
         return self.unreleased_changes_template.format(
             host=self.host_url,
             version=version,
             previous_version=previous_version,
             latest_version=latest_version,
-        )
+        )
```

### Comparing `python-kacl-0.3.4/kacl/parser.py` & `python-kacl-0.4.0/kacl/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,69 @@
-from .element import KACLElement
-
 import re
 
+from kacl.element import KACLElement
+
+
 class KACLParser:
-    semver_regex = r'(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)(?:-((?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+([0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?'
+    semver_regex = r"(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)(?:-((?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+([0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?"
 
     @staticmethod
     def parse_header(text, start_depth, end_depth=None, line_offset=0):
         if not end_depth:
             end_depth = start_depth
 
         elements = []
-        reg_expr_start = r'(\n{depth}|^{depth})\s+?(.*)\n'.format(depth="#"*start_depth)
-        reg_expr_end = r'(\n{depth}|^{depth})\s+?(.*)\n'.format(depth="#"*end_depth)
+        reg_expr_start = r"(\n{depth}|^{depth})\s+?(.*)\n".format(
+            depth="#" * start_depth
+        )
+        reg_expr_end = r"(\n{depth}|^{depth})\s+?(.*)\n".format(depth="#" * end_depth)
         for match in re.finditer(reg_expr_start, text):
             # find end of section
             raw = match.group().strip()
             title = match.group(2).strip()
             start = match.start()
             end = match.end()
-            line_number = text[:start].count('\n')+line_offset
-            if match.group()[0] == '\n':
+            line_number = text[:start].count("\n") + line_offset
+            if match.group()[0] == "\n":
                 line_number += 2
             else:
                 line_number += 1
 
             next_match = re.search(reg_expr_end, text[end:])
             body = None
             if next_match:
-                body = text[end:next_match.start()+end]
+                body = text[end : next_match.start() + end]
             else:
                 body = text[end:]
-            elements.append(KACLElement(raw=raw, title=title,
-                                        body=body, line_number=line_number))
+            elements.append(
+                KACLElement(raw=raw, title=title, body=body, line_number=line_number)
+            )
 
         return elements
 
     @staticmethod
     def parse_link_references(text):
         link_references = dict()
         begin = None
-        reg_expr = r'\n\[(.*)\]:(.*)'
+        reg_expr = r"\n\[(.*)\]:(.*)"
         for match in re.finditer(reg_expr, text):
             if begin is None:
                 begin = match.start()
             version = match.group(1).strip()
             link = match.group(2).strip()
-            line_number = text[:match.start()].count('\n')+1
-            link_references[version] = KACLElement(raw=match.group().strip(), title=version, body=link, line_number=line_number)
+            line_number = text[: match.start()].count("\n") + 1
+            link_references[version] = KACLElement(
+                raw=match.group().strip(),
+                title=version,
+                body=link,
+                line_number=line_number,
+            )
 
         return begin, link_references
 
     @staticmethod
     def parse_sem_ver(text, regex=None):
-        if regex == None:
+        if regex is None:
             regex = KACLParser.semver_regex
         m = re.search(regex, text)
         if m:
             return m.group().strip()
```

### Comparing `python-kacl-0.3.4/kacl/serializer.py` & `python-kacl-0.4.0/kacl/serializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,67 @@
-from .document import KACLDocument
-from .element import KACLElement
-from .version import KACLVersion
-from .changes import KACLChanges
+from kacl.changes import KACLChanges
+from kacl.document import KACLDocument
+from kacl.element import KACLElement
+from kacl.version import KACLVersion
+
 
 class KACLMarkdownSerializer:
     def __init__(self):
         pass
 
     def serialize(self, document):
         if isinstance(document, KACLDocument):
-            data = [ self.__serialize_header(document.header()),
-                    document.header().body() ]
+            data = [
+                self.__serialize_header(document.header()),
+                document.header().body(),
+            ]
 
             link_references = []
             for version in document.versions():
-                data.extend([ self.__serialize_version(version), '' ])
+                data.extend([self.__serialize_version(version), ""])
                 if version.has_link_reference():
                     link_references.append(self.__serialize_link_reference(version))
 
             data.extend(link_references)
 
-            if data[-1] != '':
-                data.append('')
+            if data[-1] != "":
+                data.append("")
 
-            return '\n'.join(data)
+            return "\n".join(data)
         elif isinstance(document, KACLVersion):
             return self.__serialize_version(document)
 
     def __serialize_header(self, obj):
         if isinstance(obj, KACLChanges):
-            return f'### {obj.title()}'
+            return f"### {obj.title()}"
         elif isinstance(obj, KACLVersion):
-            version_decorator_left = ''
-            version_decorator_right = ''
+            version_decorator_left = ""
+            version_decorator_right = ""
             if obj.has_link_reference():
-                version_decorator_left = '['
-                version_decorator_right = ']'
+                version_decorator_left = "["
+                version_decorator_right = "]"
             if obj.date():
-                return f'## {version_decorator_left}{obj.version()}{version_decorator_right} - {obj.date()}'
+                return f"## {version_decorator_left}{obj.version()}{version_decorator_right} - {obj.date()}"
             else:
-                return f'## {version_decorator_left}{obj.version()}{version_decorator_right}'
+                return f"## {version_decorator_left}{obj.version()}{version_decorator_right}"
         elif isinstance(obj, KACLElement):
-            return f'# {obj.title()}'
+            return f"# {obj.title()}"
 
     def __serialize_version(self, obj):
-        lines = [ self.__serialize_header(obj) ]
+        lines = [self.__serialize_header(obj)]
         for title, changes in obj.sections().items():
-            lines.extend([
-                self.__serialize_header(changes),
-                self.__serialize_list(changes.items()),
-                ''
-            ])
+            lines.extend(
+                [
+                    self.__serialize_header(changes),
+                    self.__serialize_list(changes.items()),
+                    "",
+                ]
+            )
 
-        return '\n'.join(lines).strip()
+        return "\n".join(lines).strip()
 
     def __serialize_list(self, obj):
-        lines = [ f'- {x}' for x in obj ]
-        return '\n'.join(lines)
+        lines = [f"- {x}" for x in obj]
+        return "\n".join(lines)
 
     def __serialize_link_reference(self, obj):
-        return f'[{obj.version()}]: {obj.link()}'
+        return f"[{obj.version()}]: {obj.link()}"
```

### Comparing `python-kacl-0.3.4/kacl/validation.py` & `python-kacl-0.4.0/kacl/validation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,16 @@
-class KACLValidationError():
-    def __init__(self, line="", line_number=0, start_character_pos=None, end_character_pos=None, error_message=""):
+class KACLValidationError:
+    def __init__(
+        self,
+        line="",
+        line_number=0,
+        start_character_pos=None,
+        end_character_pos=None,
+        error_message="",
+    ):
         self.__line_number = line_number
         self.__start_character_pos = start_character_pos
         self.__end_character_pos = end_character_pos
         self.__error_message = error_message
         self.__line = line
 
     def line_number(self):
@@ -15,40 +22,50 @@
     def line(self):
         return self.__line
 
     def error_message(self):
         return self.__error_message
 
 
-class KACLValidation():
+class KACLValidation:
     def __init__(self):
         self.__validation_errors = []
 
     def is_valid(self):
-        return (len(self.__validation_errors) == 0)
+        return len(self.__validation_errors) == 0
 
     def errors(self):
         return self.__validation_errors
 
-    def add_error(self, line, line_number, error_message, start_character_pos=None, end_character_pos=None):
-        self.__validation_errors.append(KACLValidationError(line=line,
-                                                            line_number=line_number,
-                                                            start_character_pos=start_character_pos,
-                                                            end_character_pos=end_character_pos,
-                                                            error_message=error_message))
-
+    def add_error(
+        self,
+        line,
+        line_number,
+        error_message,
+        start_character_pos=None,
+        end_character_pos=None,
+    ):
+        self.__validation_errors.append(
+            KACLValidationError(
+                line=line,
+                line_number=line_number,
+                start_character_pos=start_character_pos,
+                end_character_pos=end_character_pos,
+                error_message=error_message,
+            )
+        )
 
     def convert_to_dict(self):
         validation_map = dict()
-        validation_map['valid'] = (len(self.__validation_errors) == 0)
+        validation_map["valid"] = len(self.__validation_errors) == 0
         errors = []
         for error in self.__validation_errors:
             error_map = {
                 "line": error.line(),
                 "line_number": error.line_number(),
                 "start_char_pos": error.position()[0],
                 "end_character_pos": error.position()[1],
-                "error_message": error.error_message()
+                "error_message": error.error_message(),
             }
             errors.append(error_map)
-        validation_map['errors'] = errors
+        validation_map["errors"] = errors
         return validation_map
```

### Comparing `python-kacl-0.3.4/kacl/version.py` & `python-kacl-0.4.0/kacl/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-from .element import KACLElement
-from .changes import KACLChanges
-from .parser import KACLParser
-
 import re
+
 import semver
 
+from kacl.changes import KACLChanges
+from kacl.element import KACLElement
+from kacl.parser import KACLParser
+
 
 class KACLVersion(KACLElement):
-    def __init__(self, element=KACLElement(), version="", date="", sections=None, link=None):
-        KACLElement.__init__(self,
-                             raw=element.raw(),
-                             title=element.title(),
-                             body=element.body(),
-                             line_number=element.line_number())
+    def __init__(
+        self, element=KACLElement(), version="", date="", sections=None, link=None
+    ):
+        KACLElement.__init__(
+            self,
+            raw=element.raw(),
+            title=element.title(),
+            body=element.body(),
+            line_number=element.line_number(),
+        )
         self.__date = date
         self.__version = version
         if sections is None:
             self.__sections = dict()
         else:
             self.__sections = sections
         self.__link_reference = None
@@ -25,66 +30,71 @@
     def link(self):
         if self.__link_reference:
             return self.__link_reference.body()
 
     def set_link(self, link):
         if isinstance(link, KACLElement):
             self.__link_reference = link
-        elif link != None:
+        elif link is not None:
             self.__link_reference = KACLElement(title=self.version(), body=link)
 
     def has_link_reference(self):
         if not self.__link_reference:
             return False
         else:
-            return (self.__link_reference.body() != None and len(self.__link_reference.body()))
+            return self.__link_reference.body() is not None and len(
+                self.__link_reference.body()
+            )
 
     def date(self):
         if not len(self.__date):
             title = self.title()
-            m = re.search(r'\d\d\d\d-\d\d-\d\d', title)
+            m = re.search(r"\d\d\d\d-\d\d-\d\d", title)
             if m:
                 self.__date = m.group().strip()
 
         return self.__date
 
     def version(self):
         if not len(self.__version):
             title = self.title()
             version = KACLParser.parse_sem_ver(title)
             if version:
                 self.__version = version
-            elif 'unreleased' in title.lower():
+            elif "unreleased" in title.lower():
                 self.__version = "Unreleased"
 
         return self.__version
 
     def semver(self):
         return semver.VersionInfo.parse(self.version())
 
     def set_version(self, version):
         self.__version = version
 
     def sections(self):
         if not len(self.__sections) and len(self.body().strip()):
             self.__sections = dict()
-            sections = KACLParser.parse_header(text=self.body(),
-                                               start_depth=3,
-                                               end_depth=3,
-                                               line_offset=self.line_number())
+            sections = KACLParser.parse_header(
+                text=self.body(),
+                start_depth=3,
+                end_depth=3,
+                line_offset=self.line_number(),
+            )
             for section in sections:
                 sec = KACLChanges(section)
                 self.__sections[sec.title()] = sec
         return self.__sections
 
     def changes(self, section):
         sections = self.sections()
         if sections and section in sections:
             return sections[section]
 
         return None
 
     def add(self, section, change):
         if section not in self.sections():
-            self.__sections[section] = KACLChanges(KACLElement(
-                title=section, body="", line_number=None))
+            self.__sections[section] = KACLChanges(
+                KACLElement(title=section, body="", line_number=None)
+            )
         self.__sections[section].add(change)
```

### Comparing `python-kacl-0.3.4/python_kacl.egg-info/PKG-INFO` & `python-kacl-0.4.0/python_kacl.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.3.4
+Version: 0.4.0
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
-Home-page: http://github.com/mschmieder/python-kacl
+Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-kacl
 
-[![Build Status](https://travis-ci.org/mschmieder/python-kacl.svg?branch=master)](https://travis-ci.org/mschmieder/python-kacl)
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=mschmieder_python-kacl&metric=coverage)](https://sonarcloud.io/dashboard?id=mschmieder_python-kacl)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=mschmieder_python-kacl&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=mschmieder_python-kacl)
+[![Build Status](https://gitlab.com/schmieder.matthias/python-kacl/badges/main/pipeline.svg?ignore_skipped=true](https://gitlab.com/schmieder.matthias/python-kacl)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=coverage)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
+[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
 
 A tool for verifying and modifying changelog in the [**K**eep-**A-C**hange-**L**og](https://keepachangelog.com/en/1.0.0/) format.
 
 - [python-kacl](#python-kacl)
   - [Installation](#installation)
     - [From Source](#from-source)
     - [Pip Package](#pip-package)
@@ -51,15 +52,15 @@
 - docker
 
 All approaches are described in detail within this section.
 
 ### From Source
 
 ```bash
-git clone https://github.com/mschmieder/python-kacl
+git clone https://gitlab.com/schmieder.matthias/python-kacl
 cd python-kacl
 ```
 
 **Global Install**
 
 ```bash
 pip3 install .
@@ -92,15 +93,15 @@
 ```
 
 ### pre-commit
 
 The package can also be used as a pre-commit hook. Just add the following to your `.pre-commit-config.yaml`
 
 ```yaml
-- repo: https://github.com/mschmieder/python-kacl
+- repo: https://gitlab.com/schmieder.matthias/python-kacl
   rev: 'v0.3.0'
   hooks:
     - id: kacl-verify
 ```
 
 ## CLI
 
@@ -316,16 +317,16 @@
 ### Added
 - `release` command will make sure changelog is valid before doing any changes.
 
 ## 0.2.16 - 2020-01-07
 ### Fixed
 - fixed issue #3 that did not detect linked versions with missing links
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/tree/v1.0.0...HEAD
-[1.0.0]: https://github.com/mschmieder/python-kacl/compare/v0.2.16...v1.0.0
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/tree/v1.0.0...HEAD
+[1.0.0]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v0.2.16...v1.0.0
 ```
 
 **Usage with fixed version**
 
 ```bash
 kacl-cli release 1.0.0
 ```
@@ -345,15 +346,15 @@
 - implemented basic cli with `new`, `get`, `release`, `verify`
 - added `--json` option to `verify` command
 
 ## 0.1.0 - 2019-12-12
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v1.0.0...HEAD
 ```
 
 Example CHANGELOG.md (after):
 
 ```markdown
 # Changelog
 All notable changes to this project will be documented in this file.
@@ -369,15 +370,15 @@
 - implemented basic cli with `new`, `get`, `release`, `verify`
 - added `--json` option to `verify` command
 
 ## 0.1.0 - 2019-12-12
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v1.0.0...HEAD
 ```
 
 **Usage with version increment**
 
 ```bash
 kacl-cli release patch
 ```
@@ -399,30 +400,30 @@
 - implemented basic cli with `new`, `get`, `release`, `verify`
 - added `--json` option to `verify` command
 
 ## 0.1.0 - 2019-12-12
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD
+[Unreleased]: https://gitlab.com/schmieder.matthias/python-kacl/compare/v1.0.0...HEAD
 ```
 
 ## Link Generation
 
 `kacl-cli` let's you easily generate links to your versions. You can automatically generate all links following the desired patterns using `kacl-cli link generate`.
 The link generation can also be easily included into the `release` command and will take care of updating the `unreleased` and `latest_version` section.
 
 ```bash
 Usage: kacl-cli link generate [OPTIONS]
 
 Options:
   -m, --modify                    This option will add the changes directly
                                   into changelog file.
   --host-url TEXT                 Host url to the git service. (i.e
-                                  https://github.com/mschmieder/python-kacl)
+                                  https://gitlab.com/schmieder.matthias/python-kacl)
   --compare-versions-template TEXT
                                   Template string for version comparison link.
   --unreleased-changes-template TEXT
                                   Template string for unreleased changes link.
   --initial-version-template TEXT
                                   Template string for initial version link.
   --help                          Show this message and exit.
@@ -527,15 +528,15 @@
 
 ## Development
 
 With these instructions you can easily setup a development environment
 
 ```bash
 # clone the project
-git clone https://github.com/mschmieder/python-kacl
+git clone https://gitlab.com/schmieder.matthias/python-kacl
 cd python-kacl
 
 # create a virtual env
 python3 -m venv .venv
 source ./venv/bin/activate
 
 # install in development mode
```

### Comparing `python-kacl-0.3.4/python_kacl.egg-info/SOURCES.txt` & `python-kacl-0.4.0/python_kacl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-kacl-0.3.4/setup.py` & `python-kacl-0.4.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-from setuptools import setup
+import os
 import pathlib
+from os import path
+
 import pkg_resources
 from setuptools import find_packages
-from os import path
-import re
+from setuptools import setup
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = re.search(r'^__version__\s*=\s*"(.*)"',
-                    open('kacl/__init__.py').read(),
-                    re.M).group(1)
-
-setup(name='python-kacl',
-      version=version,
-      description='Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"',
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      url='http://github.com/mschmieder/python-kacl',
-      author='Matthias Schmieder',
-      author_email='schmieder.matthias@gmail.com',
-      entry_points={
-           "console_scripts": ['kacl-cli = kacl.kacl_cli:start']
-      },
-      license='MIT',
-      packages=find_packages(),
-      include_package_data=True,
-      python_requires='>=3.6',
-      install_requires=[
-        'click',
-        'semver',
-        'gitpython',
-        'pyyaml'
-      ],
-      zip_safe=False,
-      classifiers= [
-          "License :: OSI Approved :: MIT License",
-          "Programming Language :: Python :: 3",
-          "Programming Language :: Python :: 3.6",
-          "Intended Audience :: Developers",
-          "Topic :: Software Development :: Version Control"
-      ])
+version = "0.4.0"
+
+version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
+
+# read the requirements from requirements.txt
+requirements = []
+with pathlib.Path("requirements.txt").open() as requirements_txt:
+    requirements = [
+        str(requirement)
+        for requirement in pkg_resources.parse_requirements(requirements_txt)
+    ]
+
+
+setup(
+    name="python-kacl",
+    version=version,
+    description='Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://gitlab.com/schmieder.matthias/python-kacl.git",
+    author="Matthias Schmieder",
+    author_email="schmieder.matthias@gmail.com",
+    entry_points={"console_scripts": ["kacl-cli = kacl.kacl_cli:start"]},
+    license="MIT",
+    packages=find_packages(),
+    include_package_data=True,
+    python_requires=">=3.6",
+    install_requires=requirements,
+    zip_safe=False,
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Version Control",
+    ],
+)
```

### Comparing `python-kacl-0.3.4/tests/snapshot_directory.py` & `python-kacl-0.4.0/tests/snapshot_directory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import os
 from pathlib import Path
 
 
-def snapshot_directory(snapshot, directory_path, dir_excludes=[".git"], file_excludes=[], sanitize_callbacks={}):
+def snapshot_directory(
+    snapshot,
+    directory_path,
+    dir_excludes=[".git"],
+    file_excludes=[],
+    sanitize_callbacks={},
+):
     snapshot_dir = {}
 
     for root, dirs, files in os.walk(directory_path, topdown=True):
         dirs[:] = [d for d in dirs if d not in dir_excludes]
 
         for file in files:
             if file in file_excludes:
```

### Comparing `python-kacl-0.3.4/tests/test_cli.py` & `python-kacl-0.4.0/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,129 +1,144 @@
+import json
+import os
+import shutil
+
 from click.testing import CliRunner
+from freezegun import freeze_time
+
 from kacl.kacl_cli import cli
 from tests.snapshot_directory import snapshot_directory
-from freezegun import freeze_time
 
-import json
-import os
-import shutil
 
 def test_verify():
     runner = CliRunner()
-    result = runner.invoke(cli, ['-f', 'tests/data/CHANGELOG.md' , 'verify'])
+    result = runner.invoke(cli, ["-f", "tests/data/CHANGELOG.md", "verify"])
     assert result.exit_code == 0
-    assert result.output == 'Success\n'
+    assert result.output == "Success\n"
+
+    result = runner.invoke(cli, ["-f", "tests/data/CHANGELOG_invalid.md", "verify"])
+    assert result.exit_code == 10  # spawns 8 errors
 
-    result = runner.invoke(cli, ['-f', 'tests/data/CHANGELOG_invalid.md' , 'verify'])
-    assert result.exit_code == 10 # spawns 8 errors
 
 def test_verify_with_json_output():
     runner = CliRunner()
-    result = runner.invoke(cli, ['-f', 'tests/data/CHANGELOG_invalid.md', 'verify', '--json'])
+    result = runner.invoke(
+        cli, ["-f", "tests/data/CHANGELOG_invalid.md", "verify", "--json"]
+    )
     validation_result = json.loads(result.output)
 
     assert len(validation_result["errors"]) == 10
-    assert validation_result["valid"] == False
+    assert validation_result["valid"] is False
+
 
 @freeze_time("2023-01-01")
 def test_release_patch(tmp_path, snapshot):
     runner = CliRunner()
     resources_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data/")
-    changelog_file = os.path.join(resources_dir, 'CHANGELOG_with_changes.md')
+    changelog_file = os.path.join(resources_dir, "CHANGELOG_with_changes.md")
 
     with runner.isolated_filesystem(temp_dir=tmp_path) as project_root_path:
-        shutil.copyfile(changelog_file, os.path.join(project_root_path, 'CHANGELOG.md'))
+        shutil.copyfile(changelog_file, os.path.join(project_root_path, "CHANGELOG.md"))
         result = runner.invoke(
             cli,
             [
-                '-f', 'CHANGELOG.md',
+                "-f",
+                "CHANGELOG.md",
                 "release",
                 "patch",
                 "-m",
             ],
             catch_exceptions=False,
         )
         assert result.exit_code == 0, result.output
         snapshot_directory(snapshot=snapshot, directory_path=project_root_path)
 
+
 @freeze_time("2023-01-01")
 def test_release_minor(tmp_path, snapshot):
     runner = CliRunner()
     resources_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data/")
-    changelog_file = os.path.join(resources_dir, 'CHANGELOG_with_changes.md')
+    changelog_file = os.path.join(resources_dir, "CHANGELOG_with_changes.md")
 
     with runner.isolated_filesystem(temp_dir=tmp_path) as project_root_path:
-        shutil.copyfile(changelog_file, os.path.join(project_root_path, 'CHANGELOG.md'))
+        shutil.copyfile(changelog_file, os.path.join(project_root_path, "CHANGELOG.md"))
         result = runner.invoke(
             cli,
             [
-                '-f', 'CHANGELOG.md',
+                "-f",
+                "CHANGELOG.md",
                 "release",
                 "minor",
                 "-m",
             ],
             catch_exceptions=False,
         )
         assert result.exit_code == 0, result.output
         snapshot_directory(snapshot=snapshot, directory_path=project_root_path)
 
+
 @freeze_time("2023-01-01")
 def test_release_major(tmp_path, snapshot):
     runner = CliRunner()
     resources_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data/")
-    changelog_file = os.path.join(resources_dir, 'CHANGELOG_with_changes.md')
+    changelog_file = os.path.join(resources_dir, "CHANGELOG_with_changes.md")
 
     with runner.isolated_filesystem(temp_dir=tmp_path) as project_root_path:
-        shutil.copyfile(changelog_file, os.path.join(project_root_path, 'CHANGELOG.md'))
+        shutil.copyfile(changelog_file, os.path.join(project_root_path, "CHANGELOG.md"))
         result = runner.invoke(
             cli,
             [
-                '-f', 'CHANGELOG.md',
+                "-f",
+                "CHANGELOG.md",
                 "release",
                 "major",
                 "-m",
             ],
             catch_exceptions=False,
         )
         assert result.exit_code == 0, result.output
         snapshot_directory(snapshot=snapshot, directory_path=project_root_path)
 
+
 @freeze_time("2023-01-01")
 def test_release_custom(tmp_path, snapshot):
     runner = CliRunner()
     resources_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data/")
-    changelog_file = os.path.join(resources_dir, 'CHANGELOG_with_changes.md')
+    changelog_file = os.path.join(resources_dir, "CHANGELOG_with_changes.md")
 
     with runner.isolated_filesystem(temp_dir=tmp_path) as project_root_path:
-        shutil.copyfile(changelog_file, os.path.join(project_root_path, 'CHANGELOG.md'))
+        shutil.copyfile(changelog_file, os.path.join(project_root_path, "CHANGELOG.md"))
         result = runner.invoke(
             cli,
             [
-                '-f', 'CHANGELOG.md',
+                "-f",
+                "CHANGELOG.md",
                 "release",
                 "2.1.1",
                 "-m",
             ],
             catch_exceptions=False,
         )
         assert result.exit_code == 0, result.output
         snapshot_directory(snapshot=snapshot, directory_path=project_root_path)
 
+
 @freeze_time("2023-01-01")
 def test_add_change_security(tmp_path, snapshot):
     runner = CliRunner()
     resources_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data/")
-    changelog_file = os.path.join(resources_dir, 'CHANGELOG_with_changes.md')
+    changelog_file = os.path.join(resources_dir, "CHANGELOG_with_changes.md")
 
     with runner.isolated_filesystem(temp_dir=tmp_path) as project_root_path:
-        shutil.copyfile(changelog_file, os.path.join(project_root_path, 'CHANGELOG.md'))
+        shutil.copyfile(changelog_file, os.path.join(project_root_path, "CHANGELOG.md"))
         result = runner.invoke(
             cli,
             [
-                '-f', 'CHANGELOG.md',
+                "-f",
+                "CHANGELOG.md",
                 "add",
                 "Security",
                 "Important Security Change",
                 "-m",
             ],
             catch_exceptions=False,
         )
@@ -134,15 +149,16 @@
 def test_config(tmp_path, snapshot):
     runner = CliRunner()
     resources_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data/")
 
     result = runner.invoke(
         cli,
         [
-            '-c', os.path.join(resources_dir, 'config.yml'),
-            '-f', 'CHANGELOG.md',
-            'verify'
+            "-c",
+            os.path.join(resources_dir, "config.yml"),
+            "-f",
+            "CHANGELOG.md",
+            "verify",
         ],
         catch_exceptions=False,
     )
     assert result.exit_code != 0, result.output
-
```

### Comparing `python-kacl-0.3.4/tests/test_kacl.py` & `python-kacl-0.4.0/tests/test_kacl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,315 +1,350 @@
+import os
 from unittest import TestCase
 
+import yaml
+
 import kacl
 from kacl.config import KACLConfig
-import os
-import yaml
+from kacl.exception import KACLException
 
 
 class TestKacl(TestCase):
     def test_load_valid(self):
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG.md"
+        )
         changelog = kacl.load(changelog_file)
 
-        self.assertEqual(changelog.title(), 'Changelog')
+        self.assertEqual(changelog.title(), "Changelog")
         self.assertGreater(len(changelog.versions()), 0)
 
-        version = changelog.get('1.0.0')
+        version = changelog.get("1.0.0")
         self.assertIsNotNone(version)
 
-        added_changes = version.changes('Added')
+        added_changes = version.changes("Added")
         self.assertIsNotNone(added_changes)
 
         added_items = added_changes.items()
         self.assertIsNotNone(added_items)
 
     def test_dump(self):
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG.md"
+        )
         changelog = kacl.load(changelog_file)
         changelog_dump = kacl.dump(changelog)
         self.assertIsNotNone(changelog_dump)
 
-        with open(changelog_file, 'r') as reference_file:
+        with open(changelog_file, "r") as reference_file:
             changelog_reference = reference_file.read()
         reference_file.close()
 
-        changelog_dump_lines = changelog_dump.split('\n')
-        changelog_reference_lines = changelog_reference.split('\n')
+        changelog_dump_lines = changelog_dump.split("\n")
+        changelog_reference_lines = changelog_reference.split("\n")
 
-        self.assertEqual(len(changelog_dump_lines),
-                         len(changelog_reference_lines))
+        self.assertEqual(len(changelog_dump_lines), len(changelog_reference_lines))
         self.assertEqual(changelog_dump, changelog_reference)
 
     def test_add_change(self):
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG.md"
+        )
 
         changelog = kacl.load(changelog_file)
 
-        msg = 'This is my first added change'
-        changelog.add('Added', msg)
+        msg = "This is my first added change"
+        changelog.add("Added", msg)
 
         changelog_dump = kacl.dump(changelog)
         self.assertIsNotNone(changelog_dump)
 
         changelog_changed = kacl.parse(changelog_dump)
         self.assertIsNotNone(changelog_changed)
 
-        unreleased = changelog_changed.get('Unreleased')
+        unreleased = changelog_changed.get("Unreleased")
         self.assertIsNotNone(unreleased)
 
         unreleased_change_sections = unreleased.sections()
         self.assertIsNotNone(unreleased_change_sections)
-        self.assertIn('Added', unreleased_change_sections)
+        self.assertIn("Added", unreleased_change_sections)
 
-        unreleased_changes_added = unreleased.changes('Added')
+        unreleased_changes_added = unreleased.changes("Added")
         self.assertIsNotNone(unreleased_changes_added)
 
         self.assertIn(msg, unreleased_changes_added.items())
 
-
     def test_release(self):
-        valid_files = [
-            'CHANGELOG.md',
-            'CHANGELOG_unrelease_only.md'
-        ]
+        valid_files = ["CHANGELOG.md", "CHANGELOG_unrelease_only.md"]
 
         for filename in valid_files:
-            changelog_file = os.path.join(os.path.dirname(
-                os.path.realpath(__file__)), "data", filename)
+            changelog_file = os.path.join(
+                os.path.dirname(os.path.realpath(__file__)), "data", filename
+            )
             changelog = kacl.load(changelog_file)
 
-            msg = 'This is my first added change'
-            changelog.add('Added', msg)
+            msg = "This is my first added change"
+            changelog.add("Added", msg)
 
             self.assertTrue(changelog.has_changes())
 
-            changelog.release(version='2.0.0', link='https://my-new-version/2.0.0.html')
+            changelog.release(version="2.0.0", link="https://my-new-version/2.0.0.html")
 
             changelog_dump = kacl.dump(changelog)
             self.assertIsNotNone(changelog_dump)
 
             changelog_changed = kacl.parse(changelog_dump)
             self.assertIsNotNone(changelog_changed)
 
-            version = changelog_changed.get('2.0.0')
+            version = changelog_changed.get("2.0.0")
             self.assertIsNotNone(version)
 
-            self.assertIn(msg, version.changes('Added').items())
-
+            self.assertIn(msg, version.changes("Added").items())
 
     def test_invalid(self):
         invalid_files = [
-            'CHANGELOG_invalid.md',
-            'CHANGELOG_missing_sections.md',
-            'CHANGELOG_no_unreleased.md'
+            "CHANGELOG_invalid.md",
+            "CHANGELOG_missing_sections.md",
+            "CHANGELOG_no_unreleased.md",
         ]
 
         for filename in invalid_files:
-            changelog_file = os.path.join(os.path.dirname(
-                os.path.realpath(__file__)), "data", filename)
+            changelog_file = os.path.join(
+                os.path.dirname(os.path.realpath(__file__)), "data", filename
+            )
             changelog = kacl.load(changelog_file)
             self.assertFalse(changelog.is_valid())
 
     def test_valid(self):
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG.md"
+        )
         changelog = kacl.load(changelog_file)
         self.assertTrue(changelog.is_valid())
 
         validation = changelog.validate()
         self.assertGreaterEqual(len(validation.errors()), 0)
 
     def test_valid_keepachangelogcom(self):
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG_keepachangelog.com.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)),
+            "data/CHANGELOG_keepachangelog.com.md",
+        )
         changelog = kacl.load(changelog_file)
         self.assertTrue(changelog.is_valid())
 
         validation = changelog.validate()
         self.assertGreaterEqual(len(validation.errors()), 0)
 
     def test_valid_project_changelog(self):
-        changelog_file = os.path.join(os.path.dirname(os.path.dirname(
-            os.path.realpath(__file__))), "CHANGELOG.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.dirname(os.path.realpath(__file__))), "CHANGELOG.md"
+        )
         changelog = kacl.load(changelog_file)
         self.assertTrue(changelog.is_valid())
 
         validation = changelog.validate()
         self.assertGreaterEqual(len(validation.errors()), 0)
 
     def test_load_empty(self):
         changelog = kacl.parse("")
         self.assertFalse(changelog.is_valid())
 
     def test_release_without_changes(self):
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG_no_unreleased.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)),
+            "data/CHANGELOG_no_unreleased.md",
+        )
         changelog = kacl.load(changelog_file)
 
         self.assertFalse(changelog.has_changes())
-        self.assertRaises(Exception, changelog.release, "1.1.1", 'https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD' )
-
+        self.assertRaises(
+            Exception,
+            changelog.release,
+            "1.1.1",
+            "https://gitlab.com/schmieder.matthias/python-kacl.git/-/compare/v1.0.0...HEAD",
+        )
 
     def test_release_existing_version(self):
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG.md"
+        )
         changelog = kacl.load(changelog_file)
 
-        msg = 'This is my first added change'
-        changelog.add('Added', msg)
+        msg = "This is my first added change"
+        changelog.add("Added", msg)
 
         self.assertTrue(changelog.has_changes())
-        self.assertRaises(Exception, changelog.release, "1.0.0", 'https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD' )
+        self.assertRaises(
+            Exception,
+            changelog.release,
+            "1.0.0",
+            "https://gitlab.com/schmieder.matthias/python-kacl.git/-/compare/v1.0.0...HEAD",
+        )
 
     def test_release_without_older_version(self):
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG.md"
+        )
         changelog = kacl.load(changelog_file)
 
-        msg = 'This is my first added change'
-        changelog.add('Added', msg)
+        msg = "This is my first added change"
+        changelog.add("Added", msg)
 
         self.assertTrue(changelog.has_changes())
-        self.assertRaises(Exception, changelog.release, "0.9.0", 'https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD' )
+        self.assertRaises(
+            Exception,
+            changelog.release,
+            "0.9.0",
+            "https://gitlab.com/schmieder.matthias/python-kacl.git/-/compare/v1.0.0...HEAD",
+        )
 
     def test_release_with_non_semver(self):
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG.md"
+        )
         changelog = kacl.load(changelog_file)
 
-        msg = 'This is my first added change'
-        changelog.add('Added', msg)
+        msg = "This is my first added change"
+        changelog.add("Added", msg)
 
         self.assertTrue(changelog.has_changes())
-        self.assertRaises(Exception, changelog.release, "a0.9.0", 'https://github.com/mschmieder/python-kacl/compare/v1.0.0...HEAD' )
-
+        self.assertRaises(
+            Exception,
+            changelog.release,
+            "a0.9.0",
+            "https://gitlab.com/schmieder.matthias/python-kacl.git/-/compare/v1.0.0...HEAD",
+        )
 
     def test_release_with_increment(self):
         tests = {
             "major": "2.0.0",
             "minor": "1.1.0",
             "patch": "1.0.1",
         }
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG.md"
+        )
 
         for increment, expected_version in tests.items():
             changelog = kacl.load(changelog_file)
 
-            msg = 'This is my first added change'
-            changelog.add('Added', msg)
+            msg = "This is my first added change"
+            changelog.add("Added", msg)
 
             self.assertTrue(changelog.has_changes())
-            changelog.release(increment = increment)
+            changelog.release(increment=increment)
             self.assertEqual(expected_version, changelog.current_version())
 
-        fail_tests = {
-            "post": "1.0.0-post.1"
-        }
+        fail_tests = {"post": "1.0.0-post.1"}
 
         for increment, expected_version in fail_tests.items():
             changelog = kacl.load(changelog_file)
 
-            msg = 'This is my first added change'
-            changelog.add('Added', msg)
+            msg = "This is my first added change"
+            changelog.add("Added", msg)
 
             self.assertTrue(changelog.has_changes())
-            self.assertRaises(kacl.KACLException, changelog.release, increment=increment)
+            self.assertRaises(KACLException, changelog.release, increment=increment)
 
     def test_release_with_increment_extension(self):
         tests = {
             "major": "2.0.0",
             "minor": "1.1.0",
             "patch": "1.0.1",
-            "post": "1.0.0-post.1"
+            "post": "1.0.0-post.1",
         }
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG.md"
+        )
 
         for increment, expected_version in tests.items():
             changelog = kacl.load(changelog_file)
-            changelog.config.post_release_version_prefix = 'post'
+            changelog.config.post_release_version_prefix = "post"
 
-            msg = 'This is my first added change'
-            changelog.add('Added', msg)
+            msg = "This is my first added change"
+            changelog.add("Added", msg)
 
             self.assertTrue(changelog.has_changes())
-            changelog.release(increment = increment)
+            changelog.release(increment=increment)
             self.assertEqual(expected_version, changelog.current_version())
 
-
     def test_post_release_with_increment(self):
         tests = {
             "major": "2.0.0",
             "minor": "1.1.0",
             "patch": "1.0.1",
-            "post": "1.0.0-post.2"
+            "post": "1.0.0-post.2",
         }
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG_post.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG_post.md"
+        )
 
         for increment, expected_version in tests.items():
             changelog = kacl.load(changelog_file)
 
-            msg = 'This is my first added change'
-            changelog.add('Added', msg)
+            msg = "This is my first added change"
+            changelog.add("Added", msg)
 
             self.assertTrue(changelog.has_changes())
-            changelog.release(increment = increment)
+            changelog.release(increment=increment)
             self.assertEqual(expected_version, changelog.current_version())
 
-
     def test_unreleased_missing_sections(self):
-        changelog_file = os.path.join(os.path.dirname(
-            os.path.realpath(__file__)), "data/CHANGELOG_missing_sections.md")
+        changelog_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)),
+            "data/CHANGELOG_missing_sections.md",
+        )
 
         changelog = kacl.load(changelog_file)
-        validation = changelog.validate()
+        changelog.validate()
         self.assertFalse(changelog.is_valid())
 
     def test_config(self):
-        config_file = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data/config.yml")
+        config_file = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "data/config.yml"
+        )
         kacl_config = KACLConfig(config_file=config_file)
 
         default_config = dict()
-        with open('kacl/config/kacl-default.yml', 'r') as f:
-            default_config = yaml.safe_load(f)['kacl']
+        with open("kacl/config/kacl-default.yml", "r") as f:
+            default_config = yaml.safe_load(f)["kacl"]
 
         # changes in config_file
         # changelog_file: CHANGELOG.md
         # allowed_header_titles:
         #   - ChangeLog
         # allowed_version_sections:
         #   - Security
         # git:
         #   commit: False
 
-        self.assertNotEqual(kacl_config.allowed_header_titles, default_config['allowed_header_titles'] )
-        self.assertEqual(kacl_config.allowed_header_titles, ['ChangeLog'] )
-
-        self.assertNotEqual(kacl_config.allowed_version_sections, default_config['allowed_version_sections'] )
-        self.assertEqual(kacl_config.allowed_version_sections, ['Security'] )
-
-        self.assertNotEqual(kacl_config.git_create_commit, default_config['git']['commit'] )
-        self.assertEqual(kacl_config.git_create_commit, True )
-
+        self.assertNotEqual(
+            kacl_config.allowed_header_titles, default_config["allowed_header_titles"]
+        )
+        self.assertEqual(kacl_config.allowed_header_titles, ["ChangeLog"])
+
+        self.assertNotEqual(
+            kacl_config.allowed_version_sections,
+            default_config["allowed_version_sections"],
+        )
+        self.assertEqual(kacl_config.allowed_version_sections, ["Security"])
+
+        self.assertNotEqual(
+            kacl_config.git_create_commit, default_config["git"]["commit"]
+        )
+        self.assertEqual(kacl_config.git_create_commit, True)
 
     def test_link_generation(self):
-        valid_files = [
-            #'CHANGELOG.md',
-            'CHANGELOG_unrelease_only.md'
-        ]
+        valid_files = ["CHANGELOG_unrelease_only.md"]
 
         for filename in valid_files:
-            changelog_file = os.path.join(os.path.dirname(
-                os.path.realpath(__file__)), "data", filename)
+            changelog_file = os.path.join(
+                os.path.dirname(os.path.realpath(__file__)), "data", filename
+            )
             changelog = kacl.load(changelog_file)
 
             changelog = kacl.load(changelog_file)
             changelog.generate_links()
 
             versions = changelog.versions()
             for v in versions:
```

