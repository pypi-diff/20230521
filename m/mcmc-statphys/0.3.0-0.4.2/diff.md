# Comparing `tmp/mcmc_statphys-0.3.0.tar.gz` & `tmp/mcmc_statphys-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcmc_statphys-0.3.0.tar", last modified: Thu May 18 09:22:07 2023, max compression
+gzip compressed data, was "mcmc_statphys-0.4.2.tar", last modified: Sun May 21 04:42:21 2023, max compression
```

## Comparing `mcmc_statphys-0.3.0.tar` & `mcmc_statphys-0.4.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 09:22:07.177195 mcmc_statphys-0.3.0/
--rw-rw-rw-   0        0        0      170 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3721 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1408 2023-05-18 09:21:00.000000 mcmc_statphys-0.3.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4333 2023-05-18 09:22:07.178193 mcmc_statphys-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2087 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 09:22:06.966188 mcmc_statphys-0.3.0/docs/
--rw-rw-rw-   0        0        0      634 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/docs/authors.rst
--rw-rw-rw-   0        0        0     5006 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/docs/history.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 09:22:06.982145 mcmc_statphys-0.3.0/docs/img/
--rw-rw-rw-   0        0        0    12977 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png
--rw-rw-rw-   0        0        0      333 2023-05-16 16:00:10.000000 mcmc_statphys-0.3.0/docs/index.rst
--rw-rw-rw-   0        0        0     1209 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/docs/installation.rst
--rwxrwxrwx   0        0        0      811 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/docs/readme.rst
--rw-rw-rw-   0        0        0    17170 2023-05-18 09:21:00.000000 mcmc_statphys-0.3.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 09:22:07.007133 mcmc_statphys-0.3.0/mcmc_statphys/
--rw-rw-rw-   0        0        0      247 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/mcmc_statphys/__init__.py
--rw-rw-rw-   0        0        0    32646 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/mcmc_statphys/algorithm.py
--rw-rw-rw-   0        0        0     2582 2023-05-18 09:21:00.000000 mcmc_statphys-0.3.0/mcmc_statphys/analysis.py
--rw-rw-rw-   0        0        0      434 2023-05-14 12:02:25.000000 mcmc_statphys-0.3.0/mcmc_statphys/cli.py
--rw-rw-rw-   0        0        0     2900 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/mcmc_statphys/draw.py
--rw-rw-rw-   0        0        0     8023 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/mcmc_statphys/model.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:22:07.067910 mcmc_statphys-0.3.0/mcmc_statphys.egg-info/
--rw-rw-rw-   0        0        0     4333 2023-05-18 09:22:06.000000 mcmc_statphys-0.3.0/mcmc_statphys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      903 2023-05-18 09:22:06.000000 mcmc_statphys-0.3.0/mcmc_statphys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 09:22:06.000000 mcmc_statphys-0.3.0/mcmc_statphys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-18 09:22:06.000000 mcmc_statphys-0.3.0/mcmc_statphys.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-0.3.0/mcmc_statphys.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-05-18 09:22:06.000000 mcmc_statphys-0.3.0/mcmc_statphys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-18 09:22:06.000000 mcmc_statphys-0.3.0/mcmc_statphys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      408 2023-05-18 09:22:07.181185 mcmc_statphys-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1556 2023-05-18 09:21:48.000000 mcmc_statphys-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:22:07.106815 mcmc_statphys-0.3.0/tests/
--rw-rw-rw-   0        0        0       44 2023-05-14 13:37:58.000000 mcmc_statphys-0.3.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:22:07.175203 mcmc_statphys-0.3.0/tests/test/
--rw-rw-rw-   0        0        0      229 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/tests/test/__init__.py
--rw-rw-rw-   0        0        0    32668 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/tests/test/algorithm.py
--rw-rw-rw-   0        0        0     1406 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/tests/test/analysis.py
--rw-rw-rw-   0        0        0      434 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/tests/test/cli.py
--rw-rw-rw-   0        0        0     2900 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/tests/test/draw.py
--rw-rw-rw-   0        0        0     8383 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/tests/test/model.py
--rw-rw-rw-   0        0        0    15639 2023-05-17 15:06:51.000000 mcmc_statphys-0.3.0/tests/test.ipynb
--rw-rw-rw-   0        0        0     1046 2023-05-17 14:16:19.000000 mcmc_statphys-0.3.0/tests/test_mcmc_statphys.py
+drwxrwxrwx   0        0        0        0 2023-05-21 04:42:21.069191 mcmc_statphys-0.4.2/
+-rw-rw-rw-   0        0        0      170 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3726 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1592 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4623 2023-05-21 04:42:21.070186 mcmc_statphys-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2193 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-21 04:42:20.783689 mcmc_statphys-0.4.2/docs/
+-rw-rw-rw-   0        0        0      634 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/authors.rst
+-rw-rw-rw-   0        0        0     4923 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/history.rst
+drwxrwxrwx   0        0        0        0 2023-05-21 04:42:20.786682 mcmc_statphys-0.4.2/docs/img/
+-rw-rw-rw-   0        0        0    12977 2023-05-17 14:16:19.000000 mcmc_statphys-0.4.2/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png
+-rw-rw-rw-   0        0        0      333 2023-05-16 16:00:10.000000 mcmc_statphys-0.4.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1209 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      811 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/make.bat
+-rw-rw-rw-   0        0        0    10277 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/docs/modules.rst
+-rw-rw-rw-   0        0        0       28 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/docs/readme.rst
+-rw-rw-rw-   0        0        0    17406 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-05-21 04:42:20.820930 mcmc_statphys-0.4.2/mcmc_statphys/
+-rw-rw-rw-   0        0        0      247 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/mcmc_statphys/__init__.py
+-rw-rw-rw-   0        0        0    14945 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/mcmc_statphys/algorithm.py
+-rw-rw-rw-   0        0        0     2582 2023-05-20 10:32:21.000000 mcmc_statphys-0.4.2/mcmc_statphys/analysis.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 12:02:25.000000 mcmc_statphys-0.4.2/mcmc_statphys/cli.py
+-rw-rw-rw-   0        0        0     5788 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/mcmc_statphys/draw.py
+-rw-rw-rw-   0        0        0     8776 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/mcmc_statphys/model.py
+drwxrwxrwx   0        0        0        0 2023-05-21 04:42:20.934555 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/
+-rw-rw-rw-   0        0        0     4623 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 04:42:20.000000 mcmc_statphys-0.4.2/mcmc_statphys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      520 2023-05-21 04:42:21.077172 mcmc_statphys-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1556 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 04:42:20.968465 mcmc_statphys-0.4.2/tests/
+-rw-rw-rw-   0        0        0       44 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 04:42:21.067194 mcmc_statphys-0.4.2/tests/one/
+-rw-rw-rw-   0        0        0      229 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/__init__.py
+-rw-rw-rw-   0        0        0    14945 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/algorithm.py
+-rw-rw-rw-   0        0        0     1406 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/analysis.py
+-rw-rw-rw-   0        0        0      434 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/cli.py
+-rw-rw-rw-   0        0        0     5788 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/draw.py
+-rw-rw-rw-   0        0        0     8776 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/one/model.py
+-rw-rw-rw-   0        0        0     2891 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.2/tests/test.ipynb
+-rw-rw-rw-   0        0        0      952 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.2/tests/test_mcmc_statphys.py
```

### Comparing `mcmc_statphys-0.3.0/CONTRIBUTING.rst` & `mcmc_statphys-0.4.2/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
+3. The pull request should work for Python 3.5, 3.6, 3.7, 3.8 and 3.9, and for PyPy. Check
    https://travis-ci.com/uynajgi/mcmc_statphys/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `mcmc_statphys-0.3.0/HISTORY.rst` & `mcmc_statphys-0.4.2/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,28 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 [Unreleased]
 ------------
 
