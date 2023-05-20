# Comparing `tmp/wsgi_lithium-0.2.0.tar.gz` & `tmp/wsgi_lithium-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsgi_lithium-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wsgi_lithium-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wsgi_lithium-0.2.0.tar` & `wsgi_lithium-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4336 2023-05-20 02:37:14.064353 wsgi_lithium-0.2.0/.gitignore
--rw-r--r--   0        0        0     1079 2023-05-20 02:26:08.402988 wsgi_lithium-0.2.0/LICENSE
--rw-r--r--   0        0        0      360 2023-05-20 19:06:01.544901 wsgi_lithium-0.2.0/README.md
--rw-r--r--   0        0        0      583 2023-05-20 19:05:18.592720 wsgi_lithium-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2576 2023-05-20 19:03:23.456212 wsgi_lithium-0.2.0/wsgi_lithium/__init__.py
--rw-r--r--   0        0        0     5993 2023-05-20 19:03:13.100164 wsgi_lithium-0.2.0/wsgi_lithium/gunicorn_utils.py
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 wsgi_lithium-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4336 2023-05-20 02:37:14.064353 wsgi_lithium-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1079 2023-05-20 02:26:08.402988 wsgi_lithium-0.3.0/LICENSE
+-rw-r--r--   0        0        0      857 2023-05-20 23:17:19.717554 wsgi_lithium-0.3.0/README.md
+-rw-r--r--   0        0        0      583 2023-05-20 23:18:34.251975 wsgi_lithium-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2938 2023-05-20 23:11:45.791778 wsgi_lithium-0.3.0/wsgi_lithium/__init__.py
+-rw-r--r--   0        0        0     5993 2023-05-20 19:03:13.100164 wsgi_lithium-0.3.0/wsgi_lithium/gunicorn_utils.py
+-rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 wsgi_lithium-0.3.0/PKG-INFO
```

### Comparing `wsgi_lithium-0.2.0/.gitignore` & `wsgi_lithium-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wsgi_lithium-0.2.0/LICENSE` & `wsgi_lithium-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wsgi_lithium-0.2.0/pyproject.toml` & `wsgi_lithium-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "wsgi_lithium"
 authors = [{name = "Léo El Amri", email = "leo@superlel.me"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
-version = "0.2.0"
+version = "0.3.0"
 description = "An HTTP to WSGI server that relies on Python's included batteries"
 readme = "README.md"
 requires-python = ">=3.7"
 
 [project.urls]
 repository = "https://github.com/lel-amri/wsgi-lithium"
```

### Comparing `wsgi_lithium-0.2.0/wsgi_lithium/__init__.py` & `wsgi_lithium-0.3.0/wsgi_lithium/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 import getopt
 from typing import Any, NoReturn, Union
 import socket
 import sys
-from wsgiref.simple_server import WSGIServer, WSGIRequestHandler
+from wsgiref.simple_server import WSGIServer, WSGIRequestHandler as WSGIRequestHandler_
 from .gunicorn_utils import import_app, parse_address, is_ipv6
 
 
 class WSGIServer6(WSGIServer):
     address_family = socket.AF_INET6
 
 
+class WSGIRequestHandler(WSGIRequestHandler_):
+    def get_environ(self) -> None:
+        env = super().get_environ()
+        virtual_location = self.headers.get('virtual-location')
+        if virtual_location is not None:
+            env["SCRIPT_NAME"] = virtual_location
+            del env["HTTP_VIRTUAL_LOCATION"]
+        return env
+
+
 USAGE: str = """\
 Usage: {name:s} [-b ADDRESS | --bind ADDRESS] APPLICATION
 
 ADDRESS:
     A string in HOST:PORT format, where HOST is a valid IP address and PORT is a
     valid TCP port.
```

### Comparing `wsgi_lithium-0.2.0/wsgi_lithium/gunicorn_utils.py` & `wsgi_lithium-0.3.0/wsgi_lithium/gunicorn_utils.py`

 * *Files identical despite different names*

