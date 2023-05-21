# Comparing `tmp/vhatable-1.0.1.tar.gz` & `tmp/vhatable-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhatable-1.0.1.tar", last modified: Sun Apr 23 17:45:48 2023, max compression
+gzip compressed data, was "vhatable-1.0.2.tar", last modified: Sun May 21 12:57:47 2023, max compression
```

## Comparing `vhatable-1.0.1.tar` & `vhatable-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-04-23 17:45:48.022043 vhatable-1.0.1/
--rw-r--r--   0 fred      (1000) fred      (1000)    35138 2022-01-30 18:20:55.000000 vhatable-1.0.1/LICENSE.txt
--rw-r--r--   0 fred      (1000) fred      (1000)      609 2023-04-23 17:45:48.018710 vhatable-1.0.1/PKG-INFO
--rw-r--r--   0 fred      (1000) fred      (1000)      336 2022-01-30 18:20:55.000000 vhatable-1.0.1/README.rst
--rw-r--r--   0 fred      (1000) fred      (1000)       38 2023-04-23 17:45:48.022043 vhatable-1.0.1/setup.cfg
--rwxr-xr-x   0 fred      (1000) fred      (1000)     2840 2022-01-15 02:09:48.000000 vhatable-1.0.1/setup.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-04-23 17:45:48.018710 vhatable-1.0.1/vhatable/
--rw-r--r--   0 fred      (1000) fred      (1000)      958 2023-04-23 15:34:37.000000 vhatable-1.0.1/vhatable/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9318 2023-04-23 15:34:41.000000 vhatable-1.0.1/vhatable/cell.py
--rw-r--r--   0 fred      (1000) fred      (1000)    22474 2023-04-23 15:34:37.000000 vhatable-1.0.1/vhatable/core.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6758 2023-04-23 15:39:49.000000 vhatable-1.0.1/vhatable/filters.py
--rw-r--r--   0 fred      (1000) fred      (1000)    20587 2023-04-23 15:37:15.000000 vhatable-1.0.1/vhatable/sample.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-04-23 17:45:48.018710 vhatable-1.0.1/vhatable.egg-info/
--rwxr-xr-x   0 fred      (1000) fred      (1000)      609 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/PKG-INFO
--rwxr-xr-x   0 fred      (1000) fred      (1000)      319 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/SOURCES.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)        1 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/dependency_links.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)       67 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/entry_points.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)       84 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/requires.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)        9 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/top_level.txt
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-05-21 12:57:47.292606 vhatable-1.0.2/
+-rw-r--r--   0 fred      (1000) fred      (1000)    35138 2022-01-30 18:20:55.000000 vhatable-1.0.2/LICENSE.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)      609 2023-05-21 12:57:47.292606 vhatable-1.0.2/PKG-INFO
+-rw-r--r--   0 fred      (1000) fred      (1000)      336 2022-01-30 18:20:55.000000 vhatable-1.0.2/README.rst
+-rw-r--r--   0 fred      (1000) fred      (1000)       38 2023-05-21 12:57:47.292606 vhatable-1.0.2/setup.cfg
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     2840 2022-01-15 02:09:48.000000 vhatable-1.0.2/setup.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-05-21 12:57:47.292606 vhatable-1.0.2/vhatable/
+-rw-r--r--   0 fred      (1000) fred      (1000)      958 2023-04-23 17:45:48.000000 vhatable-1.0.2/vhatable/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9318 2023-04-23 15:34:41.000000 vhatable-1.0.2/vhatable/cell.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    23243 2023-05-21 12:57:26.000000 vhatable-1.0.2/vhatable/core.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6758 2023-04-23 15:39:49.000000 vhatable-1.0.2/vhatable/filters.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    20587 2023-04-23 15:37:15.000000 vhatable-1.0.2/vhatable/sample.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-05-21 12:57:47.292606 vhatable-1.0.2/vhatable.egg-info/
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      609 2023-05-21 12:57:47.000000 vhatable-1.0.2/vhatable.egg-info/PKG-INFO
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      319 2023-05-21 12:57:47.000000 vhatable-1.0.2/vhatable.egg-info/SOURCES.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)        1 2023-05-21 12:57:47.000000 vhatable-1.0.2/vhatable.egg-info/dependency_links.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)       67 2023-05-21 12:57:47.000000 vhatable-1.0.2/vhatable.egg-info/entry_points.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)       84 2023-05-21 12:57:47.000000 vhatable-1.0.2/vhatable.egg-info/requires.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)        9 2023-05-21 12:57:47.000000 vhatable-1.0.2/vhatable.egg-info/top_level.txt
```

### Comparing `vhatable-1.0.1/LICENSE.txt` & `vhatable-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vhatable-1.0.1/PKG-INFO` & `vhatable-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vhatable
-Version: 1.0.1
+Version: 1.0.2
 Summary: vhatable.
 Home-page: https://github.com/fred49/vhatable
 Author: Frederic MARTIN
 Author-email: frederic.martin.fma@gmail.com
 License: GPL3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vhatable-1.0.1/setup.py` & `vhatable-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `vhatable-1.0.1/vhatable/__init__.py` & `vhatable-1.0.2/vhatable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 # Copyright 2014-2016 Frédéric MARTIN
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 # from .core import *
 from . import core
 from . import cell
 from . import filters
```

### Comparing `vhatable-1.0.1/vhatable/cell.py` & `vhatable-1.0.2/vhatable/cell.py`

 * *Files identical despite different names*

### Comparing `vhatable-1.0.1/vhatable/core.py` & `vhatable-1.0.2/vhatable/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
 
