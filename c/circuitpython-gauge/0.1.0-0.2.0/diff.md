# Comparing `tmp/circuitpython-gauge-0.1.0.tar.gz` & `tmp/circuitpython-gauge-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-gauge-0.1.0.tar", last modified: Wed Mar 15 01:01:55 2023, max compression
+gzip compressed data, was "circuitpython-gauge-0.2.0.tar", last modified: Sat May 20 20:53:08 2023, max compression
```

## Comparing `circuitpython-gauge-0.1.0.tar` & `circuitpython-gauge-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:01:55.251621 circuitpython-gauge-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:01:55.247620 circuitpython-gauge-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:01:55.247620 circuitpython-gauge-0.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:01:55.247620 circuitpython-gauge-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:01:55.247620 circuitpython-gauge-0.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-03-15 01:01:55.251621 circuitpython-gauge-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:01:55.251621 circuitpython-gauge-0.1.0/circuitpython_gauge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-03-15 01:01:55.000000 circuitpython-gauge-0.1.0/circuitpython_gauge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-15 01:01:55.000000 circuitpython-gauge-0.1.0/circuitpython_gauge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 01:01:55.000000 circuitpython-gauge-0.1.0/circuitpython_gauge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-15 01:01:55.000000 circuitpython-gauge-0.1.0/circuitpython_gauge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-15 01:01:55.000000 circuitpython-gauge-0.1.0/circuitpython_gauge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:01:55.251621 circuitpython-gauge-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:01:55.251621 circuitpython-gauge-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:01:55.251621 circuitpython-gauge-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-15 01:01:46.000000 circuitpython-gauge-0.1.0/examples/gauge_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-03-15 01:01:46.000000 circuitpython-gauge-0.1.0/gauge.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-15 01:01:46.000000 circuitpython-gauge-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-15 01:01:32.000000 circuitpython-gauge-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 01:01:55.251621 circuitpython-gauge-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:53:08.623996 circuitpython-gauge-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:53:08.619996 circuitpython-gauge-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:53:08.619996 circuitpython-gauge-0.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:53:08.619996 circuitpython-gauge-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:53:08.619996 circuitpython-gauge-0.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-20 20:53:08.623996 circuitpython-gauge-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:53:08.623996 circuitpython-gauge-0.2.0/circuitpython_gauge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-20 20:53:08.000000 circuitpython-gauge-0.2.0/circuitpython_gauge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-20 20:53:08.000000 circuitpython-gauge-0.2.0/circuitpython_gauge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:53:08.000000 circuitpython-gauge-0.2.0/circuitpython_gauge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 20:53:08.000000 circuitpython-gauge-0.2.0/circuitpython_gauge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 20:53:08.000000 circuitpython-gauge-0.2.0/circuitpython_gauge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:53:08.623996 circuitpython-gauge-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1668925 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/7miijo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:53:08.623996 circuitpython-gauge-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/gauge.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/gauge.png
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/quick_start.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:53:08.623996 circuitpython-gauge-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-20 20:53:01.000000 circuitpython-gauge-0.2.0/examples/gauge_as7341_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-20 20:53:01.000000 circuitpython-gauge-0.2.0/examples/gauge_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-20 20:53:01.000000 circuitpython-gauge-0.2.0/examples/gauge_threshold_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-05-20 20:53:01.000000 circuitpython-gauge-0.2.0/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-20 20:53:01.000000 circuitpython-gauge-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-20 20:52:52.000000 circuitpython-gauge-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 20:53:08.623996 circuitpython-gauge-0.2.0/setup.cfg
```

### Comparing `circuitpython-gauge-0.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-gauge-0.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-gauge-0.1.0/.gitignore` & `circuitpython-gauge-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-gauge-0.1.0/.pre-commit-config.yaml` & `circuitpython-gauge-0.2.0/.pre-commit-config.yaml`

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

### Comparing `circuitpython-gauge-0.1.0/.pylintrc` & `circuitpython-gauge-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-gauge-0.1.0/CODE_OF_CONDUCT.md` & `circuitpython-gauge-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-gauge-0.1.0/LICENSE` & `circuitpython-gauge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-gauge-0.1.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-gauge-0.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-gauge-0.1.0/LICENSES/MIT.txt` & `circuitpython-gauge-0.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-gauge-0.1.0/LICENSES/Unlicense.txt` & `circuitpython-gauge-0.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-gauge-0.1.0/PKG-INFO` & `circuitpython-gauge-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: circuitpython-gauge
-Version: 0.1.0
+Version: 0.2.0
 Summary: CircuitPython Gauge
