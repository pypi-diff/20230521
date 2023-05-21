# Comparing `tmp/migdalor-0.0.2.dev3.tar.gz` & `tmp/migdalor-0.0.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migdalor-0.0.2.dev3.tar", last modified: Sun May 21 10:03:45 2023, max compression
+gzip compressed data, was "migdalor-0.0.2.dev4.tar", last modified: Sun May 21 10:07:38 2023, max compression
```

## Comparing `migdalor-0.0.2.dev3.tar` & `migdalor-0.0.2.dev4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      682 2023-05-21 08:55:51.058971 migdalor-0.0.2.dev3/README.md
--rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev3/migdalor/__init__.py
--rw-r--r--   0        0        0     3790 2023-05-20 20:12:37.723054 migdalor-0.0.2.dev3/migdalor/cluster.py
--rw-r--r--   0        0        0     1324 2023-05-21 10:03:01.929340 migdalor-0.0.2.dev3/migdalor/discovery.py
--rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev3/migdalor/logger.py
--rw-r--r--   0        0        0      641 2023-05-21 10:03:45.543125 migdalor-0.0.2.dev3/pyproject.toml
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev3/PKG-INFO
+-rw-r--r--   0        0        0      682 2023-05-21 08:55:51.058971 migdalor-0.0.2.dev4/README.md
+-rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev4/migdalor/__init__.py
+-rw-r--r--   0        0        0     3790 2023-05-20 20:12:37.723054 migdalor-0.0.2.dev4/migdalor/cluster.py
+-rw-r--r--   0        0        0     1323 2023-05-21 10:07:17.573969 migdalor-0.0.2.dev4/migdalor/discovery.py
+-rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev4/migdalor/logger.py
+-rw-r--r--   0        0        0      641 2023-05-21 10:07:38.329014 migdalor-0.0.2.dev4/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev4/PKG-INFO
```

### Comparing `migdalor-0.0.2.dev3/README.md` & `migdalor-0.0.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev3/migdalor/cluster.py` & `migdalor-0.0.2.dev4/migdalor/cluster.py`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev3/migdalor/discovery.py` & `migdalor-0.0.2.dev4/migdalor/discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import socket
 
 from migdalor.logger import logger
 
-RawNodeAddress = tuple[socket.AddressFamily, socket.SocketKind, str, int, tuple[str, int]]
+RawNodeAddress = tuple[socket.AddressFamily, socket.SocketKind, int, str, tuple[str, int]]
 NodeAddress = tuple[str, int]
 
 
 class NodeDiscovery:
     async def get_all_nodes(self) -> set[NodeAddress]:
         raise NotImplementedError
 
@@ -28,15 +28,15 @@
             self._port,
             family=socket.AF_UNSPEC,
             type=socket.SOCK_STREAM,
         )
 
         logger.debug(f"raw node addresses ({raw_node_addresses})")
 
-        return {(ip, port) for _, _, ip, port, _ in raw_node_addresses}
+        return {address for _, _, _, _, address in raw_node_addresses}
 
 
 class StaticDiscovery(NodeDiscovery):
     """
     Use predefined static list of node addresses to discover. Useful for testing purposes mostly
     """
```

### Comparing `migdalor-0.0.2.dev3/pyproject.toml` & `migdalor-0.0.2.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "migdalor"
-version = "0.0.2.dev3"
+version = "0.0.2.dev4"
 description = "A cluster membership library for modern asyncio Python distributed systems running in Kubernetes"
 authors = [
     { name = "Roman Glushko", email = "roman.glushko.m@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.9"
 readme = "README.md"
```

### Comparing `migdalor-0.0.2.dev3/PKG-INFO` & `migdalor-0.0.2.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migdalor
-Version: 0.0.2.dev3
+Version: 0.0.2.dev4
 Summary: A cluster membership library for modern asyncio Python distributed systems running in Kubernetes
 Author-Email: Roman Glushko <roman.glushko.m@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <p align="center">
```

