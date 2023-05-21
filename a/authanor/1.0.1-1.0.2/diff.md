# Comparing `tmp/authanor-1.0.1.tar.gz` & `tmp/authanor-1.0.2.tar.gz`

## Comparing `authanor-1.0.1.tar` & `authanor-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 authanor-1.0.1/Makefile
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 authanor-1.0.1/README.md
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 authanor-1.0.1/_vimrc_local.vim
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 authanor-1.0.1/config.mk
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 authanor-1.0.1/requirements.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/README.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    10513 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/make.bat
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/source/index.rst
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/source/api/database.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/source/api/modules.rst
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/source/api/testing.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/_version.py
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/database/__init__.py
--rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/database/handler.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/database/models.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/database/utils.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/testing/__init__.py
--rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/testing/helpers.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/database/test_db.py
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/database/test_handler.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/database/test_models.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/database/test_utils.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/helpers/test_helpers.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 authanor-1.0.1/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-1.0.1/COPYING
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-1.0.1/LICENSE
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 authanor-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 authanor-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 authanor-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 authanor-1.0.2/Makefile
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 authanor-1.0.2/README.md
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 authanor-1.0.2/_vimrc_local.vim
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 authanor-1.0.2/config.mk
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 authanor-1.0.2/requirements.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 authanor-1.0.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/source/api/database.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/source/api/modules.rst
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 authanor-1.0.2/docs/source/api/testing.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/_version.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/database/__init__.py
+-rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/database/handler.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/database/models.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/database/utils.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/testing/__init__.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 authanor-1.0.2/src/authanor/testing/helpers.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/conftest.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/database/test_db.py
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/database/test_handler.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/database/test_models.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/database/test_utils.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 authanor-1.0.2/tests/helpers/test_helpers.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 authanor-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-1.0.2/COPYING
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 authanor-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 authanor-1.0.2/PKG-INFO
```

### Comparing `authanor-1.0.1/Makefile` & `authanor-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/README.md` & `authanor-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/config.mk` & `authanor-1.0.2/config.mk`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/.pytest_cache/v/cache/nodeids` & `authanor-1.0.2/.pytest_cache/v/cache/nodeids`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9901960784313726%*

 * *Differences: {'insert': "[(98, 'tests/database/test_utils.py::test_transaction_decorator')]"}*

```diff
@@ -93,11 +93,12 @@
     "tests/database/test_models.py::TestAuthorizedModels::test_select_for_user",
     "tests/database/test_models.py::TestAuthorizedModels::test_select_for_user_guaranteed_joins",
     "tests/database/test_models.py::TestAuthorizedModels::test_select_specified_for_user",
     "tests/database/test_models.py::TestAuthorizedModels::test_user_id_join_chain",
     "tests/database/test_models.py::TestModels::test_model_initialization",
     "tests/database/test_models.py::TestModels::test_model_representation[mapping0-Entry(x=2, y='test2', user_id=1)]",
     "tests/database/test_models.py::TestModels::test_model_representation[mapping1-Entry(x=2, y='test2 and some other long...', user_id=1)]",
+    "tests/database/test_utils.py::test_transaction_decorator",
     "tests/database/test_utils.py::test_validate_sort_order[ASC-expectation0]",
     "tests/database/test_utils.py::test_validate_sort_order[DESC-expectation1]",
     "tests/database/test_utils.py::test_validate_sort_order[test-expectation2]"
 ]
```

### Comparing `authanor-1.0.1/docs/Makefile` & `authanor-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/docs/make.bat` & `authanor-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/docs/source/conf.py` & `authanor-1.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/docs/source/api/database.rst` & `authanor-1.0.2/docs/source/api/database.rst`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/src/authanor/database/__init__.py` & `authanor-1.0.2/src/authanor/database/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from flask import current_app
 from sqlalchemy import MetaData, create_engine, event
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import scoped_session, sessionmaker
 
 from .models import Model
+from .utils import db_transaction
 
 DIALECT = "sqlite"
 DBAPI = "pysqlite"
 
 
 class SQLAlchemy:
     """Store an interface to SQLAlchemy database objects."""
