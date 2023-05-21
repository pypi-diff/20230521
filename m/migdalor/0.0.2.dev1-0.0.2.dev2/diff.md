# Comparing `tmp/migdalor-0.0.2.dev1.tar.gz` & `tmp/migdalor-0.0.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migdalor-0.0.2.dev1.tar", last modified: Sun May 21 08:54:35 2023, max compression
+gzip compressed data, was "migdalor-0.0.2.dev2.tar", last modified: Sun May 21 09:38:58 2023, max compression
```

## Comparing `migdalor-0.0.2.dev1.tar` & `migdalor-0.0.2.dev2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      660 2023-05-21 08:51:55.408414 migdalor-0.0.2.dev1/README.md
--rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev1/migdalor/__init__.py
--rw-r--r--   0        0        0     3790 2023-05-20 20:12:37.723054 migdalor-0.0.2.dev1/migdalor/cluster.py
--rw-r--r--   0        0        0     1315 2023-05-20 20:15:53.901977 migdalor-0.0.2.dev1/migdalor/discovery.py
--rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev1/migdalor/logger.py
--rw-r--r--   0        0        0      545 2023-05-21 08:54:35.897140 migdalor-0.0.2.dev1/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev1/PKG-INFO
+-rw-r--r--   0        0        0      682 2023-05-21 08:55:51.058971 migdalor-0.0.2.dev2/README.md
+-rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev2/migdalor/__init__.py
+-rw-r--r--   0        0        0     3790 2023-05-20 20:12:37.723054 migdalor-0.0.2.dev2/migdalor/cluster.py
+-rw-r--r--   0        0        0     1220 2023-05-21 09:38:24.112979 migdalor-0.0.2.dev2/migdalor/discovery.py
+-rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev2/migdalor/logger.py
+-rw-r--r--   0        0        0      641 2023-05-21 09:38:58.740305 migdalor-0.0.2.dev2/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev2/PKG-INFO
```

### Comparing `migdalor-0.0.2.dev1/README.md` & `migdalor-0.0.2.dev2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <p align="center">
 <img src="https://github.com/roma-glushko/migdalor/blob/main/docs/imgs/logo-wide.png?raw=true" width="100%" alt="Migdalor - a Kubernetes native cluster management for modern Python>" />
 </p>
 
 # Migdalor
 
-Migdalor is a cluster membership library for modern asyncio Python distributed systems.
+Migdalor is a cluster membership library for modern asyncio Python distributed systems running in Kubernetes.
 
 Migdalor doesn't require a separate broker (e.g. Redis, etcd, Zookeeper, Chabby, etc) to work, but leverage Kubernetes out-of-the-box capabilities
 to solve the peer discovery problem.
 
 ## Features
 
 - Modern Asyncio Python 🐍
```

### Comparing `migdalor-0.0.2.dev1/migdalor/cluster.py` & `migdalor-0.0.2.dev2/migdalor/cluster.py`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev1/migdalor/discovery.py` & `migdalor-0.0.2.dev2/migdalor/discovery.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 import asyncio
 import socket
 
 RawNodeAddress = tuple[socket.AddressFamily, socket.SocketKind, str, int, tuple[str, int]]
 NodeAddress = tuple[str, int]
 
 
-def parse_address(service_address: str) -> NodeAddress:
-    # TODO: implement
-    ...
-
-
 class NodeDiscovery:
     async def get_all_nodes(self) -> set[NodeAddress]:
         raise NotImplementedError
 
 
 class KubernetesServiceDiscovery(NodeDiscovery):
     """
     Perform node discovery via the Kubernetes headless service
     """
 
-    def __init__(self, service_address: str) -> None:
-        self._hostname, self._port = parse_address(service_address)
+    def __init__(self, service_address: NodeAddress) -> None:
+        self._hostname, self._port = service_address
 
     async def get_all_nodes(self) -> set[NodeAddress]:
         loop = asyncio.get_running_loop()
 
         raw_node_addresses: list[RawNodeAddress] = await loop.getaddrinfo(
             self._hostname,
             self._port,
```

### Comparing `migdalor-0.0.2.dev1/pyproject.toml` & `migdalor-0.0.2.dev2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "migdalor"
-version = "0.0.2.dev1"
-description = ""
+version = "0.0.2.dev2"
+description = "A cluster membership library for modern asyncio Python distributed systems running in Kubernetes"
 authors = [
     { name = "Roman Glushko", email = "roman.glushko.m@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.9"
 readme = "README.md"
```

### Comparing `migdalor-0.0.2.dev1/PKG-INFO` & `migdalor-0.0.2.dev2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: migdalor
-Version: 0.0.2.dev1
+Version: 0.0.2.dev2
+Summary: A cluster membership library for modern asyncio Python distributed systems running in Kubernetes
 Author-Email: Roman Glushko <roman.glushko.m@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://github.com/roma-glushko/migdalor/blob/main/docs/imgs/logo-wide.png?raw=true" width="100%" alt="Migdalor - a Kubernetes native cluster management for modern Python>" />
 </p>
 
 # Migdalor
 
-Migdalor is a cluster membership library for modern asyncio Python distributed systems.
+Migdalor is a cluster membership library for modern asyncio Python distributed systems running in Kubernetes.
 
 Migdalor doesn't require a separate broker (e.g. Redis, etcd, Zookeeper, Chabby, etc) to work, but leverage Kubernetes out-of-the-box capabilities
 to solve the peer discovery problem.
 
 ## Features
 
 - Modern Asyncio Python 🐍
```