-Author-email: Adafruit Industries <circuitpython@adafruit.com>
+Author-email: "Jose D. Montoya" <gauge@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_Gauge
 Keywords: adafruit,blinka,circuitpython,micropython,gauge,gauge,plot,graphial,gage,uplot,meter
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
@@ -25,39 +25,35 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_Gauge/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_Gauge/actions
     :alt: Build Status
 
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-gauge?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-gauge
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython Gauge
+CircuitPython Gauge. Simple customizable gauge widget.
+
+.. image:: https://github.com/jposada202020/CircuitPython_gauge/blob/main/docs/gauge.png
+
+.. image:: https://github.com/jposada202020/CircuitPython_gauge/blob/main/docs/7miijo.gif
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
-Please ensure all dependencies are available on the CircuitPython filesystem.
-This is easily achieved by downloading
-`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
-or individual libraries can be installed using
-`circup <https://github.com/adafruit/circup>`_.Installing from PyPI
-
-
-.. note:: This library is not available on PyPI yet. Install documentation is included
-   as a standard element. Stay tuned for PyPI availability!
-
-
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-gauge/>`_.
 To install for current user:
 
 .. code-block:: shell
 
     pip3 install circuitpython-gauge
@@ -101,16 +97,13 @@
     circup update
 
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://circuitpython-gauge.readthedocs.io/>`_.
 
-For information on building library documentation, please check out
-`this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/jposada202020/CircuitPython_Gauge/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `circuitpython-gauge-0.1.0/README.rst` & `circuitpython-gauge-0.2.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -7,39 +7,35 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_Gauge/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_Gauge/actions
     :alt: Build Status
 
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-gauge?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-gauge
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython Gauge
+CircuitPython Gauge. Simple customizable gauge widget.
+
+.. image:: https://github.com/jposada202020/CircuitPython_gauge/blob/main/docs/gauge.png
+
+.. image:: https://github.com/jposada202020/CircuitPython_gauge/blob/main/docs/7miijo.gif
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
-Please ensure all dependencies are available on the CircuitPython filesystem.
-This is easily achieved by downloading
-`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
-or individual libraries can be installed using
-`circup <https://github.com/adafruit/circup>`_.Installing from PyPI
-
-
-.. note:: This library is not available on PyPI yet. Install documentation is included
-   as a standard element. Stay tuned for PyPI availability!
-
-
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-gauge/>`_.
 To install for current user:
 
 .. code-block:: shell
 
     pip3 install circuitpython-gauge
@@ -83,16 +79,13 @@
     circup update
 
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://circuitpython-gauge.readthedocs.io/>`_.
 
-For information on building library documentation, please check out
-`this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/jposada202020/CircuitPython_Gauge/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `circuitpython-gauge-0.1.0/circuitpython_gauge.egg-info/PKG-INFO` & `circuitpython-gauge-0.2.0/circuitpython_gauge.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: circuitpython-gauge
-Version: 0.1.0
+Version: 0.2.0
 Summary: CircuitPython Gauge
-Author-email: Adafruit Industries <circuitpython@adafruit.com>
+Author-email: "Jose D. Montoya" <gauge@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_Gauge
 Keywords: adafruit,blinka,circuitpython,micropython,gauge,gauge,plot,graphial,gage,uplot,meter
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
@@ -25,39 +25,35 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_Gauge/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_Gauge/actions
     :alt: Build Status
 
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-gauge?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-gauge
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython Gauge
+CircuitPython Gauge. Simple customizable gauge widget.
+
+.. image:: https://github.com/jposada202020/CircuitPython_gauge/blob/main/docs/gauge.png
+
+.. image:: https://github.com/jposada202020/CircuitPython_gauge/blob/main/docs/7miijo.gif
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
-Please ensure all dependencies are available on the CircuitPython filesystem.
-This is easily achieved by downloading
-`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
-or individual libraries can be installed using
-`circup <https://github.com/adafruit/circup>`_.Installing from PyPI
-
-
-.. note:: This library is not available on PyPI yet. Install documentation is included
-   as a standard element. Stay tuned for PyPI availability!
-
-
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-gauge/>`_.
 To install for current user:
 
 .. code-block:: shell
 
     pip3 install circuitpython-gauge
@@ -101,16 +97,13 @@
     circup update
 
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://circuitpython-gauge.readthedocs.io/>`_.
 
