# Comparing `tmp/lakeapi-0.4.5.tar.gz` & `tmp/lakeapi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakeapi-0.4.5.tar", last modified: Mon Jan  9 14:54:27 2023, max compression
+gzip compressed data, was "lakeapi-0.5.0.tar", last modified: Sun May 21 15:31:03 2023, max compression
```

## Comparing `lakeapi-0.4.5.tar` & `lakeapi-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-01-09 14:54:27.823211 lakeapi-0.4.5/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      150 2022-10-10 10:44:58.000000 lakeapi-0.4.5/AUTHORS.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     3322 2022-12-09 09:20:38.000000 lakeapi-0.4.5/CONTRIBUTING.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      916 2023-01-09 14:53:15.000000 lakeapi-0.4.5/HISTORY.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)    10142 2022-10-10 10:44:58.000000 lakeapi-0.4.5/LICENSE
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      262 2022-10-10 10:44:58.000000 lakeapi-0.4.5/MANIFEST.in
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       97 2022-10-10 10:44:58.000000 lakeapi-0.4.5/NOTICE.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     3673 2023-01-09 14:54:27.823211 lakeapi-0.4.5/PKG-INFO
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     1970 2022-12-09 09:30:14.000000 lakeapi-0.4.5/README.rst
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-01-09 14:54:27.819211 lakeapi-0.4.5/docs/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      608 2022-10-10 10:44:58.000000 lakeapi-0.4.5/docs/Makefile
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-01-09 14:54:27.819211 lakeapi-0.4.5/docs/_build/
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-01-09 14:54:27.819211 lakeapi-0.4.5/docs/_build/html/
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-01-09 14:54:27.819211 lakeapi-0.4.5/docs/_build/html/_static/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      286 2022-10-10 10:55:29.000000 lakeapi-0.4.5/docs/_build/html/_static/file.png
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       90 2022-10-10 10:55:29.000000 lakeapi-0.4.5/docs/_build/html/_static/minus.png
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       90 2022-10-10 10:55:29.000000 lakeapi-0.4.5/docs/_build/html/_static/plus.png
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       28 2022-10-10 10:44:58.000000 lakeapi-0.4.5/docs/authors.rst
--rwxrwxr-x   0 lefty     (1000) lefty     (1000)     4773 2022-10-10 10:44:58.000000 lakeapi-0.4.5/docs/conf.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       33 2022-10-10 10:44:58.000000 lakeapi-0.4.5/docs/contributing.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       28 2022-10-10 10:44:58.000000 lakeapi-0.4.5/docs/history.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      305 2022-10-10 10:44:58.000000 lakeapi-0.4.5/docs/index.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     1129 2022-12-09 09:20:42.000000 lakeapi-0.4.5/docs/installation.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      292 2022-12-09 09:30:14.000000 lakeapi-0.4.5/docs/lakeapi.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      769 2022-10-10 10:44:58.000000 lakeapi-0.4.5/docs/make.bat
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       58 2022-12-09 09:27:03.000000 lakeapi-0.4.5/docs/modules.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       27 2022-10-10 10:44:58.000000 lakeapi-0.4.5/docs/readme.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      658 2022-10-10 10:44:58.000000 lakeapi-0.4.5/docs/usage.rst
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-01-09 14:54:27.819211 lakeapi-0.4.5/lakeapi/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      246 2023-01-09 14:52:55.000000 lakeapi-0.4.5/lakeapi/__init__.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      535 2023-01-09 14:51:02.000000 lakeapi-0.4.5/lakeapi/_cache.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     6991 2022-11-30 15:17:44.000000 lakeapi-0.4.5/lakeapi/_read.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)    47543 2022-11-30 15:17:44.000000 lakeapi-0.4.5/lakeapi/_read_parquet.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)    15335 2022-11-30 13:48:11.000000 lakeapi-0.4.5/lakeapi/_utils.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     9875 2022-12-08 13:19:28.000000 lakeapi-0.4.5/lakeapi/main.py
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-01-09 14:54:27.823211 lakeapi-0.4.5/lakeapi.egg-info/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     3673 2023-01-09 14:54:27.000000 lakeapi-0.4.5/lakeapi.egg-info/PKG-INFO
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      775 2023-01-09 14:54:27.000000 lakeapi-0.4.5/lakeapi.egg-info/SOURCES.txt
--rw-rw-r--   0 lefty     (1000) lefty     (1000)        1 2023-01-09 14:54:27.000000 lakeapi-0.4.5/lakeapi.egg-info/dependency_links.txt
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       45 2023-01-09 14:54:27.000000 lakeapi-0.4.5/lakeapi.egg-info/entry_points.txt
--rw-rw-r--   0 lefty     (1000) lefty     (1000)        1 2023-01-09 14:54:27.000000 lakeapi-0.4.5/lakeapi.egg-info/not-zip-safe
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      194 2023-01-09 14:54:27.000000 lakeapi-0.4.5/lakeapi.egg-info/requires.txt
--rw-rw-r--   0 lefty     (1000) lefty     (1000)        8 2023-01-09 14:54:27.000000 lakeapi-0.4.5/lakeapi.egg-info/top_level.txt
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      497 2023-01-09 14:54:27.823211 lakeapi-0.4.5/setup.cfg
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     1657 2023-01-09 14:52:55.000000 lakeapi-0.4.5/setup.py
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-01-09 14:54:27.823211 lakeapi-0.4.5/tests/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       37 2022-10-10 10:44:58.000000 lakeapi-0.4.5/tests/__init__.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      858 2022-10-10 11:00:09.000000 lakeapi-0.4.5/tests/test_lakeapi.py
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-05-21 15:31:03.663038 lakeapi-0.5.0/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      150 2022-10-08 18:58:50.000000 lakeapi-0.5.0/AUTHORS.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     3324 2023-01-24 19:55:04.000000 lakeapi-0.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     1047 2023-05-21 15:29:47.000000 lakeapi-0.5.0/HISTORY.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    10142 2022-10-08 20:59:37.000000 lakeapi-0.5.0/LICENSE
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      262 2022-10-08 18:58:50.000000 lakeapi-0.5.0/MANIFEST.in
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       97 2022-10-08 21:00:18.000000 lakeapi-0.5.0/NOTICE.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     3855 2023-05-21 15:31:03.663038 lakeapi-0.5.0/PKG-INFO
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     2000 2023-01-24 19:57:35.000000 lakeapi-0.5.0/README.rst
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-05-21 15:31:03.659038 lakeapi-0.5.0/docs/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      608 2022-10-08 18:58:50.000000 lakeapi-0.5.0/docs/Makefile
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-05-21 15:31:03.659038 lakeapi-0.5.0/docs/_build/
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-05-21 15:31:03.659038 lakeapi-0.5.0/docs/_build/html/
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-05-21 15:31:03.659038 lakeapi-0.5.0/docs/_build/html/_static/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      286 2022-10-09 07:37:32.000000 lakeapi-0.5.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       90 2022-10-09 07:37:32.000000 lakeapi-0.5.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       90 2022-10-09 07:37:32.000000 lakeapi-0.5.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       28 2022-10-08 18:58:50.000000 lakeapi-0.5.0/docs/authors.rst
+-rwxrwxr-x   0 lefty     (1000) lefty     (1000)     4773 2022-10-08 18:58:50.000000 lakeapi-0.5.0/docs/conf.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       33 2022-10-08 18:58:50.000000 lakeapi-0.5.0/docs/contributing.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       28 2022-10-08 18:58:50.000000 lakeapi-0.5.0/docs/history.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      305 2022-10-08 18:58:50.000000 lakeapi-0.5.0/docs/index.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     1133 2023-01-24 19:55:16.000000 lakeapi-0.5.0/docs/installation.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      292 2023-01-24 19:53:28.000000 lakeapi-0.5.0/docs/lakeapi.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      805 2022-10-08 18:58:50.000000 lakeapi-0.5.0/docs/make.bat
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       58 2022-10-09 07:37:47.000000 lakeapi-0.5.0/docs/modules.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       27 2022-10-08 18:58:50.000000 lakeapi-0.5.0/docs/readme.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      658 2022-10-09 16:50:24.000000 lakeapi-0.5.0/docs/usage.rst
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-05-21 15:31:03.663038 lakeapi-0.5.0/lakeapi/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      246 2023-05-21 15:30:27.000000 lakeapi-0.5.0/lakeapi/__init__.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      553 2023-01-24 19:53:28.000000 lakeapi-0.5.0/lakeapi/_cache.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     6991 2022-11-19 10:31:15.000000 lakeapi-0.5.0/lakeapi/_read.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    47543 2022-11-19 10:31:40.000000 lakeapi-0.5.0/lakeapi/_read_parquet.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    15335 2022-11-19 10:30:43.000000 lakeapi-0.5.0/lakeapi/_utils.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    10008 2023-05-21 15:10:09.000000 lakeapi-0.5.0/lakeapi/main.py
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-05-21 15:31:03.663038 lakeapi-0.5.0/lakeapi.egg-info/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     3855 2023-05-21 15:31:03.000000 lakeapi-0.5.0/lakeapi.egg-info/PKG-INFO
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      775 2023-05-21 15:31:03.000000 lakeapi-0.5.0/lakeapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)        1 2023-05-21 15:31:03.000000 lakeapi-0.5.0/lakeapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       46 2023-05-21 15:31:03.000000 lakeapi-0.5.0/lakeapi.egg-info/entry_points.txt
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)        1 2023-05-21 15:31:03.000000 lakeapi-0.5.0/lakeapi.egg-info/not-zip-safe
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      194 2023-05-21 15:31:03.000000 lakeapi-0.5.0/lakeapi.egg-info/requires.txt
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)        8 2023-05-21 15:31:03.000000 lakeapi-0.5.0/lakeapi.egg-info/top_level.txt
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      497 2023-05-21 15:31:03.663038 lakeapi-0.5.0/setup.cfg
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     1658 2023-05-21 15:30:27.000000 lakeapi-0.5.0/setup.py
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-05-21 15:31:03.663038 lakeapi-0.5.0/tests/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       37 2022-10-08 18:58:50.000000 lakeapi-0.5.0/tests/__init__.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      858 2022-10-13 08:11:12.000000 lakeapi-0.5.0/tests/test_lakeapi.py
```

### Comparing `lakeapi-0.4.5/CONTRIBUTING.rst` & `lakeapi-0.5.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at https://github.com/crypto-lake/lakeapi/issues.
+Report bugs at https://github.com/crypto-lake/lake-api/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
@@ -41,15 +41,15 @@
 Lake API could always use more documentation, whether as part of the
 official Lake API docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/crypto-lake/lakeapi/issues.
