# Comparing `tmp/communica-0.2.1b1.tar.gz` & `tmp/communica-0.2.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communica-0.2.1b1.tar", last modified: Sun May 21 11:32:12 2023, max compression
+gzip compressed data, was "communica-0.2.1b2.tar", last modified: Sun May 21 11:43:54 2023, max compression
```

## Comparing `communica-0.2.1b1.tar` & `communica-0.2.1b2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 11:32:12.007991 communica-0.2.1b1/
--rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.1b1/LICENSE.txt
--rw-rw-rw-   0        0        0     2233 2023-05-21 11:32:12.007491 communica-0.2.1b1/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.1b1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 11:32:11.982992 communica-0.2.1b1/communica/
--rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.1b1/communica/__init__.py
--rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.1b1/communica/clients.py
-drwxrwxrwx   0        0        0        0 2023-05-21 11:32:11.993993 communica-0.2.1b1/communica/connectors/
--rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.1b1/communica/connectors/__init__.py
--rw-rw-rw-   0        0        0     2803 2023-03-24 12:30:50.000000 communica-0.2.1b1/communica/connectors/_stream_local.py
--rw-rw-rw-   0        0        0     5455 2023-05-01 12:51:49.000000 communica-0.2.1b1/communica/connectors/base.py
--rw-rw-rw-   0        0        0    28038 2023-05-08 07:38:53.000000 communica-0.2.1b1/communica/connectors/rabbitmq.py
--rw-rw-rw-   0        0        0    10130 2023-05-04 12:12:20.000000 communica-0.2.1b1/communica/connectors/stream.py
--rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.1b1/communica/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-21 11:32:11.997993 communica-0.2.1b1/communica/pairs/
--rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.1b1/communica/pairs/__init__.py
--rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.1b1/communica/pairs/base.py
--rw-rw-rw-   0        0        0     9588 2023-05-08 10:26:04.000000 communica-0.2.1b1/communica/pairs/route.py
--rw-rw-rw-   0        0        0    16081 2023-05-08 10:15:06.000000 communica-0.2.1b1/communica/pairs/simple.py
-drwxrwxrwx   0        0        0        0 2023-05-21 11:32:12.002492 communica-0.2.1b1/communica/serializers/
--rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.1b1/communica/serializers/__init__.py
--rw-rw-rw-   0        0        0     1274 2023-05-09 20:44:57.000000 communica-0.2.1b1/communica/serializers/adaptix.py
--rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.2.1b1/communica/serializers/base.py
--rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.1b1/communica/serializers/json.py
--rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.1b1/communica/servers.py
--rw-rw-rw-   0        0        0     4246 2023-05-08 07:38:20.000000 communica-0.2.1b1/communica/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-21 11:32:11.989492 communica-0.2.1b1/communica.egg-info/
--rw-rw-rw-   0        0        0     2233 2023-05-21 11:32:11.000000 communica-0.2.1b1/communica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      811 2023-05-21 11:32:11.000000 communica-0.2.1b1/communica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 11:32:11.000000 communica-0.2.1b1/communica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-21 11:32:11.000000 communica-0.2.1b1/communica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-21 11:32:11.000000 communica-0.2.1b1/communica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1130 2023-05-21 11:31:45.000000 communica-0.2.1b1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 11:32:12.008491 communica-0.2.1b1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 11:32:12.005992 communica-0.2.1b1/tests/
--rw-rw-rw-   0        0        0     2146 2023-05-04 12:13:21.000000 communica-0.2.1b1/tests/test_connectors.py
--rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.1b1/tests/test_entities.py
--rw-rw-rw-   0        0        0     2481 2023-04-23 14:30:49.000000 communica-0.2.1b1/tests/test_rmq_conn_check_policy.py
--rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.1b1/tests/test_serializers.py
+drwxrwxrwx   0        0        0        0 2023-05-21 11:43:54.701376 communica-0.2.1b2/
+-rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.1b2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2233 2023-05-21 11:43:54.700877 communica-0.2.1b2/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.1b2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 11:43:54.680376 communica-0.2.1b2/communica/
+-rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.1b2/communica/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.1b2/communica/clients.py
+drwxrwxrwx   0        0        0        0 2023-05-21 11:43:54.689877 communica-0.2.1b2/communica/connectors/
+-rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.1b2/communica/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-05-21 11:38:53.000000 communica-0.2.1b2/communica/connectors/_stream_local.py
+-rw-rw-rw-   0        0        0     5455 2023-05-01 12:51:49.000000 communica-0.2.1b2/communica/connectors/base.py
+-rw-rw-rw-   0        0        0    28038 2023-05-08 07:38:53.000000 communica-0.2.1b2/communica/connectors/rabbitmq.py
+-rw-rw-rw-   0        0        0    10130 2023-05-21 11:36:08.000000 communica-0.2.1b2/communica/connectors/stream.py
+-rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.1b2/communica/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-21 11:43:54.692376 communica-0.2.1b2/communica/pairs/
+-rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.1b2/communica/pairs/__init__.py
+-rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.1b2/communica/pairs/base.py
+-rw-rw-rw-   0        0        0     9588 2023-05-08 10:26:04.000000 communica-0.2.1b2/communica/pairs/route.py
+-rw-rw-rw-   0        0        0    16081 2023-05-08 10:15:06.000000 communica-0.2.1b2/communica/pairs/simple.py
+drwxrwxrwx   0        0        0        0 2023-05-21 11:43:54.696876 communica-0.2.1b2/communica/serializers/
+-rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.1b2/communica/serializers/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-05-09 20:44:57.000000 communica-0.2.1b2/communica/serializers/adaptix.py
+-rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.2.1b2/communica/serializers/base.py
+-rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.1b2/communica/serializers/json.py
+-rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.1b2/communica/servers.py
+-rw-rw-rw-   0        0        0     4246 2023-05-08 07:38:20.000000 communica-0.2.1b2/communica/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-21 11:43:54.685876 communica-0.2.1b2/communica.egg-info/
+-rw-rw-rw-   0        0        0     2233 2023-05-21 11:43:54.000000 communica-0.2.1b2/communica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      811 2023-05-21 11:43:54.000000 communica-0.2.1b2/communica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 11:43:54.000000 communica-0.2.1b2/communica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-21 11:43:54.000000 communica-0.2.1b2/communica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-21 11:43:54.000000 communica-0.2.1b2/communica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1130 2023-05-21 11:43:46.000000 communica-0.2.1b2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 11:43:54.701376 communica-0.2.1b2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 11:43:54.700376 communica-0.2.1b2/tests/
+-rw-rw-rw-   0        0        0     2146 2023-05-04 12:13:21.000000 communica-0.2.1b2/tests/test_connectors.py
+-rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.1b2/tests/test_entities.py
+-rw-rw-rw-   0        0        0     2481 2023-04-23 14:30:49.000000 communica-0.2.1b2/tests/test_rmq_conn_check_policy.py
+-rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.1b2/tests/test_serializers.py
```

### Comparing `communica-0.2.1b1/LICENSE.txt` & `communica-0.2.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/PKG-INFO` & `communica-0.2.1b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.2.1b1
+Version: 0.2.1b2
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.2.1b1/README.md` & `communica-0.2.1b2/README.md`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica/connectors/_stream_local.py` & `communica-0.2.1b2/communica/connectors/_stream_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 
 
     async def open_connection(
             address: str
     ) -> 'tuple[asyncio.StreamReader, asyncio.StreamWriter]':
         loop = asyncio.get_event_loop()
         if not hasattr(loop, 'create_pipe_connection'):
-            raise TypeError('Named pipes are not supported')
+            raise TypeError('Named pipes are not supported on current platform')
 
         reader = asyncio.StreamReader(loop=loop)
         protocol = asyncio.StreamReaderProtocol(reader, loop=loop)
         transport, _ = await loop.create_pipe_connection(
             lambda: protocol, format_address(address))
         writer = asyncio.StreamWriter(transport, protocol, reader, loop)
         return reader, writer
 
     async def start_server(
             client_connected_cb, address: str
     ) -> asyncio.AbstractServer:
         loop = asyncio.get_event_loop()
         if not hasattr(loop, 'start_serving_pipe'):
-            raise TypeError('Named pipes are not supported')
+            raise TypeError('Named pipes are not supported on current platform')
 
         def factory():
             reader = asyncio.StreamReader(loop=loop)
             protocol = asyncio.StreamReaderProtocol(
                 reader, client_connected_cb, loop=loop)
             return protocol
 
@@ -67,15 +67,15 @@
     import tempfile
 
     SOCK_DIR = os.path.join(tempfile.gettempdir(), 'communica')
 
     async def open_connection(
             address: str
     ) -> 'tuple[asyncio.StreamReader, asyncio.StreamWriter]':
-        sock_path = os.path.join(SOCK_DIR, address)
+        sock_path = format_address(address)
         return await asyncio.open_unix_connection(sock_path)
 
     async def start_server(
             client_connected_cb, address: str
     ) -> asyncio.AbstractServer:
         sock_path = format_address(address)
         return await asyncio.start_unix_server(client_connected_cb, sock_path)
```