-
-
 import json
 import time
 import logging
 import logging.handlers
 
 from collections import OrderedDict
 from functools import wraps
@@ -95,15 +93,16 @@
     def filters(self, row, filters):
         """TODO"""
         if filters is not None:
             if isinstance(filters, list):
                 matches = 0
                 enabled_filters = 0
                 for func in filters:
-                    self.log.debug("filter: %s (enabled=%s)", func, func.is_enable())
+                    self.log.debug(
+                            "filter: %s (enabled=%s)", func, func.is_enable())
                     if func.is_enable():
                         enabled_filters += 1
                         if func(row):
                             matches += 1
                 self.log.debug("matches: %s", matches)
                 self.log.debug("enabled_filters: %s", enabled_filters)
                 if enabled_filters == 0:
@@ -341,15 +340,16 @@
         records = []
         classname = str(self.__class__.__name__.lower())
         self.log = logging.getLogger(classname)
         for row in self.get_raw():
             record = []
             for k in self.keys:
                 try:
-                    t_format = "{key:" + str(self._maxlengthkey) + "s} | {value:s}"
+                    slength = str(self._maxlengthkey)
+                    t_format = "{key:" + slength + "s} | {value:s}"
                     dataa = None
                     column_data = row.get(k)
                     if isinstance(column_data, str):
                         dataa = {"key": k, "value": column_data}
                     else:
                         column_data_str = str(column_data)
                         dataa = {"key": k, "value": column_data_str}
@@ -364,15 +364,16 @@
             records.append("\n".join(record))
         out = []
         cptline = 0
         for record in records:
             cptline += 1
             header = "-[ RECORD " + str(cptline) + " ]-"
             # pylint: disable=unused-variable
-            header += "".join(["-" for i in range(max_length_line - len(header))])
+            range_limit = max_length_line - len(header)
+            header += "".join(["-" for i in range(range_limit)])
             out.append(header)
             out.append(record)
         return "\n".join(out)
 
     def add_row(self, row):
         """TODO"""
         super().add_row(row)
@@ -437,15 +438,25 @@
             table.add_row(data)
         return table.get_string()
 
 
 class Action:
     """TODO"""
 
-    no_cell = True
+    # we must convert row to cells, otherwise filters won't work.
+    # Filters are expecting cells, not raw data.
+    # Changing from True to False  will break every already existing actions
+    versions = {1: {'no_cell': True}, 2: {'no_cell': False}}
+    # Default version will be 1 to avoid breaking changes.
+    version = 1
+
+    def __getattr__(self, attr):
+        if attr == "no_cell":
+            return self.versions[self.version][attr]
+        raise AttributeError(attr)
 
     def __init__(self):
         self.cli_mode = False
         self.verbose = False
         self.dry_run = False
         self.debug = 0
         classname = str(self.__class__.__name__.lower())
@@ -489,15 +500,22 @@
         # pylint: disable=no-self-use
         print((json.dumps(obj, sort_keys=True, indent=2)))
 
     def __call__(self, args, cli, endpoint, data):
         raise NotImplementedError()
 
 
-class CountAction(Action):
+class ActionV2:
+    """TODO"""
+    # pylint: disable=too-few-public-methods
+
+    version = 2
+
+
+class CountAction(ActionV2):
     """TODO"""
     # pylint: disable=too-few-public-methods
 
     DEFAULT_TOTAL = "Ressources found : %(count)s"
 
     def __call__(self, args, cli, endpoint, data):
         """TODO"""
@@ -645,14 +663,16 @@
 
     def add_pre_render_class(self, clazz):
         """TODO"""
         self._pre_render_classes.append(clazz)
 
     def build(self):
         # pylint: disable=too-many-branches
+        # pylint: disable=too-many-statements
+        # pylint: disable=too-many-locals
         # This method is a little bit diry, need some refactoring.
         """Build table object"""
         if self.json or self.csv:
             self.vertical = True
         if self.json:
             self.raw = True
             self.no_cell = True
@@ -689,16 +709,17 @@
         attrs = [
             "vertical", "json", "raw", "raw_json", "csv", "cli", "endpoint",
             "reverse", "extended", "no_cell", "debug", "verbose", "cli_mode",
         ]
         for attr in attrs:
             setattr(table, attr, getattr(self, attr))
         if self.sort_by is None:
-            if self.default_sort_column and self.default_sort_column in columns:
-                table.sortby = self.default_sort_column
+            if self.default_sort_column:
+                if self.default_sort_column in columns:
+                    table.sortby = self.default_sort_column
         else:
             if self.sort_by in columns:
                 table.sortby = self.sort_by
         self.log.debug("default_sort_column: %s", self.default_sort_column)
         self.log.debug("sort_by: %s", self.sort_by)
         self.log.debug("final sortby: %s", table.sortby)
         # very ugly. need big refactoring of all tables.
```

### Comparing `vhatable-1.0.1/vhatable/filters.py` & `vhatable-1.0.2/vhatable/filters.py`

 * *Files identical despite different names*

### Comparing `vhatable-1.0.1/vhatable/sample.py` & `vhatable-1.0.2/vhatable/sample.py`

 * *Files identical despite different names*

### Comparing `vhatable-1.0.1/vhatable.egg-info/PKG-INFO` & `vhatable-1.0.2/vhatable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vhatable
-Version: 1.0.1
+Version: 1.0.2
 Summary: vhatable.
 Home-page: https://github.com/fred49/vhatable
 Author: Frederic MARTIN
 Author-email: frederic.martin.fma@gmail.com
 License: GPL3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

