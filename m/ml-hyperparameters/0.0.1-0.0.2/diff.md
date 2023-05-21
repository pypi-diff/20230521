# Comparing `tmp/ml_hyperparameters-0.0.1.tar.gz` & `tmp/ml_hyperparameters-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ml_hyperparameters-0.0.1.tar", last modified: Sat May 20 12:02:31 2023, max compression
+gzip compressed data, was "dist\ml_hyperparameters-0.0.2.tar", last modified: Sun May 21 12:28:14 2023, max compression
```

## Comparing `ml_hyperparameters-0.0.1.tar` & `ml_hyperparameters-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 12:02:31.219260 ml_hyperparameters-0.0.1/
--rw-rw-rw-   0        0        0      635 2023-05-20 12:02:31.218011 ml_hyperparameters-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 12:02:31.215669 ml_hyperparameters-0.0.1/ml_hyperparameters.egg-info/
--rw-rw-rw-   0        0        0      635 2023-05-20 12:02:31.000000 ml_hyperparameters-0.0.1/ml_hyperparameters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-20 12:02:31.000000 ml_hyperparameters-0.0.1/ml_hyperparameters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 12:02:31.000000 ml_hyperparameters-0.0.1/ml_hyperparameters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-20 12:02:31.000000 ml_hyperparameters-0.0.1/ml_hyperparameters.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 12:02:31.000000 ml_hyperparameters-0.0.1/ml_hyperparameters.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 12:02:31.220457 ml_hyperparameters-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      922 2023-05-20 12:02:16.000000 ml_hyperparameters-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 12:28:14.635417 ml_hyperparameters-0.0.2/
+-rw-rw-rw-   0        0        0      567 2023-05-21 12:28:14.635417 ml_hyperparameters-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-05-21 12:16:29.000000 ml_hyperparameters-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 12:28:14.628926 ml_hyperparameters-0.0.2/ml_hyperparameters.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-05-21 12:28:14.000000 ml_hyperparameters-0.0.2/ml_hyperparameters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-21 12:28:14.000000 ml_hyperparameters-0.0.2/ml_hyperparameters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 12:28:14.000000 ml_hyperparameters-0.0.2/ml_hyperparameters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-21 12:28:14.000000 ml_hyperparameters-0.0.2/ml_hyperparameters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 12:28:14.000000 ml_hyperparameters-0.0.2/ml_hyperparameters.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 12:28:14.635417 ml_hyperparameters-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      922 2023-05-21 12:27:21.000000 ml_hyperparameters-0.0.2/setup.py
```

### Comparing `ml_hyperparameters-0.0.1/PKG-INFO` & `ml_hyperparameters-0.0.2/ml_hyperparameters.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-Metadata-Version: 1.1
-Name: ml_hyperparameters
-Version: 0.0.1
+Metadata-Version: 2.1
+Name: ml-hyperparameters
+Version: 0.0.2
 Summary: A basic library to help find the best hyperparameters in sklearn
-Home-page: UNKNOWN
 Author: Tom Neumann
 Author-email: tomn505@gmail.com
-License: UNKNOWN
-Description: A library that uses magic to find the best hyperparameters in a modular way
 Keywords: python,sklearn,hyperparameter finder
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
+
+A library that uses magic to find the best hyperparameters in a modular way
```

### Comparing `ml_hyperparameters-0.0.1/setup.py` & `ml_hyperparameters-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 NAME = "ml_hyperparameters"
 DESCRIPTION = "A basic library to help find the best hyperparameters in sklearn"
 LONG_DESCRIPTION = "A library that uses magic to find the best hyperparameters in a modular way"
 
 setup(
     name=NAME,
     version=VERSION,
```

