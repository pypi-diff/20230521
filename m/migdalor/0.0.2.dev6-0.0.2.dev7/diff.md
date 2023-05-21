# Comparing `tmp/migdalor-0.0.2.dev6.tar.gz` & `tmp/migdalor-0.0.2.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migdalor-0.0.2.dev6.tar", last modified: Sun May 21 11:13:59 2023, max compression
+gzip compressed data, was "migdalor-0.0.2.dev7.tar", last modified: Sun May 21 11:39:24 2023, max compression
```

## Comparing `migdalor-0.0.2.dev6.tar` & `migdalor-0.0.2.dev7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      682 2023-05-21 08:55:51.058971 migdalor-0.0.2.dev6/README.md
--rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev6/migdalor/__init__.py
--rw-r--r--   0        0        0     4107 2023-05-21 11:10:21.832492 migdalor-0.0.2.dev6/migdalor/cluster.py
--rw-r--r--   0        0        0     1323 2023-05-21 10:07:17.573969 migdalor-0.0.2.dev6/migdalor/discovery.py
--rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev6/migdalor/logger.py
--rw-r--r--   0        0        0      641 2023-05-21 11:13:59.605126 migdalor-0.0.2.dev6/pyproject.toml
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev6/PKG-INFO
+-rw-r--r--   0        0        0      682 2023-05-21 08:55:51.058971 migdalor-0.0.2.dev7/README.md
+-rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev7/migdalor/__init__.py
+-rw-r--r--   0        0        0     4155 2023-05-21 11:38:40.102180 migdalor-0.0.2.dev7/migdalor/cluster.py
+-rw-r--r--   0        0        0     1323 2023-05-21 10:07:17.573969 migdalor-0.0.2.dev7/migdalor/discovery.py
+-rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev7/migdalor/logger.py
+-rw-r--r--   0        0        0      641 2023-05-21 11:39:24.538468 migdalor-0.0.2.dev7/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev7/PKG-INFO
```

### Comparing `migdalor-0.0.2.dev6/README.md` & `migdalor-0.0.2.dev7/README.md`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev6/migdalor/cluster.py` & `migdalor-0.0.2.dev7/migdalor/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,16 @@
 
         added_nodes = current_nodes - previous_other_nodes
         removed_nodes = previous_other_nodes - current_nodes
 
         self._other_nodes = current_nodes
 
         try:
-            self._nodes_updated.notify_all()
+            async with self._nodes_updated:
+                self._nodes_updated.notify_all()
         except RuntimeError:
             # no one was waiting for the lock and that's fine
             pass
 
         if added_nodes:
             await self._on_nodes_added(added_nodes)
```

### Comparing `migdalor-0.0.2.dev6/migdalor/discovery.py` & `migdalor-0.0.2.dev7/migdalor/discovery.py`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev6/pyproject.toml` & `migdalor-0.0.2.dev7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "migdalor"
-version = "0.0.2.dev6"
+version = "0.0.2.dev7"
 description = "A cluster membership library for modern asyncio Python distributed systems running in Kubernetes"
 authors = [
     { name = "Roman Glushko", email = "roman.glushko.m@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.9"
 readme = "README.md"
```

### Comparing `migdalor-0.0.2.dev6/PKG-INFO` & `migdalor-0.0.2.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migdalor
-Version: 0.0.2.dev6
+Version: 0.0.2.dev7
 Summary: A cluster membership library for modern asyncio Python distributed systems running in Kubernetes
 Author-Email: Roman Glushko <roman.glushko.m@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <p align="center">
```

