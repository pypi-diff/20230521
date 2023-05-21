# Comparing `tmp/umbridge-1.2.2.tar.gz` & `tmp/umbridge-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umbridge-1.2.2.tar", last modified: Fri May 12 10:38:04 2023, max compression
+gzip compressed data, was "umbridge-1.2.3.tar", last modified: Sun May 21 07:57:38 2023, max compression
```

## Comparing `umbridge-1.2.2.tar` & `umbridge-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:38:04.993322 umbridge-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 10:37:52.000000 umbridge-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-12 10:38:04.993322 umbridge-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-12 10:37:52.000000 umbridge-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:38:04.993322 umbridge-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-12 10:37:52.000000 umbridge-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:38:04.989321 umbridge-1.2.2/umbridge/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 10:37:52.000000 umbridge-1.2.2/umbridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-12 10:37:52.000000 umbridge-1.2.2/umbridge/pymc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19958 2023-05-12 10:37:52.000000 umbridge-1.2.2/umbridge/um.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:38:04.993322 umbridge-1.2.2/umbridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-12 10:38:04.000000 umbridge-1.2.2/umbridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 10:38:04.000000 umbridge-1.2.2/umbridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:38:04.000000 umbridge-1.2.2/umbridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-12 10:38:04.000000 umbridge-1.2.2/umbridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 10:38:04.000000 umbridge-1.2.2/umbridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:57:38.051923 umbridge-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 07:57:27.000000 umbridge-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-21 07:57:38.051923 umbridge-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-21 07:57:27.000000 umbridge-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 07:57:38.051923 umbridge-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 07:57:27.000000 umbridge-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:57:38.051923 umbridge-1.2.3/umbridge/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-21 07:57:27.000000 umbridge-1.2.3/umbridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-21 07:57:27.000000 umbridge-1.2.3/umbridge/emcee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-21 07:57:27.000000 umbridge-1.2.3/umbridge/pymc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19958 2023-05-21 07:57:27.000000 umbridge-1.2.3/umbridge/um.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:57:38.051923 umbridge-1.2.3/umbridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-21 07:57:38.000000 umbridge-1.2.3/umbridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-21 07:57:38.000000 umbridge-1.2.3/umbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 07:57:38.000000 umbridge-1.2.3/umbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-21 07:57:38.000000 umbridge-1.2.3/umbridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 07:57:38.000000 umbridge-1.2.3/umbridge.egg-info/top_level.txt
```

### Comparing `umbridge-1.2.2/LICENSE` & `umbridge-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `umbridge-1.2.2/PKG-INFO` & `umbridge-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umbridge
-Version: 1.2.2
+Version: 1.2.3
 Summary: UM-Bridge (the UQ and Model Bridge) provides a unified interface for numerical models that is accessible from virtually any programming language or framework. It is primarily intended for coupling advanced models (e.g. simulations of complex physical processes) to advanced statistical or optimization methods.
 Home-page: https://github.com/UM-Bridge/umbridge
 Author: UM-Bridge
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `umbridge-1.2.2/README.md` & `umbridge-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `umbridge-1.2.2/setup.py` & `umbridge-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="umbridge",
-    version="1.2.2",
+    version="1.2.3",
     author="UM-Bridge",
     author_email="",
     description="UM-Bridge (the UQ and Model Bridge) provides a unified interface for numerical models that is accessible from virtually any programming language or framework. It is primarily intended for coupling advanced models (e.g. simulations of complex physical processes) to advanced statistical or optimization methods.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp", "requests", "asyncio"],
     url="https://github.com/UM-Bridge/umbridge",
```

### Comparing `umbridge-1.2.2/umbridge/pymc.py` & `umbridge-1.2.3/umbridge/pymc.py`

 * *Files identical despite different names*

### Comparing `umbridge-1.2.2/umbridge/um.py` & `umbridge-1.2.3/umbridge/um.py`

 * *Files identical despite different names*

### Comparing `umbridge-1.2.2/umbridge.egg-info/PKG-INFO` & `umbridge-1.2.3/umbridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umbridge
-Version: 1.2.2
+Version: 1.2.3
 Summary: UM-Bridge (the UQ and Model Bridge) provides a unified interface for numerical models that is accessible from virtually any programming language or framework. It is primarily intended for coupling advanced models (e.g. simulations of complex physical processes) to advanced statistical or optimization methods.
 Home-page: https://github.com/UM-Bridge/umbridge
 Author: UM-Bridge
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

