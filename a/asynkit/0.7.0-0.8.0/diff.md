# Comparing `tmp/asynkit-0.7.0.tar.gz` & `tmp/asynkit-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynkit-0.7.0.tar", max compression
+gzip compressed data, was "asynkit-0.8.0.tar", max compression
```

## Comparing `asynkit-0.7.0.tar` & `asynkit-0.8.0.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0     1081 2023-03-26 20:21:08.716572 asynkit-0.7.0/LICENSE
--rw-r--r--   0        0        0    17826 2023-03-26 20:21:08.716572 asynkit-0.7.0/README.md
--rw-r--r--   0        0        0     1654 2023-03-26 20:21:08.716572 asynkit-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      173 2023-03-26 20:21:08.716572 asynkit-0.7.0/src/asynkit/__init__.py
--rw-r--r--   0        0        0    12701 2023-03-26 20:21:08.716572 asynkit-0.7.0/src/asynkit/coroutine.py
--rw-r--r--   0        0        0    10701 2023-03-26 20:21:08.716572 asynkit-0.7.0/src/asynkit/eventloop.py
--rw-r--r--   0        0        0        0 2023-03-26 20:21:08.716572 asynkit-0.7.0/src/asynkit/experimental/__init__.py
--rw-r--r--   0        0        0     4293 2023-03-26 20:21:08.716572 asynkit-0.7.0/src/asynkit/experimental/anyio.py
--rw-r--r--   0        0        0    10598 2023-03-26 20:21:08.716572 asynkit-0.7.0/src/asynkit/monitor.py
--rw-r--r--   0        0        0        0 2023-03-26 20:21:08.716572 asynkit-0.7.0/src/asynkit/py.typed
--rw-r--r--   0        0        0     1300 2023-03-26 20:21:08.720572 asynkit-0.7.0/src/asynkit/tools.py
--rw-r--r--   0        0        0    18776 1970-01-01 00:00:00.000000 asynkit-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-21 13:35:17.074606 asynkit-0.8.0/LICENSE
+-rw-r--r--   0        0        0    18163 2023-05-21 13:35:17.074606 asynkit-0.8.0/README.md
+-rw-r--r--   0        0        0     1884 2023-05-21 13:35:17.074606 asynkit-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      224 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/compat.py
+-rw-r--r--   0        0        0    12701 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/coroutine.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/experimental/__init__.py
+-rw-r--r--   0        0        0     4293 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/experimental/anyio.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/__init__.py
+-rw-r--r--   0        0        0     4164 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/default.py
+-rw-r--r--   0        0        0     4815 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/eventloop.py
+-rw-r--r--   0        0        0     2981 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/extensions.py
+-rw-r--r--   0        0        0     2922 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/schedulingloop.py
+-rw-r--r--   0        0        0      281 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/types.py
+-rw-r--r--   0        0        0    10597 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/monitor.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/py.typed
+-rw-r--r--   0        0        0     5352 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/scheduling.py
+-rw-r--r--   0        0        0     1209 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/tools.py
+-rw-r--r--   0        0        0    19113 1970-01-01 00:00:00.000000 asynkit-0.8.0/PKG-INFO
```

### Comparing `asynkit-0.7.0/LICENSE` & `asynkit-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asynkit-0.7.0/README.md` & `asynkit-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This module provides some handy tools for those wishing to have better control over the
 way Python's `asyncio` module does things.
 
 - Helper tools for controlling coroutine execution, such as `CoroStart` and `Monitor`
 - Utility classes such as `GeneratorObject`
 - Coroutine helpers such as `coro_iter()`
