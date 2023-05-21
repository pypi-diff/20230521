# Comparing `tmp/async_extensions-1.3.0.tar.gz` & `tmp/async_extensions-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_extensions-1.3.0.tar", max compression
+gzip compressed data, was "async_extensions-1.4.0.tar", max compression
```

## Comparing `async_extensions-1.3.0.tar` & `async_extensions-1.4.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1092 2023-05-17 22:52:57.634115 async_extensions-1.3.0/LICENSE
--rw-r--r--   0        0        0     2578 2023-05-17 22:52:57.634115 async_extensions-1.3.0/README.md
--rw-r--r--   0        0        0     2968 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/__init__.py
--rw-r--r--   0        0        0      732 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/blocking.py
--rw-r--r--   0        0        0      431 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/cancel.py
--rw-r--r--   0        0        0     1174 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/channel.py
--rw-r--r--   0        0        0     1581 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/close.py
--rw-r--r--   0        0        0     7825 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/collect.py
--rw-r--r--   0        0        0      118 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/constants.py
--rw-r--r--   0        0        0       80 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/current.py
--rw-r--r--   0        0        0       88 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/errors.py
--rw-r--r--   0        0        0      101 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/file.py
--rw-r--r--   0        0        0      174 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/low_level.py
--rw-r--r--   0        0        0       44 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/path.py
--rw-r--r--   0        0        0       87 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/process.py
--rw-r--r--   0        0        0        0 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/py.typed
--rw-r--r--   0        0        0      396 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/run.py
--rw-r--r--   0        0        0       76 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/signal.py
--rw-r--r--   0        0        0       77 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/sleep.py
--rw-r--r--   0        0        0     1327 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/standard.py
--rw-r--r--   0        0        0      143 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/synchronization.py
--rw-r--r--   0        0        0      253 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/task_group.py
--rw-r--r--   0        0        0      176 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/types.py
--rw-r--r--   0        0        0      617 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/typing.py
--rw-r--r--   0        0        0      732 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/wait.py
--rw-r--r--   0        0        0     2438 2023-05-17 22:52:57.634115 async_extensions-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 async_extensions-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-21 09:20:36.972542 async_extensions-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2578 2023-05-21 09:20:36.972542 async_extensions-1.4.0/README.md
+-rw-r--r--   0        0        0     2968 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/__init__.py
+-rw-r--r--   0        0        0      732 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/blocking.py
+-rw-r--r--   0        0        0      431 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/cancel.py
+-rw-r--r--   0        0        0     1174 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/channel.py
+-rw-r--r--   0        0        0     1583 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/close.py
+-rw-r--r--   0        0        0     7800 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/collect.py
+-rw-r--r--   0        0        0      118 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/constants.py
+-rw-r--r--   0        0        0       80 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/current.py
+-rw-r--r--   0        0        0       88 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/errors.py
+-rw-r--r--   0        0        0      101 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/file.py
+-rw-r--r--   0        0        0      174 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/low_level.py
+-rw-r--r--   0        0        0       44 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/path.py
+-rw-r--r--   0        0        0       87 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/process.py
+-rw-r--r--   0        0        0        0 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/py.typed
+-rw-r--r--   0        0        0      396 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/run.py
+-rw-r--r--   0        0        0       76 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/signal.py
+-rw-r--r--   0        0        0       77 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/sleep.py
+-rw-r--r--   0        0        0     1319 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/standard.py
+-rw-r--r--   0        0        0      143 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/synchronization.py
+-rw-r--r--   0        0        0      243 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/task_group.py
+-rw-r--r--   0        0        0      176 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/types.py
+-rw-r--r--   0        0        0      732 2023-05-21 09:20:36.972542 async_extensions-1.4.0/async_extensions/wait.py
+-rw-r--r--   0        0        0     2498 2023-05-21 09:20:36.972542 async_extensions-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 async_extensions-1.4.0/PKG-INFO
```

### Comparing `async_extensions-1.3.0/LICENSE` & `async_extensions-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_extensions-1.3.0/README.md` & `async_extensions-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^1.3.0"
+async-extensions = "^1.4.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

