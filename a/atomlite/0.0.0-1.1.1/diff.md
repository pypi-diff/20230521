# Comparing `tmp/atomlite-0.0.0.tar.gz` & `tmp/atomlite-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomlite-0.0.0.tar", last modified: Sun May  7 23:18:05 2023, max compression
+gzip compressed data, was "atomlite-1.1.1.tar", last modified: Sun May 21 13:52:44 2023, max compression
```

## Comparing `atomlite-0.0.0.tar` & `atomlite-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 23:18:05.597263 atomlite-0.0.0/
--rw-r--r--   0 root         (0) root         (0)      277 2023-05-07 23:18:05.597263 atomlite-0.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1084 2023-05-07 23:15:57.000000 atomlite-0.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 23:18:05.597263 atomlite-0.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 23:18:05.593263 atomlite-0.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 23:18:05.593263 atomlite-0.0.0/src/atomlite/
--rw-rw-r--   0 root         (0) root         (0)      410 2023-05-07 23:15:57.000000 atomlite-0.0.0/src/atomlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 23:18:05.597263 atomlite-0.0.0/src/atomlite/_internal/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-07 23:15:57.000000 atomlite-0.0.0/src/atomlite/_internal/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7721 2023-05-07 23:15:57.000000 atomlite-0.0.0/src/atomlite/_internal/database.py
--rw-rw-r--   0 root         (0) root         (0)     5618 2023-05-07 23:15:57.000000 atomlite-0.0.0/src/atomlite/_internal/json.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-07 23:15:57.000000 atomlite-0.0.0/src/atomlite/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 23:18:05.593263 atomlite-0.0.0/src/atomlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)      277 2023-05-07 23:18:05.000000 atomlite-0.0.0/src/atomlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      364 2023-05-07 23:18:05.000000 atomlite-0.0.0/src/atomlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 23:18:05.000000 atomlite-0.0.0/src/atomlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-07 23:18:05.000000 atomlite-0.0.0/src/atomlite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-07 23:18:05.000000 atomlite-0.0.0/src/atomlite.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 23:18:05.597263 atomlite-0.0.0/tests/
--rw-rw-r--   0 root         (0) root         (0)     8089 2023-05-07 23:15:57.000000 atomlite-0.0.0/tests/test_database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:52:44.874645 atomlite-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      277 2023-05-21 13:52:44.874645 atomlite-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-05-21 13:52:31.000000 atomlite-1.1.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-05-21 13:52:31.000000 atomlite-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 13:52:44.874645 atomlite-1.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:52:44.870645 atomlite-1.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:52:44.870645 atomlite-1.1.1/src/atomlite/
+-rw-r--r--   0 root         (0) root         (0)      410 2023-05-21 13:52:31.000000 atomlite-1.1.1/src/atomlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:52:44.874645 atomlite-1.1.1/src/atomlite/_internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-21 13:52:31.000000 atomlite-1.1.1/src/atomlite/_internal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8351 2023-05-21 13:52:31.000000 atomlite-1.1.1/src/atomlite/_internal/database.py
+-rw-r--r--   0 root         (0) root         (0)     5618 2023-05-21 13:52:31.000000 atomlite-1.1.1/src/atomlite/_internal/json.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-21 13:52:31.000000 atomlite-1.1.1/src/atomlite/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:52:44.870645 atomlite-1.1.1/src/atomlite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      277 2023-05-21 13:52:44.000000 atomlite-1.1.1/src/atomlite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      375 2023-05-21 13:52:44.000000 atomlite-1.1.1/src/atomlite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 13:52:44.000000 atomlite-1.1.1/src/atomlite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-21 13:52:44.000000 atomlite-1.1.1/src/atomlite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-21 13:52:44.000000 atomlite-1.1.1/src/atomlite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:52:44.874645 atomlite-1.1.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-05-21 13:52:31.000000 atomlite-1.1.1/tests/test_database.py
```

### Comparing `atomlite-0.0.0/pyproject.toml` & `atomlite-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
+requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atomlite"
 maintainers = [
   { name = "Lukas Turcani", email = "lukasturcani93@gmail.com" },
 ]