-- `asyncio` event-loop extensions
+- Scheduling helpers for `asyncio`, and extended event-loop implementations
 - _eager_ execution of Tasks
 - Limited support for `anyio` and `trio`.
 
 # Installation
 
 ```bash
 $ pip install asynkit
@@ -293,63 +293,23 @@
 the same way as an `AsyncGenerator` object.  It can be iterated over and supports the
 `asend()`, `athrow()` and `aclose()` methods.
 
 A `GeneratorObject` is a flexible way to asynchronously generate results without
 resorting to `Task` and `Queue` objects.
 
 
-# Event loop tools
+# Scheduling tools
 
-Also provided is a mixin for the built-in event loop implementations in python, providing some primitives for advanced
-scheduling of tasks.
-
-## `SchedulingMixin` mixin class
-
-This class adds some handy scheduling functions to the event loop. They primarily
-work with the _ready queue_, a queue of callbacks representing tasks ready
-to be executed.
-
-- `ready_len(self)` - returns the length of the ready queue
-- `ready_pop(self, pos=-1)` - pops an entry off the queue
-- `ready_insert(self, pos, element)` - inserts a previously popped element into the queue
-- `ready_rotate(self, n)` - rotates the queue
-- `call_insert(self, pos, ...)` - schedules a callback at position `pos` in the queue
-
-## Concrete event loop classes
-
-Concrete subclasses of Python's built-in event loop classes are provided.
-
-- `SchedulingSelectorEventLoop` is a subclass of `asyncio.SelectorEventLoop` with the `SchedulingMixin`
-- `SchedulingProactorEventLoop` is a subclass of `asyncio.ProactorEventLoop` with the `SchedulingMixin` on those platforms that support it.
-
-## Event Loop Policy
-
-A policy class is provided to automatically create the appropriate event loops.
-
-- `SchedulingEventLoopPolicy` is a subclass of `asyncio.DefaultEventLoopPolicy` which instantiates either of the above event loop classes as appropriate.
-
-Use this either directly:
-
-```python
-asyncio.set_event_loop_policy(asynkit.SchedulingEventLoopPolicy())
-asyncio.run(myprogram())
-```
-
-or with a context manager:
-
-```python
-with asynkit.event_loop_policy():
-    asyncio.run(myprogram())
-```
+A set of functions are provided to perform advanced scheduling of `Task` objects
+with `asyncio`.  They work with the built-in event loop, and also with any eventloop
+implementing the `AbstractSchedulingLoop` abstract base class, such as the `SchedulingMixin`
+class which can be used to extend the built-in event loops.
 
 ## Scheduling functions
 
-A couple of functions are provided making use of these scheduling features.
-They require a `SchedulingMixin` event loop to be current.
-
 ### `sleep_insert(pos)`
 
 Similar to `asyncio.sleep()` but sleeps only for `pos` places in the runnable queue.
 Whereas `asyncio.sleep(0)` will place the executing task at the end of the queue, which is
 appropriate for fair scheduling, in some advanced cases you want to wake up sooner than that, perhaps
 after a specific task.
 
@@ -386,29 +346,73 @@
 up right after it blocks. The effect is similar to using `asynkit.eager()` but
 it achieves its goals solely by modifying the runnable queue. A `Task` is always
 created, unlike `eager`, which only creates a task if the target blocks.
 
 ## Runnable task helpers
 
 A few functions are added to help working with tasks.
-They require a `SchedulingMixin` event loop to be current.
 
 The following identity applies:
 ```python
