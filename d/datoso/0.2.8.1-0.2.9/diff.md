# Comparing `tmp/datoso-0.2.8.1.tar.gz` & `tmp/datoso-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.2.8.1.tar", last modified: Thu May 11 19:32:17 2023, max compression
+gzip compressed data, was "datoso-0.2.9.tar", last modified: Sun May 21 15:58:54 2023, max compression
```

## Comparing `datoso-0.2.8.1.tar` & `datoso-0.2.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.087267 datoso-0.2.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-11 19:31:59.000000 datoso-0.2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 19:31:59.000000 datoso-0.2.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-05-11 19:32:17.087267 datoso-0.2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-11 19:31:59.000000 datoso-0.2.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-11 19:31:59.000000 datoso-0.2.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 19:32:17.087267 datoso-0.2.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.071267 datoso-0.2.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.075267 datoso-0.2.8.1/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.079267 datoso-0.2.8.1/src/datoso/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/actions/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.083267 datoso-0.2.8.1/src/datoso/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/commands/doctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.083267 datoso-0.2.8.1/src/datoso/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/configuration/folder_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/configuration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.083267 datoso-0.2.8.1/src/datoso/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.083267 datoso-0.2.8.1/src/datoso/database/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/database/models/datfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.083267 datoso-0.2.8.1/src/datoso/database/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/database/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/database/seeds/dat_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/database/seeds/dat_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/datoso.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.087267 datoso-0.2.8.1/src/datoso/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/helpers/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/helpers/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.087267 datoso-0.2.8.1/src/datoso/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/repositories/dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/repositories/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.087267 datoso-0.2.8.1/src/datoso/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/seeds/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/seeds/unknown_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-11 19:31:59.000000 datoso-0.2.8.1/src/datoso/systems.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:17.075267 datoso-0.2.8.1/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-05-11 19:32:17.000000 datoso-0.2.8.1/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-11 19:32:17.000000 datoso-0.2.8.1/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:32:17.000000 datoso-0.2.8.1/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 19:32:17.000000 datoso-0.2.8.1/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-11 19:32:17.000000 datoso-0.2.8.1/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 19:32:17.000000 datoso-0.2.8.1/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.487207 datoso-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-21 15:58:42.000000 datoso-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-21 15:58:42.000000 datoso-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-21 15:58:54.487207 datoso-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-21 15:58:42.000000 datoso-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-21 15:58:42.000000 datoso-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-21 15:58:54.487207 datoso-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.479207 datoso-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/actions/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/commands/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/configuration/folder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/configuration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/models/datfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/database/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/seeds/dat_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/database/seeds/dat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/datoso.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/helpers/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/helpers/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.487207 datoso-0.2.9/src/datoso/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/repositories/dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/repositories/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.487207 datoso-0.2.9/src/datoso/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/seeds/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/seeds/unknown_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42443 2023-05-21 15:58:42.000000 datoso-0.2.9/src/datoso/systems.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:58:54.483207 datoso-0.2.9/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 15:58:54.000000 datoso-0.2.9/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.2.8.1/LICENSE` & `datoso-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/PKG-INFO` & `datoso-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.8.1
+Version: 0.2.9
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.2.8.1/README.md` & `datoso-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/pyproject.toml` & `datoso-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/__main__.py` & `datoso-0.2.9/src/datoso/__main__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/actions/processor.py` & `datoso-0.2.9/src/datoso/actions/processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Process actions.
 """
 # pylint: disable=too-few-public-methods
 from contextlib import suppress
 import os
 import shutil
+from dateutil import parser
 from datoso.configuration import config
 from datoso.helpers import FileUtils
 from datoso.repositories.dedupe import Dedupe
 from datoso.database.models.datfile import Dat
 
 class Processor:
     """ Process actions. """
@@ -112,16 +113,19 @@
                 if old_file != new_file or config.getboolean('GENERAL', 'Overwrite', fallback=False) or not os.path.exists(destination):
                     if not old_file:
                         result = "Created"
                     elif old_file != new_file:
                         result = "Updated"
                     elif config.getboolean('GENERAL', 'Overwrite', fallback=False):
                         result = "Overwritten"
-                    self.previous['new_file'] = destination
-                    FileUtils.copy(origin, destination)
+                    if parser.parse(self.database.date, fuzzy=True) > parser.parse(self.previous['date'], fuzzy=True):
+                        result = "No Action Taken, Newer Found"
+                    else:
+                        self.previous['new_file'] = destination
+                        FileUtils.copy(origin, destination)
                 else:
                     result = "Exists"
             else:
                 self.previous['new_file'] = None
                 result = "Ignored"
         else:
             FileUtils.copy(origin, destination)
```

### Comparing `datoso-0.2.8.1/src/datoso/commands/doctor.py` & `datoso-0.2.9/src/datoso/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/commands/seed.py` & `datoso-0.2.9/src/datoso/commands/seed.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class Seed:
     """ Seed class """
     name = None
     path = None
     actions = {}
     # working_path = os.path.abspath(os.path.join(os.getcwd(), config.get('PATHS', 'WorkingPath')))
-    status_to_show = ['Updated', 'Created', 'Error', 'Disabled', 'Deduped']
+    status_to_show = ['Updated', 'Created', 'Error', 'Disabled', 'Deduped', 'No Action Taken, Newer Found']
 
     def __init__(self, **kwargs) -> None:
         self.__dict__.update(kwargs)
         actions = get_seed(self.name, 'actions')
         if actions:
             self.actions = actions.get_actions()
 
@@ -40,18 +40,19 @@
     def process_dats(self, fltr=None):
         """ Process dats."""
         def delete_line(line):
             # pylint: disable=expression-not-assigned
             [print('\b \b', end='') for x in range(0, len(line))]
             print(' ' * (len(line)), end='')
             print('\r', end='')
-        def get_preffix(name):
+        def get_preffix(name) -> str:
             seed = get_seed(name)
             return seed.__preffix__ if seed else name
-        dat_origin = os.path.join(FileUtils.parse_folder(config['PATHS'].get('DownloadPath', 'tmp')), get_preffix(self.name), 'dats')
+        tmp_path = config['PATHS'].get('DownloadPath', 'tmp')
+        dat_origin = os.path.join(FileUtils.parse_folder(tmp_path), get_preffix(self.name), 'dats')
         line = ''
         for path, actions in self.actions.items():
             new_path = path.format(dat_origin=dat_origin)
             actions = self.format_actions(actions, data={'dat_destination': config['PATHS'].get('DatPath', 'DatRoot')})
             for file in os.listdir(new_path) if os.path.isdir(new_path) else []:
                 if config['PROCESS'].get('DatIgnoreRegEx'):
                     ignore_regex = re.compile(config['PROCESS']['DatIgnoreRegEx'])
```

### Comparing `datoso-0.2.8.1/src/datoso/configuration/folder_helper.py` & `datoso-0.2.9/src/datoso/configuration/folder_helper.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/configuration/logger.py` & `datoso-0.2.9/src/datoso/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/database/__init__.py` & `datoso-0.2.9/src/datoso/database/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/database/models/datfile.py` & `datoso-0.2.9/src/datoso/database/models/datfile.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/database/seeds/dat_repos.py` & `datoso-0.2.9/src/datoso/database/seeds/dat_repos.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/database/seeds/dat_rules.py` & `datoso-0.2.9/src/datoso/database/seeds/dat_rules.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/datoso.ini` & `datoso-0.2.9/src/datoso/datoso.ini`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/helpers/__init__.py` & `datoso-0.2.9/src/datoso/helpers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,35 +96,38 @@
             with suppress(FileNotFoundError):
                 shutil.rmtree(destination)
             shutil.copytree(origin, destination)
         except FileNotFoundError:
             raise FileNotFoundError(f"File {origin} not found.")
 
     @staticmethod
+    def remove_folder(path):
+        """ Remove folder. """
+        with suppress(PermissionError):
+            shutil.rmtree(path)
+
+    @staticmethod
     def remove(path):
         """ Remove file or folder. """
         try:
             os.unlink(path)
         except IsADirectoryError:
-            try:
-                shutil.rmtree(path)
-            except PermissionError:
-                pass
+            FileUtils.remove_folder(path)
         except FileNotFoundError:
             pass
 
     @staticmethod
-    def parse_folder(path):
+    def parse_folder(path) -> str:
         """ Get folder from config. """
         if path is not None and path.startswith(('/', '~')):
             return os.path.expanduser(path)
         else:
             return os.path.join(os.getcwd(), path)
 
     @staticmethod
     def move(origin, destination):
         """ Move file to destination. """
         os.makedirs(os.path.dirname(destination), exist_ok=True)
         try:
             shutil.move(origin, destination)
-        except shutil.Error as error:
+        except shutil.Error:
             FileUtils.remove(origin)
```

### Comparing `datoso-0.2.8.1/src/datoso/helpers/executor.py` & `datoso-0.2.9/src/datoso/helpers/executor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/helpers/plugins.py` & `datoso-0.2.9/src/datoso/helpers/plugins.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/repositories/dat.py` & `datoso-0.2.9/src/datoso/repositories/dat.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/repositories/dedupe.py` & `datoso-0.2.9/src/datoso/repositories/dedupe.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/seeds/unknown_seed.py` & `datoso-0.2.9/src/datoso/seeds/unknown_seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/seeds.txt` & `datoso-0.2.9/src/datoso/seeds.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso/systems.json` & `datoso-0.2.9/src/datoso/systems.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9924812030075187%*

 * *Differences: {'insert': "[(16, OrderedDict([('company', 'Arduboy Inc'), ('system', 'Arduboy'), ('system_type', "*

 * *           "'Console')])), (168, OrderedDict([('company', 'Panic'), ('system', 'Playdate'), "*

 * *           "('system_type', 'Console')]))]"}*

```diff
@@ -107,14 +107,19 @@
     },
     {
         "company": "Apple-Bandai",
         "system": "Pippin",
         "system_type": "Console"
     },
     {
+        "company": "Arduboy Inc",
+        "system": "Arduboy",
+        "system_type": "Console"
+    },
+    {
         "company": "Atari",
         "extra_configs": {
             "empty_suffix": {
                 "nointro": "Floppies"
             }
         },
         "system": "8-bit Family",
@@ -1178,14 +1183,19 @@
     },
     {
         "company": "Ouya",
         "system": "Ouya",
         "system_type": "Handheld"
     },
     {
+        "company": "Panic",
+        "system": "Playdate",
+        "system_type": "Console"
+    },
+    {
         "company": "Palm",
         "extra_configs": {
             "empty_suffix": {
                 "nointro": "Roms"
             }
         },
         "override": {
```

### Comparing `datoso-0.2.8.1/src/datoso.egg-info/PKG-INFO` & `datoso-0.2.9/src/datoso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.8.1
+Version: 0.2.9
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.2.8.1/src/datoso.egg-info/SOURCES.txt` & `datoso-0.2.9/src/datoso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.8.1/src/datoso.egg-info/requires.txt` & `datoso-0.2.9/src/datoso.egg-info/requires.txt`

 * *Files identical despite different names*