-For information on building library documentation, please check out
-`this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/jposada202020/CircuitPython_Gauge/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `circuitpython-gauge-0.1.0/circuitpython_gauge.egg-info/SOURCES.txt` & `circuitpython-gauge-0.2.0/circuitpython_gauge.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
-README.rst.license
 gauge.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
@@ -19,18 +18,21 @@
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 circuitpython_gauge.egg-info/PKG-INFO
 circuitpython_gauge.egg-info/SOURCES.txt
 circuitpython_gauge.egg-info/dependency_links.txt
 circuitpython_gauge.egg-info/requires.txt
 circuitpython_gauge.egg-info/top_level.txt
+docs/7miijo.gif
 docs/api.rst
-docs/api.rst.license
 docs/conf.py
 docs/examples.rst
-docs/examples.rst.license
+docs/gauge.jpg
+docs/gauge.png
 docs/index.rst
-docs/index.rst.license
+docs/quick_start.rst
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
-examples/gauge_simpletest.py
+examples/gauge_as7341_text.py
+examples/gauge_simpletest.py
+examples/gauge_threshold_setting.py
```

### Comparing `circuitpython-gauge-0.1.0/docs/_static/favicon.ico` & `circuitpython-gauge-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-gauge-0.1.0/docs/conf.py` & `circuitpython-gauge-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-gauge-0.1.0/gauge.py` & `circuitpython-gauge-0.2.0/gauge.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,41 +29,42 @@
 
 import displayio
 import terminalio
 from bitmaptools import draw_line
 from vectorio import Polygon
 from ulab import numpy as np
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_Gauge.git"
 
 # pylint: disable=too-many-arguments, too-many-instance-attributes, too-many-locals
 # pylint: disable=too-many-statements, unnecessary-comprehension
 # pylint: disable=unused-import, import-outside-toplevel, undefined-variable
 # pylint: disable=invalid-name, dangerous-default-value
 
 
 class gauge(displayio.Group):
     """
     scales Class to add different elements to the screen.
     The origin point set by ``x`` and ``y`` properties
 
-    :param int x: origin x coordinate
-    :param int y: origin y coordinate
+    :param int x: origin x coordinate. Defaults to 0.
+    :param int y: origin y coordinate. Defaults to 0.
     :param int width: plot box width in pixels. Defaults to 100.
     :param int height: plot box height in pixels. Defaults to 100.
     :param int padding: padding for the scale box in all directions
     :param list|None scale_range: x range limits. Defaults to None
 
     :param int background_color: background color in HEX. Defaults to black ``0x000000``
     :param int box_color: allows to choose the box line color. Defaults to white ''0xFFFFFF``
 
+    :param np.array|list ticks: axis ticks values
     :param int tick_lenght: x axes tick height in pixels. Defaults to 28.
     :param int tick_color: x axes tick height in pixels. Defaults to 0xFFFFFF.
-    :param str|None: Argument to locate the ticks. Left, center or all
+    :param str|None tick_pos: Argument to locate the ticks. Left, center or all
     :param int pointer_lenght: width of the bar. Defaults to 10.
     :param int scale: scale of the widget
 
 
     """
 
     def __init__(
@@ -72,24 +73,28 @@
         y: int = 0,
         width: int = 100,
         height: int = 100,
         padding: int = 1,
         scale_range: Optional[list] = [0, 150],
         background_color: int = 0x000000,
         box_color: int = 0xFF8500,
+        ticks: Optional[Union[np.array, list]] = None,
         tick_lenght: int = 28,
         tick_color: int = 0xFFFFFF,
+        tick_color_threshold: int = 0xFF0000,
         tick_pos: Optional[str] = None,
         pointer_lenght: int = 10,
         scale: int = 1,
+        show_text: bool = False,
+        text_format: Optional[str] = None,
     ) -> None:
