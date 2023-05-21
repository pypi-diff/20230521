# Comparing `tmp/circuitpython-scales-0.5.1.tar.gz` & `tmp/circuitpython-scales-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-scales-0.5.1.tar", last modified: Fri Jan 27 02:34:51 2023, max compression
+gzip compressed data, was "circuitpython-scales-0.6.0.tar", last modified: Sun May 21 17:38:01 2023, max compression
```

## Comparing `circuitpython-scales-0.5.1.tar` & `circuitpython-scales-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 02:34:51.116816 circuitpython-scales-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 02:34:51.108816 circuitpython-scales-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 02:34:51.112816 circuitpython-scales-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 02:34:51.112816 circuitpython-scales-0.5.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-01-27 02:34:51.116816 circuitpython-scales-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 02:34:51.116816 circuitpython-scales-0.5.1/circuitpython_scales.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-01-27 02:34:51.000000 circuitpython-scales-0.5.1/circuitpython_scales.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-01-27 02:34:51.000000 circuitpython-scales-0.5.1/circuitpython_scales.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 02:34:51.000000 circuitpython-scales-0.5.1/circuitpython_scales.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-27 02:34:51.000000 circuitpython-scales-0.5.1/circuitpython_scales.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-27 02:34:51.000000 circuitpython-scales-0.5.1/circuitpython_scales.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 02:34:51.116816 circuitpython-scales-0.5.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 02:34:51.116816 circuitpython-scales-0.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/scales.png
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/docs/scales.png.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 02:34:51.116816 circuitpython-scales-0.5.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-27 02:34:40.000000 circuitpython-scales-0.5.1/examples/scales_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-01-27 02:34:40.000000 circuitpython-scales-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-27 02:34:30.000000 circuitpython-scales-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15580 2023-01-27 02:34:40.000000 circuitpython-scales-0.5.1/scales.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 02:34:51.116816 circuitpython-scales-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-01-27 02:34:40.000000 circuitpython-scales-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:38:01.785333 circuitpython-scales-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:38:01.781333 circuitpython-scales-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:38:01.781333 circuitpython-scales-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:38:01.785333 circuitpython-scales-0.6.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-21 17:38:01.785333 circuitpython-scales-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:38:01.785333 circuitpython-scales-0.6.0/circuitpython_scales.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-21 17:38:01.000000 circuitpython-scales-0.6.0/circuitpython_scales.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-21 17:38:01.000000 circuitpython-scales-0.6.0/circuitpython_scales.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:38:01.000000 circuitpython-scales-0.6.0/circuitpython_scales.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 17:38:01.000000 circuitpython-scales-0.6.0/circuitpython_scales.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 17:38:01.000000 circuitpython-scales-0.6.0/circuitpython_scales.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:38:01.785333 circuitpython-scales-0.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:38:01.785333 circuitpython-scales-0.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/docs/scales.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:38:01.785333 circuitpython-scales-0.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-21 17:37:52.000000 circuitpython-scales-0.6.0/examples/scales_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-21 17:37:52.000000 circuitpython-scales-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-21 17:37:41.000000 circuitpython-scales-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-05-21 17:37:52.000000 circuitpython-scales-0.6.0/scales.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:38:01.785333 circuitpython-scales-0.6.0/setup.cfg
```

### Comparing `circuitpython-scales-0.5.1/.pre-commit-config.yaml` & `circuitpython-scales-0.6.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
     rev: 22.3.0
     hooks:
       - id: black
-  - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
-    hooks:
-      - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
```

### Comparing `circuitpython-scales-0.5.1/.pylintrc` & `circuitpython-scales-0.6.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-scales-0.5.1/CODE_OF_CONDUCT.md` & `circuitpython-scales-0.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-scales-0.5.1/LICENSE` & `circuitpython-scales-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-scales-0.5.1/LICENSES/CC-BY-4.0.txt` & `circuitpython-scales-0.6.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-scales-0.5.1/LICENSES/MIT.txt` & `circuitpython-scales-0.6.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-scales-0.5.1/LICENSES/Unlicense.txt` & `circuitpython-scales-0.6.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-scales-0.5.1/PKG-INFO` & `circuitpython-scales-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: circuitpython-scales
-Version: 0.5.1
+Version: 0.6.0
 Summary: Graphic Scales to represent values in a scale in CircuitPython
