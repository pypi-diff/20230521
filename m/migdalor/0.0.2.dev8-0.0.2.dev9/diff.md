# Comparing `tmp/migdalor-0.0.2.dev8.tar.gz` & `tmp/migdalor-0.0.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migdalor-0.0.2.dev8.tar", last modified: Sun May 21 12:37:04 2023, max compression
+gzip compressed data, was "migdalor-0.0.2.dev9.tar", last modified: Sun May 21 14:09:54 2023, max compression
```

## Comparing `migdalor-0.0.2.dev8.tar` & `migdalor-0.0.2.dev9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      682 2023-05-21 08:55:51.058971 migdalor-0.0.2.dev8/README.md
--rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev8/migdalor/__init__.py
--rw-r--r--   0        0        0     4029 2023-05-21 12:08:19.109239 migdalor-0.0.2.dev8/migdalor/cluster.py
--rw-r--r--   0        0        0     1323 2023-05-21 10:07:17.573969 migdalor-0.0.2.dev8/migdalor/discovery.py
--rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev8/migdalor/logger.py
--rw-r--r--   0        0        0      641 2023-05-21 12:37:04.353762 migdalor-0.0.2.dev8/pyproject.toml
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev8/PKG-INFO
+-rw-r--r--   0        0        0      682 2023-05-21 08:55:51.058971 migdalor-0.0.2.dev9/README.md
+-rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev9/migdalor/__init__.py
+-rw-r--r--   0        0        0     4328 2023-05-21 14:08:58.439808 migdalor-0.0.2.dev9/migdalor/cluster.py
+-rw-r--r--   0        0        0     1319 2023-05-21 13:47:46.833402 migdalor-0.0.2.dev9/migdalor/discovery.py
+-rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev9/migdalor/logger.py
+-rw-r--r--   0        0        0      641 2023-05-21 14:09:54.807198 migdalor-0.0.2.dev9/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev9/PKG-INFO
```

### Comparing `migdalor-0.0.2.dev8/README.md` & `migdalor-0.0.2.dev9/README.md`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev8/migdalor/cluster.py` & `migdalor-0.0.2.dev9/migdalor/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,22 +75,29 @@
 
     async def _update_nodes_periodically(self, updates_every_secs: float) -> None:
         # init the node list as soon as possible
         await self._update_nodes()
 
         while True:
             try:
-                await self._update_nodes()
                 await asyncio.sleep(updates_every_secs)
+                await self._update_nodes()
             except asyncio.CancelledError:
+                logger.debug("update cluster task canceled")
                 return
 
     async def _update_nodes(self) -> None:
         current_nodes = await self._discovery.get_all_nodes()
-        current_nodes.remove(self._node_address)
+
+        try:
+            current_nodes.remove(self._node_address)
+        except KeyError:
+            # if self IP is not on the list, then it's fine
+            # there is no guarantees that, for example, Kubernetes would update its DNS before the node is starting up
+            ...
 
         previous_other_nodes = self._other_nodes
 
         logger.debug("update cluster", extra={"current": current_nodes, "previous": previous_other_nodes})
 
         logger.debug(
             "updating cluster nodes",
```

### Comparing `migdalor-0.0.2.dev8/migdalor/discovery.py` & `migdalor-0.0.2.dev9/migdalor/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import socket
 
 from migdalor.logger import logger
 
-RawNodeAddress = tuple[socket.AddressFamily, socket.SocketKind, int, str, tuple[str, int]]
 NodeAddress = tuple[str, int]
+RawNodeAddress = tuple[socket.AddressFamily, socket.SocketKind, int, str, NodeAddress]
 
 
 class NodeDiscovery:
     async def get_all_nodes(self) -> set[NodeAddress]:
         raise NotImplementedError
```

### Comparing `migdalor-0.0.2.dev8/pyproject.toml` & `migdalor-0.0.2.dev9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "migdalor"
-version = "0.0.2.dev8"
+version = "0.0.2.dev9"
 description = "A cluster membership library for modern asyncio Python distributed systems running in Kubernetes"
 authors = [
     { name = "Roman Glushko", email = "roman.glushko.m@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.9"
 readme = "README.md"
```

### Comparing `migdalor-0.0.2.dev8/PKG-INFO` & `migdalor-0.0.2.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migdalor
-Version: 0.0.2.dev8
+Version: 0.0.2.dev9
 Summary: A cluster membership library for modern asyncio Python distributed systems running in Kubernetes
 Author-Email: Roman Glushko <roman.glushko.m@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <p align="center">
```

