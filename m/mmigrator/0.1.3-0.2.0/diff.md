# Comparing `tmp/mmigrator-0.1.3.tar.gz` & `tmp/mmigrator-0.2.0.tar.gz`

## Comparing `mmigrator-0.1.3.tar` & `mmigrator-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 mmigrator-0.1.3/package.sh
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mmigrator-0.1.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/__init__.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/cli.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/config_manager.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/constants.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/db.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/migration.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/migration_manager.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/types/__init__.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mmigrator-0.1.3/tests/helpers.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mmigrator-0.1.3/tests/test_migration_manager.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mmigrator-0.1.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mmigrator-0.1.3/LICENSE
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 mmigrator-0.1.3/README.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mmigrator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mmigrator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 mmigrator-0.2.0/mmigrator.config.json
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 mmigrator-0.2.0/package.sh
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mmigrator-0.2.0/requirements.txt
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mmigrator-0.2.0/migrations/20230521104216_one.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mmigrator-0.2.0/migrations/20230521104220_two.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mmigrator-0.2.0/migrations/20230521104224_three.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/__init__.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/cli.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/constants.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/db.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/migration.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/migration_manager.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/config_manager/__init__.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/config_manager/config_manager.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/config_manager/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.2.0/src/mmigrator/types/__init__.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mmigrator-0.2.0/tests/helpers.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mmigrator-0.2.0/tests/test_migration_manager.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mmigrator-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mmigrator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 mmigrator-0.2.0/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mmigrator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 mmigrator-0.2.0/PKG-INFO
```

### Comparing `mmigrator-0.1.3/src/mmigrator/cli.py` & `mmigrator-0.2.0/src/mmigrator/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 #!/usr/bin/env python3
 
 import sys
 from .migration_manager import MigrationManager
 from .constants import HELP_TEMPLATE
 
 
-def main():
-    args = sys.argv[1:]
+args = sys.argv[1:]
+
+
+def get_args_with_option(option) -> (str, str):
+    arg, *opt = args
+
+    if len(opt) and opt[0] != option:
+        raise Exception(f'Unrecognized parameter {opt}')
+
+    return arg, opt[0] if len(opt) else None
 
+
+def main():
     if len(args) == 0:
         exit()
     
     if args[0] == 'help':
         print(HELP_TEMPLATE)
     
     elif args[0] == 'init':
         MigrationManager.init()
     
     elif args[0] in ['new', 'g']:
         MigrationManager().generate(args[1])
     
     elif args[0] == 'migrate':
-        MigrationManager().migrate()
+        _, run_silently = get_args_with_option('--silent')
+
+        MigrationManager().migrate(silent=bool(run_silently))
     
     elif args[0] == 'revert':
-        MigrationManager().revert()
+        _, run_silently = get_args_with_option('--silent')
+
+        MigrationManager().revert(silent=bool(run_silently))
```

### Comparing `mmigrator-0.1.3/src/mmigrator/config_manager.py` & `mmigrator-0.2.0/src/mmigrator/config_manager/config_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import json
 import re
-from .process import process
-from .constants import CONFIG_FILE_NAME, CONFIG_FILE_TEMPLATE
+from ..process import process
+from ..constants import CONFIG_FILE_NAME, CONFIG_FILE_TEMPLATE
+from .helpers import load_var
 
 
 class ConfigManager(object):
     @staticmethod
     def init_config():
         @process('Initializing configs')
         def init():
@@ -16,33 +17,14 @@
                 f.write(conf)
             
         if not os.path.exists(CONFIG_FILE_NAME):
             init()
 
     @staticmethod
     def read_config() -> dict:
-        def load_var(filename: str, varname: str) -> str:
-            var_value = None
-
-            with open(filename, 'r') as f:
-                data = f.read()
-                
-            if re.match(r'^.*\.json$', filename):
-                data = json.loads(data)
-                var_value = data.get(varname)
-            else:
-                m = re.search(fr'{varname}\s?=\s?(.+)', data)
-                if m:
-                    var_value = m[1]
-            
-            if not var_value:
-                raise Exception(f'Cannot parse {varname} variable from file {filename}')
-            
-            return var_value
-
         with open(CONFIG_FILE_NAME, 'r') as f:
             cfg = json.loads(f.read())
 
         for k, v in cfg['connection'].items():
             if v and re.match(r'^.+\[.+\]$', v):
                 file, var = re.sub(r'[\[\]]', ' ', v).strip().split(' ')
                 cfg['connection'][k] = load_var(file, var)
```

### Comparing `mmigrator-0.1.3/src/mmigrator/db.py` & `mmigrator-0.2.0/src/mmigrator/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from typing import Any, Mapping
+
 import pymongo
+from pymongo.database import Database
 
 
-def connect_db(connection: dict):
+def connect_db(connection: dict) -> Database[Mapping[str, Any] | Any]:
     mongo_user = connection['user']
     mongo_db = connection['database']
     mongo_password = connection['password']
     mongo_host = connection['host']
     mongo_port = connection['port']
 
     if not (mongo_host or mongo_port or mongo_port):
```

### Comparing `mmigrator-0.1.3/src/mmigrator/migration.py` & `mmigrator-0.2.0/src/mmigrator/migration.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,16 +43,24 @@
         module = util.module_from_spec(spec)
         sys.modules[self.__dist] = module
         spec.loader.exec_module(module)
         func = getattr(module, func_name)
         
         return func
     