-        if width not in range(50, 481) and scale == 1:
+        if width not in range(20, 481) and scale == 1:
             print("Be sure to verify your values. Defaulting to width=100")
             width = 100
-        if height not in range(50, 321) and scale == 1:
+        if height not in range(20, 321) and scale == 1:
             print("Be sure to verify your values. Defaulting to height=100")
             height = 100
         if x + width > 481:
             print(
                 "Modify this settings. Some of the graphics will not shown int the screen"
             )
             print("Defaulting to x=0")
@@ -114,43 +119,55 @@
         self._newxmax = width - padding
 
         self._center = (self._newxmax - self._newxmin) // 2
 
         self._newymin = height - padding
         self._newymax = padding
 
-        self.ticksy = np.array([element for element in range(self.ymin, self.ymax, 10)])
+        if ticks:
+            self.ticks = np.array(ticks)
+        else:
+            self.ticks = np.array(
+                [element for element in range(self.ymin, self.ymax, 10)]
+            )
 
-        self._showtext = True
+        self._showtext = show_text
 
         self._tickcolor = tick_color
-        self._pointer_palette = displayio.Palette(2)
+        self._tick_color_threshold = tick_color_threshold
+        self._pointer_palette = displayio.Palette(3)
         self._pointer_palette.make_transparent(0)
         self._pointer_palette[1] = self._tickcolor
+        self._pointer_palette[2] = self._tick_color_threshold
         self.pointer = None
         self._pointer_lenght = pointer_lenght
         self._tick_lenght = tick_lenght
         if tick_pos == "left":
             self._tickpos = self._newxmin
         elif tick_pos == "center":
             self._tickpos = self._center - self._tick_lenght // 2
         else:
             self._tickpos = self._newxmin
             self._tick_lenght = self._width
 
         self.value = 0
+        self.threshold = 0
 
         self._showticks = True
 
-        self._plotbitmap = displayio.Bitmap(width, height, 4)
+        if text_format == "float":
+            self._text_format = True
+        else:
+            self._text_format = False
+
+        self._plotbitmap = displayio.Bitmap(width, height, 6)
 
-        self.pointer_size = 6
         self._drawbox()
 
-        self._plot_palette = displayio.Palette(4)
+        self._plot_palette = displayio.Palette(6)
         self._plot_palette[0] = background_color
         self._plot_palette[1] = box_color
         self._plot_palette[2] = self._tickcolor
 
         self.points = None
         self.y0 = None
         self.x0 = None
@@ -169,53 +186,46 @@
         """
         Draw the plot box
 
         :return: None
 
         """
 
