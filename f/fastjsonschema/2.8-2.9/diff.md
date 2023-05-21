# Comparing `tmp/fastjsonschema-2.8.tar.gz` & `tmp/fastjsonschema-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastjsonschema-2.8.tar", last modified: Sat Jan  5 11:36:17 2019, max compression
+gzip compressed data, was "dist/fastjsonschema-2.9.tar", last modified: Mon Mar  4 09:31:42 2019, max compression
```

## Comparing `fastjsonschema-2.8.tar` & `fastjsonschema-2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2019-01-05 11:36:17.000000 fastjsonschema-2.8/
--rw-r--r--   0 michal    (1000) michal    (1000)      494 2018-10-04 17:03:48.000000 fastjsonschema-2.8/README.rst
--rw-r--r--   0 michal    (1000) michal    (1000)       38 2019-01-05 11:36:17.000000 fastjsonschema-2.8/setup.cfg
--rw-r--r--   0 michal    (1000) michal    (1000)     1547 2019-01-05 11:36:17.000000 fastjsonschema-2.8/PKG-INFO
-drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2019-01-05 11:36:17.000000 fastjsonschema-2.8/fastjsonschema/
--rw-r--r--   0 michal    (1000) michal    (1000)      390 2018-09-27 08:39:36.000000 fastjsonschema-2.8/fastjsonschema/exceptions.py
--rw-r--r--   0 michal    (1000) michal    (1000)      500 2018-07-21 07:35:38.000000 fastjsonschema-2.8/fastjsonschema/indent.py
--rw-r--r--   0 michal    (1000) michal    (1000)      312 2018-07-21 07:35:38.000000 fastjsonschema-2.8/fastjsonschema/__main__.py
--rw-r--r--   0 michal    (1000) michal    (1000)     5186 2018-09-14 14:57:30.000000 fastjsonschema-2.8/fastjsonschema/ref_resolver.py
--rw-r--r--   0 michal    (1000) michal    (1000)    26387 2019-01-05 11:32:44.000000 fastjsonschema-2.8/fastjsonschema/draft04.py
--rw-r--r--   0 michal    (1000) michal    (1000)     4257 2019-01-05 11:27:41.000000 fastjsonschema-2.8/fastjsonschema/draft07.py
--rw-r--r--   0 michal    (1000) michal    (1000)       16 2019-01-05 11:35:35.000000 fastjsonschema-2.8/fastjsonschema/version.py
--rw-r--r--   0 michal    (1000) michal    (1000)     7670 2019-01-05 11:27:41.000000 fastjsonschema-2.8/fastjsonschema/draft06.py
--rw-r--r--   0 michal    (1000) michal    (1000)     7676 2019-01-05 11:27:41.000000 fastjsonschema-2.8/fastjsonschema/__init__.py
--rw-r--r--   0 michal    (1000) michal    (1000)     9402 2018-09-14 14:57:30.000000 fastjsonschema-2.8/fastjsonschema/generator.py
-drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2019-01-05 11:36:17.000000 fastjsonschema-2.8/fastjsonschema.egg-info/
--rwxr-xr-x   0 michal    (1000) michal    (1000)       15 2019-01-05 11:36:16.000000 fastjsonschema-2.8/fastjsonschema.egg-info/top_level.txt
--rwxr-xr-x   0 michal    (1000) michal    (1000)      104 2019-01-05 11:36:16.000000 fastjsonschema-2.8/fastjsonschema.egg-info/requires.txt
--rwxr-xr-x   0 michal    (1000) michal    (1000)     1547 2019-01-05 11:36:16.000000 fastjsonschema-2.8/fastjsonschema.egg-info/PKG-INFO
--rwxr-xr-x   0 michal    (1000) michal    (1000)      479 2019-01-05 11:36:17.000000 fastjsonschema-2.8/fastjsonschema.egg-info/SOURCES.txt
--rwxr-xr-x   0 michal    (1000) michal    (1000)        1 2019-01-05 11:36:16.000000 fastjsonschema-2.8/fastjsonschema.egg-info/dependency_links.txt
--rw-r--r--   0 michal    (1000) michal    (1000)     1739 2018-08-25 14:08:29.000000 fastjsonschema-2.8/setup.py
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2019-03-04 09:31:42.000000 fastjsonschema-2.9/
+-rw-r--r--   0 michal    (1000) michal    (1000)      494 2018-10-04 17:03:48.000000 fastjsonschema-2.9/README.rst
+-rw-r--r--   0 michal    (1000) michal    (1000)       38 2019-03-04 09:31:42.000000 fastjsonschema-2.9/setup.cfg
+-rw-r--r--   0 michal    (1000) michal    (1000)     1547 2019-03-04 09:31:42.000000 fastjsonschema-2.9/PKG-INFO
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2019-03-04 09:31:42.000000 fastjsonschema-2.9/fastjsonschema/
+-rw-r--r--   0 michal    (1000) michal    (1000)      390 2018-09-27 08:39:36.000000 fastjsonschema-2.9/fastjsonschema/exceptions.py
+-rw-r--r--   0 michal    (1000) michal    (1000)      500 2018-07-21 07:35:38.000000 fastjsonschema-2.9/fastjsonschema/indent.py
+-rw-r--r--   0 michal    (1000) michal    (1000)      312 2018-07-21 07:35:38.000000 fastjsonschema-2.9/fastjsonschema/__main__.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     5011 2019-03-04 09:29:00.000000 fastjsonschema-2.9/fastjsonschema/ref_resolver.py
+-rw-r--r--   0 michal    (1000) michal    (1000)    26387 2019-01-05 11:32:44.000000 fastjsonschema-2.9/fastjsonschema/draft04.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     4257 2019-01-05 11:27:41.000000 fastjsonschema-2.9/fastjsonschema/draft07.py
+-rw-r--r--   0 michal    (1000) michal    (1000)       16 2019-03-04 09:29:24.000000 fastjsonschema-2.9/fastjsonschema/version.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     7670 2019-01-05 11:27:41.000000 fastjsonschema-2.9/fastjsonschema/draft06.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     7676 2019-01-05 11:27:41.000000 fastjsonschema-2.9/fastjsonschema/__init__.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     9402 2018-09-14 14:57:30.000000 fastjsonschema-2.9/fastjsonschema/generator.py
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2019-03-04 09:31:42.000000 fastjsonschema-2.9/fastjsonschema.egg-info/
+-rwxr-xr-x   0 michal    (1000) michal    (1000)       15 2019-03-04 09:31:42.000000 fastjsonschema-2.9/fastjsonschema.egg-info/top_level.txt
+-rwxr-xr-x   0 michal    (1000) michal    (1000)       95 2019-03-04 09:31:42.000000 fastjsonschema-2.9/fastjsonschema.egg-info/requires.txt
+-rwxr-xr-x   0 michal    (1000) michal    (1000)     1547 2019-03-04 09:31:42.000000 fastjsonschema-2.9/fastjsonschema.egg-info/PKG-INFO
+-rwxr-xr-x   0 michal    (1000) michal    (1000)      479 2019-03-04 09:31:42.000000 fastjsonschema-2.9/fastjsonschema.egg-info/SOURCES.txt
+-rwxr-xr-x   0 michal    (1000) michal    (1000)        1 2019-03-04 09:31:42.000000 fastjsonschema-2.9/fastjsonschema.egg-info/dependency_links.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)     1688 2019-03-04 09:29:00.000000 fastjsonschema-2.9/setup.py
```

### Comparing `fastjsonschema-2.8/PKG-INFO` & `fastjsonschema-2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastjsonschema
-Version: 2.8
+Version: 2.9
 Summary: Fastest Python implementation of JSON schema
 Home-page: https://github.com/seznam/python-fastjsonschema
 Author: Michal Horejsek
 Author-email: horejsekmichal@gmail.com
 License: BSD
 Description: ===========================
         Fast JSON schema for Python
