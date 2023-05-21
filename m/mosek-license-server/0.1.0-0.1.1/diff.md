# Comparing `tmp/mosek_license_server-0.1.0.tar.gz` & `tmp/mosek_license_server-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosek_license_server-0.1.0.tar", max compression
+gzip compressed data, was "mosek_license_server-0.1.1.tar", max compression
```

## Comparing `mosek_license_server-0.1.0.tar` & `mosek_license_server-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-20 15:32:46.105387 mosek_license_server-0.1.0/mosek_license/__init__.py
--rw-r--r--   0        0        0      499 2023-05-20 15:32:46.105387 mosek_license_server-0.1.0/mosek_license/license.py
--rw-r--r--   0        0        0      409 2023-05-20 15:33:04.970196 mosek_license_server-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1161 2023-05-20 15:32:46.105387 mosek_license_server-0.1.0/readme.md
--rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 mosek_license_server-0.1.0/setup.py
--rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 mosek_license_server-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-21 04:33:23.366391 mosek_license_server-0.1.1/mosek_license/__init__.py
+-rw-r--r--   0        0        0      499 2023-05-21 04:33:23.366391 mosek_license_server-0.1.1/mosek_license/license.py
+-rw-r--r--   0        0        0      470 2023-05-21 04:33:39.190631 mosek_license_server-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1982 2023-05-21 04:33:23.366391 mosek_license_server-0.1.1/readme.md
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 mosek_license_server-0.1.1/setup.py
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 mosek_license_server-0.1.1/PKG-INFO
```

### Comparing `mosek_license_server-0.1.0/PKG-INFO` & `mosek_license_server-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 Metadata-Version: 2.1
 Name: mosek-license-server
-Version: 0.1.0
+Version: 0.1.1
 Summary: Expose a mosek license via a nginx server
+Home-page: https://github.com/tschm/mosek-license-server
 License: Apache 2.0
 Author: Thomas Schmelzer
 Author-email: thomas.schmelzer@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: urllib3
+Project-URL: Repository, https://github.com/tschm/mosek-license-server
 Description-Content-Type: text/markdown
 
 # Mosek License Server
 
+[![PyPI version](https://badge.fury.io/py/mosek-license-server.svg)](https://badge.fury.io/py/mosek-license-server)
+[![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/tschm/mosek-license-server/blob/main/LICENSE)
+[![PyPI download month](https://img.shields.io/pypi/dm/mosek-license-server.svg)](https://pypi.python.org/pypi/mosek-license-server/)
+
 Using a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license
 on a server to be accessible from various research machines without sharing the actual
 license file in the underlying repositories.
 
 This repository serves two purposes. It exposes the server but it is also the home
 for a little Python package to inject the license into your programs.
 
+We solve a common problem here. Assume $20$ researchers work on $50$ different strategies.
+Using local copies of the same license file is a tedious exercise as the file needs to get 
+updated once a year. 
+Rather, each strategy would connect to the server to fetch a license using the mosek_license
+Python package. Once the strategy expires we only need to update the server.
+No change for the strategies is required.
+
 ## License server
 
 ### Copy your license file into folder 
 
 Copy the license file you have received (from Mosek) into the license folder.
 Name it `mosek'.
```