-asyncio.all_tasks(loop) = asynkit.runnable_tasks(loop) | asynkit.blocked_tasks(loop) | {asyncio.current_task(loop)}
+asyncio.all_tasks() = asynkit.runnable_tasks() | asynkit.blocked_tasks() | asyncio.current_task()
 ```
 
 ### `runnable_tasks(loop=None)`
 
 Returns a set of the tasks that are currently runnable in the given loop
 
 ### `blocked_tasks(loop=None)`
 
 Returns a set of the tasks that are currently blocked on some future in the given loop.
 
+## Event Loop tools
+
+Also provided is a mixin for the built-in event loop implementations in python, providing some primitives for advanced scheduling of tasks.  These primitives are what is used by the
+scheduling functions above, and so custom event loop implementations can provide custom
+implementations of these methods.
+
+### `SchedulingMixin` mixin class
+
+This class adds some handy scheduling functions to the event loop. They primarily
+work with the _ready queue_, a queue of callbacks representing tasks ready
+to be executed.
+
+- `ready_len(self)` - returns the length of the ready queue
+- `ready_pop(self, pos=-1)` - pops an entry off the queue
+- `ready_insert(self, pos, element)` - inserts a previously popped element into the queue
+- `ready_rotate(self, n)` - rotates the queue
+- `call_insert(self, pos, ...)` - schedules a callback at position `pos` in the queue
+
+### Concrete event loop classes
+
+Concrete subclasses of Python's built-in event loop classes are provided.
+
+- `SchedulingSelectorEventLoop` is a subclass of `asyncio.SelectorEventLoop` with the `SchedulingMixin`
+- `SchedulingProactorEventLoop` is a subclass of `asyncio.ProactorEventLoop` with the `SchedulingMixin` on those platforms that support it.
+
+### Event Loop Policy
+
+A policy class is provided to automatically create the appropriate event loops.
+
+- `SchedulingEventLoopPolicy` is a subclass of `asyncio.DefaultEventLoopPolicy` which instantiates either of the above event loop classes as appropriate.
+
+Use this either directly:
+
+```python
+asyncio.set_event_loop_policy(asynkit.SchedulingEventLoopPolicy())
+asyncio.run(myprogram())
+```
+
+or with a context manager:
+
+```python
+with asynkit.event_loop_policy():
+    asyncio.run(myprogram())
+```
+
 # Coroutine helpers
 
 A couple of functions are provided to introspect the state of coroutine objects. They
 work on both regular __async__ coroutines, __classic__ coroutines (using `yield from`) and
 __async generators__.
 
 - `coro_is_new(coro)` -
```