+The best way to send feedback is to file an issue at https://github.com/crypto-lake/lake-api/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
```

### Comparing `lakeapi-0.4.5/LICENSE` & `lakeapi-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi-0.4.5/PKG-INFO` & `lakeapi-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: lakeapi
-Version: 0.4.5
+Version: 0.5.0
 Summary: API for accessing Lake crypto market data
-Home-page: https://github.com/crypto-lake/lakeapi
+Home-page: https://github.com/crypto-lake/lake-api
 Author: Jan Skoda
 Author-email: skoda@jskoda.cz
 License: Apache 2 license
 Keywords: lakeapi
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -37,15 +38,15 @@
 .. image:: https://github.com/crypto-lake/lake-api/actions/workflows/dev.yml/badge.svg
      :target: https://github.com/crypto-lake/lake-api/actions/workflows/dev.yml
      :alt: Build status
 
 
 API for accessing Lake crypto market data.
 
-Lake is a service providing historical cryptocurrency market data in high detail, including `order book data <https://crypto-lake.com/order-book-data/>`_, tick trades and 1m trade candles. It is tuned for convenient quant and machine-learning purposes and so offers high performance, caching and parallelization.
+Lake is a service providing `historical cryptocurrency market data <https://crypto-lake.com/>`_ in high detail, including `order book data <https://crypto-lake.com/order-book-data/>`_, tick trades and 1m trade candles. It is tuned for convenient quant and machine-learning purposes and so offers high performance, caching and parallelization.
 
 
 * Web: https://crypto-lake.com/
 * Documentation: https://lake-api.readthedocs.io.
 * Online example -- executable collab notebook: https://colab.research.google.com/drive/1E7MSUT8xqYTMVLiq_rMBLNcZmI_KusK3
 
 
