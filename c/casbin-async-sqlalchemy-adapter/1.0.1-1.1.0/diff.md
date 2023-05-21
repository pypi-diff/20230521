# Comparing `tmp/casbin_async_sqlalchemy_adapter-1.0.1.tar.gz` & `tmp/casbin_async_sqlalchemy_adapter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_async_sqlalchemy_adapter-1.0.1.tar", last modified: Thu May 18 14:04:37 2023, max compression
+gzip compressed data, was "casbin_async_sqlalchemy_adapter-1.1.0.tar", last modified: Sun May 21 17:35:52 2023, max compression
```

## Comparing `casbin_async_sqlalchemy_adapter-1.0.1.tar` & `casbin_async_sqlalchemy_adapter-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-18 14:04:37.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-18 14:04:37.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:04:37.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 14:04:37.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 14:04:37.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-21 17:35:51.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-21 17:35:51.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:35:51.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-21 17:35:51.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-21 17:35:51.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/tests/test_adapter.py
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.1/LICENSE` & `casbin_async_sqlalchemy_adapter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.0.1/PKG-INFO` & `casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: casbin_async_sqlalchemy_adapter
-Version: 1.0.1
+Name: casbin-async-sqlalchemy-adapter
+Version: 1.1.0
 Summary: Asynchronous SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-sqlalchemy-adapter
 Author: wrapping-2000
 Author-email: wenpengchen@njust.edu.cn
 License: Apache 2.0
 Keywords: asynccasbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 async-sqlalchemy-adapter
 ====
 Async SQLAlchemy Adapter for PyCasbin<br>
 [![GitHub Actions](https://github.com/pycasbin/async-sqlalchemy-adapter/workflows/build/badge.svg?branch=master)](https://github.com/pycasbin/async-sqlalchemy-adapter/actions)
@@ -31,19 +31,19 @@
 
 Asynchronous SQLAlchemy Adapter is the [SQLAlchemy](https://www.sqlalchemy.org) adapter for [PyCasbin](https://github.com/casbin/pycasbin). With this library, Casbin can load policy from SQLAlchemy supported database or save policy to it.
 
 Based on [Officially Supported Databases](http://www.sqlalchemy.org/), The current supported databases are:
 
 - PostgreSQL
 - MySQL
+- MariaDB
 - SQLite
 - Oracle
 - Microsoft SQL Server
 - Firebird
-- Sybase
 
 ## Installation
 
 ```
 pip install casbin_async_sqlalchemy_adapter
 ```
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.1/README.md` & `casbin_async_sqlalchemy_adapter-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 Asynchronous SQLAlchemy Adapter is the [SQLAlchemy](https://www.sqlalchemy.org) adapter for [PyCasbin](https://github.com/casbin/pycasbin). With this library, Casbin can load policy from SQLAlchemy supported database or save policy to it.
 
 Based on [Officially Supported Databases](http://www.sqlalchemy.org/), The current supported databases are:
 
 - PostgreSQL
 - MySQL
+- MariaDB
 - SQLite
 - Oracle
 - Microsoft SQL Server
 - Firebird
-- Sybase
 
 ## Installation
 
 ```
 pip install casbin_async_sqlalchemy_adapter
 ```
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter/__init__.py` & `casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter/adapter.py` & `casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import warnings
 from contextlib import asynccontextmanager
 
 from casbin import persist
 from sqlalchemy import Column, Integer, String
-from sqlalchemy import create_engine, or_
+from sqlalchemy import or_
 from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.future import select
 from sqlalchemy.orm import sessionmaker
 
 Base = declarative_base()
 
@@ -58,56 +58,57 @@
     v4 = []
     v5 = []
 
 
 class Adapter(persist.Adapter):
     """the interface for Casbin adapters."""
 
-    def __init__(self, engine, db_class=None, filtered=False):
+    def __init__(self, engine, db_class=None, filtered=False, warning=True):
         if isinstance(engine, str):
             self._engine = create_async_engine(engine, future=True)
         else:
             self._engine = engine
 
         if db_class is None:
             db_class = CasbinRule
+            if warning:
+                warnings.warn(
+                    'Using default CasbinRule table, please note the use of the "Adapter().create_table()" method to '
+                    'create the table, and ignore this warning if you are using a custom CasbinRule table.',
+                    RuntimeWarning,
+                )
         else:
-            for attr in (
-                    "id",
-                    "ptype",
-                    "v0",
-                    "v1",
-                    "v2",
-                    "v3",
-                    "v4",
-                    "v5",
-            ):  # id attr was used by filter
+            for attr in ("id", "ptype", "v0", "v1", "v2", "v3", "v4", "v5"):  # id attr was used by filter
                 if not hasattr(db_class, attr):
                     raise Exception(f"{attr} not found in custom DatabaseClass.")
             Base.metadata = db_class.metadata
 
         self._db_class = db_class
         self.session_local = sessionmaker(
             self._engine, expire_on_commit=False, class_=AsyncSession
         )
 
-        Base.metadata.create_all(self._engine)
         self._filtered = filtered
 
     @asynccontextmanager
     async def _session_scope(self):
         """Provide an asynchronous transactional scope around a series of operations."""
         async with self.session_local() as session:
             try:
                 yield session
                 await session.commit()
             except Exception as e:
                 await session.rollback()
                 raise e
 
+    async def create_table(self):
+        """Creates default casbin rule table."""
+        async with self._engine.begin() as conn:
+            await conn.run_sync(Base.metadata.create_all)
+
     async def load_policy(self, model):
         """loads all policy rules from the storage."""
         async with self._session_scope() as session:
             lines = await session.execute(select(self._db_class))
             for line in lines.scalars():
                 persist.load_policy_line(str(line), model)
 
@@ -202,17 +203,15 @@
                 if v != "":
                     v_value = getattr(self._db_class, "v{}".format(field_index + i))
                     query = query.filter(v_value == v)
             r = await query.delete()
 
         return True if r > 0 else False
 
-    async def update_policy(
-            self, sec: str, ptype: str, old_rule: [str], new_rule: [str]
-    ) -> None:
+    async def update_policy(self, sec: str, ptype: str, old_rule: [str], new_rule: [str]) -> None:
         """
         Update the old_rule with the new_rule in the database (storage).
 
         :param sec: section type
         :param ptype: policy type
         :param old_rule: the old rule that needs to be modified
         :param new_rule: the new rule to replace the old rule
@@ -235,41 +234,29 @@
             # overwrite the old rule with the new rule
             for index in range(len(longest_rule)):
                 if index < len(new_rule):
                     setattr(old_rule_line, "v{}".format(index), new_rule[index])
                 else:
                     setattr(old_rule_line, "v{}".format(index), None)
 
-    async def update_policies(
-            self,
-            sec: str,
-            ptype: str,
-            old_rules: [
-                [str],
-            ],
-            new_rules: [
-                [str],
-            ],
-    ) -> None:
+    async def update_policies(self, sec: str, ptype: str, old_rules: [[str], ], new_rules: [[str], ]) -> None:
         """
         Update the old_rules with the new_rules in the database (storage).
 
         :param sec: section type
         :param ptype: policy type
         :param old_rules: the old rules that need to be modified
         :param new_rules: the new rules to replace the old rules
 
         :return: None
         """
         for i in range(len(old_rules)):
             await self.update_policy(sec, ptype, old_rules[i], new_rules[i])
 
-    async def update_filtered_policies(
-            self, sec, ptype, new_rules: [[str]], field_index, *field_values
-    ) -> [[str]]:
+    async def update_filtered_policies(self, sec, ptype, new_rules: [[str]], field_index, *field_values) -> [[str]]:
         """update_filtered_policies updates all the policies on the basis of the filter."""
 
         filter = Filter()
         filter.ptype = ptype
 
         # Creating Filter from the field_index & field_values provided
         for i in range(len(field_values)):
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO` & `casbin_async_sqlalchemy_adapter-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: casbin-async-sqlalchemy-adapter
-Version: 1.0.1
+Name: casbin_async_sqlalchemy_adapter
+Version: 1.1.0
 Summary: Asynchronous SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-sqlalchemy-adapter
 Author: wrapping-2000
 Author-email: wenpengchen@njust.edu.cn
 License: Apache 2.0
 Keywords: asynccasbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 async-sqlalchemy-adapter
 ====
 Async SQLAlchemy Adapter for PyCasbin<br>
 [![GitHub Actions](https://github.com/pycasbin/async-sqlalchemy-adapter/workflows/build/badge.svg?branch=master)](https://github.com/pycasbin/async-sqlalchemy-adapter/actions)
@@ -31,19 +31,19 @@
 
 Asynchronous SQLAlchemy Adapter is the [SQLAlchemy](https://www.sqlalchemy.org) adapter for [PyCasbin](https://github.com/casbin/pycasbin). With this library, Casbin can load policy from SQLAlchemy supported database or save policy to it.
 
 Based on [Officially Supported Databases](http://www.sqlalchemy.org/), The current supported databases are:
 
 - PostgreSQL
 - MySQL
+- MariaDB
 - SQLite
 - Oracle
 - Microsoft SQL Server
 - Firebird
-- Sybase
 
 ## Installation
 
 ```
 pip install casbin_async_sqlalchemy_adapter
 ```
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.1/setup.py` & `casbin_async_sqlalchemy_adapter-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from setuptools import setup, find_packages, __version__
 from os import path
 
+from setuptools import setup, find_packages
+
 desc_file = "README.md"
 
 with open(desc_file, "r") as fh:
     long_description = fh.read()
 
 here = path.abspath(path.dirname(__file__))
 # get the dependencies and installs
@@ -43,20 +44,20 @@
         "access control",
         "abac",
         "acl",
         "permission",
     ],
     packages=find_packages(),
     install_requires=install_requires,
-    python_requires=">=3.3",
+    python_requires=">=3.7",
     license="Apache 2.0",
     classifiers=[
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     data_files=[desc_file],
 )
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.1/tests/test_adapter.py` & `casbin_async_sqlalchemy_adapter-1.1.0/tests/test_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,141 +8,139 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import asyncio
 import os
-from casbin_async_sqlalchemy_adapter import Adapter
-from casbin_async_sqlalchemy_adapter import Base
-from casbin_async_sqlalchemy_adapter import CasbinRule
-from casbin_async_sqlalchemy_adapter.adapter import Filter
+import unittest
 from unittest import IsolatedAsyncioTestCase
-from unittest import TestCase
-from unittest import async_case
+
 import casbin
-from sqlalchemy import create_engine, Column, Integer, String
+from sqlalchemy import create_engine, Column, Integer, String, select
+from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
 from sqlalchemy.orm import sessionmaker
-from concurrent.futures import ThreadPoolExecutor
-from functools import partial
+
+from casbin_async_sqlalchemy_adapter import Adapter
+from casbin_async_sqlalchemy_adapter import Base
+from casbin_async_sqlalchemy_adapter import CasbinRule
 
 
 def get_fixture(path):
     dir_path = os.path.split(os.path.realpath(__file__))[0] + "/"
     return os.path.abspath(dir_path + path)
 
 
-def get_enforcer():
-    engine = create_engine("sqlite://")
-    # engine = create_engine('sqlite:///' + os.path.split(os.path.realpath(__file__))[0] + '/test.db', echo=True)
+async def get_enforcer():
+    engine = create_async_engine("sqlite+aiosqlite://", future=True)
+    # engine = create_async_engine('sqlite+aiosqlite:///' + os.path.split(os.path.realpath(__file__))[0] + '/test.db',
+    # echo=True)
     adapter = Adapter(engine)
+    await adapter.create_table()
 
-    session = sessionmaker(bind=engine)
-    Base.metadata.create_all(engine)
-    s = session()
-    s.query(CasbinRule).delete()
-    s.add(CasbinRule(ptype="p", v0="alice", v1="data1", v2="read"))
-    s.add(CasbinRule(ptype="p", v0="bob", v1="data2", v2="write"))
-    s.add(CasbinRule(ptype="p", v0="data2_admin", v1="data2", v2="read"))
-    s.add(CasbinRule(ptype="p", v0="data2_admin", v1="data2", v2="write"))
-    s.add(CasbinRule(ptype="g", v0="alice", v1="data2_admin"))
-    s.commit()
-    s.close()
+    async_session = sessionmaker(engine, expire_on_commit=False, class_=AsyncSession)
+    async with async_session() as s:
+        s.add(CasbinRule(ptype="p", v0="alice", v1="data1", v2="read"))
+        s.add(CasbinRule(ptype="p", v0="bob", v1="data2", v2="write"))
+        s.add(CasbinRule(ptype="p", v0="data2_admin", v1="data2", v2="read"))
+        s.add(CasbinRule(ptype="p", v0="data2_admin", v1="data2", v2="write"))
+        s.add(CasbinRule(ptype="g", v0="alice", v1="data2_admin"))
+        await s.commit()
 
     return casbin.Enforcer(get_fixture("rbac_model.conf"), adapter)
 
 
 class TestConfig(IsolatedAsyncioTestCase):
-    def test_custom_db_class(self):
+    async def test_custom_db_class(self):
         class CustomRule(Base):
             __tablename__ = "casbin_rule2"
 
             id = Column(Integer, primary_key=True)
             ptype = Column(String(255))
             v0 = Column(String(255))
             v1 = Column(String(255))
             v2 = Column(String(255))
             v3 = Column(String(255))
             v4 = Column(String(255))
             v5 = Column(String(255))
             not_exist = Column(String(255))
 
-        engine = create_engine("sqlite://")
-        adapter = Adapter(engine, CustomRule)
-
-        session = sessionmaker(bind=engine)
-        Base.metadata.create_all(engine)
-        s = session()
-        s.add(CustomRule(not_exist="NotNone"))
-        s.commit()
-        self.assertEqual(s.query(CustomRule).all()[0].not_exist, "NotNone")
+        engine = create_async_engine("sqlite+aiosqlite://", future=True)
+        async with engine.begin() as conn:
+            await conn.run_sync(Base.metadata.create_all)
+
+        session = sessionmaker(engine, expire_on_commit=False, class_=AsyncSession)
+        async with session() as s:
+            s.add(CustomRule(not_exist="NotNone"))
+            await s.commit()
+            a = await s.execute(select(CustomRule))
+            self.assertEqual(a.scalars().all()[0].not_exist, "NotNone")
 
     async def test_enforcer_basic(self):
-        e = get_enforcer()
+        e = await get_enforcer()
         self.assertFalse(e.enforce("alice", "data4", "read"))
         model = e.get_model()
         model.clear_policy()
         model.add_policy("p", "p", ["alice", "data4", "read"])
 
         self.assertTrue(e.enforce("alice", "data4", "read"))
 
     async def test_add_policy(self):
-        e = get_enforcer()
+        e = await get_enforcer()
 
         self.assertFalse(e.enforce("eve", "data3", "read"))
         self.assertFalse(e.enforce("eve", "data4", "read"))
 
         model = e.get_model()
         model.clear_policy()
         model.add_policy("p", "p", ["eve", "data3", "read"])
         model.add_policy("p", "p", ["eve", "data4", "read"])
 
         self.assertTrue(e.enforce("eve", "data3", "read"))
         self.assertTrue(e.enforce("eve", "data4", "read"))
 
     async def test_add_policies(self):
-        e = get_enforcer()
+        e = await get_enforcer()
 
         self.assertFalse(e.enforce("eve", "data3", "read"))
         self.assertFalse(e.enforce("eve", "data4", "read"))
         model = e.get_model()
         model.clear_policy()
         model.add_policies("p", "p", [("eve", "data3", "read"), ("eve", "data4", "read")])
 
         self.assertTrue(e.enforce("eve", "data3", "read"))
         self.assertTrue(e.enforce("eve", "data4", "read"))
 
     async def test_save_policy(self):
-        e = get_enforcer()
+        e = await get_enforcer()
         self.assertFalse(e.enforce("alice", "data4", "read"))
 
         model = e.get_model()
         model.clear_policy()
 
         model.add_policy("p", "p", ["alice", "data4", "read"])
 
         adapter = e.get_adapter()
         adapter.save_policy(model)
         self.assertTrue(e.enforce("alice", "data4", "read"))
 
     async def test_remove_policy(self):
-        e = get_enforcer()
+        e = await get_enforcer()
         self.assertFalse(e.enforce("alice", "data4", "read"))
 
         model = e.get_model()
         model.clear_policy()
         model.add_policy("p", "p", ["alice", "data4", "read"])
         self.assertTrue(e.enforce("alice", "data4", "read"))
         model.remove_policy("p", "p", ["alice", "data4", "read"])
         self.assertFalse(e.enforce("alice", "data4", "read"))
 
     async def test_remove_policies(self):
-        e = get_enforcer()
+        e = await get_enforcer()
 
         self.assertFalse(e.enforce("eve", "data3", "read"))
         self.assertFalse(e.enforce("eve", "data4", "read"))
         model = e.get_model()
         model.clear_policy()
         model.add_policies("p", "p", [("eve", "data3", "read"), ("eve", "data4", "read")])
 
@@ -150,15 +148,15 @@
         self.assertTrue(e.enforce("eve", "data4", "read"))
         model.remove_policies("p", "p", [("eve", "data3", "read"), ("eve", "data4", "read")])
 
         self.assertFalse(e.enforce("eve", "data3", "read"))
         self.assertFalse(e.enforce("eve", "data4", "read"))
 
     async def test_remove_filtered_policy(self):
-        e = get_enforcer()
+        e = await get_enforcer()
 
         self.assertFalse(e.enforce("eve", "data3", "read"))
         self.assertFalse(e.enforce("eve", "data4", "read"))
         self.assertFalse(e.enforce("alice", "data1", "read"))
 
         model = e.get_model()
         model.clear_policy()
@@ -199,15 +197,15 @@
 
         s.add(rule)
         s.commit()
         self.assertRegex(repr(rule), r'<CasbinRule \d+: "p, alice, data1, read">')
         s.close()
 
     async def test_filtered_policy(self):
-        e = get_enforcer()
+        e = await get_enforcer()
 
         model = e.get_model()
         model.clear_policy()
         model.add_policy("p", "p", ["alice", "data1", "read"])
         model.add_policy("p", "p", ["alice", "data3", "read"])
         model.add_policy("p", "p", ["alice", "data2", "write"])
         model.add_policy("p", "p", ["bob", "data2", "read"])
@@ -215,15 +213,15 @@
         model.add_policy("p", "p", ["bob", "data3", "read"])
 
         print(model.get_filtered_policy("p", "p", 0, "alice"))
         print(model.get_filtered_policy("p", "p", 1, "data1"))
         print(model.get_filtered_policy("p", "p", 2, "read"))
 
     async def test_update_policy(self):
-        e = get_enforcer()
+        e = await get_enforcer()
         model = e.get_model()
         model.clear_policy()
         model.add_policy("p", "p", ["alice", "data1", "read"])
         model.add_policy("p", "p", ["alice", "data3", "read"])
         model.add_policy("p", "p", ["alice", "data2", "write"])
 
         model.update_policy("p", "p", ["alice", "data1", "read"], ["bob", "data2", "read"])
@@ -234,15 +232,15 @@
         self.assertFalse(e.enforce("alice", "data3", "read"))
         self.assertFalse(e.enforce("alice", "data2", "write"))
         self.assertTrue(e.enforce("bob", "data2", "read"))
         self.assertTrue(e.enforce("bob", "data1", "write"))
         self.assertTrue(e.enforce("bob", "data3", "read"))
 
     async def test_update_policies(self):
-        e = get_enforcer()
+        e = await get_enforcer()
         model = e.get_model()
         model.clear_policy()
 
         old_rule_0 = ["alice", "data1", "read"]
         old_rule_1 = ["bob", "data2", "write"]
         old_rule_2 = ["data2_admin", "data2", "read"]
         old_rule_3 = ["data2_admin", "data2", "write"]
@@ -267,7 +265,11 @@
         self.assertTrue(e.enforce("bob", "data_test", "write"))
 
         self.assertFalse(e.enforce("data2_admin", "data2", "read"))
         self.assertTrue(e.enforce("data2_admin", "data_test", "read"))
 
         self.assertFalse(e.enforce("data2_admin", "data2", "write"))
         self.assertTrue(e.enforce("data2_admin", "data_test", "write"))
+
+
+if __name__ == '__main__':
+    unittest.main()
```