### Comparing `communica-0.2.1b1/communica/connectors/base.py` & `communica-0.2.1b2/communica/connectors/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica/connectors/rabbitmq.py` & `communica-0.2.1b2/communica/connectors/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica/connectors/stream.py` & `communica-0.2.1b2/communica/connectors/stream.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica/exceptions.py` & `communica-0.2.1b2/communica/exceptions.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica/pairs/base.py` & `communica-0.2.1b2/communica/pairs/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica/pairs/route.py` & `communica-0.2.1b2/communica/pairs/route.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica/pairs/simple.py` & `communica-0.2.1b2/communica/pairs/simple.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica/serializers/adaptix.py` & `communica-0.2.1b2/communica/serializers/adaptix.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica/serializers/base.py` & `communica-0.2.1b2/communica/serializers/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica/utils.py` & `communica-0.2.1b2/communica/utils.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/communica.egg-info/PKG-INFO` & `communica-0.2.1b2/communica.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.2.1b1
+Version: 0.2.1b2
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.2.1b1/communica.egg-info/SOURCES.txt` & `communica-0.2.1b2/communica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/pyproject.toml` & `communica-0.2.1b2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "communica"
-version = "0.2.1b1"
+version = "0.2.1b2"
 authors = [
   { name="Elchin Sarkarov", email="elchin751@gmail.com" },
 ]
 description = "Easy to use IPC library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `communica-0.2.1b1/tests/test_connectors.py` & `communica-0.2.1b2/tests/test_connectors.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/tests/test_entities.py` & `communica-0.2.1b2/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/tests/test_rmq_conn_check_policy.py` & `communica-0.2.1b2/tests/test_rmq_conn_check_policy.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b1/tests/test_serializers.py` & `communica-0.2.1b2/tests/test_serializers.py`

 * *Files identical despite different names*