+[0.4.0] - 2023-05-20
+--------------------
+
+Added
+~~~~~
+
+* Add `imshow` in `draw`
+* Add `animate` in `draw`
+
+Fixed
+~~~~~
+
+* Fix: `Wolff` and `Anneal` uid does not return
+
 [0.3.0] - 2023-05-18
 --------------------
 
 Added
 ~~~~~
 
 * Add `cv` in `analysis` to calculate the cv
```

### Comparing `mcmc_statphys-0.3.0/LICENSE` & `mcmc_statphys-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.3.0/PKG-INFO` & `mcmc_statphys-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcmc_statphys
-Version: 0.3.0
+Version: 0.4.2
 Summary: A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
 Home-page: https://github.com/uynajgi/mcmc_statphys
 Author: Uynaj GI
 Author-email: suquan12148@outlook.com
 License: MIT license
 Keywords: mcmc_statphys
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -63,14 +63,20 @@
 
 the latest version of mcmc_statphys: 
 
 .. code-block:: console
 
     $ pip install mcmc_statphys
 
+upgrade to the latest version:
+
+.. code-block:: console
+
+    $ pip install --upgrade mcmc_statphys
+
 Bugs
 ----
 
 Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub`_ and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`_).
 
 .. _here: https://github.com/uynajgi/mcmc_statphys/issues
 .. _GitHub: https://github.com/uynajgi/mcmc_statphys/
@@ -93,14 +99,28 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 [Unreleased]
 ------------
 
+[0.4.0] - 2023-05-20
+--------------------
+
+Added
+~~~~~
+
+* Add `imshow` in `draw`
+* Add `animate` in `draw`
+
+Fixed
+~~~~~
+
+* Fix: `Wolff` and `Anneal` uid does not return
+
 [0.3.0] - 2023-05-18
 --------------------
 
 Added
 ~~~~~
 
 * Add `cv` in `analysis` to calculate the cv
```

### Comparing `mcmc_statphys-0.3.0/README.rst` & `mcmc_statphys-0.4.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,20 @@
 
 the latest version of mcmc_statphys: 
 
 .. code-block:: console
 
     $ pip install mcmc_statphys
 
+upgrade to the latest version:
+
+.. code-block:: console
+
+    $ pip install --upgrade mcmc_statphys
+
 Bugs
 ----
 
 Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub`_ and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`_).
 
 .. _here: https://github.com/uynajgi/mcmc_statphys/issues
 .. _GitHub: https://github.com/uynajgi/mcmc_statphys/