-Home-page: https://github.com/jposada202020/CircuitPython_scales.git
-Author: Jose David M.
 Author-email: "Jose D. Montoya" <scales@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_scales.git
 Keywords: hardware,micropython,circuitpython,graphic,quantity,widget,displayio,color,widget,scale
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
@@ -27,14 +25,21 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_scales/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_scales/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-scales.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-scales
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-scales?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-scales
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Allows display data in a graduated level
```

### Comparing `circuitpython-scales-0.5.1/README.rst` & `circuitpython-scales-0.6.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,21 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_scales/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_scales/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-scales.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-scales
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-scales?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-scales
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Allows display data in a graduated level
```

### Comparing `circuitpython-scales-0.5.1/circuitpython_scales.egg-info/PKG-INFO` & `circuitpython-scales-0.6.0/circuitpython_scales.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: circuitpython-scales
-Version: 0.5.1
+Version: 0.6.0
 Summary: Graphic Scales to represent values in a scale in CircuitPython
-Home-page: https://github.com/jposada202020/CircuitPython_scales.git
-Author: Jose David M.
 Author-email: "Jose D. Montoya" <scales@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_scales.git
 Keywords: hardware,micropython,circuitpython,graphic,quantity,widget,displayio,color,widget,scale
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
@@ -27,14 +25,21 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_scales/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_scales/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-scales.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-scales
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-scales?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-scales
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Allows display data in a graduated level
```

### Comparing `circuitpython-scales-0.5.1/circuitpython_scales.egg-info/SOURCES.txt` & `circuitpython-scales-0.6.0/circuitpython_scales.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
-README.rst.license
 pyproject.toml
 requirements.txt
 scales.py
-setup.py
 .github/workflows/build.yml
 .github/workflows/release_gh.yml
 .github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 circuitpython_scales.egg-info/PKG-INFO
 circuitpython_scales.egg-info/SOURCES.txt
 circuitpython_scales.egg-info/dependency_links.txt
 circuitpython_scales.egg-info/requires.txt
 circuitpython_scales.egg-info/top_level.txt
 docs/api.rst
-docs/api.rst.license
 docs/conf.py
 docs/examples.rst
-docs/examples.rst.license
 docs/index.rst
-docs/index.rst.license
 docs/scales.png
-docs/scales.png.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/scales_simpletest.py
```

### Comparing `circuitpython-scales-0.5.1/docs/_static/favicon.ico` & `circuitpython-scales-0.6.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-scales-0.5.1/docs/conf.py` & `circuitpython-scales-0.6.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
-# TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 autodoc_mock_imports = [
     "digitalio",
     "vectorio",
     "bitmaptools",
     "terminalio",
     "adafruit_display_text",
     "displayio",
+    "ulab",
 ]
 
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.4", None),
+    "python": ("https://docs.python.org/3", None),
     "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
 }
 
 # Show the docstring from both the class and its __init__() method.
 autoclass_content = "both"
 
 # Add any paths that contain templates here, relative to this directory.
@@ -49,15 +49,15 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = " CircuitPython scales Library"
-copyright = "2021 Jose David M."
+copyright = "2021-2023 Jose David M."
 author = "Jose David M."
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -91,20 +91,16 @@
 # If true, '()' will be appended to :func: etc. cross-reference text.
 #
 add_function_parentheses = True
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
-# If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
-
-# If this is True, todo emits a warning for each TODO entries. The default is False.
-todo_emit_warnings = True
-
+todo_emit_warnings = False
 napoleon_numpy_docstring = False
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
```

### Comparing `circuitpython-scales-0.5.1/docs/scales.png` & `circuitpython-scales-0.6.0/docs/scales.png`

 * *Files identical despite different names*

### Comparing `circuitpython-scales-0.5.1/pyproject.toml` & `circuitpython-scales-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-scales"
 description = "Graphic Scales to represent values in a scale in CircuitPython"
