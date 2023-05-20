# Comparing `tmp/latch_postgres-0.1.8.tar.gz` & `tmp/latch_postgres-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_postgres-0.1.8.tar", max compression
+gzip compressed data, was "latch_postgres-0.1.9.tar", max compression
```

## Comparing `latch_postgres-0.1.8.tar` & `latch_postgres-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.8/LICENSE
--rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-10 16:20:18.720567 latch_postgres-0.1.8/latch_postgres/__init__.py
--rw-r--r--   0        0        0    24455 2023-05-19 02:39:34.353217 latch_postgres-0.1.8/latch_postgres/postgres.py
--rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.8/latch_postgres/py.typed
--rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.8/latch_postgres/retries.py
--rw-r--r--   0        0        0     1735 2023-05-19 02:39:36.113871 latch_postgres-0.1.8/latch_postgres/transactions.py
--rw-r--r--   0        0        0     1018 2023-05-19 02:40:06.887265 latch_postgres-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.8/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.9/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 16:20:18.720567 latch_postgres-0.1.9/latch_postgres/__init__.py
+-rw-r--r--   0        0        0    23835 2023-05-19 21:23:24.451349 latch_postgres-0.1.9/latch_postgres/postgres.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.9/latch_postgres/py.typed
+-rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.9/latch_postgres/retries.py
+-rw-r--r--   0        0        0     1735 2023-05-19 02:39:36.113871 latch_postgres-0.1.9/latch_postgres/transactions.py
+-rw-r--r--   0        0        0     1018 2023-05-19 21:24:22.397809 latch_postgres-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.9/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.9/PKG-INFO
```

### Comparing `latch_postgres-0.1.8/LICENSE` & `latch_postgres-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.8/latch_postgres/postgres.py` & `latch_postgres-0.1.9/latch_postgres/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,39 +280,24 @@
                     ):
                         await conn.query_opt(dict, cmd)
 
                 async def run_composite_setup():
                     with tracer.start_as_current_span(
                         "composite type setup",
                     ):
-                        composite_type_infos: list[CompositeInfo | None] = []
                         with tracer.start_as_current_span(
-                            "fetch composite type info",
+                            "register composite types",
                         ):
-                            composite_type_infos = await asyncio.gather(
-                                *[
-                                    CompositeInfo.fetch(conn, db_type)
-                                    for db_type in self.composite_type_map
-                                ]
-                            )
-
-                        for t, db_type in zip(
-                            composite_type_infos, self.composite_type_map
-                        ):
-                            with tracer.start_as_current_span(
-                                f"registering {db_type}",
-                            ):
-                                if t is None:
+                            for db_type, f in self.composite_type_map.items():
+                                type_info = await CompositeInfo.fetch(conn, db_type)
+                                if type_info is None:
                                     raise RuntimeError(
                                         f"failed to fetch composite info for {db_type}"
                                     )
-
-                                register_composite(
-                                    t, conn, self.composite_type_map[db_type]
-                                )
+                                register_composite(type_info, conn, f)
 
                 async def run_enum_setup():
                     with tracer.start_as_current_span(
                         "enum setup",
                     ):
                         with tracer.start_as_current_span(
                             "fetch type info",
```

### Comparing `latch_postgres-0.1.8/latch_postgres/retries.py` & `latch_postgres-0.1.9/latch_postgres/retries.py`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.8/latch_postgres/transactions.py` & `latch_postgres-0.1.9/latch_postgres/transactions.py`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.8/pyproject.toml` & `latch_postgres-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-postgres"
-version = "0.1.8"
+version = "0.1.9"
 description = "Postges wrapper for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_postgres"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_postgres-0.1.8/setup.py` & `latch_postgres-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'typing-extensions>=4.4.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'latch-postgres',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Postges wrapper for latch python backend services',
     'long_description': '# python-postgres\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_postgres-0.1.8/PKG-INFO` & `latch_postgres-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-postgres
-Version: 0.1.8
+Version: 0.1.9
 Summary: Postges wrapper for latch python backend services
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

