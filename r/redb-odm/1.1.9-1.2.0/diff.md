# Comparing `tmp/redb-odm-1.1.9.tar.gz` & `tmp/redb-odm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redb-odm-1.1.9.tar", last modified: Wed May  3 13:56:14 2023, max compression
+gzip compressed data, was "redb-odm-1.2.0.tar", last modified: Sun May 21 00:23:10 2023, max compression
```

## Comparing `redb-odm-1.1.9.tar` & `redb-odm-1.2.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.191357 redb-odm-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 13:55:56.000000 redb-odm-1.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-03 13:56:14.191357 redb-odm-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:55:56.000000 redb-odm-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/behaviors/soft_deletion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/core/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/json_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/json_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/json_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/json_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/json_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/migo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/migo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/migo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/migo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/migo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.191357 redb-odm-1.1.9/redb/mongo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/mongo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/mongo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/mongo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/mongo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.191357 redb-odm-1.1.9/redb_odm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-03 13:56:14.000000 redb-odm-1.1.9/redb_odm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-03 13:56:14.000000 redb-odm-1.1.9/redb_odm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:56:14.000000 redb-odm-1.1.9/redb_odm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 13:56:14.000000 redb-odm-1.1.9/redb_odm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 13:56:14.000000 redb-odm-1.1.9/redb_odm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 13:55:56.000000 redb-odm-1.1.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 13:55:56.000000 redb-odm-1.1.9/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 13:55:56.000000 redb-odm-1.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:56:14.191357 redb-odm-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-03 13:55:56.000000 redb-odm-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.191357 redb-odm-1.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_bson_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_json_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_mongo_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_return_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:23:10.789566 redb-odm-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 00:22:50.000000 redb-odm-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-21 00:23:10.785566 redb-odm-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 00:22:50.000000 redb-odm-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:23:10.773566 redb-odm-1.2.0/redb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:23:10.777566 redb-odm-1.2.0/redb/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/behaviors/i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/behaviors/soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:23:10.781566 redb-odm-1.2.0/redb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/core/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:23:10.781566 redb-odm-1.2.0/redb/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/interface/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/interface/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/interface/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/interface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/interface/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/interface/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:23:10.781566 redb-odm-1.2.0/redb/json_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/json_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/json_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/json_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/json_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:23:10.785566 redb-odm-1.2.0/redb/migo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/migo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/migo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/migo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/migo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:23:10.785566 redb-odm-1.2.0/redb/mongo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/mongo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/mongo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/mongo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-21 00:22:50.000000 redb-odm-1.2.0/redb/mongo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:23:10.785566 redb-odm-1.2.0/redb_odm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-21 00:23:10.000000 redb-odm-1.2.0/redb_odm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-21 00:23:10.000000 redb-odm-1.2.0/redb_odm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:23:10.000000 redb-odm-1.2.0/redb_odm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-21 00:23:10.000000 redb-odm-1.2.0/redb_odm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 00:23:10.000000 redb-odm-1.2.0/redb_odm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 00:22:50.000000 redb-odm-1.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 00:22:50.000000 redb-odm-1.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-21 00:22:50.000000 redb-odm-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:23:10.789566 redb-odm-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-21 00:22:50.000000 redb-odm-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:23:10.785566 redb-odm-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-21 00:22:50.000000 redb-odm-1.2.0/tests/test_bson_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-21 00:22:50.000000 redb-odm-1.2.0/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-21 00:22:50.000000 redb-odm-1.2.0/tests/test_i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-21 00:22:50.000000 redb-odm-1.2.0/tests/test_json_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-21 00:22:50.000000 redb-odm-1.2.0/tests/test_mongo_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-21 00:22:50.000000 redb-odm-1.2.0/tests/test_return_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-21 00:22:50.000000 redb-odm-1.2.0/tests/test_soft_deletion.py
```

### Comparing `redb-odm-1.1.9/redb/behaviors/soft_deletion.py` & `redb-odm-1.2.0/redb/behaviors/soft_deletion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-from typing import Sequence
+from typing import Type, TypeVar
 
 from ..core import Document
-from ..interface.errors import DocumentNotFound
 from ..core.document import IncludeColumns, OptionalDocumentData, SortColumns
+from ..interface.errors import DocumentNotFound
 from ..interface.fields import ClassField, IncludeColumn
 
-from typing import Type, TypeVar
-
-
 T = TypeVar("T")
 
 
 class SoftDeletinDoc(Document):
     is_deleted: bool = False
 
     @classmethod
