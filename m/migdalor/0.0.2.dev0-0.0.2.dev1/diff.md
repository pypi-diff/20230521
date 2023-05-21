# Comparing `tmp/migdalor-0.0.2.dev0.tar.gz` & `tmp/migdalor-0.0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migdalor-0.0.2.dev0.tar", last modified: Sun May 21 08:35:35 2023, max compression
+gzip compressed data, was "migdalor-0.0.2.dev1.tar", last modified: Sun May 21 08:54:35 2023, max compression
```

## Comparing `migdalor-0.0.2.dev0.tar` & `migdalor-0.0.2.dev1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      601 2023-05-10 19:50:56.807951 migdalor-0.0.2.dev0/README.md
--rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev0/migdalor/__init__.py
--rw-r--r--   0        0        0     3790 2023-05-20 20:12:37.723054 migdalor-0.0.2.dev0/migdalor/cluster.py
--rw-r--r--   0        0        0     1315 2023-05-20 20:15:53.901977 migdalor-0.0.2.dev0/migdalor/discovery.py
--rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev0/migdalor/logger.py
--rw-r--r--   0        0        0      544 2023-05-21 08:35:35.097836 migdalor-0.0.2.dev0/pyproject.toml
--rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0      660 2023-05-21 08:51:55.408414 migdalor-0.0.2.dev1/README.md
+-rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev1/migdalor/__init__.py
+-rw-r--r--   0        0        0     3790 2023-05-20 20:12:37.723054 migdalor-0.0.2.dev1/migdalor/cluster.py
+-rw-r--r--   0        0        0     1315 2023-05-20 20:15:53.901977 migdalor-0.0.2.dev1/migdalor/discovery.py
+-rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev1/migdalor/logger.py
+-rw-r--r--   0        0        0      545 2023-05-21 08:54:35.897140 migdalor-0.0.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev1/PKG-INFO
```

### Comparing `migdalor-0.0.2.dev0/README.md` & `migdalor-0.0.2.dev1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-<img src="/docs/imgs/logo-wide.png" width="100%" alt="Migdalor - a Kubernetes native cluster management for modern Python>" />
+<img src="https://github.com/roma-glushko/migdalor/blob/main/docs/imgs/logo-wide.png?raw=true" width="100%" alt="Migdalor - a Kubernetes native cluster management for modern Python>" />
 </p>
 
 # Migdalor
 
 Migdalor is a cluster membership library for modern asyncio Python distributed systems.
 
 Migdalor doesn't require a separate broker (e.g. Redis, etcd, Zookeeper, Chabby, etc) to work, but leverage Kubernetes out-of-the-box capabilities
```

### Comparing `migdalor-0.0.2.dev0/migdalor/cluster.py` & `migdalor-0.0.2.dev1/migdalor/cluster.py`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev0/migdalor/discovery.py` & `migdalor-0.0.2.dev1/migdalor/discovery.py`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev0/pyproject.toml` & `migdalor-0.0.2.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "migdalor"
-version = "0.0.2.dev"
+version = "0.0.2.dev1"
 description = ""
 authors = [
     { name = "Roman Glushko", email = "roman.glushko.m@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.9"
 readme = "README.md"
```

### Comparing `migdalor-0.0.2.dev0/PKG-INFO` & `migdalor-0.0.2.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: migdalor
-Version: 0.0.2.dev0
+Version: 0.0.2.dev1
 Author-Email: Roman Glushko <roman.glushko.m@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <p align="center">
-<img src="/docs/imgs/logo-wide.png" width="100%" alt="Migdalor - a Kubernetes native cluster management for modern Python>" />
+<img src="https://github.com/roma-glushko/migdalor/blob/main/docs/imgs/logo-wide.png?raw=true" width="100%" alt="Migdalor - a Kubernetes native cluster management for modern Python>" />
 </p>
 
 # Migdalor
 
 Migdalor is a cluster membership library for modern asyncio Python distributed systems.
 
 Migdalor doesn't require a separate broker (e.g. Redis, etcd, Zookeeper, Chabby, etc) to work, but leverage Kubernetes out-of-the-box capabilities
```