@@ -88,14 +89,20 @@
 working directory.
 
 
 =======
 History
 =======
 
+0.5.0 (2023-05-21)
+------------------
+
+* support for funding, open_interest and liquidations list_data
+* improve data type typing
+
 0.4.5 (2023-01-09)
 ------------------
 
 * grow default cache size limit from 3 GB to 10 GB
 
 0.4.3 (2022-12-09)
 ------------------
@@ -144,7 +151,9 @@
 
 * Python2.7 support and documentation improvements.
 
 0.1.0 (2022-10-08)
 ------------------
 
 * First release on PyPI.
+
+
```

### Comparing `lakeapi-0.4.5/README.rst` & `lakeapi-0.5.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 .. image:: https://github.com/crypto-lake/lake-api/actions/workflows/dev.yml/badge.svg
      :target: https://github.com/crypto-lake/lake-api/actions/workflows/dev.yml
      :alt: Build status
 
 
 API for accessing Lake crypto market data.
 
-Lake is a service providing historical cryptocurrency market data in high detail, including `order book data <https://crypto-lake.com/order-book-data/>`_, tick trades and 1m trade candles. It is tuned for convenient quant and machine-learning purposes and so offers high performance, caching and parallelization.
+Lake is a service providing `historical cryptocurrency market data <https://crypto-lake.com/>`_ in high detail, including `order book data <https://crypto-lake.com/order-book-data/>`_, tick trades and 1m trade candles. It is tuned for convenient quant and machine-learning purposes and so offers high performance, caching and parallelization.
 
 
 * Web: https://crypto-lake.com/
 * Documentation: https://lake-api.readthedocs.io.
 * Online example -- executable collab notebook: https://colab.research.google.com/drive/1E7MSUT8xqYTMVLiq_rMBLNcZmI_KusK3