```

### Comparing `mcmc_statphys-0.3.0/docs/Makefile` & `mcmc_statphys-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.3.0/docs/conf.py` & `mcmc_statphys-0.4.2/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # serve to show the default.
 
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
+
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
 
-import mcmc_statphys
+sys.path.insert(0, os.path.abspath('..'))
 
+# import mcmc_statphys
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
@@ -51,17 +52,17 @@
 author = "Uynaj GI"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = mcmc_statphys.__version__
+version = '0.4.2'
 # The full version, including alpha/beta/rc tags.
-release = mcmc_statphys.__version__
+release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
@@ -73,15 +74,14 @@
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
-
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = 'alabaster'
 
@@ -92,21 +92,19 @@
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
-
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'mcmc_statphysdoc'
 
-
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
 
@@ -123,40 +121,27 @@
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'mcmc_statphys.tex',
-     'mcmc_statphys Documentation',
+    (master_doc, 'mcmc_statphys.tex', 'mcmc_statphys Documentation',
      'Uynaj GI', 'manual'),
 ]
 
-
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'mcmc_statphys',
-     'mcmc_statphys Documentation',
-     [author], 1)
-]
-
+man_pages = [(master_doc, 'mcmc_statphys', 'mcmc_statphys Documentation',
+              [author], 1)]
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'mcmc_statphys',
-     'mcmc_statphys Documentation',
-     author,
-     'mcmc_statphys',
-     'One line description of project.',
-     'Miscellaneous'),
+    (master_doc, 'mcmc_statphys', 'mcmc_statphys Documentation', author,
+     'mcmc_statphys', 'One line description of project.', 'Miscellaneous'),
 ]
-
-
-
```

### Comparing `mcmc_statphys-0.3.0/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png` & `mcmc_statphys-0.4.2/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.3.0/docs/installation.rst` & `mcmc_statphys-0.4.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.3.0/docs/make.bat` & `mcmc_statphys-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.3.0/docs/usage.rst` & `mcmc_statphys-0.4.2/docs/usage.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Usages
 ======
 
-``mcmc_statphys`` is a python package for Monte Carlo simulations of
-statistical physics models. It is designed to be easy to use and easy to
-extend. It is also designed to be easy to use in a Jupyter notebook.
+``mcmc_statphys`` is a python package for Monte Carlo simulations of statistical physics models. It is designed to be easy to use and easy to extend. It is also designed to be easy to use in a Jupyter notebook.
 
 To use mcmc_statphys in a project
 
 .. code:: python
 
    import mcmc_statphys as mcpy
 
 Quick Start
 -----------
 
 Choose a model
 ~~~~~~~~~~~~~~
 
-First, create a model object that you want to simulate. For example, to
-create a 2D Ising model with 10x10 spins (Default: H=0, J=1)
+First, create a model object that you want to simulate. For example, to create a 2D Ising model with 10x10 spins (Default: H=0, J=1)
 
 *all results mey be different, it’s normal.*
 
 .. code:: python
 
    from mcmc_statphys.model import Ising
 
@@ -47,38 +44,32 @@
    #        [ 1,  1, -1, -1, -1,  1,  1, -1,  1, -1],
    #        [-1,  1, -1,  1,  1,  1,  1,  1,  1, -1],
    #        [ 1,  1, -1, -1,  1, -1, -1,  1,  1, -1]], dtype=int8)
 
 Choose a algorithm
 ~~~~~~~~~~~~~~~~~~
 
-Next, create a algorithm object that you want to use. For example, to
-create a Metropolis algorithm with 1000 steps
+Next, create a algorithm object that you want to use. For example, to create a Metropolis algorithm with 1000 steps
 
 .. code:: python
 
    from mcmc_statphys.algorithm import Metropolis
    algo = Metropolis(model=model)
 
-Now you can choose a sample method and get the result,
-e.g. ``equil_sample``:
+Now you can choose a sample method and get the result, e.g. ``equil_sample``:
 
 .. code:: python
 
    uid = algo.equil_sample(T=1.0, max_iter=1000) # set the sample temperature and max iteration
    # progress bar
    # 100%|██████████| 1000/1000 [00:09<00:00, 101.74it/s]
    uid
    '607ecc20f46d11ed948300e04c6807cc' # your uid must be different, because it is unique
 
-Notice that the ``uid`` is the unique id of the sample. In this package,
-we use ``uid`` to identify a sample process. We save the data of the
-sample in a attribute called ``iter_data`` of the algorithm object,
-which type is a ``pd.DataFrame``. You can get the data of the sample by
-using ``iter_data.loc[uid]``:
+Notice that the ``uid`` is the unique id of the sample. In this package, we use ``uid`` to identify a sample process. We save the data of the sample in a attribute called ``iter_data`` of the algorithm object, which type is a ``pd.DataFrame``. You can get the data of the sample by using ``iter_data.loc[uid]``:
 
 .. code:: python
 
    algo.iter_data.loc[uid]
 
 +===+=============+============+============+============+============+
 | i | T           | H          | energy     | mag        | spin       |
