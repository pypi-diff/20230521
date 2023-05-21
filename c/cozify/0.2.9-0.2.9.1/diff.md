# Comparing `tmp/cozify-0.2.9.tar.gz` & `tmp/cozify-0.2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cozify-0.2.9.tar", last modified: Sat Dec 16 21:03:41 2017, max compression
+gzip compressed data, was "dist/cozify-0.2.9.1.tar", last modified: Wed Dec 20 15:18:24 2017, max compression
```

## Comparing `cozify-0.2.9.tar` & `cozify-0.2.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 artanicus  (1000) artanicus  (1000)        0 2017-12-16 21:03:41.000000 cozify-0.2.9/
-drwxrwxr-x   0 artanicus  (1000) artanicus  (1000)        0 2017-12-16 21:03:41.000000 cozify-0.2.9/cozify/
-drwxrwxr-x   0 artanicus  (1000) artanicus  (1000)        0 2017-12-16 21:03:41.000000 cozify-0.2.9/cozify/test/
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)        0 2017-11-19 19:40:46.000000 cozify-0.2.9/cozify/test/__init__.py
--rwxrwxr-x   0 artanicus  (1000) artanicus  (1000)      384 2017-11-19 19:40:46.000000 cozify-0.2.9/cozify/test/debug.py
--rwxrwxr-x   0 artanicus  (1000) artanicus  (1000)     2835 2017-12-16 19:33:17.000000 cozify-0.2.9/cozify/test/test_cloud.py
--rwxrwxr-x   0 artanicus  (1000) artanicus  (1000)      126 2017-11-19 19:40:46.000000 cozify-0.2.9/cozify/test/test_config.py
--rwxrwxr-x   0 artanicus  (1000) artanicus  (1000)     1799 2017-12-16 19:33:17.000000 cozify-0.2.9/cozify/test/test_hub.py
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)      984 2017-09-22 12:46:55.000000 cozify-0.2.9/cozify/Error.py
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)       22 2017-12-16 19:33:17.000000 cozify-0.2.9/cozify/__init__.py
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)    15932 2017-12-16 19:33:17.000000 cozify-0.2.9/cozify/cloud.py
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     3828 2017-12-16 19:33:17.000000 cozify-0.2.9/cozify/config.py
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     9790 2017-12-16 21:00:13.000000 cozify-0.2.9/cozify/hub.py
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     1114 2017-10-14 13:56:51.000000 cozify-0.2.9/cozify/multisensor.py
-drwxrwxr-x   0 artanicus  (1000) artanicus  (1000)        0 2017-12-16 21:03:41.000000 cozify-0.2.9/cozify.egg-info/
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     5371 2017-12-16 21:03:41.000000 cozify-0.2.9/cozify.egg-info/PKG-INFO
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)      414 2017-12-16 21:03:41.000000 cozify-0.2.9/cozify.egg-info/SOURCES.txt
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)        1 2017-12-16 21:03:41.000000 cozify-0.2.9/cozify.egg-info/dependency_links.txt
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)        9 2017-12-16 21:03:41.000000 cozify-0.2.9/cozify.egg-info/requires.txt
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)        7 2017-12-16 21:03:41.000000 cozify-0.2.9/cozify.egg-info/top_level.txt
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     1134 2017-04-06 13:46:06.000000 cozify-0.2.9/LICENSE
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)       82 2017-10-14 14:36:55.000000 cozify-0.2.9/MANIFEST.in
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     3939 2017-12-16 19:33:17.000000 cozify-0.2.9/README.rst
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     1149 2017-11-19 19:40:46.000000 cozify-0.2.9/setup.py
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     5371 2017-12-16 21:03:41.000000 cozify-0.2.9/PKG-INFO
--rw-rw-r--   0 artanicus  (1000) artanicus  (1000)       38 2017-12-16 21:03:41.000000 cozify-0.2.9/setup.cfg
+drwxrwxr-x   0 artanicus  (1000) artanicus  (1000)        0 2017-12-20 15:18:24.000000 cozify-0.2.9.1/
+drwxrwxr-x   0 artanicus  (1000) artanicus  (1000)        0 2017-12-20 15:18:24.000000 cozify-0.2.9.1/cozify/
+drwxrwxr-x   0 artanicus  (1000) artanicus  (1000)        0 2017-12-20 15:18:24.000000 cozify-0.2.9.1/cozify/test/
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)        0 2017-11-19 19:40:46.000000 cozify-0.2.9.1/cozify/test/__init__.py
+-rwxrwxr-x   0 artanicus  (1000) artanicus  (1000)      384 2017-12-20 15:15:30.000000 cozify-0.2.9.1/cozify/test/debug.py
+-rwxrwxr-x   0 artanicus  (1000) artanicus  (1000)     2835 2017-12-20 15:15:30.000000 cozify-0.2.9.1/cozify/test/test_cloud.py
+-rwxrwxr-x   0 artanicus  (1000) artanicus  (1000)      126 2017-11-19 19:40:46.000000 cozify-0.2.9.1/cozify/test/test_config.py
+-rwxrwxr-x   0 artanicus  (1000) artanicus  (1000)     1799 2017-12-20 15:15:30.000000 cozify-0.2.9.1/cozify/test/test_hub.py
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)      984 2017-09-22 12:46:55.000000 cozify-0.2.9.1/cozify/Error.py
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)       24 2017-12-20 15:17:16.000000 cozify-0.2.9.1/cozify/__init__.py
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)    15932 2017-12-20 15:15:30.000000 cozify-0.2.9.1/cozify/cloud.py
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     3828 2017-12-16 19:33:17.000000 cozify-0.2.9.1/cozify/config.py
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     9790 2017-12-20 15:16:24.000000 cozify-0.2.9.1/cozify/hub.py
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     1114 2017-10-14 13:56:51.000000 cozify-0.2.9.1/cozify/multisensor.py
+drwxrwxr-x   0 artanicus  (1000) artanicus  (1000)        0 2017-12-20 15:18:24.000000 cozify-0.2.9.1/cozify.egg-info/
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     5373 2017-12-20 15:18:24.000000 cozify-0.2.9.1/cozify.egg-info/PKG-INFO
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)      414 2017-12-20 15:18:24.000000 cozify-0.2.9.1/cozify.egg-info/SOURCES.txt
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)        1 2017-12-20 15:18:24.000000 cozify-0.2.9.1/cozify.egg-info/dependency_links.txt
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)        9 2017-12-20 15:18:24.000000 cozify-0.2.9.1/cozify.egg-info/requires.txt
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)        7 2017-12-20 15:18:24.000000 cozify-0.2.9.1/cozify.egg-info/top_level.txt
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     1134 2017-04-06 13:46:06.000000 cozify-0.2.9.1/LICENSE
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)       82 2017-10-14 14:36:55.000000 cozify-0.2.9.1/MANIFEST.in
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     3939 2017-12-20 15:15:30.000000 cozify-0.2.9.1/README.rst
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     1149 2017-11-19 19:40:46.000000 cozify-0.2.9.1/setup.py
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)     5373 2017-12-20 15:18:24.000000 cozify-0.2.9.1/PKG-INFO
+-rw-rw-r--   0 artanicus  (1000) artanicus  (1000)       38 2017-12-20 15:18:24.000000 cozify-0.2.9.1/setup.cfg
```

### Comparing `cozify-0.2.9/cozify/test/test_cloud.py` & `cozify-0.2.9.1/cozify/test/test_cloud.py`

 * *Files identical despite different names*

### Comparing `cozify-0.2.9/cozify/test/test_hub.py` & `cozify-0.2.9.1/cozify/test/test_hub.py`

 * *Files identical despite different names*

### Comparing `cozify-0.2.9/cozify/Error.py` & `cozify-0.2.9.1/cozify/Error.py`

 * *Files identical despite different names*

### Comparing `cozify-0.2.9/cozify/cloud.py` & `cozify-0.2.9.1/cozify/cloud.py`

 * *Files identical despite different names*

### Comparing `cozify-0.2.9/cozify/config.py` & `cozify-0.2.9.1/cozify/config.py`

 * *Files identical despite different names*

### Comparing `cozify-0.2.9/cozify/hub.py` & `cozify-0.2.9.1/cozify/hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import requests, json, logging
 from . import config as c
 from . import cloud
 
 from .Error import APIError
 