```

### Comparing `fastjsonschema-2.8/fastjsonschema/ref_resolver.py` & `fastjsonschema-2.9/fastjsonschema/ref_resolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import contextlib
 import json
 import re
 from urllib import parse as urlparse
 from urllib.parse import unquote
 from urllib.request import urlopen
 
-import requests
 
 from .exceptions import JsonSchemaException
 
 
 def resolve_path(schema, fragment):
     """
     Return definition from path.
@@ -43,29 +42,24 @@
 
 def resolve_remote(uri, handlers):
     """
     Resolve a remote ``uri``.
 
     .. note::
 
-        Requests_ library is used to fetch ``http`` or ``https``
-        requests from the remote ``uri``, if handlers does not
-        define otherwise.
-
-        For unknown schemes urlib is used with UTF-8 encoding.
-
-    .. _Requests: http://pypi.python.org/pypi/requests/
+        urllib library is used to fetch requests from the remote ``uri``
+        if handlers does notdefine otherwise.
     """
     scheme = urlparse.urlsplit(uri).scheme
     if scheme in handlers:
         result = handlers[scheme](uri)
-    elif scheme in ['http', 'https']:
-        result = requests.get(uri).json()
     else:
-        result = json.loads(urlopen(uri).read().decode('utf-8'))
+        req = urlopen(uri)
+        encoding = req.info().get_content_charset() or 'utf-8'
+        result = json.loads(req.read().decode(encoding),)
     return result
 
 
 class RefResolver:
     """
     Resolve JSON References.
     """
```

### Comparing `fastjsonschema-2.8/fastjsonschema/draft04.py` & `fastjsonschema-2.9/fastjsonschema/draft04.py`

 * *Files identical despite different names*

### Comparing `fastjsonschema-2.8/fastjsonschema/draft07.py` & `fastjsonschema-2.9/fastjsonschema/draft07.py`

 * *Files identical despite different names*

### Comparing `fastjsonschema-2.8/fastjsonschema/draft06.py` & `fastjsonschema-2.9/fastjsonschema/draft06.py`

 * *Files identical despite different names*

### Comparing `fastjsonschema-2.8/fastjsonschema/__init__.py` & `fastjsonschema-2.9/fastjsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `fastjsonschema-2.8/fastjsonschema/generator.py` & `fastjsonschema-2.9/fastjsonschema/generator.py`

 * *Files identical despite different names*

### Comparing `fastjsonschema-2.8/fastjsonschema.egg-info/PKG-INFO` & `fastjsonschema-2.9/fastjsonschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastjsonschema
-Version: 2.8
+Version: 2.9
 Summary: Fastest Python implementation of JSON schema
 Home-page: https://github.com/seznam/python-fastjsonschema
 Author: Michal Horejsek
 Author-email: horejsekmichal@gmail.com
 License: BSD
 Description: ===========================
         Fast JSON schema for Python
```

### Comparing `fastjsonschema-2.8/setup.py` & `fastjsonschema-2.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,14 @@
     exec(open('fastjsonschema/version.py').read())
 
 
 setup(
     name='fastjsonschema',
     version=VERSION,
     packages=['fastjsonschema'],
-
-    install_requires=[
-        'requests',
-    ],
     extras_require={
         'devel': [
             'colorama',
             'jsonschema',
             'json-spec',
             'pylint',
             'pytest',
```