@@ -96,29 +87,27 @@
 +---+-------------+------------+------------+------------+------------+
 | 5 | 1.0         | 0          | 20.0       | 10         | …          |
 +---+-------------+------------+------------+------------+------------+
 
 Details of how to use the ``pandas`` can be found in the `User
 Guide <https://pandas.pydata.org/docs/user_guide/index.html>`__
 
-The uid mean that you can continue the sample process by using the same
-uid. For example, you can continue the sample process by using the same
-uid:
+The uid mean that you can continue the sample process by using the same uid. For example, you can continue the sample process by using the same uid:
 
 .. code:: python
 
    from uuid import uuid1
    uid1 = uuid1().hex
    uid2 = uuid1().hex
    algo2 = Metropolis(model=model)
    algo2.iter_sample(T=1.0, uid=uid1)
    algo2.iter_sample(T=1.0, uid=uid2)
    algo2.iter_data
 
-+---+---+-------------+------------+------------+------------+------------+
++===+===+=============+============+============+============+============+
 | u | i | T           | H          | energy     | mag        | spin       |
 | i | t |             |            |            | netization |            |
 | d | e |             |            |            |            |            |
 |   | r |             |            |            |            |            |
 +===+===+=============+============+============+============+============+
 | u | i | T           | H          | energy     | mag        | spin       |
 | i | t |             |            |            | netization |            |
@@ -195,15 +184,15 @@
 Continue the sample process by using the same uid:
 
 .. code:: python
 
    algo2.iter_sample(T=1.0, uid=uid2)
    algo2.iter_data
 
-+---+---+-------------+------------+------------+------------+------------+
++===+===+=============+============+============+============+============+
 | u | i | T           | H          | energy     | mag        | spin       |
 | i | t |             |            |            | netization |            |
 | d | e |             |            |            |            |            |
 |   | r |             |            |            |            |            |
 +===+===+=============+============+============+============+============+
 | u | i | T           | H          | energy     | mag        | spin       |
 | i | t |             |            |            | netization |            |
@@ -278,36 +267,41 @@
 +---+---+-------------+------------+------------+------------+------------+
 |   | 2 | 1.0         | 0          | 20.0       | 8          | …          |
 +---+---+-------------+------------+------------+------------+------------+
 
 Analyze the data
 ~~~~~~~~~~~~~~~~
 
-If you want to analyze the data, you can use the ``analyze`` module. For
-example, to get the energy distribution of the sample:
+If you want to analyze the data, you can use the ``analyze`` module. For example, to get the energy distribution of the sample:
 
 .. code:: python
 
    from mcmc_statphys import analysis
    uid3 = algo.equil_sample(T=1.0, max_iter=1000)
    energy_mean = analysis.mean(algo,uid=uid3,column='energy') # Attention: put algo not algo.iter_data
    energy_mean
    # -124.172
    # e.t.c.
 
 Plot the data
 ~~~~~~~~~~~~~
 
-If you want to plot the data, you can use the ``draw`` module. For
-example, to plot the energy distribution of the sample:
+If you want to plot the data, you can use the ``draw`` module. For example, to plot the energy distribution of the sample:
 
 .. code:: python
 
    from mcmc_statphys import draw
    uid4 = algo.equil_sample(T=1.0, max_iter=1000)
    fig = draw.Plot(algo)
    fig.curve(uid=uid4, column='energy')
 
-.. figure:: /docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png
-   :alt: iter-energy
 
-   iter-energy
+Animate the data
+
+If you want to animate the data, you can use the ``animate`` module. For example, to animate the spin of the sample:
+
+.. code:: python
+
+   from mcmc_statphys import draw
+   uid5 = algo.equil_sample(T=1.0, max_iter=1000)
+   ani = animate.Animation(algo)
+   ani.animate(uid=uid5) # the animation will be saved in the ./uid folder
```

### Comparing `mcmc_statphys-0.3.0/mcmc_statphys/analysis.py` & `mcmc_statphys-0.4.2/mcmc_statphys/analysis.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.3.0/mcmc_statphys/model.py` & `mcmc_statphys-0.4.2/mcmc_statphys/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,22 @@
 from typing import Any, Tuple
 
 # here put the import lib
 import numpy as np
 
 
 class Ising(object):
-    def __init__(
-        self,
-        L: int,
-        Jij: float = 1,
-        H: float = 0,
-        dim: int = 2,
-        *args: Any,
-        **kwargs: Any
-    ):
+
+    def __init__(self,
+                 L: int,
+                 Jij: float = 1,
+                 H: float = 0,
+                 dim: int = 2,
+                 *args: Any,
+                 **kwargs: Any):
         L = int(L)
         self.L = L
         self.dim = dim
         self.N = L**dim
         self.Jij = Jij
         self.H = H
         self._init_spin(type="ising")