@@ -36,14 +36,17 @@
 documentation = "https://atomlite.readthedocs.io"
 
 [tool.setuptools.package-data]
 atomlite = [
   "py.typed",
 ]
 
+[tool.setuptools_scm]
+fallback_version = "0.0.0"
+
 [tool.ruff]
 line-length = 79
 extend-select = ["I"]
 
 [tool.black]
 line-length = 79
```

### Comparing `atomlite-0.0.0/src/atomlite/_internal/database.py` & `atomlite-1.1.1/src/atomlite/_internal/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -118,47 +118,57 @@
             "molecule JSON NOT NULL, "
             "properties JSON NOT NULL)",
         )
 
     def add_entries(
         self,
         entries: Entry | collections.abc.Iterable[Entry],
+        commit: bool = True,
     ) -> None:
         """
         Add molecular entries to the database.
 
         Parameters:
             entries (Entry | list[Entry]):
                 The molecules to add to the database.
+            commit:
+                If ``True`` changes will be automatically
+                commited to the database file.
         """
         if isinstance(entries, Entry):
             entries = (entries,)
 
         self.connection.executemany(
             f"INSERT INTO {self._molecule_table} "
             "VALUES (:key, :molecule, :properties)",
             map(_entry_to_sqlite, entries),
         )
+        if commit:
+            self.connection.commit()
 
     def update_entries(
         self,
         entries: Entry | collections.abc.Iterable[Entry],
         merge_properties: bool = True,
+        commit: bool = True,
     ) -> None:
         """
         Update molecules in the database.
 
         Parameters:
             entries (Entry | list[Entry]):
                 The molecule entries to update in the database.
             merge_properties:
                 If ``True``, the molecular properties will be
                 merged rather than replaced. Properties present
                 in both the update and the database will be
                 overwritten.
+            commit:
+                If ``True`` changes will be automatically
+                commited to the database file.
         """
         if isinstance(entries, Entry):
             entries = (entries,)
 
         if merge_properties:
             self.connection.executemany(
                 f"UPDATE {self._molecule_table} "
@@ -170,14 +180,16 @@
         else:
             self.connection.executemany(
                 f"UPDATE {self._molecule_table} "
                 "SET molecule=:molecule, properties=:properties "
                 "WHERE key=:key",
                 map(_entry_to_sqlite, entries),
             )
+        if commit:
+            self.connection.commit()
 
     def get_entries(
         self,
         keys: str | collections.abc.Iterable[str] | None = None,
     ) -> "DatabaseGetMolecules":
         """
         Get molecular entries from the database.
@@ -223,26 +235,30 @@
                 properties=json.loads(properties),
             )
 
     def update_properties(
         self,
         entries: PropertyEntry | collections.abc.Iterable[PropertyEntry],
         merge_properties: bool = True,
+        commit: bool = True,
     ) -> None:
         """
         Update molecular properties.
 
         Parameters:
             entries (Entry | list[Entry]):
                 The entries to update in the database.
             merge_properties:
                 If ``True``, the molecular properties will be
                 merged rather than replaced. Properties present
                 in both the update and the database will be
                 overwritten.
+            commit:
+                If ``True`` changes will be automatically
+                commited to the database file.
         """
         if isinstance(entries, PropertyEntry):
             entries = (entries,)
 
         if merge_properties:
             self.connection.executemany(
                 f"UPDATE {self._molecule_table} "
@@ -253,7 +269,9 @@
         else:
             self.connection.executemany(
                 f"UPDATE {self._molecule_table} "
                 "SET properties=:properties "
                 "WHERE key=:key",
                 map(_property_entry_to_sqlite, entries),
             )
+        if commit:
+            self.connection.commit()
```

### Comparing `atomlite-0.0.0/src/atomlite/_internal/json.py` & `atomlite-1.1.1/src/atomlite/_internal/json.py`

 * *Files identical despite different names*

### Comparing `atomlite-0.0.0/tests/test_database.py` & `atomlite-1.1.1/tests/test_database.py`

 * *Files identical despite different names*

