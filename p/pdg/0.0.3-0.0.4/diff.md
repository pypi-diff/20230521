# Comparing `tmp/pdg-0.0.3.tar.gz` & `tmp/pdg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pdg-0.0.3.tar", last modified: Thu Oct 13 05:59:22 2022, max compression
+gzip compressed data, was "dist/pdg-0.0.4.tar", last modified: Sun May 21 19:43:32 2023, max compression
```

## Comparing `pdg-0.0.3.tar` & `pdg-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 jb        (1000) users      (100)        0 2022-10-13 05:59:22.000000 pdg-0.0.3/
--rw-r--r--   0 jb        (1000) users      (100)       18 2021-05-12 23:20:12.000000 pdg-0.0.3/LICENSE
--rw-r--r--   0 jb        (1000) users      (100)       21 2021-05-13 04:48:13.000000 pdg-0.0.3/MANIFEST.in
--rw-r--r--   0 jb        (1000) users      (100)     1340 2022-10-13 05:59:22.000000 pdg-0.0.3/PKG-INFO
--rw-r--r--   0 jb        (1000) users      (100)      469 2022-10-13 05:43:46.000000 pdg-0.0.3/README.md
-drwxr-xr-x   0 jb        (1000) users      (100)        0 2022-10-13 05:59:22.000000 pdg-0.0.3/pdg/
--rw-r--r--   0 jb        (1000) users      (100)     1012 2022-10-13 05:47:35.000000 pdg-0.0.3/pdg/__init__.py
--rw-r--r--   0 jb        (1000) users      (100)     2403 2022-10-13 01:20:25.000000 pdg-0.0.3/pdg/api.py
--rw-r--r--   0 jb        (1000) users      (100)     3588 2022-02-22 00:32:01.000000 pdg-0.0.3/pdg/data.py
--rw-r--r--   0 jb        (1000) users      (100)      200 2022-02-21 06:51:04.000000 pdg-0.0.3/pdg/errors.py
--rw-r--r--   0 jb        (1000) users      (100)     2297 2022-02-21 22:10:10.000000 pdg-0.0.3/pdg/particle.py
--rw-r--r--   0 jb        (1000) users      (100)  1814528 2022-10-13 04:24:32.000000 pdg-0.0.3/pdg/pdg.sqlite
--rw-r--r--   0 jb        (1000) users      (100)      390 2022-02-21 00:40:58.000000 pdg-0.0.3/pdg/utils.py
-drwxr-xr-x   0 jb        (1000) users      (100)        0 2022-10-13 05:59:22.000000 pdg-0.0.3/pdg.egg-info/
--rw-r--r--   0 jb        (1000) users      (100)     1340 2022-10-13 05:59:22.000000 pdg-0.0.3/pdg.egg-info/PKG-INFO
--rw-r--r--   0 jb        (1000) users      (100)      269 2022-10-13 05:59:22.000000 pdg-0.0.3/pdg.egg-info/SOURCES.txt
--rw-r--r--   0 jb        (1000) users      (100)        1 2022-10-13 05:59:22.000000 pdg-0.0.3/pdg.egg-info/dependency_links.txt
--rw-r--r--   0 jb        (1000) users      (100)       11 2022-10-13 05:59:22.000000 pdg-0.0.3/pdg.egg-info/requires.txt
--rw-r--r--   0 jb        (1000) users      (100)        4 2022-10-13 05:59:22.000000 pdg-0.0.3/pdg.egg-info/top_level.txt
--rw-r--r--   0 jb        (1000) users      (100)       38 2022-10-13 05:59:22.000000 pdg-0.0.3/setup.cfg
--rw-r--r--   0 jb        (1000) users      (100)     1660 2022-10-13 05:47:35.000000 pdg-0.0.3/setup.py
+drwxr-xr-x   0 jb        (1000) users      (100)        0 2023-05-21 19:43:32.000000 pdg-0.0.4/
+-rw-r--r--   0 jb        (1000) users      (100)     2490 2023-04-18 00:36:31.000000 pdg-0.0.4/LICENSE.txt
+-rw-r--r--   0 jb        (1000) users      (100)       25 2023-05-21 19:11:59.000000 pdg-0.0.4/MANIFEST.in
+-rw-r--r--   0 jb        (1000) users      (100)     1284 2023-05-21 19:43:32.000000 pdg-0.0.4/PKG-INFO
+-rw-r--r--   0 jb        (1000) users      (100)      469 2023-05-21 18:51:03.000000 pdg-0.0.4/README.md
+drwxr-xr-x   0 jb        (1000) users      (100)        0 2023-05-21 19:43:32.000000 pdg-0.0.4/pdg/
+-rw-r--r--   0 jb        (1000) users      (100)     1157 2023-05-20 00:02:21.000000 pdg-0.0.4/pdg/__init__.py
+-rw-r--r--   0 jb        (1000) users      (100)    11843 2023-05-20 00:32:21.000000 pdg-0.0.4/pdg/api.py
+-rw-r--r--   0 jb        (1000) users      (100)    17068 2023-05-19 03:19:19.000000 pdg-0.0.4/pdg/data.py
+-rw-r--r--   0 jb        (1000) users      (100)      912 2023-05-14 03:00:02.000000 pdg-0.0.4/pdg/decay.py
+-rw-r--r--   0 jb        (1000) users      (100)      601 2023-05-19 02:24:13.000000 pdg-0.0.4/pdg/errors.py
+-rw-r--r--   0 jb        (1000) users      (100)    11476 2023-05-19 03:56:47.000000 pdg-0.0.4/pdg/particle.py
+-rw-r--r--   0 jb        (1000) users      (100)  4534272 2023-05-21 19:06:53.000000 pdg-0.0.4/pdg/pdg.sqlite
+-rw-r--r--   0 jb        (1000) users      (100)      987 2023-05-14 00:32:20.000000 pdg-0.0.4/pdg/units.py
+-rw-r--r--   0 jb        (1000) users      (100)     3006 2023-05-19 02:32:23.000000 pdg-0.0.4/pdg/utils.py
+drwxr-xr-x   0 jb        (1000) users      (100)        0 2023-05-21 19:43:32.000000 pdg-0.0.4/pdg.egg-info/
+-rw-r--r--   0 jb        (1000) users      (100)     1284 2023-05-21 19:43:32.000000 pdg-0.0.4/pdg.egg-info/PKG-INFO
+-rw-r--r--   0 jb        (1000) users      (100)      299 2023-05-21 19:43:32.000000 pdg-0.0.4/pdg.egg-info/SOURCES.txt
+-rw-r--r--   0 jb        (1000) users      (100)        1 2023-05-21 19:43:32.000000 pdg-0.0.4/pdg.egg-info/dependency_links.txt
+-rw-r--r--   0 jb        (1000) users      (100)       16 2023-05-21 19:43:32.000000 pdg-0.0.4/pdg.egg-info/requires.txt
+-rw-r--r--   0 jb        (1000) users      (100)        4 2023-05-21 19:43:32.000000 pdg-0.0.4/pdg.egg-info/top_level.txt
+-rw-r--r--   0 jb        (1000) users      (100)       38 2023-05-21 19:43:32.000000 pdg-0.0.4/setup.cfg
+-rw-r--r--   0 jb        (1000) users      (100)     1610 2023-05-20 00:25:06.000000 pdg-0.0.4/setup.py
```

### Comparing `pdg-0.0.3/PKG-INFO` & `pdg-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pdg
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python API for accessing PDG data
 Home-page: https://pdg.lbl.gov
 Author: Particle Data Group
 Author-email: jberinger@lbl.gov