-version = "0.5.1"
+version = "0.6.0"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "scales@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_scales.git"}
 keywords = [
     "hardware",
```

### Comparing `circuitpython-scales-0.5.1/scales.py` & `circuitpython-scales-0.6.0/scales.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2021 Jose David M.
+# SPDX-FileCopyrightText: Copyright (c) 2021, 2023 Jose David M.
 #
 # SPDX-License-Identifier: MIT
 """
 
 `scales`
 ================================================================================
 
@@ -10,57 +10,54 @@
 
 
 * Author(s): Jose David M.
 
 Implementation Notes
 --------------------
 
-This library is closely related with Cartesian. The Cartesian library was developed first.
-After this, new granular classes were created for Axes. and new methods to calculate the
-conversion between range, pixels and values given
+Scales version in CircuitPython
 
 """
 
 ################################
 # A scales library for CircuitPython, using `displayio`` and `vectorio``
 #
 # Features:
-#  - Customizable range and divisions
 #  - Vertical and Horizontal direction
 #  - Animation to use with different sensor
-#
-# Future options to consider:
-# ---------------------------
-# Different pointers
-# Pointer using real values
+
+try:
+    from typing import Union, Tuple, Optional
+except ImportError:
+    pass
 
 import displayio
 import terminalio
 from adafruit_display_text.bitmap_label import Label
 from vectorio import Polygon, Rectangle
+import ulab.numpy as np
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_scales.git"
 
-
-# pylint: disable=too-many-instance-attributes, too-many-arguments, too-few-public-methods
-
-
+# pylint: disable=too-many-arguments, too-few-public-methods,too-many-instance-attributes
+# pylint: disable=invalid-unary-operand-type
 class Axes(displayio.Group):
     """
     :param int x: pixel position. Defaults to :const:`0`
     :param int y: pixel position. Defaults to :const:`0`
 
     :param int,int limits: tuple of value range for the scale. Defaults to (0, 100)
-    :param int divisions: Divisions number
+    :param list ticks: list to ticks to display. If this is not enter a equally spaced scale
+     will be created between the given limits.
 
     :param str direction: direction of the scale either :attr:`horizontal` or :attr:`vertical`
      defaults to :attr:`horizontal`
 
     :param int stroke: width in pixels of the scale axes. Defaults to :const:`3`
 
     :param int length: scale length in pixels. Defaults to :const:`100`
@@ -70,174 +67,189 @@
     """
 
     def __init__(
         self,
         x: int = 0,
         y: int = 0,
         limits: Tuple[int, int] = (0, 100),
-        divisions: int = 10,
+        ticks: Optional[Union[np.array, list]] = None,
         direction: str = "horizontal",
         stroke: int = 3,
         length: int = 100,
         color: int = 0x990099,
     ):
 
         super().__init__()
 
-        self.x = x
-        self.y = y
-        self.limits = limits
-
-        self.divisions = divisions
-
         if direction == "horizontal":
             self.direction = True
         else:
             self.direction = False
 
+        self.x = x
+        self.y = y
+        self.limits = limits
+
+        self._valuemin = limits[0]
+        self._valuemax = limits[1]
+        self._newvalmin = length
+        self._newvalmax = 0
+
         self.stroke = stroke
         self.length = length
 
+        if ticks:
+            self.ticks = np.array(ticks)
+        else:
+            self.ticks = np.array(list(range(self._valuemin, self._valuemax, 10)))
+
+        self.ticksynorm = np.array(
+            transform(
+                self._valuemin,
+                self._valuemax,
+                self._newvalmax,
+                self._newvalmin,
+                self.ticks,
+            ),
+            dtype=np.int16,
+        )
+
         self._palette = displayio.Palette(2)
         self._palette.make_transparent(0)
         self._palette[1] = color
 
         self._tick_length = None
         self._tick_stroke = None
-        self.ticks = None
-        self.text_ticks = None
 
-    def _draw_line(self):
+        self.text_ticks = []
+
+    def _draw_line(self) -> None:
         """Private function to draw the Axe.
         :return: None
         """
         if self.direction:
             self.append(rectangle_draw(0, 0, self.stroke, self.length, self._palette))
         else:
             self.append(
                 rectangle_draw(0, -self.length, self.length, self.stroke, self._palette)
             )
 
-    # pylint: disable=invalid-unary-operand-type
-    def _draw_ticks(self, tick_length: int = 10, tick_stroke: int = 4):
+    def _draw_ticks(self, tick_length: int = 10, tick_stroke: int = 4) -> None:
         """Private function to draw the ticks
         :param int tick_length: tick length in pixels
         :param int tick_stroke: tick thickness in pixels
         :return: None
         """
+
         self._tick_length = tick_length
         self._tick_stroke = tick_stroke
-        self._conversion()
 
         if self.direction:
-            for val in self.ticks[:-1]:
+            for val in self.ticksynorm[:-1]:
                 self.append(
                     rectangle_draw(
-                        val - 1, -self._tick_length, self._tick_length, 3, self._palette
+                        int(val) - 1,
+                        -self._tick_length,
+                        self._tick_length,
+                        3,
+                        self._palette,
                     )
                 )
         else:
-            for val in self.ticks[:-1]:
+            for val in self.ticksynorm[:-1]:
                 self.append(
-                    rectangle_draw(0, -val, 3, self._tick_length, self._palette)
+                    rectangle_draw(0, -int(val), 3, self._tick_length, self._palette)
                 )
 
-    def _conversion(self):
-        """Private function that creates the ticks distance and text.
-        :return: None
-        """
-        self.ticks = []
-        self.text_ticks = []
-        espace = round(self.length / self.divisions)
-        rang_discrete = self.limits[1] - self.limits[0]
-        factorp = self.length / rang_discrete
-        for i in range(espace, self.length + 1, espace):
-            self.ticks.append(i)
-            self.text_ticks.append(str(int(self.limits[0] + i * 1 / factorp)))
-
-    def _draw_text(self):
+    def _draw_text(self) -> None:
         """Private function to draw the text, uses values found in ``_conversion``
         :return: None
         """
         index = 0
         separation = 20
         font_width = 12
         if self.direction:
-            for tick_text in self.text_ticks[:-1]:
-                dist_x = self.ticks[index] - font_width // 2
+            print("aca")
+            for tick_text in self.ticks[:-1]:
+                dist_x = self.ticksynorm[index] - font_width // 2
                 dist_y = separation // 2
-                tick_label = Label(terminalio.FONT, text=tick_text, x=dist_x, y=dist_y)
+                text = str(int(tick_text))
+                tick_label = Label(terminalio.FONT, text=text, x=dist_x, y=dist_y)
                 self.append(tick_label)
                 index = index + 1
         else:
-            for tick_text in self.text_ticks[:-1]:
+            for tick_text in self.ticks[:-1]:
                 dist_x = -separation
-                dist_y = -self.ticks[index]
-                tick_label = Label(terminalio.FONT, text=tick_text, x=dist_x, y=dist_y)
+                dist_y = -self.ticksynorm[index]
+                text = str(int(tick_text))
+                tick_label = Label(terminalio.FONT, text=text, x=dist_x, y=dist_y)
                 self.append(tick_label)
                 index = index + 1
 
 
 class Scale(Axes):
     """
     :param int x: pixel position. Defaults to :const:`0`
     :param int y: pixel position. Defaults to :const:`0`
 
     :param str direction: direction of the scale either :attr:`horizontal` or :attr:`vertical`
      defaults to :attr:`horizontal`
 
-    :param int stroke: width in pixels of the scale axes. Defaults to 3
+    :param int stroke: width in pixels of the axes line. Defaults to :const:`3` pixels
 
-    :param int length: scale length in pixels. Defaults to 100
-     that extends the touch response boundary, defaults to 0
+    :param int length: scale length in pixels. Defaults to :const:`100` pixels
 
-    :param int color: 24-bit hex value axes line color, Defaults to purple :const:`0x990099`
+    :param int color: 24-bit hex value axes line color, Defaults to Purple :const:`0x990099`
 
-    :param int width: scale width in pixels. Defaults to :const:`50`
+    :param int width: scale width in pixels. Defaults to :const:`50` pixels
 
     :param limits: tuple of value range for the scale. Defaults to :const:`(0, 100)`
-    :param int divisions: Divisions number
+    :param list ticks: list to ticks to display. If this is not enter a equally spaced scale
+     will be created between the given limits.
 
     :param int back_color: 24-bit hex value axes line color.
      Defaults to Light Blue :const:`0x9FFFFF`
 
     :param int tick_length: Scale tick length in pixels. Defaults to :const:`10`
     :param int tick_stroke: Scale tick width in pixels. Defaults to :const:`4`
 
+    :param int pointer_length: length in pixels for the point. Defaults to :const:`20` pixels
+    :param int pointer_stroke: pointer thickness in pixels. Defaults to :const:`6` pixels
+
 
     **Quickstart: Importing and using Scales**
 
-    Here is one way of importing the `Scale` class so you can use it as
+    Here is one way of importing the `Scale` class, so you can use it as
     the name ``my_scale``:
 
-    .. code-block:: python
+    .. code-block::
 
-        from Graphics import Scale
+        from scale import Scale
 
-    Now you can create an vertical Scale at pixel position x=50, y=180 with 3 divisions and a range
+    Now you can create a vertical Scale at pixel position x=50, y=180 and a range
     of 0 to 80 using:
 
-    .. code-block:: python
+    .. code-block::
 
-        my_scale = Scale(x=50, y=180, direction="vertical", divisions=3, limits=(0, 80))
+        my_scale = Scale(x=50, y=180, direction="vertical", limits=(0, 80))
 
     Once you setup your display, you can now add ``my_scale`` to your display using:
 
-    .. code-block:: python
+    .. code-block::
 
         display.show(my_scale)
 
     If you want to have multiple display elements, you can create a group and then
     append the scale and the other elements to the group. Then, you can add the full
     group to the display as in this example:
 
     .. code-block:: python
 
         my_scale= Scale(x=20, y=30)
-        my_group = displayio.Group(max_size=10) # make a group that can hold 10 items
+        my_group = displayio.Group() # make a group
         my_group.append(my_scale) # Add my_slider to the group
 
         #
         # Append other display elements to the group
         #
 
         display.show(my_group) # add the group to the display
@@ -252,17 +264,15 @@
 
         - **size**: :attr:`length` and :attr:`width`
 
         - **color**: :attr:`color`, :attr:`back_color`
 
         - **linewidths**: :attr:`stroke` and :attr:`tick_stroke`
 
-        - **value**: Set :attr:`value` to the initial value (`True` or `False`)
-
-        - **range and divisions**: :attr:`limits` and :attr:`divisions`
+        - **range**: :attr:`limits`
 
 
     .. figure:: scales.png
       :scale: 100 %
       :align: center
       :alt: Diagram of scales
 
@@ -277,44 +287,64 @@
         y: int = 0,
         direction: str = "horizontal",
         stroke: int = 3,
         length: int = 100,
         color: int = 0x990099,
         width: int = 50,
         limits: Tuple[int, int] = (0, 100),
-        divisions: int = 10,
         back_color: int = 0x9FFFFF,
-        tick_length: int = 10,
+        ticks: Optional[Union[np.array, list]] = None,
+        tick_length: int = 5,
         tick_stroke: int = 4,
+        pointer_length: int = 20,
+        pointer_stroke: int = 6,
     ):
 
         super().__init__(
             x=x,
             y=y,
             direction=direction,
             stroke=stroke,
             length=length,
             limits=limits,
-            divisions=divisions,
+            ticks=ticks,
             color=color,
         )
 
         self._width = width
         self._back_color = back_color
         self._draw_background()
         self._draw_line()
         self._draw_ticks()
+        self.value = 0
 
         self._tick_length = tick_length
         self._tick_stroke = tick_stroke
+        self._pointer_length = pointer_length
+        self._pointer_stroke = pointer_stroke
+
+        # Pointer Definitions
+        self._x0 = 0
+        self._y0 = 0
 
+        if self.direction:
+            self.center = width // 2
+            self._x1 = pointer_stroke
+            self._y1 = pointer_length
+            self._posx = 0
+            self._posy = -self.center - self._pointer_length // 2
+        else:
+            self.center = width // 2
+            self._x1 = pointer_length
+            self._y1 = pointer_stroke
+            self._posx = self.center - self._pointer_length // 2
+            self._posy = -10
         self.pointer = None
 
         self._draw_text()
-
         self._draw_pointer()
 
     def _draw_background(self):
         """Private function to draw the background for the scale
         :return: None
         """
         back_palette = displayio.Palette(2)
@@ -329,164 +359,65 @@
             self.append(
                 rectangle_draw(0, -self.length, self.length, self._width, back_palette)
             )
 
     def _draw_pointer(
         self,
         color: int = 0xFF0000,
-        val_ini: int = 15,
-        space: int = 3,
-        pointer_length: int = 20,
-        pointer_stroke: int = 6,
     ):
         """Private function to initial draw the pointer.
 
         :param int color: 24-bit hex value axes line color. Defaults to red :const:`0xFF0000`
         :param int val_ini: initial value to draw the pointer
-        :param int space: separation in pixels from the ticker to the pointer.
-         Defaults to :const:`3`
-        :param int pointer_length: length in pixels for the point. Defaults to :const:`20`
-        :param int pointer_stroke: pointer thickness in pixels. Defaults to :const:`6`
+
 
         :return: None
 
         """
 
         pointer_palette = displayio.Palette(2)
         pointer_palette.make_transparent(0)
         pointer_palette[1] = color
 
-        self._pointer_length = pointer_length
-        self._space = space
-        self._pointer_stroke = pointer_stroke
-
-        if self.direction:
-            points = [
-                (
-                    self.x - self._pointer_stroke // 2 + val_ini,
-                    self.y - self.stroke - self._tick_length - self._space,
-                ),
-                (
-                    self.x - self._pointer_stroke // 2 + val_ini,
-                    self.y
-                    - self.stroke
-                    - self._tick_length
-                    - self._space
-                    - self._pointer_length,
-                ),
-                (
-                    self.x + self._pointer_stroke // 2 + val_ini,
-                    self.y
-                    - self.stroke
-                    - self._tick_length
-                    - self._space
-                    - self._pointer_length,
-                ),
-                (
-                    self.x + self._pointer_stroke // 2 + val_ini,
-                    self.y - self.stroke - self._tick_length - self._space,
-                ),
-            ]
-
-        else:
-            points = [
-                (
-                    self.stroke + self._tick_length + space,
-                    self.y + self._pointer_stroke // 2 - val_ini,
-                ),
-                (
-                    self.stroke
-                    + self._tick_length
-                    + self._space
-                    + self._pointer_length,
-                    self.y + self._pointer_stroke // 2 - val_ini,
-                ),
-                (
-                    self.stroke
-                    + self._tick_length
-                    + self._space
-                    + self._pointer_length,
-                    self.y - self._pointer_stroke // 2 - val_ini,
-                ),
-                (
-                    self.stroke + self._tick_length + self._space,
-                    self.y - self._pointer_stroke // 2 - val_ini,
-                ),
-            ]
-
+        points = [
+            (self._x0, self._y0),
+            (self._x1, self._y0),
+            (self._x1, self._y1),
+            (self._x0, self._y1),
+        ]
         self.pointer = Polygon(
             pixel_shader=pointer_palette,
             points=points,
-            x=0,
-            y=-self.y,
+            x=self._posx,
+            y=self._posy,
             color_index=1,
         )
 
         self.append(self.pointer)
 
-    def animate_pointer(self, value):
+    def animate_pointer(self, new_value):
         """Public function to animate the pointer
 
-        :param value: value to draw the pointer
+        :param new_value: value to draw the pointer
         :return: None
 
         """
-
+        value = int(
+            transform(
+                self._valuemin,
+                self._valuemax,
+                self._newvalmax,
+                self._newvalmin,
+                new_value,
+            )
+        )
         if self.direction:
-            self.pointer.points = [
-                (
-                    self.x - self._pointer_stroke // 2 + value,
-                    self.y - self.stroke - self._tick_length - self._space,
-                ),
-                (
-                    self.x - self._pointer_stroke // 2 + value,
-                    self.y
-                    - self.stroke
-                    - self._tick_length
-                    - self._space
-                    - self._pointer_length,
-                ),
-                (
-                    self.x + self._pointer_stroke // 2 + value,
-                    self.y
-                    - self.stroke
-                    - self._tick_length
-                    - self._space
-                    - self._pointer_length,
-                ),
-                (
-                    self.x + self._pointer_stroke // 2 + value,
-                    self.y - self.stroke - self._tick_length - self._space,
-                ),
-            ]
+            self.pointer.x = value - self._pointer_stroke // 2
         else:
-            self.pointer.points = [
-                (
-                    self.stroke + self._tick_length + self._space,
-                    self.y + self._pointer_stroke // 2 - value,
-                ),
-                (
-                    self.stroke
-                    + self._tick_length
-                    + self._space
-                    + self._pointer_length,
-                    self.y + self._pointer_stroke // 2 - value,
-                ),
-                (
-                    self.stroke
-                    + self._tick_length
-                    + self._space
-                    + self._pointer_length,
-                    self.y - self._pointer_stroke // 2 - value,
-                ),
-                (
-                    self.stroke + self._tick_length + self._space,
-                    self.y - self._pointer_stroke // 2 - value,
-                ),
-            ]
+            self.pointer.y = -value - self._pointer_stroke // 2
 
 
 # pylint: disable=invalid-name
 def rectangle_draw(x0: int, y0: int, height: int, width: int, palette):
     """rectangle_draw function
 
     Draws a rectangle using or `vectorio.Rectangle`
@@ -500,7 +431,33 @@
     :param `~displayio.Palette` palette: palette object to be used to draw the rectangle
 
     """
 
     return Rectangle(
         pixel_shader=palette, width=width, height=height, x=x0, y=y0, color_index=1
     )
+
+
+def transform(
+    oldrangemin: Union[float, int],
+    oldrangemax: Union[float, int],
+    newrangemin: Union[float, int],
+    newrangemax: Union[float, int],
+    value: Union[float, int],
+) -> Union[float, int]:
+    """
+    This function converts the original value into a new defined value in the new range
+
+    :param int|float oldrangemin: minimum of the original range
+    :param int|float oldrangemax: maximum of the original range
+    :param int|float newrangemin: minimum of the new range
+    :param int|float newrangemax: maximum of the new range
+    :param int|float value: value to be converted
+
+    :return int|float: converted value
+
+    """
+
+    return (
+        ((value - oldrangemin) * (newrangemax - newrangemin))
+        / (oldrangemax - oldrangemin)
+    ) + newrangemin
```