```

### Comparing `authanor-1.0.1/src/authanor/database/handler.py` & `authanor-1.0.2/src/authanor/database/handler.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/src/authanor/database/models.py` & `authanor-1.0.2/src/authanor/database/models.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/src/authanor/testing/helpers.py` & `authanor-1.0.2/src/authanor/testing/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,34 +55,69 @@
     all tests. On the other hand, the `app_transaction_context` fixture
     may be manually included in any test, which causes an ephemeral app
     to be created (and then used) only for that one test. To avoid
     cluttering test signatures, the `transaction_lifetime` decorator
     helper is provided to signal that a test should use the ephemeral
     app rather than calling the `app_transaction_context` fixture
     directly.
+
+    Parameters
+    ----------
+    factory : func
+        A factory function to build an app (e.g., `create_app`).
+    config :  callable
+        An object that will produce or be instantiated as a
+        Flask app configuration.
+    **config_kwargs :
+        Keyword arguments that will be passed to any apps generated by
+        this `AppTestManager` object.
     """
 
     persistent_app = None
     ephemeral_app = None
 
-    def __init__(self, factory):
-        self.app_factory = factory
+    def __init__(self, factory, config=None, **config_kwargs):
+        self._app_factory = factory
+        self._test_config_cls = config if config else DefaultTestingConfig
+        self._test_config_kwargs = config_kwargs
         registry["app_manager"] = self
 
     def get_app(self):
         if self.ephemeral_app:
             app = self.ephemeral_app
         else:
             app = self.persistent_app
         return app
 
     def generate_app(self, test_database_path, *args, **kwargs):
-        # Create a testing app
-        test_config = self.prepare_test_config(test_database_path, *args, **kwargs)
-        app = self.app_factory(test_config)
+        """
+        Generate an app instance for testing.
+
+        Parameters
+        ----------
+        test_database_path : str
+            The path to the database to be used in testing.
+        *args :
+            Positional arguments passed to the configuration object
+            constructor.
+        **kwargs :
+            Keyword arguments passed to the configuration object
+            constructor. Keyword arguments passed to this method will
+            overwrite default keyword arguments passed to the instance
+            constructor.
+
+        Returns
+        -------
+        app : flask.Flask
+            An app instance to be managed by this `AppTestManager`
+            object.
+        """
+        config_kwargs = self._test_config_kwargs | kwargs
+        test_config = self._test_config_cls(test_database_path, *args, **config_kwargs)
+        app = self._app_factory(test_config)
         self.setup_test_database(app)
         return app
 
     def persistent_context(self):
         return self.app_test_context("persistent_app")
 
     def ephemeral_context(self):
@@ -120,19 +155,14 @@
         db_fd, db_path = tempfile.mkstemp()
         yield namedtuple("TemporaryFile", ["fd", "path"])(db_fd, db_path)
         # After function execution, close the file and remove it
         os.close(db_fd)
         os.unlink(db_path)
 
     @staticmethod
-    def prepare_test_config(test_db_path, *args, **kwargs):
-        """Prepare a configuration object for the app. It must define a database."""
-        return DefaultTestingConfig(test_db_path)
-
-    @staticmethod
     def setup_test_database(app):
         pass
 
 
 def transaction_lifetime(test_function):
     """
     Create a decorator to leverage an ephemeral app.
```

### Comparing `authanor-1.0.1/tests/conftest.py` & `authanor-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/tests/database/test_handler.py` & `authanor-1.0.2/tests/database/test_handler.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/tests/database/test_models.py` & `authanor-1.0.2/tests/database/test_models.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/tests/helpers/test_helpers.py` & `authanor-1.0.2/tests/helpers/test_helpers.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/.gitignore` & `authanor-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/COPYING` & `authanor-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `authanor-1.0.1/pyproject.toml` & `authanor-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -81,9 +81,9 @@
 ]
 
 [tool.black]
 force-exclude = 'src/authanor/_version.py'
 
 [tool.isort]
 profile = 'black'
-src_paths = ['src/authanor', 'test']
+src_paths = ['src/authanor', 'tests']
 known_local_folder = ["test_helpers"]
```

### Comparing `authanor-1.0.1/PKG-INFO` & `authanor-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authanor
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Pythonic SQLALchemy interface to enforce authorization criteria.
 Project-URL: Download, https://pypi.org/project/authanor
 Project-URL: Homepage, https://github.com/mitchnegus/authanor
 Project-URL: Repository, https://github.com/mitchnegus/authanor
 Project-URL: Changelog, https://github.com/mitchnegus/authanor/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
```