-License: To be determined.
+License: Modified BSD
 Description: Python API to access PDG data
         =============================
         
         The Python package pdg provides access to the particle physics data
         published by the  Particle Data Group (PDG) in the
         *Review of Particle Physics*.
         For general information about PDG and the *Review of Particle Physics*
@@ -17,18 +17,17 @@
         
         **Please note: This package is still under active development. The
         data provided by the present version should not be used in
         scientific publications.**
         
 Keywords: PDG,particle physics
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
```

### Comparing `pdg-0.0.3/pdg/__init__.py` & `pdg-0.0.4/pdg/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
 Python API to access PDG data.
 
 The Python package pdg provides access to the particle physics data
-published by the  Particle Data Group (PDG) in the Review of Particle Physics.
+published by the Particle Data Group (PDG) in the Review of Particle Physics.
 For general information about PDG and the Review of Particle Physics
 please visit https://pdg.lbl.gov.
-
-PLEASE NOTE: This package is still under active development and the
-data provided by the present version should not be used in scientific publications.
 """
 __author__ = 'Particle Data Group'
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 
 
 import os
 from pdg.api import PdgApi
+from pdg.errors import PdgApiError
 
 
 # Constants
 SQLITE_FILENAME = 'pdg.sqlite'      # Default SQLite database file used by this API
-MIN_SCHEMA_VERSION = 0.0            # Minimum schema version required by this version of the API
+MIN_SCHEMA_VERSION = 0.1            # Minimum schema version required by this version of the API
 
 
-def connect(database_url=None):
+def connect(database_url=None, pedantic=False):
     """Connect to PDG database and return configured PDG API object."""
     if database_url is None:
-        return PdgApi('sqlite:///%s' % os.path.join(os.path.dirname(__file__), SQLITE_FILENAME))
+        api = PdgApi('sqlite:///%s' % os.path.join(os.path.dirname(__file__), SQLITE_FILENAME), pedantic)
     else:
-        return PdgApi(database_url)
+        api = PdgApi(database_url, pedantic)
+    schema_version = float(api.info('schema_version'))
+    if schema_version < MIN_SCHEMA_VERSION:
+        raise PdgApiError('database schema v%s too old - need at least v%s' % (schema_version, MIN_SCHEMA_VERSION))
+    return api
```

### Comparing `pdg-0.0.3/pdg.egg-info/PKG-INFO` & `pdg-0.0.4/pdg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pdg
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python API for accessing PDG data
 Home-page: https://pdg.lbl.gov
 Author: Particle Data Group
 Author-email: jberinger@lbl.gov
-License: To be determined.
+License: Modified BSD
 Description: Python API to access PDG data
         =============================
         
         The Python package pdg provides access to the particle physics data
         published by the  Particle Data Group (PDG) in the
         *Review of Particle Physics*.
         For general information about PDG and the *Review of Particle Physics*
@@ -17,18 +17,17 @@
         
         **Please note: This package is still under active development. The
         data provided by the present version should not be used in
         scientific publications.**
         
 Keywords: PDG,particle physics
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
```

### Comparing `pdg-0.0.3/setup.py` & `pdg-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,33 +15,32 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setup(
     name = 'pdg',
-    version = '0.0.3',
+    version = '0.0.4',
     author = 'Particle Data Group',
     author_email = 'jberinger@lbl.gov',
     description = 'Python API for accessing PDG data',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://pdg.lbl.gov',
-    license = 'To be determined.',
+    license = 'Modified BSD',
     packages = find_packages(),
     package_data={"pdg": ["pdg.sqlite"]},
-    install_requires = ['SQLAlchemy'],
+    install_requires = ['SQLAlchemy>=1.4'],
     classifiers = [
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Topic :: Database :: Front-Ends',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Physics'
         ],
     keywords = 'PDG, particle physics',
     cmdclass={
         'register': register,
```