@@ -46,45 +45,45 @@
         Args:
             type (str, optional): The type of the spin / cn: 自旋的类型 (Defaults \'ising\')
 
         Raises:
             ValueError: Invalid type of spin / cn: 无效的自旋类型
         """
         if type == "ising":
-            self.spin = np.random.choice([-1, 1], size=(self.L,) * self.dim)
+            self.spin = np.random.choice([-1, 1], size=(self.L, ) * self.dim)
             self.spin = self.spin.astype(np.int8)
         elif type == "heisenberg":
-            self.spin = 2 * np.random.rand(self.L, self.L, self.L, self.dim) - 1
+            self.spin = 2 * np.random.rand(self.L, self.L, self.L,
+                                           self.dim) - 1
             self.spin = self.spin.astype(np.float32)
         elif type == "XY":
             self.spin = 2 * np.random.rand(self.L, self.L, self.dim) - 1
             self.spin = self.spin.astype(np.float32)
         elif type == "potts":
             p = kwargs.pop("p", 2)
-            self.spin = np.random.choice(range(p), size=(self.L,) * self.dim)
+            self.spin = np.random.choice(range(p), size=(self.L, ) * self.dim)
             self.spin = self.spin.astype(np.int8)
         else:
             raise ValueError("Invalid type of spin")
-        self.tpye = type
+        self.type = type
 
     def _get_neighbor(self, index: Tuple[int, ...]) -> Tuple[int, ...]:
         """Get the neighbor of the site / cn: 获取格点的邻居
 
         Args:
             index (Tuple[int, ...]): The index of the site / cn: 格点的坐标
 
         Returns:
             Tuple[int, ...]: The neighbor of the site / cn: 格点的邻居
         """
         neighbors = []
         for i in range(self.dim):
             for j in [-1, 1]:
-                neighbors.append(
-                    index[:i] + ((index[i] + j) % self.L,) + index[i + 1:]
-                )
+                neighbors.append(index[:i] + ((index[i] + j) % self.L, ) +
+                                 index[i + 1:])
         neighbors = list(set(neighbors))  # 去重
         return neighbors
 
     def _get_neighbor_spin(self, index: Tuple[int, ...]) -> Tuple[int, ...]:
         """Get the spin of the neighbor of the site / cn: 获取格点的邻居的自旋
 
         Args:
@@ -109,20 +108,20 @@
             ValueError: Invalid type of spin / cn: 无效的自旋类型
 
         Returns:
             float: The energy of the site / cn: 格点的能量
         """
         neighbors_spin = self._get_neighbor_spin(index)
         energy = 0
-        if self.tpye == "ising" or self.tpye == "heisenberg" or self.tpye == "XY":
+        if self.type == "ising" or self.type == "heisenberg" or self.type == "XY":
             for neighbor_spin in neighbors_spin:
                 energy -= self.Jij * np.dot(self.spin[index], neighbor_spin)
-            if self.tpye == "ising":
+            if self.type == "ising":
                 energy -= self.H * self.spin[index]
-        elif self.tpye == "potts":
+        elif self.type == "potts":
             for neighbor_spin in neighbors_spin:
                 if self.spin[index] == neighbor_spin:
                     energy -= self.Jij
         else:
             raise ValueError("Invalid type of spin")
         return energy
 
@@ -167,63 +166,86 @@
     # 获取类的属性
     def _get_info(self) -> Tuple[np.ndarray, float, float]:
         """Get the info of the system / cn: 获取系统的信息
 
         Returns:
             Tuple[np.ndarray, float, float]: The info of the system / cn: 系统的信息
         """
-        return self.spin, self._get_total_energy(), self._get_total_magnetization()
+        return self.spin, self.energy, self.magnetization
 
     def _get_per_info(self):
         return self.spin, self._get_per_energy(), self._get_per_magnetization()
 
     def _change_site_spin(self, index: Tuple[int, ...]):
         """Change the spin of the site / cn: 改变格点的自旋
 
         Args:
             index (Tuple[int, ...]): The index of the site / cn: 格点的坐标
 
         Raises:
             ValueError: Invalid type of spin / cn: 无效的自旋类型
         """
-        if self.tpye == "ising":
+        if self.type == "ising":
             self.spin[index] *= -1
-        elif self.tpye == "heisenberg" or self.tpye == "XY":
+        elif self.type == "heisenberg" or self.type == "XY":
             self.spin[index] = 2 * np.random.rand(self.dim) - 1
-        elif self.tpye == "potts":
+        elif self.type == "potts":
             self.spin[index] = np.random.choice(range(self.p))
         else:
             raise ValueError("Invalid type of spin")
 
     def _change_delta_energy(self, index: Tuple[int, ...]):
         """Get the delta energy of the site"""
+        old_site = self.spin[index]
         old_site_energy = self._get_site_energy(index)
         self._change_site_spin(index)
+        new_site = self.spin[index]
         new_site_energy = self._get_site_energy(index)
         detle_energy = new_site_energy - old_site_energy
+        self.energy += detle_energy
+        self.magnetization += (new_site - old_site)
         return detle_energy
 
     def set_spin(self, spin):
-        # TODO[0.3.0]: 增加 spin 格式审查
+        # TODO[0.4.0]: 增加 spin 格式审查
         self.spin = spin
         self._get_total_energy()
         self._get_total_magnetization()
 
+    def get_energy(self) -> float:
+        """Get the total energy of the system / cn: 获取系统的总能量
+
+        Returns:
+            float: The total energy of the system / cn: 系统的总能量
+        """
+        return self.energy
+
+    def get_magnetization(self) -> float:
+        """Get the magnetization of the system / cn: 获取系统的总磁矩
+
+        Returns:
+            float: The per magnetization of the system / cn: 系统的单位磁矩
+        """
+        return self.magntization
+
 
 class Heisenberg(Ising):
+
     def __init__(self, L, Jij=1, H=0, *args, **kwargs):
         super().__init__(L, Jij, H, dim=3, *args, **kwargs)
         self._init_spin(type="heisenberg")
 
 
 class XY(Ising):
+
     def __init__(self, L, Jij=1, H=0, *args, **kwargs):
         super().__init__(L, Jij, H, dim=2, *args, **kwargs)
         self._init_spin(type="XY")
 
 
 class Potts(Ising):
+
     def __init__(self, L, Jij=1, H=0, dim=2, p=3, *args, **kwargs):
         # p is the number of states of the system
         self.p = p
         super().__init__(L, Jij, H, dim, *args, **kwargs)
         self._init_spin(type="potts", p=p)
```

### Comparing `mcmc_statphys-0.3.0/mcmc_statphys.egg-info/PKG-INFO` & `mcmc_statphys-0.4.2/mcmc_statphys.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcmc-statphys
-Version: 0.3.0
+Version: 0.4.2
 Summary: A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
 Home-page: https://github.com/uynajgi/mcmc_statphys
 Author: Uynaj GI
 Author-email: suquan12148@outlook.com
 License: MIT license
 Keywords: mcmc_statphys
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -63,14 +63,20 @@
 
 the latest version of mcmc_statphys: 
 
 .. code-block:: console
 
     $ pip install mcmc_statphys
 
+upgrade to the latest version:
+
+.. code-block:: console
+
+    $ pip install --upgrade mcmc_statphys
+
 Bugs
 ----
 
 Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub`_ and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`_).
 
 .. _here: https://github.com/uynajgi/mcmc_statphys/issues
 .. _GitHub: https://github.com/uynajgi/mcmc_statphys/
@@ -93,14 +99,28 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 [Unreleased]
 ------------
 
+[0.4.0] - 2023-05-20
+--------------------
+
+Added
+~~~~~
+
+* Add `imshow` in `draw`
+* Add `animate` in `draw`
+
+Fixed
+~~~~~
+
+* Fix: `Wolff` and `Anneal` uid does not return
+
 [0.3.0] - 2023-05-18
 --------------------
 
 Added
 ~~~~~
 
 * Add `cv` in `analysis` to calculate the cv
```

### Comparing `mcmc_statphys-0.3.0/mcmc_statphys.egg-info/SOURCES.txt` & `mcmc_statphys-0.4.2/mcmc_statphys.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
+docs/modules.rst
 docs/readme.rst
 docs/usage.rst
 docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png
 mcmc_statphys/__init__.py
 mcmc_statphys/algorithm.py
 mcmc_statphys/analysis.py
 mcmc_statphys/cli.py
@@ -29,13 +30,13 @@
 mcmc_statphys.egg-info/entry_points.txt
 mcmc_statphys.egg-info/not-zip-safe
 mcmc_statphys.egg-info/requires.txt
 mcmc_statphys.egg-info/top_level.txt
 tests/__init__.py
 tests/test.ipynb
 tests/test_mcmc_statphys.py
-tests/test/__init__.py
-tests/test/algorithm.py
-tests/test/analysis.py
-tests/test/cli.py
-tests/test/draw.py
-tests/test/model.py
+tests/one/__init__.py
+tests/one/algorithm.py
+tests/one/analysis.py
+tests/one/cli.py
+tests/one/draw.py
+tests/one/model.py
```

### Comparing `mcmc_statphys-0.3.0/setup.py` & `mcmc_statphys-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='mcmc_statphys',
     name='mcmc_statphys',
     packages=find_packages(include=['mcmc_statphys', 'mcmc_statphys.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/uynajgi/mcmc_statphys',
-    version='0.3.0',
+    version='0.4.2',
     zip_safe=False,
 )
```

### Comparing `mcmc_statphys-0.3.0/tests/test/analysis.py` & `mcmc_statphys-0.4.2/tests/one/analysis.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.3.0/tests/test/model.py` & `mcmc_statphys-0.4.2/tests/one/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,235 +1,251 @@
 # -*- encoding: utf-8 -*-
-'''
+"""
 @File    :   IsingObj.py
 @Time    :   2023/05/13 10:49:12
 @Author  :   UynajGI
 @Version :   beta0.0.1
 @Contact :   betterWL@hotmail.com
 @License :   (CC-BY-4.0)Copyright 2023
-'''
+"""
 
 from typing import Any, Tuple
 
 # here put the import lib
 import numpy as np
 
 
 class Ising(object):
 
     def __init__(self,
                  L: int,
                  Jij: float = 1,
                  H: float = 0,
-                 dimension: int = 2,
+                 dim: int = 2,
                  *args: Any,
                  **kwargs: Any):
         L = int(L)
         self.L = L
-        self.dimension = dimension
-        self.N = L**dimension
+        self.dim = dim
+        self.N = L**dim
         self.Jij = Jij
         self.H = H
-        self._init_spin(type='ising')
+        self._init_spin(type="ising")
         self._get_total_energy()
         self._get_total_magnetization()
 
     def __len__(self):
         return self.L
 
     def __getitem__(self, index: Tuple[int, ...]):
         return self.spin[index]
 
-    def _init_spin(self, type='ising', *args, **kwargs):
-        """ Initialize the spin of the system
+    def _init_spin(self, type="ising", *args, **kwargs):
+        """Initialize the spin of the system
 
         Args:
             type (str, optional): The type of the spin / cn: 自旋的类型 (Defaults \'ising\')
 
         Raises:
             ValueError: Invalid type of spin / cn: 无效的自旋类型
         """
-        if type == 'ising':
-            self.spin = np.random.choice([-1, 1],
-                                         size=(self.L, ) * self.dimension)
+        if type == "ising":
+            self.spin = np.random.choice([-1, 1], size=(self.L, ) * self.dim)
             self.spin = self.spin.astype(np.int8)
-        elif type == 'heisenberg':
+        elif type == "heisenberg":
             self.spin = 2 * np.random.rand(self.L, self.L, self.L,
-                                           self.dimension) - 1
+                                           self.dim) - 1
             self.spin = self.spin.astype(np.float32)
-        elif type == 'XY':
-            self.spin = 2 * np.random.rand(self.L, self.L, self.dimension) - 1
+        elif type == "XY":
+            self.spin = 2 * np.random.rand(self.L, self.L, self.dim) - 1
             self.spin = self.spin.astype(np.float32)
-        elif type == 'potts':
-            p = kwargs.pop('p', 2)
-            self.spin = np.random.choice(range(p),
-                                         size=(self.L, ) * self.dimension)
+        elif type == "potts":
+            p = kwargs.pop("p", 2)
+            self.spin = np.random.choice(range(p), size=(self.L, ) * self.dim)
             self.spin = self.spin.astype(np.int8)
         else:
-            raise ValueError('Invalid type of spin')
-        self.tpye = type
+            raise ValueError("Invalid type of spin")
+        self.type = type
 
     def _get_neighbor(self, index: Tuple[int, ...]) -> Tuple[int, ...]:
-        """ Get the neighbor of the site / cn: 获取格点的邻居
+        """Get the neighbor of the site / cn: 获取格点的邻居
 
         Args:
             index (Tuple[int, ...]): The index of the site / cn: 格点的坐标
 
         Returns:
             Tuple[int, ...]: The neighbor of the site / cn: 格点的邻居
         """
         neighbors = []
-        for i in range(self.dimension):
+        for i in range(self.dim):
             for j in [-1, 1]:
                 neighbors.append(index[:i] + ((index[i] + j) % self.L, ) +
                                  index[i + 1:])
         neighbors = list(set(neighbors))  # 去重
         return neighbors
 
     def _get_neighbor_spin(self, index: Tuple[int, ...]) -> Tuple[int, ...]:
-        """ Get the spin of the neighbor of the site / cn: 获取格点的邻居的自旋
+        """Get the spin of the neighbor of the site / cn: 获取格点的邻居的自旋
 
         Args:
             index (Tuple[int, ...]): The index of the site / cn: 格点的坐标
 
         Returns:
             Tuple[int, ...]: The spin of the neighbor of the site / cn: 格点的邻居的自旋
         """
         neighbors = self._get_neighbor(index)
         neighbors_spin = []
         for neighbor in neighbors:
             neighbors_spin.append(self.spin[neighbor])
         return neighbors_spin
 
     def _get_site_energy(self, index: Tuple[int, ...]) -> float:
-        """ Get the energy of the site / cn: 获取格点的能量
+        """Get the energy of the site / cn: 获取格点的能量
 
         Args:
             index (Tuple[int, ...]): The index of the site / cn: 格点的坐标
 
         Raises:
             ValueError: Invalid type of spin / cn: 无效的自旋类型
 
         Returns:
             float: The energy of the site / cn: 格点的能量
         """
         neighbors_spin = self._get_neighbor_spin(index)
         energy = 0
-        if self.tpye == 'ising' or self.tpye == 'heisenberg' or self.tpye == 'XY':
+        if self.type == "ising" or self.type == "heisenberg" or self.type == "XY":
             for neighbor_spin in neighbors_spin:
                 energy -= self.Jij * np.dot(self.spin[index], neighbor_spin)
-            if self.tpye == 'ising':
+            if self.type == "ising":
                 energy -= self.H * self.spin[index]
-        elif self.tpye == 'potts':
+        elif self.type == "potts":
             for neighbor_spin in neighbors_spin:
                 if self.spin[index] == neighbor_spin:
                     energy -= self.Jij
         else:
-            raise ValueError('Invalid type of spin')
+            raise ValueError("Invalid type of spin")
         return energy
 
     def _get_per_energy(self) -> float:
-        """ Get the per energy of the system / cn: 获取系统的单位能量
+        """Get the per energy of the system / cn: 获取系统的单位能量
 
         Returns:
             float: The per energy of the system / cn: 系统的单位能量
         """
         energy = 0
         for index in np.ndindex(self.spin.shape):
             energy += self._get_site_energy(index)
         return energy / self.N / 2
 
     def _get_total_energy(self) -> float:
-        """ Get the total energy of the system / cn: 获取系统的总能量
+        """Get the total energy of the system / cn: 获取系统的总能量
 
         Returns:
             float: The total energy of the system / cn: 系统的总能量
         """
-        total_energy = self._get_per_energy() * self.N
-        self.total_energy = total_energy
-        return total_energy
+        energy = self._get_per_energy() * self.N
+        self.energy = energy
+        return energy
 
     def _get_per_magnetization(self) -> float:
-        """ Get the per magnetization of the system / cn:
+        """Get the per magnetization of the system / cn:
 
         Returns:
             float: The per magnetization of the system / cn: 系统的单位磁矩
         """
         return self._get_total_magnetization() / self.N
 
     def _get_total_magnetization(self) -> float:
-        """ Get the magnetization of the system / cn: 获取系统的总磁矩
+        """Get the magnetization of the system / cn: 获取系统的总磁矩
 
         Returns:
             float: The magnetization of the system / cn: 系统的总磁矩
         """
-        self.total_magnetization = np.sum(self.spin,
-                                          axis=tuple(range(self.dimension)))
-        return self.total_magnetization
+        self.magnetization = np.sum(self.spin, axis=tuple(range(self.dim)))
+        return self.magnetization
 
     # 获取类的属性
     def _get_info(self) -> Tuple[np.ndarray, float, float]:
-        """ Get the info of the system / cn: 获取系统的信息
+        """Get the info of the system / cn: 获取系统的信息
 
         Returns:
             Tuple[np.ndarray, float, float]: The info of the system / cn: 系统的信息
         """
-        return self.spin, self._get_total_energy(
-        ), self._get_total_magnetization()
+        return self.spin, self.energy, self.magnetization
 
     def _get_per_info(self):
         return self.spin, self._get_per_energy(), self._get_per_magnetization()
 
     def _change_site_spin(self, index: Tuple[int, ...]):
-        """ Change the spin of the site / cn: 改变格点的自旋
+        """Change the spin of the site / cn: 改变格点的自旋
 
         Args:
             index (Tuple[int, ...]): The index of the site / cn: 格点的坐标
 
         Raises:
             ValueError: Invalid type of spin / cn: 无效的自旋类型
         """
-        if self.tpye == 'ising':
+        if self.type == "ising":
             self.spin[index] *= -1
-        elif self.tpye == 'heisenberg' or self.tpye == 'XY':
-            self.spin[index] = 2 * np.random.rand(self.dimension) - 1
-        elif self.tpye == 'potts':
+        elif self.type == "heisenberg" or self.type == "XY":
+            self.spin[index] = 2 * np.random.rand(self.dim) - 1
+        elif self.type == "potts":
             self.spin[index] = np.random.choice(range(self.p))
         else:
-            raise ValueError('Invalid type of spin')
+            raise ValueError("Invalid type of spin")
 
     def _change_delta_energy(self, index: Tuple[int, ...]):
-        '''Get the delta energy of the site'''
+        """Get the delta energy of the site"""
+        old_site = self.spin[index]
         old_site_energy = self._get_site_energy(index)
         self._change_site_spin(index)
+        new_site = self.spin[index]
         new_site_energy = self._get_site_energy(index)
         detle_energy = new_site_energy - old_site_energy
+        self.energy += detle_energy
+        self.magnetization += (new_site - old_site)
         return detle_energy
 
     def set_spin(self, spin):
-        # TODO[0.3.0]: 增加 spin 格式审查
+        # TODO[0.4.0]: 增加 spin 格式审查
         self.spin = spin
         self._get_total_energy()
         self._get_total_magnetization()
 
+    def get_energy(self) -> float:
+        """Get the total energy of the system / cn: 获取系统的总能量
+
+        Returns:
+            float: The total energy of the system / cn: 系统的总能量
+        """
+        return self.energy
+
+    def get_magnetization(self) -> float:
+        """Get the magnetization of the system / cn: 获取系统的总磁矩
+
+        Returns:
+            float: The per magnetization of the system / cn: 系统的单位磁矩
+        """
+        return self.magntization
+
 
 class Heisenberg(Ising):
 
     def __init__(self, L, Jij=1, H=0, *args, **kwargs):
-        super().__init__(L, Jij, H, dimension=3, *args, **kwargs)
-        self._init_spin(type='heisenberg')
+        super().__init__(L, Jij, H, dim=3, *args, **kwargs)
+        self._init_spin(type="heisenberg")
 
 
 class XY(Ising):
 
     def __init__(self, L, Jij=1, H=0, *args, **kwargs):
-        super().__init__(L, Jij, H, dimension=2, *args, **kwargs)
-        self._init_spin(type='XY')
+        super().__init__(L, Jij, H, dim=2, *args, **kwargs)
+        self._init_spin(type="XY")
 
 
 class Potts(Ising):
 
-    def __init__(self, L, Jij=1, H=0, dimension=2, p=3, *args, **kwargs):
+    def __init__(self, L, Jij=1, H=0, dim=2, p=3, *args, **kwargs):
         # p is the number of states of the system
         self.p = p
-        super().__init__(L, Jij, H, dimension, *args, **kwargs)
-        self._init_spin(type='potts', p=p)
+        super().__init__(L, Jij, H, dim, *args, **kwargs)
+        self._init_spin(type="potts", p=p)
```