-apiPath = '/cc/1.6'
+apiPath = '/cc/1.7'
 remote = False
 autoremote = True
 
 def getDevices(hubName=None, hubId=None):
     """Get up to date full devices data set as a dict
 
     Args:
```

### Comparing `cozify-0.2.9/cozify/multisensor.py` & `cozify-0.2.9.1/cozify/multisensor.py`

 * *Files identical despite different names*

### Comparing `cozify-0.2.9/cozify.egg-info/PKG-INFO` & `cozify-0.2.9.1/cozify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cozify
-Version: 0.2.9
+Version: 0.2.9.1
 Summary: Unofficial Python bindings and helpers for the unpublished Cozify API.
 Home-page: https://github.com/Artanicus/python-cozify
 Author: artanicus
 Author-email: python-cozify@nocturnal.fi
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: python-cozify
```

### Comparing `cozify-0.2.9/LICENSE` & `cozify-0.2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cozify-0.2.9/README.rst` & `cozify-0.2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `cozify-0.2.9/setup.py` & `cozify-0.2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `cozify-0.2.9/PKG-INFO` & `cozify-0.2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cozify
-Version: 0.2.9
+Version: 0.2.9.1
 Summary: Unofficial Python bindings and helpers for the unpublished Cozify API.
 Home-page: https://github.com/Artanicus/python-cozify
 Author: artanicus
 Author-email: python-cozify@nocturnal.fi
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: python-cozify
```

