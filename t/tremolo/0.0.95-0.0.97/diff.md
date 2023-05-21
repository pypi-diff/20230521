# Comparing `tmp/tremolo-0.0.95.tar.gz` & `tmp/tremolo-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.95.tar", last modified: Mon May 15 04:17:18 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.97.tar", last modified: Sun May 21 09:14:48 2023, max compression
```

## Comparing `tremolo-0.0.95.tar` & `tremolo-0.0.97.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-15 04:17:18.000000 tremolo-0.0.95/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.95/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-15 04:17:18.000000 tremolo-0.0.95/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     4019 2023-05-15 04:15:11.000000 tremolo-0.0.95/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-15 04:17:18.000000 tremolo-0.0.95/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-15 04:14:43.000000 tremolo-0.0.95/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     5850 2023-05-14 00:12:56.000000 tremolo-0.0.95/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/contexts.py
--rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/__init__.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo/lib/h1parser/
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/h1parser/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/h1parser/parse_header.py
--rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13737 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     9307 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    11322 2023-05-12 01:18:27.000000 tremolo-0.0.95/tremolo/lib/http_response.py
--rw-r--r--   0 tux       (1000) users      (100)      844 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/object_pool.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-21 09:14:48.000000 tremolo-0.0.97/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.97/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-21 09:14:48.000000 tremolo-0.0.97/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     4019 2023-05-15 04:15:11.000000 tremolo-0.0.97/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-21 09:14:48.000000 tremolo-0.0.97/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-21 09:08:50.000000 tremolo-0.0.97/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     5666 2023-05-19 13:26:48.000000 tremolo-0.0.97/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/contexts.py
+-rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    10617 2023-05-19 14:03:18.000000 tremolo-0.0.97/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/lib/__init__.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo/lib/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/lib/h1parser/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/lib/h1parser/parse_header.py
+-rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13962 2023-05-21 09:10:36.000000 tremolo-0.0.97/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     9281 2023-05-19 23:50:26.000000 tremolo-0.0.97/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    11322 2023-05-20 00:56:10.000000 tremolo-0.0.97/tremolo/lib/http_response.py
+-rw-r--r--   0 tux       (1000) users      (100)      772 2023-05-19 07:52:08.000000 tremolo-0.0.97/tremolo/lib/object_pool.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-19 02:59:43.000000 tremolo-0.0.97/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.95/LICENSE.txt` & `tremolo-0.0.97/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/PKG-INFO` & `tremolo-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.95
+Version: 0.0.97
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tremolo-0.0.95/README.md` & `tremolo-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/setup.py` & `tremolo-0.0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/h1parser/*']},
-    version='0.0.95',
+    version='0.0.97',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.95/tremolo/__main__.py` & `tremolo-0.0.97/tremolo/__main__.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/asgi_lifespan.py` & `tremolo-0.0.97/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/asgi_server.py` & `tremolo-0.0.97/tremolo/asgi_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,50 +11,46 @@
 from .contexts import ServerContext
 from .exceptions import ExpectationFailed, InternalServerError
 from .lib.http_protocol import HTTPProtocol
 
 class ASGIServer(HTTPProtocol):
     def __init__(self, **kwargs):
         self._app = kwargs['_app']
-        self._request = None
-        self._response = None
         self._read = None
         self._task = None
         self._timer = None
         self._timeout = 30
 
         super().__init__(ServerContext(), **kwargs)
 
-    async def header_received(self, request, response):
-        if request.http_continue:
-            if request.content_length > self.options['client_max_body_size']:
+    async def header_received(self):
+        if self.request.http_continue:
+            if self.request.content_length > self.options['client_max_body_size']:
                 raise ExpectationFailed
 
-            await response.send(b'HTTP/%s 100 Continue\r\n\r\n' % request.version)
+            await self.response.send(b'HTTP/%s 100 Continue\r\n\r\n' % self.request.version)
 
         scope = {
             'type': 'http',
             'asgi': {'version': '3.0'},
-            'http_version': request.version.decode(encoding='utf-8'),
-            'method': request.method.decode(encoding='utf-8'),
+            'http_version': self.request.version.decode(encoding='utf-8'),
+            'method': self.request.method.decode(encoding='utf-8'),
             'scheme': {True: 'http',
-                       False: 'https'}[request.transport.get_extra_info('sslcontext') is None],
-            'path': unquote(request.path.decode(encoding='utf-8'), encoding='utf-8'),
-            'raw_path': request.path,
-            'query_string': request.query_string,
-            'headers': request.protocol.header.getheaders(),
-            'client': request.transport.get_extra_info('peername'),
-            'server': request.transport.get_extra_info('sockname')
+                       False: 'https'}[self.request.transport.get_extra_info('sslcontext') is None],
+            'path': unquote(self.request.path.decode(encoding='utf-8'), encoding='utf-8'),
+            'raw_path': self.request.path,
+            'query_string': self.request.query_string,
+            'headers': self.request.header.getheaders(),
+            'client': self.request.transport.get_extra_info('peername'),
+            'server': self.request.transport.get_extra_info('sockname')
         }
 
-        self._request = request
-        self._response = response
-        self._read = request.read(cache=False)
+        self._read = self.request.read(cache=False)
 
-        if not (b'transfer-encoding' in request.headers or b'content-length' in request.headers
+        if not (b'transfer-encoding' in self.request.headers or b'content-length' in self.request.headers
                 ) and self.queue[0] is not None:
             # avoid blocking on initial receive() due to empty Queue
             # in the case of bodyless requests, e.g. GET
             self.queue[0].put_nowait(b'')
 
         self._task = self.loop.create_task(self.app(scope))
 
@@ -69,74 +65,73 @@
             await self._app(scope, self.receive, self.send)
 
             if self._timer is not None:
                 self._timer.cancel()
         except asyncio.CancelledError:
             self.options['logger'].warning('task: ASGI application is cancelled due to timeout')
         except Exception as exc:
-            await self.handle_exception(InternalServerError(cause=exc), self._request, self._response)
+            await self.handle_exception(InternalServerError(cause=exc))
 
     async def receive(self):
         try:
             data = await self._read.__anext__()
 
             return {
                 'type': 'http.request',
                 'body': data,
-                'more_body': ((data != b'' and self._request.content_length == -1)
-                    or self._request.body_size < self._request.content_length)
+                'more_body': ((data != b'' and self.request.content_length == -1)
+                    or self.request.body_size < self.request.content_length)
             }
         except Exception as exc:
-            if not (self._request is None or isinstance(exc, StopAsyncIteration)):
+            if not (self.request is None or isinstance(exc, StopAsyncIteration)):
                 self.print_exception(exc)
 
             if self._timer is None:
                 self._timer = self.loop.call_at(self.loop.time() + self._timeout, self._task.cancel)
 
             return {'type': 'http.disconnect'}
 
     async def send(self, data):
         try:
             if data['type'] == 'http.response.start':
-                self._response.set_status(data['status'], HTTPStatus(data['status']).phrase)
-                self._response.append_header(b'Date: %s\r\nServer: %s\r\n' % (
-                                             datetime.utcnow().strftime('%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
-                                             self.options['server_name']))
+                self.response.set_status(data['status'], HTTPStatus(data['status']).phrase)
+                self.response.append_header(b'Date: %s\r\nServer: %s\r\n' % (
+                                            datetime.utcnow().strftime('%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
+                                            self.options['server_name']))
 
                 if 'headers' in data:
                     for header in data['headers']:
                         if not (header[0].find(b'\n') == -1 and header[1].find(b'\n') == -1):
                             await self.handle_exception(
-                                InternalServerError('name or value cannot contain illegal characters'),
-                                self._request, self._response)
+                                InternalServerError('name or value cannot contain illegal characters'))
                             return
 
                         name = header[0].lower()
 
                         if name == b'content-type':
-                            self._response.set_content_type(header[1])
+                            self.response.set_content_type(header[1])
                             continue
 
                         if name in (b'connection', b'date', b'server', b'transfer-encoding'):
                             # disallow apps from changing them, as they are managed by Tremolo
                             continue
 
                         if name == b'content-length':
-                            # will disable http chunked in the self._response.write()
-                            self._request.http_keepalive = False
+                            # will disable http chunked in the self.response.write()
+                            self.request.http_keepalive = False
 
                         if isinstance(header, list):
                             header = tuple(header)
 
-                        self._response.append_header(b'%s: %s\r\n' % header)
+                        self.response.append_header(b'%s: %s\r\n' % header)
             elif data['type'] == 'http.response.body':
                 if 'body' in data:
-                    await self._response.write(data['body'])
+                    await self.response.write(data['body'])
 
                 if 'more_body' not in data or data['more_body'] is False:
-                    await self._response.write(b'', throttle=False)
-                    await self._response.send(None)
+                    await self.response.write(b'', throttle=False)
+                    await self.response.send(None)
         except asyncio.CancelledError:
             pass
         except Exception as exc:
-            if not (self._request is None or self._response is None):
+            if not (self.request is None or self.response is None):
                 self.print_exception(exc)
```

### Comparing `tremolo-0.0.95/tremolo/contexts.py` & `tremolo-0.0.97/tremolo/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/exceptions.py` & `tremolo-0.0.97/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/lib/h1parser/parse_header.py` & `tremolo-0.0.97/tremolo/lib/h1parser/parse_header.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/lib/http_exception.py` & `tremolo-0.0.97/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/lib/http_protocol.py` & `tremolo-0.0.97/tremolo/lib/http_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2023 nggit
 
 import asyncio
 import traceback
 
 from datetime import datetime
 
+from .h1parser import ParseHeader
 from .http_exception import HTTPException, BadRequest, InternalServerError
 from .http_request import HTTPRequest
 from .http_response import HTTPResponse
 
 class HTTPProtocol(asyncio.Protocol):
     def __init__(self, context, **kwargs):
         self._context = context
@@ -17,15 +18,16 @@
         try:
             self._loop = kwargs['loop']
         except KeyError:
             self._loop = asyncio.get_event_loop()
 
         self._transport = None
         self._queue = (None, None)
-        self._header = None
+        self._request = None
+        self._response = None
         self._watermarks = {'high': 65536, 'low': 8192}
 
     @property
     def context(self):
         return self._context
 
     @property
@@ -45,29 +47,30 @@
         return self._transport
 
     @property
     def queue(self):
         return self._queue
 
     @property
-    def header(self):
-        return self._header
+    def request(self):
+        return self._request
+
+    @property
+    def response(self):
+        return self._response
 
     def connection_made(self, transport):
         self._transport = transport
         self._pool = self._options['_pool'].get()
         self._queue = self._pool['queue']
-        self._header = self._pool['header']
-        self._request = None
-        self._response = None
 
         self._data = bytearray()
-        self._timeout_waiters = {'request': self._loop.create_future()}
+        self._waiters = {'request': self._loop.create_future()}
 
-        for task in (self._send_data(), self.set_timeout(self._timeout_waiters['request'],
+        for task in (self._send_data(), self.set_timeout(self._waiters['request'],
                                                          timeout=self._options['request_timeout'],
                                                          timeout_cb=self.request_timeout)):
             self.tasks.append(self._loop.create_task(task))
 
     async def request_timeout(self, timeout):
         self._options['logger'].info('request timeout after {:g}s'.format(timeout))
 
@@ -122,27 +125,27 @@
             else:
                 if self._queue[1] is not None:
                     self._request.http_keepalive = False
                     self._queue[1].put_nowait(None)
 
                 self._options['logger'].info('payload too large')
 
-    async def header_received(self, request, response):
+    async def header_received(self):
         return
 
     def print_exception(self, exc, *args):
         self._options['logger'].error(': '.join(
             (*args, exc.__class__.__name__, str(exc))
         ), exc_info={True: exc, False: False}[self._options['debug']])
 
-    async def handle_exception(self, exc, request, response):
-        if request is None or response is None:
+    async def handle_exception(self, exc):
+        if self._request is None or self._response is None or self._response.header is None:
             return
 
-        self.print_exception(exc, request.path.decode(encoding='latin-1'))
+        self.print_exception(exc, self._request.path.decode(encoding='latin-1'))
 
         encoding = 'utf-8'
 
         for v in exc.content_type.split(';'):
             v = v.lstrip()
 
             if v.startswith('charset='):
@@ -156,39 +159,39 @@
         if self.options['debug']:
             data = b'<ul><li>%s</li></ul>' % '</li><li>'.join(
                 traceback.TracebackException.from_exception(exc).format()
             ).encode(encoding=encoding)
         else:
             data = str(exc).encode(encoding=encoding)
 
-        await response.send((
+        await self._response.send((
             b'HTTP/%s %d %s\r\nContent-Type: %s\r\nContent-Length: %d\r\nConnection: close\r\n' +
-            b'Date: %s\r\nServer: %s\r\n\r\n%s') % (request.version,
+            b'Date: %s\r\nServer: %s\r\n\r\n%s') % (self._request.version,
                                                     exc.code,
                                                     exc.message.encode(encoding='latin-1'),
                                                     exc.content_type.encode(encoding='latin-1'),
                                                     len(data),
                                                     datetime.utcnow().strftime(
                                                         '%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
                                                     self._options['server_name'],
                                                     data))
 
-        response.close()
+        self._response.close()
 
     async def _handle_request_header(self, data, header_size):
-        self._data = None
+        header = ParseHeader(data, header_size=header_size, excludes=[b'proxy'])
 
-        if not self._header.parse(data, header_size=header_size, excludes=[b'proxy']).is_request:
+        if not header.is_request:
             if self._queue[1] is not None:
                 self._queue[1].put_nowait(None)
 
             self._options['logger'].info('bad request: not a request')
             return
 
-        self._request = HTTPRequest(self)
+        self._request = HTTPRequest(self, header)
         self._response = HTTPResponse(self._request)
 
         try:
             if b'connection' in self._request.headers:
                 if self._request.headers[b'connection'].lower().find(b'close') == -1:
                     self._request.http_keepalive = True
             elif self._request.version == b'1.1':
@@ -217,55 +220,66 @@
                     self._request.http_continue = True
 
                 # the initial body that accompanies the header
                 await self.put_to_queue(
                     data[header_size + 4:], queue=self._queue[0], transport=self._transport, rate=self._options['upload_rate']
                 )
 
-            await self.header_received(self._request, self._response)
+            # successfully got header, clear either the request or keepalive timeout
+            for i in self._waiters:
+                if i in ('request', 'keepalive') and not self._waiters[i].done():
+                    self._waiters[i].set_result(None)
+
+            await self.header_received()
         except Exception as exc:
             if not isinstance(exc, HTTPException):
                 exc = InternalServerError(cause=exc)
 
-            await self.handle_exception(exc, self._request, self._response)
+            await self.handle_exception(exc)
+
+    async def _receive_data(self, data, waiter):
+        await waiter
+        await self.put_to_queue(data, queue=self._queue[0], transport=self._transport, rate=self._options['upload_rate'])
 
     def data_received(self, data):
+        if not data:
+            return
+
         if self._data is not None:
             self._data.extend(data)
             header_size = self._data.find(b'\r\n\r\n')
 
             if -1 < header_size <= 8192:
                 self._transport.pause_reading()
-
-                # got header, clear either the request or keepalive timeout
-                for i in self._timeout_waiters:
-                    if i != 'send' and not self._timeout_waiters[i].done():
-                        self._timeout_waiters[i].set_result(None)
-
                 self.tasks.append(self._loop.create_task(self._handle_request_header(self._data, header_size)))
+                self._data = None
             elif header_size > 8192:
                 self._options['logger'].info('request header too large')
                 self._transport.abort()
             elif not (header_size == -1 and len(self._data) <= 8192):
                 self._options['logger'].info('bad request')
                 self._transport.abort()
 
             return
 
         self._transport.pause_reading()
-        self._loop.create_task(
-            self.put_to_queue(data, queue=self._queue[0], transport=self._transport, rate=self._options['upload_rate'])
-        )
+
+        if 'receive' in self._waiters:
+            waiter = self._waiters['receive']
+        else:
+            waiter = self._waiters['request']
+
+        self._waiters['receive'] = self._loop.create_task(self._receive_data(data, waiter))
 
     def eof_received(self):
         self._queue[0].put_nowait(None)
 
     def resume_writing(self):
-        if 'send' in self._timeout_waiters and not self._timeout_waiters['send'].done():
-            self._timeout_waiters['send'].set_result(None)
+        if 'send' in self._waiters and not self._waiters['send'].done():
+            self._waiters['send'].set_result(None)
 
     def set_watermarks(self, high=65536, low=8192):
         if self._transport is not None:
             self._watermarks['high'] = high
             self._watermarks['low'] = low
 
             self._transport.set_write_buffer_limits(high=high, low=low)
@@ -296,51 +310,51 @@
 
                 if write_buffer_size > self._watermarks['high']:
                     self._options['logger'].info(
                         '{:d} exceeds the current watermark limits (high={:d}, low={:d})'.format(write_buffer_size,
                                                                                                  self._watermarks['high'],
                                                                                                  self._watermarks['low'])
                     )
-                    self._timeout_waiters['send'] = self._loop.create_future()
+                    self._waiters['send'] = self._loop.create_future()
 
-                    await self.set_timeout(self._timeout_waiters['send'], timeout_cb=self.send_timeout)
+                    await self.set_timeout(self._waiters['send'], timeout_cb=self.send_timeout)
 
                     if self._transport is None:
                         return
 
                 self._transport.write(data)
             except asyncio.CancelledError:
                 pass
             except Exception as exc:
                 if self._transport is not None:
                     self._transport.abort()
                     self.print_exception(exc)
 
     def _handle_keepalive(self):
-        for i, task in enumerate(self.tasks):
+        for task in self.tasks[:]:
             if callable(task):
                 continue
 
             try:
                 exc = task.exception()
 
                 if exc:
                     self.print_exception(exc)
 
-                del self.tasks[i]
+                self.tasks.remove(task)
             except asyncio.InvalidStateError:
                 pass
 
         if not self._request.http_continue:
             self._data = bytearray()
             self._request.clear_body()
 
-        self._timeout_waiters['keepalive'] = self._loop.create_future()
+        self._waiters['keepalive'] = self._loop.create_future()
 
-        self.tasks.append(self._loop.create_task(self.set_timeout(self._timeout_waiters['keepalive'],
+        self.tasks.append(self._loop.create_task(self.set_timeout(self._waiters['keepalive'],
                                                                   timeout=self._options['keepalive_timeout'],
                                                                   timeout_cb=self.keepalive_timeout)))
         self._transport.resume_reading()
 
     def connection_lost(self, exc):
         for task in self.tasks:
             if callable(task):
@@ -352,16 +366,15 @@
 
                 if exc:
                     self.print_exception(exc)
             except asyncio.InvalidStateError:
                 task.cancel()
 
         self._options['_pool'].put({
-            'queue': (asyncio.Queue(), asyncio.Queue()),
-            'header': self._header
+            'queue': (asyncio.Queue(), asyncio.Queue())
         })
 
         self._transport = None
         self._queue = (None, None)
         self._request = None
         self._response = None
         self._data = None
```

### Comparing `tremolo-0.0.95/tremolo/lib/http_request.py` & `tremolo-0.0.97/tremolo/lib/http_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 
 from urllib.parse import parse_qs, parse_qsl
 
 from .http_exception import BadRequest, PayloadTooLarge, RequestTimeout
 from .request import Request
 
 class HTTPRequest(Request):
-    def __init__(self, protocol):
+    def __init__(self, protocol, header):
         super().__init__(protocol)
 
-        self.is_valid = protocol.header.is_valid_request
-        self.headers = protocol.header.headers
-        self.host = protocol.header.gethost()
+        self.header = header
+        self.headers = header.headers
+        self.is_valid = header.is_valid_request
+        self.host = header.gethost()
 
         if isinstance(self.host, list):
             self.host = self.host[0]
 
-        self.method = protocol.header.getmethod().upper()
-        self.url = protocol.header.geturl()
+        self.method = header.getmethod().upper()
+        self.url = header.geturl()
         path_size = self.url.find(b'?')
 
         if path_size == -1:
             self.path = self.url
             self.query_string = b''
         else:
             self.path = self.url[:path_size]
             self.query_string = self.url[path_size + 1:]
 
-        self.version = protocol.header.getversion()
+        self.version = header.getversion()
 
         if self.version != b'1.0':
             self.version = b'1.1'
 
         self._content_length = -1
         self._content_type = b'application/octet-stream'
         self._transfer_encoding = b'none'
@@ -260,15 +261,15 @@
 
                     paused = False
                 else:
                     body = header[header_size + 4:]
                     info = {}
 
                     if header_size <= 8192 and header.startswith(b'--%s\r\n' % boundary):
-                        header = self.protocol.header.parse(header, header_size=header_size).getheaders()
+                        header = self.header.parse(header, header_size=header_size).getheaders()
 
                         if b'content-disposition' in header:
                             for k, v in parse_qsl(header[b'content-disposition']
                                     .replace(b'; ', b'&').replace(b';', b'&').decode(encoding='latin-1')):
                                 info[k] = v.strip('"')
 
                         if b'content-length' in header:
```

### Comparing `tremolo-0.0.95/tremolo/lib/http_response.py` & `tremolo-0.0.97/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/lib/object_pool.py` & `tremolo-0.0.97/tremolo/lib/object_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # Copyright (c) 2023 nggit
 
 import asyncio
 
-from .h1parser import ParseHeader
-
 class ObjectPool:
     def __init__(self, pool_size, logger):
         self._pool_size = pool_size
         self._pools = []
         self._logger = logger
 
         for _ in range(pool_size):
             self._pools.append(self._create())
 
     def _create(self):
         return {
-            'header': ParseHeader(),
             'queue': (asyncio.Queue(), asyncio.Queue())
         }
 
     def get(self):
         try:
             return self._pools.pop()
         except IndexError:
```

### Comparing `tremolo-0.0.95/tremolo/lib/request.py` & `tremolo-0.0.97/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/lib/response.py` & `tremolo-0.0.97/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/tremolo.py` & `tremolo-0.0.97/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.97/tremolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.95
+Version: 0.0.97
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tremolo-0.0.95/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.97/tremolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