-        draw_box = [True, True, True, True]
-
-        if draw_box[0]:
-            # y axes line
-            draw_line(
-                self._plotbitmap,
-                self.padding,
-                self.padding,
-                self.padding,
-                self._height - self.padding,
-                1,
-            )
-        if draw_box[1]:
-            draw_line(
-                self._plotbitmap,
-                self.padding,
-                self._height - self.padding,
-                self._width - self.padding,
-                self._height - self.padding,
-                1,
-            )
-        if draw_box[2]:
-            draw_line(
-                self._plotbitmap,
-                self._width - self.padding,
-                self.padding,
-                self._width - self.padding,
-                self._height - self.padding,
-                1,
-            )
-        if draw_box[3]:
-            draw_line(
-                self._plotbitmap,
-                self.padding,
-                self.padding,
-                self._width - self.padding,
-                self.padding,
-                1,
-            )
+        draw_line(
+            self._plotbitmap,
+            self.padding,
+            self.padding,
+            self.padding,
+            self._height - self.padding,
+            1,
+        )
+        draw_line(
+            self._plotbitmap,
+            self.padding,
+            self._height - self.padding,
+            self._width - self.padding,
+            self._height - self.padding,
+            1,
+        )
+        draw_line(
+            self._plotbitmap,
+            self._width - self.padding,
+            self.padding,
+            self._width - self.padding,
+            self._height - self.padding,
+            1,
+        )
+        draw_line(
+            self._plotbitmap,
+            self.padding,
+            self.padding,
+            self._width - self.padding,
+            self.padding,
+            1,
+        )
 
     @staticmethod
     def transform(
         oldrangemin: Union[float, int],
         oldrangemax: Union[float, int],
         newrangemin: Union[float, int],
         newrangemax: Union[float, int],
@@ -243,41 +253,47 @@
         """
         Draw ticks in the plot area
 
         """
 
         ticksynorm = np.array(
             self.transform(
-                self.ymin, self.ymax, self._newymin, self._newymax, self.ticksy
+                self.ymin, self.ymax, self._newymin, self._newymax, self.ticks
             ),
             dtype=np.int16,
         )
 
         for i, tick in enumerate(ticksynorm):
-            if i == 0:
-                continue
             draw_line(
                 self._plotbitmap,
                 self._newxmin + self._tickpos,
                 tick,
                 self._newxmin + self._tick_lenght + self._tickpos,
                 tick,
                 2,
             )
             if self._showtext:
-                self.show_text(
-                    "{:.2f}".format(self.ticksy[i]), self._newxmin, tick, (1.0, 0.5)
-                )
+                if self._text_format:
+                    self.show_text(
+                        "{:.2f}".format(self.ticks[i]), self._newxmin, tick, (1.0, 0.5)
+                    )
+                else:
+                    self.show_text(
+                        "{:d}".format(int(self.ticks[i])),
+                        self._newxmin,
+                        tick,
+                        (1.0, 0.5),
+                    )
 
     def show_text(
         self, text: str, x: int, y: int, anchorpoint: Tuple = (0.5, 0.0)
     ) -> None:
         """
 
-        Show desired text in the scree
+        Show desired text in the screen
         :param str text: text to be displayed
         :param int x: x coordinate
         :param int y: y coordinate
         :param Tuple anchorpoint: Display_text anchor point. Defaults to (0.5, 0.0)
         :return: None
         """
         if self._showtext:
@@ -288,45 +304,66 @@
             text_toplot.anchored_position = (x, y)
             self.append(text_toplot)
 
     def _draw_pointer(self):
         self.x0 = self._center - self._pointer_lenght // 2
         self.y0 = self._newymin
         self.x1 = self._center + self._pointer_lenght // 2
-        self.y1 = self._newymin - self.pointer_size - self.value
+        self.y1 = self._newymin - self.value
 
         self.points = [
             (self.x0, self.y0),
             (self.x1, self.y0),
             (self.x1, self.y1),
             (self.x0, self.y1),
         ]
+
         self.pointer = Polygon(
             pixel_shader=self._pointer_palette,
             points=self.points,
             x=0,
             y=0,
             color_index=1,
         )
         self.append(self.pointer)
 
     def update(self, new_value):
         """
         Function to update gauge value
+
         :param new_value: value to be updated
         :return: None
+
+
         """
         self.value = int(
             self.transform(
                 self.ymin, self.ymax, self._newymax, self._newymin, new_value
             )
         )
-        if self.value >= self._newymin - self.pointer_size:
-            self.value = self._newymin - self.pointer_size
-        self.y1 = self._newymin - self.pointer_size - self.value
+
+        if self.value >= self._newymin:
+            self.value = self._newymin
+
+        self.y1 = self._newymin - self.value
         self.points = [
             (self.x0, self.y0),
             (self.x1, self.y0),
             (self.x1, self.y1),
             (self.x0, self.y1),
         ]
+
+        if self.value > self.threshold:
+            self.pointer.color_index = 2
+        else:
+            self.pointer.color_index = 1
         self.pointer.points = self.points
+
+    def set_threshold(self, value: int, color: int = 0xFF0000) -> None:
+        """
+        Defines the threshold for the gage to change color
+        :param value: value that will trigger the change
+        :param color: color to change into. Defaults to red :const:`0xFF0000`
+        :return: None
+        """
+        self._pointer_palette[2] = color
+        self.threshold = value
```

### Comparing `circuitpython-gauge-0.1.0/pyproject.toml` & `circuitpython-gauge-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-gauge"
 description = "CircuitPython Gauge"
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
-    {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
+    {name = "Jose D. Montoya", email = "gauge@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_Gauge"}
 keywords = [
     "adafruit",
     "blinka",
     "circuitpython",
     "micropython",
```