-    def migrate(self):
-        up = self.__load_func('up')
+    def migrate(self, silent=False):
+        try:
+            up = self.__load_func('up')
 
-        up(self.__db)
+            up(self.__db)
+        except Exception as e:
+            if not silent:
+                raise Exception(f'Error: {str(e)}')
     
-    def revert(self):
-        down = self.__load_func('down')
-        
-        down(self.__db)
+    def revert(self, silent=False):
+        try:
+            down = self.__load_func('down')
+
+            down(self.__db)
+        except Exception as e:
+            if not silent:
+                raise Exception(f'Error: {str(e)}')
```

### Comparing `mmigrator-0.1.3/src/mmigrator/migration_manager.py` & `mmigrator-0.2.0/src/mmigrator/migration_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 from .db import connect_db
-from .config_manager import ConfigManager
+from .config_manager.config_manager import ConfigManager
 from .migration import Migration
 from .constants import MMIGRATOR_COLLECTION
+from typing import Any, Mapping
+from pymongo.database import Database
 
 
 class MigrationManager(object):
-    __db = None
+    __db: Database[Mapping[str, Any] | Any] = None
     __config: dict = None
     __version: str = None
     __dist: str = None
 
     def __init__(self):
         MigrationManager.init()
         
@@ -29,37 +31,37 @@
     
     def generate(self, name):
         mig = Migration(name=name, dist=self.__dist)
         mig.generate()
         
         print(f'\nSuccessfully created new migration {mig.name}\n')
 
-    def revert(self):
+    def revert(self, silent=False):
         files, last_index = self.__get_files_list()
         prev_index = last_index-1
 
         if last_index < 0:
             print('No migrations to revert')
             return
         
         print('Reverting last migration...')
 
         file = files[last_index]
 
         mig = Migration(name=file, dist=self.__dist, db=self.__db)
         
-        mig.revert()
+        mig.revert(silent)
         
         if last_index > 0:
             print(f'Current migration is...{files[prev_index]}')
 
         self.__version = files[prev_index] if last_index > 0 else None
         self.__persist_version()
 
-    def migrate(self):
+    def migrate(self, silent=False):
         files, last_index = self.__get_files_list()
         files = files[last_index + 1:]
 
         if len(files) == 0:
             print('No migrations to apply')
             return
 
@@ -71,15 +73,15 @@
     
                 mig = Migration(
                     name=file,
                     dist=self.__dist,
                     db=self.__db
                 )
     
-                mig.migrate()
+                mig.migrate(silent)
 
                 self.__version = file
         except Exception as e:
             print(e)
         finally:
             self.__persist_version()
```

### Comparing `mmigrator-0.1.3/tests/helpers.py` & `mmigrator-0.2.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.3/tests/test_migration_manager.py` & `mmigrator-0.2.0/tests/test_migration_manager.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.3/LICENSE` & `mmigrator-0.2.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Copyright (c) 2018 The Python Packaging Authority
+The MIT License (MIT)
+
+Copyright (c) 2023 Serhii Kovalov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `mmigrator-0.1.3/README.md` & `mmigrator-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -67,25 +67,34 @@
 MigrationManager.generate("SomeName")
 ```
 
 ### Run migrations
 #### CLI
 ```bash
 $ mmigrator migrate
+# or add --silent flag for dry-run (skip exceptions)
+$ mmigrator migrate --silent
 ```
 
 #### from code:
 ```py
 MigrationManager.migrate()
+# or add silent=True flag for dry-run (skip exceptions)
+MigrationManager.migrate(silent=True)
+
 ```
 
 
 ### Revert migrations
 #### CLI
 ```bash
 $ mmigrator revert
+# or add --silent flag for dry-run (skip exceptions)
+$ mmigrator revert --silent
 ```
 
 #### from code:
 ```py
 MigrationManager.revert()
+# or add silent=True flag for dry-run (skip exceptions)
+MigrationManager.revert(silent=True)
 ```
```

### Comparing `mmigrator-0.1.3/pyproject.toml` & `mmigrator-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mmigrator"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
   { name="Serhii Kovalov", email="moiserge.k@gmail.com" },
 ]
 description = "Migration engine for MongoDB"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mmigrator-0.1.3/PKG-INFO` & `mmigrator-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmigrator
-Version: 0.1.3
+Version: 0.2.0
 Summary: Migration engine for MongoDB
 Project-URL: Homepage, https://github.com/sergekovalev/mmigrator
 Project-URL: Bug Tracker, https://github.com/sergekovalev/mmigrator/issues
 Author-email: Serhii Kovalov <moiserge.k@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -84,25 +84,34 @@
 MigrationManager.generate("SomeName")
 ```
 
 ### Run migrations
 #### CLI
 ```bash
 $ mmigrator migrate
+# or add --silent flag for dry-run (skip exceptions)
+$ mmigrator migrate --silent
 ```
 
 #### from code:
 ```py
 MigrationManager.migrate()
+# or add silent=True flag for dry-run (skip exceptions)
+MigrationManager.migrate(silent=True)
+
 ```
 
 
 ### Revert migrations
 #### CLI
 ```bash
 $ mmigrator revert
+# or add --silent flag for dry-run (skip exceptions)
+$ mmigrator revert --silent
 ```
 
 #### from code:
 ```py
 MigrationManager.revert()
+# or add silent=True flag for dry-run (skip exceptions)
+MigrationManager.revert(silent=True)
 ```
```