```

### Comparing `lakeapi-0.4.5/docs/Makefile` & `lakeapi-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lakeapi-0.4.5/docs/conf.py` & `lakeapi-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lakeapi-0.4.5/docs/installation.rst` & `lakeapi-0.5.0/docs/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 
 The sources for Lake API can be downloaded from the `Github repo`_.
 
 You can either clone the public repository:
 
 .. code-block:: console
 
-    $ git clone git://github.com/crypto-lake/lakeapi
+    $ git clone git://github.com/crypto-lake/lake-api
 
 Or download the `tarball`_:
 
 .. code-block:: console
 
-    $ curl -OJL https://github.com/crypto-lake/lakeapi/tarball/master
+    $ curl -OJL https://github.com/crypto-lake/lake-api/tarball/master
 
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
     $ python setup.py install
 
 
-.. _Github repo: https://github.com/crypto-lake/lakeapi
-.. _tarball: https://github.com/crypto-lake/lakeapi/tarball/master
+.. _Github repo: https://github.com/crypto-lake/lake-api
+.. _tarball: https://github.com/crypto-lake/lake-api/tarball/master
```

### Comparing `lakeapi-0.4.5/docs/usage.rst` & `lakeapi-0.5.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lakeapi-0.4.5/lakeapi/_cache.py` & `lakeapi-0.5.0/lakeapi/_cache.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from pathlib import Path
 
 bytes_limit: int = 10_000_000_000
 verbose_cache = 0
 
 _store: joblib.Memory = joblib.Memory(
 	'.lake_cache',
-	compress = 2,
+	compress = 0,
 	bytes_limit = bytes_limit,
 	verbose = verbose_cache,
+	mmap_mode = 'c',
 )
 cached: Callable[..., Callable[..., Any]] = _store.cache
 _store.reduce_size()
 
 if __name__ == '__main__':
 	import time
```

### Comparing `lakeapi-0.4.5/lakeapi/_read.py` & `lakeapi-0.5.0/lakeapi/_read.py`

 * *Files identical despite different names*

### Comparing `lakeapi-0.4.5/lakeapi/_read_parquet.py` & `lakeapi-0.5.0/lakeapi/_read_parquet.py`

 * *Files identical despite different names*

### Comparing `lakeapi-0.4.5/lakeapi/_utils.py` & `lakeapi-0.5.0/lakeapi/_utils.py`

 * *Files identical despite different names*

### Comparing `lakeapi-0.4.5/lakeapi/main.py` & `lakeapi-0.5.0/lakeapi/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import awswrangler as wr
 import pandas as pd
 from cachetools_ext.fs import FSLRUCache
 from botocache.botocache import botocache_context
 
 import lakeapi._read_parquet
 
+DataType = Literal["book", "trades", "candles", "level_1", "funding", "open_interest", "liquiditions"]
+
 cache = FSLRUCache(ttl=8 * 60 * 60, path=".lake_cache/boto", maxsize=1000)
 default_bucket = 'qnt.data/market-data/cryptofeed'
 is_anonymous_access = False
 
 
 def set_default_bucket(bucket: str) -> None:
     global default_bucket