### Comparing `asynkit-0.7.0/pyproject.toml` & `asynkit-0.8.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asynkit"
-version = "0.7.0"
+version = "0.8.0"
 description = "Async toolkit for advanced scheduling"
 authors = ["Kristján Valur Jónsson <sweskman@gmail.com>"]
 repository = "https://github.com/kristjanvalur/py-asynkit"
 readme = "README.md"
 keywords = ["asyncio", "eventloop"]
 license = "MIT"
 classifiers = [
@@ -39,37 +39,50 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 #addopts = "-ra -q"
 testpaths = [
     "tests",
 ]
+filterwarnings = [
+    'ignore:You seem to already have a custom sys.excepthook:RuntimeWarning'
+]
 
 [tool.ruff]
+select = [
+    "E", "F", "I",
+]
+src = ["src", ]
 # Ignore `F401` (unused import) in all `__init__.py` files
 # Ignore `F403` (importing *) in all `__init__.py` files
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
 
 [tool.mypy]
 
 [[tool.mypy.overrides]]
 module = "asynkit.*"
 strict = true
 
 [[tool.mypy.overrides]]
-module = "asynkit.eventloop"
+module = [
+    "asynkit.loop.eventloop",
+    "asynkit.compat",
+    "asynkit.tools",
+]
 warn_unused_ignores=false
 
 [[tool.mypy.overrides]]
-module = "asynkit.tools"
-warn_unused_ignores=false
+module = "asynkit.compat"
+disable_error_code="call-arg"
+
 
 [tool.coverage.report]
 exclude_lines = [
   "pragma: no cover",
   "@overload",
+  "@abstractmethod",
   "assert False",
   "TYPE_CHECKING",
   "PYTHON_37",
   "PYTHON_38",
   ]
```

### Comparing `asynkit-0.7.0/src/asynkit/coroutine.py` & `asynkit-0.8.0/src/asynkit/coroutine.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.7.0/src/asynkit/experimental/anyio.py` & `asynkit-0.8.0/src/asynkit/experimental/anyio.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import contextlib
-from typing import Any, AsyncIterator, Callable, Coroutine, Optional, Type
 from types import TracebackType
+from typing import Any, AsyncIterator, Callable, Coroutine, Optional, Type
 
 import pytest
 from anyio import create_task_group
 from anyio.abc import TaskGroup, TaskStatus
 
 from asynkit import CoroStart
```

### Comparing `asynkit-0.7.0/src/asynkit/monitor.py` & `asynkit-0.8.0/src/asynkit/monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import sys
 import types
 from types import TracebackType
 from typing import (
     Any,
-    AsyncIterator,
     AsyncGenerator,
+    AsyncIterator,
     Awaitable,
     Callable,
     Coroutine,
     Generator,
     Generic,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
-
 from .coroutine import coro_is_finished, coro_is_new
 
 T = TypeVar("T")
 V = TypeVar("V")
 T_co = TypeVar("T_co", covariant=True)
 T_contra = TypeVar("T_contra", contravariant=True)
```

### Comparing `asynkit-0.7.0/src/asynkit/tools.py` & `asynkit-0.8.0/src/asynkit/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import asyncio
 import sys
 from typing import (
+    TYPE_CHECKING,
     Any,
     Coroutine,
-    Generator,
-    Optional,
-    TypeVar,
-    Union,
     Deque,
     List,
-    TYPE_CHECKING,
+    Optional,
+    TypeVar,
 )
 
 # 3.8 or earlier
 PYTHON_38 = sys.version_info[:2] <= (3, 8)
 
 T = TypeVar("T")
-CoroLike = Union[Coroutine[Any, Any, T], Generator[Any, Any, T]]
 
 if TYPE_CHECKING:
     _TaskAny = asyncio.Task[Any]
 else:
     _TaskAny = asyncio.Task
 
 if PYTHON_38:  # pragma: no cover
```

### Comparing `asynkit-0.7.0/PKG-INFO` & `asynkit-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asynkit
-Version: 0.7.0
+Version: 0.8.0
 Summary: Async toolkit for advanced scheduling
 Home-page: https://github.com/kristjanvalur/py-asynkit
 License: MIT
 Keywords: asyncio,eventloop
 Author: Kristján Valur Jónsson
 Author-email: sweskman@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -28,15 +28,15 @@
 
 This module provides some handy tools for those wishing to have better control over the
 way Python's `asyncio` module does things.
 
 - Helper tools for controlling coroutine execution, such as `CoroStart` and `Monitor`
 - Utility classes such as `GeneratorObject`
 - Coroutine helpers such as `coro_iter()`
-- `asyncio` event-loop extensions
+- Scheduling helpers for `asyncio`, and extended event-loop implementations
 - _eager_ execution of Tasks
 - Limited support for `anyio` and `trio`.
 
 # Installation
 
 ```bash
 $ pip install asynkit
@@ -317,63 +317,23 @@
 the same way as an `AsyncGenerator` object.  It can be iterated over and supports the
 `asend()`, `athrow()` and `aclose()` methods.
 
 A `GeneratorObject` is a flexible way to asynchronously generate results without
 resorting to `Task` and `Queue` objects.
 
 
-# Event loop tools
+# Scheduling tools
 
-Also provided is a mixin for the built-in event loop implementations in python, providing some primitives for advanced
-scheduling of tasks.
-
-## `SchedulingMixin` mixin class
-
-This class adds some handy scheduling functions to the event loop. They primarily
-work with the _ready queue_, a queue of callbacks representing tasks ready
-to be executed.
-
-- `ready_len(self)` - returns the length of the ready queue
-- `ready_pop(self, pos=-1)` - pops an entry off the queue
-- `ready_insert(self, pos, element)` - inserts a previously popped element into the queue
-- `ready_rotate(self, n)` - rotates the queue
-- `call_insert(self, pos, ...)` - schedules a callback at position `pos` in the queue
-
-## Concrete event loop classes
-
-Concrete subclasses of Python's built-in event loop classes are provided.
-
-- `SchedulingSelectorEventLoop` is a subclass of `asyncio.SelectorEventLoop` with the `SchedulingMixin`
-- `SchedulingProactorEventLoop` is a subclass of `asyncio.ProactorEventLoop` with the `SchedulingMixin` on those platforms that support it.
-
-## Event Loop Policy
-
-A policy class is provided to automatically create the appropriate event loops.
-
-- `SchedulingEventLoopPolicy` is a subclass of `asyncio.DefaultEventLoopPolicy` which instantiates either of the above event loop classes as appropriate.
-
-Use this either directly:
-
-```python
-asyncio.set_event_loop_policy(asynkit.SchedulingEventLoopPolicy())
-asyncio.run(myprogram())
-```
-
-or with a context manager:
-
-```python
-with asynkit.event_loop_policy():
-    asyncio.run(myprogram())
-```
+A set of functions are provided to perform advanced scheduling of `Task` objects
+with `asyncio`.  They work with the built-in event loop, and also with any eventloop
+implementing the `AbstractSchedulingLoop` abstract base class, such as the `SchedulingMixin`
+class which can be used to extend the built-in event loops.
 
 ## Scheduling functions
 
-A couple of functions are provided making use of these scheduling features.
-They require a `SchedulingMixin` event loop to be current.
-
 ### `sleep_insert(pos)`
 
 Similar to `asyncio.sleep()` but sleeps only for `pos` places in the runnable queue.
 Whereas `asyncio.sleep(0)` will place the executing task at the end of the queue, which is
 appropriate for fair scheduling, in some advanced cases you want to wake up sooner than that, perhaps
 after a specific task.
 
@@ -410,29 +370,73 @@
 up right after it blocks. The effect is similar to using `asynkit.eager()` but
 it achieves its goals solely by modifying the runnable queue. A `Task` is always
 created, unlike `eager`, which only creates a task if the target blocks.
 
 ## Runnable task helpers
 
 A few functions are added to help working with tasks.
-They require a `SchedulingMixin` event loop to be current.
 
 The following identity applies:
 ```python
-asyncio.all_tasks(loop) = asynkit.runnable_tasks(loop) | asynkit.blocked_tasks(loop) | {asyncio.current_task(loop)}
+asyncio.all_tasks() = asynkit.runnable_tasks() | asynkit.blocked_tasks() | asyncio.current_task()
 ```
 
 ### `runnable_tasks(loop=None)`
 
 Returns a set of the tasks that are currently runnable in the given loop
 
 ### `blocked_tasks(loop=None)`
 
 Returns a set of the tasks that are currently blocked on some future in the given loop.
 
+## Event Loop tools
+
+Also provided is a mixin for the built-in event loop implementations in python, providing some primitives for advanced scheduling of tasks.  These primitives are what is used by the
+scheduling functions above, and so custom event loop implementations can provide custom
+implementations of these methods.
+
+### `SchedulingMixin` mixin class
+
+This class adds some handy scheduling functions to the event loop. They primarily
+work with the _ready queue_, a queue of callbacks representing tasks ready
+to be executed.
+
+- `ready_len(self)` - returns the length of the ready queue
+- `ready_pop(self, pos=-1)` - pops an entry off the queue
+- `ready_insert(self, pos, element)` - inserts a previously popped element into the queue
+- `ready_rotate(self, n)` - rotates the queue
+- `call_insert(self, pos, ...)` - schedules a callback at position `pos` in the queue
+
+### Concrete event loop classes
+
+Concrete subclasses of Python's built-in event loop classes are provided.
+
+- `SchedulingSelectorEventLoop` is a subclass of `asyncio.SelectorEventLoop` with the `SchedulingMixin`
+- `SchedulingProactorEventLoop` is a subclass of `asyncio.ProactorEventLoop` with the `SchedulingMixin` on those platforms that support it.
+
+### Event Loop Policy
+
+A policy class is provided to automatically create the appropriate event loops.
+
+- `SchedulingEventLoopPolicy` is a subclass of `asyncio.DefaultEventLoopPolicy` which instantiates either of the above event loop classes as appropriate.
+
+Use this either directly:
+
+```python
+asyncio.set_event_loop_policy(asynkit.SchedulingEventLoopPolicy())
+asyncio.run(myprogram())
+```
+
+or with a context manager:
+
+```python
+with asynkit.event_loop_policy():
+    asyncio.run(myprogram())
+```
+
 # Coroutine helpers
 
 A couple of functions are provided to introspect the state of coroutine objects. They
 work on both regular __async__ coroutines, __classic__ coroutines (using `yield from`) and
 __async generators__.
 
 - `coro_is_new(coro)` -
```