```

### Comparing `redb-odm-1.1.9/redb/core/base.py` & `redb-odm-1.2.0/redb/core/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from .instance import RedB
 
 IMPORT_ERROR_MSG = (
     "%s does not seem to be installed, maybe you forgot to `pip install redb[%s]`"
 )
 
-@dataclass_transform(kw_only_default=True, field_specifiers=(Field,))
+@dataclass_transform(kw_only_default=True, field_specifiers=(Field, ClassField))
 class DocumentMetaclass(ModelMetaclass):
     def __getattribute__(cls_or_self, name: str) -> Any:
         try:
             return super().__getattribute__(name)
         except AttributeError as e:
             if hasattr(cls_or_self, "__fields__"):
                 if name not in cls_or_self.__fields__:
```

### Comparing `redb-odm-1.1.9/redb/core/document.py` & `redb-odm-1.2.0/redb/core/document.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/core/instance.py` & `redb-odm-1.2.0/redb/core/instance.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/core/transaction.py` & `redb-odm-1.2.0/redb/core/transaction.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/core/utils.py` & `redb-odm-1.2.0/redb/core/utils.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/interface/client.py` & `redb-odm-1.2.0/redb/interface/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/interface/collection.py` & `redb-odm-1.2.0/redb/interface/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/interface/configs.py` & `redb-odm-1.2.0/redb/interface/configs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/interface/database.py` & `redb-odm-1.2.0/redb/interface/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/interface/fields.py` & `redb-odm-1.2.0/redb/interface/fields.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/interface/results.py` & `redb-odm-1.2.0/redb/interface/results.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/json_system/client.py` & `redb-odm-1.2.0/redb/json_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/json_system/collection.py` & `redb-odm-1.2.0/redb/json_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/json_system/database.py` & `redb-odm-1.2.0/redb/json_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/migo_system/client.py` & `redb-odm-1.2.0/redb/migo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/migo_system/collection.py` & `redb-odm-1.2.0/redb/migo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/migo_system/database.py` & `redb-odm-1.2.0/redb/migo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/mongo_system/client.py` & `redb-odm-1.2.0/redb/mongo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb/mongo_system/collection.py` & `redb-odm-1.2.0/redb/mongo_system/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Type
+from typing import Any, Literal, Type
 
 from pymongo.collection import Collection as PymongoCollection
 
 from redb.core import Document
 from redb.interface.collection import Collection, Json, OptionalJson, ReturnType
 from redb.interface.fields import CompoundIndex, PyMongoOperations
 from redb.interface.results import (
```

### Comparing `redb-odm-1.1.9/redb/mongo_system/database.py` & `redb-odm-1.2.0/redb/mongo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/redb_odm.egg-info/SOURCES.txt` & `redb-odm-1.2.0/redb_odm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.md
 requirements-dev.txt
 requirements-test.txt
 requirements.txt
 setup.py
 redb/behaviors/__init__.py
+redb/behaviors/i_remember.py
 redb/behaviors/soft_deletion.py
 redb/core/__init__.py
 redb/core/base.py
 redb/core/document.py
 redb/core/instance.py
 redb/core/transaction.py
 redb/core/utils.py
@@ -35,11 +36,12 @@
 redb_odm.egg-info/PKG-INFO
 redb_odm.egg-info/SOURCES.txt
 redb_odm.egg-info/dependency_links.txt
 redb_odm.egg-info/requires.txt
 redb_odm.egg-info/top_level.txt
 tests/test_bson_objs.py
 tests/test_hashing.py
+tests/test_i_remember.py
 tests/test_json_client.py
 tests/test_mongo_system.py
 tests/test_return_cls.py
 tests/test_soft_deletion.py
```

### Comparing `redb-odm-1.1.9/setup.py` & `redb-odm-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/tests/test_bson_objs.py` & `redb-odm-1.2.0/tests/test_bson_objs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/tests/test_hashing.py` & `redb-odm-1.2.0/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/tests/test_json_client.py` & `redb-odm-1.2.0/tests/test_json_client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/tests/test_mongo_system.py` & `redb-odm-1.2.0/tests/test_mongo_system.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/tests/test_return_cls.py` & `redb-odm-1.2.0/tests/test_return_cls.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.9/tests/test_soft_deletion.py` & `redb-odm-1.2.0/tests/test_soft_deletion.py`

 * *Files identical despite different names*