@@ -41,15 +43,15 @@
         return config
 
     if anonymous_access:
         is_anonymous_access = True
         awswrangler._utils.default_botocore_config = _anonymous_access_config
 
 def load_data(
-    table: Literal["book", "trades", "candles", "level_1"],
+    table: DataType,
     start: Optional[datetime.datetime] = None,
     end: Optional[datetime.datetime] = None,
     symbols: Optional[List[str]] = None,
     exchanges: Optional[List[str]] = None,
     *,
     bucket: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
@@ -140,20 +142,22 @@
         df.rename(columns={"amount": "quantity"}, inplace=True)
     if "receipt_timestamp" in df.columns:
         df.rename(columns={"receipt_timestamp": "received_time"}, inplace=True)
         df["received_time"] = pd.to_datetime(df["received_time"], unit="ns", cache=True)
     if "timestamp" in df.columns:
         df.rename(columns={"timestamp": "origin_time"}, inplace=True)
         df["origin_time"] = pd.to_datetime(df["origin_time"], unit="ns", cache=True)
+    if "next_funding_time" in df.columns:
+        df["next_funding_time"] = pd.to_datetime(df["next_funding_time"], unit="s", cache=True)
     if table == "trades":
         df.rename(columns={"id": "trade_id"}, inplace=True)
     return df
 
 def list_data(
-    table: Literal["book", "trades", "candles", "level_1", None],
+    table: Optional[DataType],
     start: Optional[datetime.datetime] = None,
     end: Optional[datetime.datetime] = None,
     symbols: Optional[List[str]] = None,
     exchanges: Optional[List[str]] = None,
     *,
     bucket: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
@@ -217,15 +221,15 @@
         'exchange': exchange.lstrip('exchange='),
         'symbol': symbol.lstrip('symbol='),
         'dt': dt.lstrip('dt='),
         'filename': filename,
     }
 
 def available_symbols(
-    table: Literal["book", "trades", "candles", "level_1", None],
+    table: Optional[DataType],
     exchanges: Optional[List[str]] = None,
     *,
     bucket: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ):
     '''
     Return pd.Series containing count of days available for exchange-symbol combinations.
```

### Comparing `lakeapi-0.4.5/lakeapi.egg-info/PKG-INFO` & `lakeapi-0.5.0/lakeapi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: lakeapi
-Version: 0.4.5
+Version: 0.5.0
 Summary: API for accessing Lake crypto market data
-Home-page: https://github.com/crypto-lake/lakeapi
+Home-page: https://github.com/crypto-lake/lake-api
 Author: Jan Skoda
 Author-email: skoda@jskoda.cz
 License: Apache 2 license
 Keywords: lakeapi
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -37,15 +38,15 @@
 .. image:: https://github.com/crypto-lake/lake-api/actions/workflows/dev.yml/badge.svg
      :target: https://github.com/crypto-lake/lake-api/actions/workflows/dev.yml
      :alt: Build status
 
 
 API for accessing Lake crypto market data.
 
-Lake is a service providing historical cryptocurrency market data in high detail, including `order book data <https://crypto-lake.com/order-book-data/>`_, tick trades and 1m trade candles. It is tuned for convenient quant and machine-learning purposes and so offers high performance, caching and parallelization.
+Lake is a service providing `historical cryptocurrency market data <https://crypto-lake.com/>`_ in high detail, including `order book data <https://crypto-lake.com/order-book-data/>`_, tick trades and 1m trade candles. It is tuned for convenient quant and machine-learning purposes and so offers high performance, caching and parallelization.
 
 
 * Web: https://crypto-lake.com/
 * Documentation: https://lake-api.readthedocs.io.
 * Online example -- executable collab notebook: https://colab.research.google.com/drive/1E7MSUT8xqYTMVLiq_rMBLNcZmI_KusK3
 
 
@@ -88,14 +89,20 @@
 working directory.
 
 
 =======
 History
 =======
 
+0.5.0 (2023-05-21)
+------------------
+
+* support for funding, open_interest and liquidations list_data
+* improve data type typing
+
 0.4.5 (2023-01-09)
 ------------------
 
 * grow default cache size limit from 3 GB to 10 GB
 
 0.4.3 (2022-12-09)
 ------------------
@@ -144,7 +151,9 @@
 
 * Python2.7 support and documentation improvements.
 
 0.1.0 (2022-10-08)
 ------------------
 
 * First release on PyPI.
+
+
```

### Comparing `lakeapi-0.4.5/lakeapi.egg-info/SOURCES.txt` & `lakeapi-0.5.0/lakeapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lakeapi-0.4.5/setup.py` & `lakeapi-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,11 +44,11 @@
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='lakeapi',
     name='lakeapi',
     packages=find_packages(include=['lakeapi', 'lakeapi.*']),
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/crypto-lake/lakeapi',
-    version='0.4.5',
+    url='https://github.com/crypto-lake/lake-api',
+    version='0.5.0',
     zip_safe=False,
 )
```

### Comparing `lakeapi-0.4.5/tests/test_lakeapi.py` & `lakeapi-0.5.0/tests/test_lakeapi.py`

 * *Files identical despite different names*

