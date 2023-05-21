# Comparing `tmp/migdalor-0.0.2.dev7.tar.gz` & `tmp/migdalor-0.0.2.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migdalor-0.0.2.dev7.tar", last modified: Sun May 21 11:39:24 2023, max compression
+gzip compressed data, was "migdalor-0.0.2.dev8.tar", last modified: Sun May 21 12:37:04 2023, max compression
```

## Comparing `migdalor-0.0.2.dev7.tar` & `migdalor-0.0.2.dev8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      682 2023-05-21 08:55:51.058971 migdalor-0.0.2.dev7/README.md
--rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev7/migdalor/__init__.py
--rw-r--r--   0        0        0     4155 2023-05-21 11:38:40.102180 migdalor-0.0.2.dev7/migdalor/cluster.py
--rw-r--r--   0        0        0     1323 2023-05-21 10:07:17.573969 migdalor-0.0.2.dev7/migdalor/discovery.py
--rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev7/migdalor/logger.py
--rw-r--r--   0        0        0      641 2023-05-21 11:39:24.538468 migdalor-0.0.2.dev7/pyproject.toml
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev7/PKG-INFO
+-rw-r--r--   0        0        0      682 2023-05-21 08:55:51.058971 migdalor-0.0.2.dev8/README.md
+-rw-r--r--   0        0        0      307 2023-05-14 18:33:53.946539 migdalor-0.0.2.dev8/migdalor/__init__.py
+-rw-r--r--   0        0        0     4029 2023-05-21 12:08:19.109239 migdalor-0.0.2.dev8/migdalor/cluster.py
+-rw-r--r--   0        0        0     1323 2023-05-21 10:07:17.573969 migdalor-0.0.2.dev8/migdalor/discovery.py
+-rw-r--r--   0        0        0       55 2023-05-14 12:39:17.992829 migdalor-0.0.2.dev8/migdalor/logger.py
+-rw-r--r--   0        0        0      641 2023-05-21 12:37:04.353762 migdalor-0.0.2.dev8/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 migdalor-0.0.2.dev8/PKG-INFO
```

### Comparing `migdalor-0.0.2.dev7/README.md` & `migdalor-0.0.2.dev8/README.md`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev7/migdalor/cluster.py` & `migdalor-0.0.2.dev8/migdalor/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,17 @@
             "updating cluster nodes",
             extra={"current": current_nodes, "prev": previous_other_nodes},
         )
 
         added_nodes = current_nodes - previous_other_nodes
         removed_nodes = previous_other_nodes - current_nodes
 
-        self._other_nodes = current_nodes
-
-        try:
-            async with self._nodes_updated:
-                self._nodes_updated.notify_all()
-        except RuntimeError:
-            # no one was waiting for the lock and that's fine
-            pass
+        async with self._nodes_updated:
+            self._other_nodes = current_nodes
+            self._nodes_updated.notify_all()
 
         if added_nodes:
             await self._on_nodes_added(added_nodes)
 
         if removed_nodes:
             await self._on_nodes_removed(removed_nodes)
```

### Comparing `migdalor-0.0.2.dev7/migdalor/discovery.py` & `migdalor-0.0.2.dev8/migdalor/discovery.py`

 * *Files identical despite different names*

### Comparing `migdalor-0.0.2.dev7/pyproject.toml` & `migdalor-0.0.2.dev8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "migdalor"
-version = "0.0.2.dev7"
+version = "0.0.2.dev8"
 description = "A cluster membership library for modern asyncio Python distributed systems running in Kubernetes"
 authors = [
     { name = "Roman Glushko", email = "roman.glushko.m@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.9"
 readme = "README.md"
```

### Comparing `migdalor-0.0.2.dev7/PKG-INFO` & `migdalor-0.0.2.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migdalor
-Version: 0.0.2.dev7
+Version: 0.0.2.dev8
 Summary: A cluster membership library for modern asyncio Python distributed systems running in Kubernetes
 Author-Email: Roman Glushko <roman.glushko.m@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <p align="center">
```