### Comparing `async_extensions-1.3.0/async_extensions/__init__.py` & `async_extensions-1.4.0/async_extensions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Asynchronous extensions."
 __url__ = "https://github.com/nekitdev/async-extensions"
 
 __title__ = "async_extensions"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
 from async_extensions.blocking import run_blocking_in_process, run_blocking_in_thread
 from async_extensions.cancel import CancelScope, create_cancel_scope, shield
 from async_extensions.channel import (
     MemoryChannel,
     MemoryChannelFactory,
     MemoryReceiveChannel,
```

### Comparing `async_extensions-1.3.0/async_extensions/blocking.py` & `async_extensions-1.4.0/async_extensions/blocking.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.3.0/async_extensions/channel.py` & `async_extensions-1.4.0/async_extensions/channel.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.3.0/async_extensions/close.py` & `async_extensions-1.4.0/async_extensions/close.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import abstractmethod as required
 from types import TracebackType as Traceback
 from typing import AsyncContextManager, Awaitable, Optional, Type, TypeVar, final
 
 from attrs import frozen
-from funcs.typing import AnyError
+from typing_aliases import AnyError
 from typing_extensions import Protocol, runtime_checkable
 
 from async_extensions.cancel import create_cancel_scope
 
 __all__ = (
     "AsyncCloseable",
     "AsyncClosing",
```

### Comparing `async_extensions-1.3.0/async_extensions/collect.py` & `async_extensions-1.4.0/async_extensions/collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Any, AsyncIterable, AsyncIterator, Awaitable, List, Tuple, TypeVar, overload
 
-from funcs.typing import AnyError, DynamicTuple, EmptyTuple
+from typing_aliases import (
+    AnyError, AnyIterable, DynamicTuple, EmptyTuple, is_async_iterable, is_iterable
+)
 from wraps.result import Error, Ok, Result
 
 from async_extensions.standard import iter_to_async_iter
 from async_extensions.task_group import create_task_group
-from async_extensions.typing import AnyIterable, is_async_iterable, is_iterable
 
 __all__ = ("collect", "collect_results", "collect_iterable", "collect_iterable_results")
 
 T = TypeVar("T")
 ErrorT = TypeVar("ErrorT", bound=AnyError)
```

### Comparing `async_extensions-1.3.0/async_extensions/standard.py` & `async_extensions-1.4.0/async_extensions/standard.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, AsyncIterable, AsyncIterator, Iterable, TypeVar, Union, overload
 
+from typing_aliases import is_instance
+
 from async_extensions.types import no_default
-from async_extensions.typing import is_instance
 
 __all__ = ("async_iter", "async_next", "iter_to_async_iter")
 
 NOT_ASYNC_ITERABLE = "{} is not an async iterable"
 NOT_ASYNC_ITERATOR = "{} is not an async iterator"
 
 T = TypeVar("T")
```

### Comparing `async_extensions-1.3.0/async_extensions/wait.py` & `async_extensions-1.4.0/async_extensions/wait.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.3.0/pyproject.toml` & `async_extensions-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-extensions"
-version = "1.3.0"
+version = "1.4.0"
 description = "Asynchronous extensions."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/async-extensions"
@@ -31,15 +31,18 @@
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
 attrs = ">= 23.1.0"
 
 anyio = ">= 3.6.2"
 solus = ">= 1.1.0"
-funcs = ">= 0.5.1"
+wraps = ">= 0.5.0"
+
+typing-aliases = ">= 1.1.0"
+typing-extensions = ">= 4.5.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
 black = "23.3.0"
 flake8-pyproject = "1.2.3"
@@ -94,15 +97,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "async-extensions"
-version = "1.3.0"
+version = "1.4.0"
 url = "https://github.com/nekitdev/async-extensions"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `async_extensions-1.3.0/PKG-INFO` & `async_extensions-1.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-extensions
-Version: 1.3.0
+Version: 1.4.0
 Summary: Asynchronous extensions.
 Home-page: https://github.com/nekitdev/async-extensions
 License: MIT
 Keywords: python,async,extensions
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: anyio (>=3.6.2)
 Requires-Dist: attrs (>=23.1.0)
-Requires-Dist: funcs (>=0.5.1)
 Requires-Dist: solus (>=1.1.0)
+Requires-Dist: typing-aliases (>=1.1.0)
+Requires-Dist: typing-extensions (>=4.5.0)
+Requires-Dist: wraps (>=0.5.0)
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/solus/issues
 Project-URL: Repository, https://github.com/nekitdev/async-extensions
 Description-Content-Type: text/markdown
 
 # `async-extensions`
@@ -67,15 +69,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^1.3.0"
+async-extensions = "^1.4.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

