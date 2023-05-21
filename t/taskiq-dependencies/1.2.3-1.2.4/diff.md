# Comparing `tmp/taskiq_dependencies-1.2.3.tar.gz` & `tmp/taskiq_dependencies-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_dependencies-1.2.3.tar", max compression
+gzip compressed data, was "taskiq_dependencies-1.2.4.tar", max compression
```

## Comparing `taskiq_dependencies-1.2.3.tar` & `taskiq_dependencies-1.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6368 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/README.md
--rw-r--r--   0        0        0     1621 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/pyproject.toml
--rw-r--r--   0        0        0      386 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/__init__.py
--rw-r--r--   0        0        0    11543 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/ctx.py
--rw-r--r--   0        0        0     3273 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/dependency.py
--rw-r--r--   0        0        0     9626 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/graph.py
--rw-r--r--   0        0        0        0 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/py.typed
--rw-r--r--   0        0        0      573 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/utils.py
--rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 taskiq_dependencies-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     6368 2023-05-21 21:34:19.764530 taskiq_dependencies-1.2.4/README.md
+-rw-r--r--   0        0        0     1621 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0      386 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/__init__.py
+-rw-r--r--   0        0        0    11773 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/ctx.py
+-rw-r--r--   0        0        0     3273 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/dependency.py
+-rw-r--r--   0        0        0     9626 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/graph.py
+-rw-r--r--   0        0        0        0 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/py.typed
+-rw-r--r--   0        0        0      573 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/utils.py
+-rw-r--r--   0        0        0     7251 1970-01-01 00:00:00.000000 taskiq_dependencies-1.2.4/PKG-INFO
```

### Comparing `taskiq_dependencies-1.2.3/README.md` & `taskiq_dependencies-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.3/pyproject.toml` & `taskiq_dependencies-1.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-dependencies"
-version = "1.2.3"
+version = "1.2.4"
 description = "FastAPI like dependency injection implementation"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 packages = [{include = "taskiq_dependencies"}]
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
```

### Comparing `taskiq_dependencies-1.2.3/taskiq_dependencies/ctx.py` & `taskiq_dependencies-1.2.4/taskiq_dependencies/ctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,16 @@
         for ctx in self.sub_contexts:
             ctx.close(*args)
         for dep in reversed(self.opened_dependencies):
             if inspect.isgenerator(dep):
                 if exception_found:
                     try:
                         dep.throw(*args)
+                    except StopIteration:
+                        continue
                     except BaseException as exc:
                         logger.warning(
                             "Exception found on dependency teardown %s",
                             exc,
                             exc_info=True,
                         )
                         continue
@@ -239,28 +241,32 @@
         for ctx in self.sub_contexts:
             await ctx.close(*args)  # type: ignore
         for dep in reversed(self.opened_dependencies):
             if inspect.isgenerator(dep):
                 if exception_found:
                     try:
                         dep.throw(*args)
+                    except StopIteration:
+                        continue
                     except BaseException as exc:
                         logger.warning(
                             "Exception found on dependency teardown %s",
                             exc,
                             exc_info=True,
                         )
                         continue
                     continue
                 for _ in dep:  # noqa: WPS328
                     pass  # noqa: WPS420
             elif inspect.isasyncgen(dep):
                 if exception_found:
                     try:
                         await dep.athrow(*args)
+                    except StopAsyncIteration:
+                        continue
                     except BaseException as exc:
                         logger.warning(
                             "Exception found on dependency teardown %s",
                             exc,
                             exc_info=True,
                         )
                         continue
```

### Comparing `taskiq_dependencies-1.2.3/taskiq_dependencies/dependency.py` & `taskiq_dependencies-1.2.4/taskiq_dependencies/dependency.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.3/taskiq_dependencies/graph.py` & `taskiq_dependencies-1.2.4/taskiq_dependencies/graph.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.3/taskiq_dependencies/utils.py` & `taskiq_dependencies-1.2.4/taskiq_dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.3/PKG-INFO` & `taskiq_dependencies-1.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
 Name: taskiq-dependencies
-Version: 1.2.3
+Version: 1.2.4
 Summary: FastAPI like dependency injection implementation
 Keywords: taskiq,dependencies,injection,async,DI
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: graphlib-backport (>=1.0.3,<2.0.0) ; python_version < "3.9"
 Description-Content-Type: text/markdown
 
 # Taskiq dependencies
 
 This project is used to add FastAPI-like dependency injection to projects.
```

