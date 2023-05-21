# Comparing `tmp/wraps-0.5.0.tar.gz` & `tmp/wraps-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wraps-0.5.0.tar", max compression
+gzip compressed data, was "wraps-0.6.0.tar", max compression
```

## Comparing `wraps-0.5.0.tar` & `wraps-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1092 2023-05-14 13:50:08.282964 wraps-0.5.0/LICENSE
--rw-r--r--   0        0        0     6517 2023-05-14 13:50:08.282964 wraps-0.5.0/README.md
--rw-r--r--   0        0        0     3332 2023-05-14 13:50:08.286964 wraps-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2566 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/__init__.py
--rw-r--r--   0        0        0     2852 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/early.py
--rw-r--r--   0        0        0    15275 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/either.py
--rw-r--r--   0        0        0     1226 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/errors.py
--rw-r--r--   0        0        0     4377 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/future.py
--rw-r--r--   0        0        0     1360 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/future_either.py
--rw-r--r--   0        0        0    12014 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/future_option.py
--rw-r--r--   0        0        0    15807 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/future_result.py
--rw-r--r--   0        0        0      340 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/markers.py
--rw-r--r--   0        0        0    41149 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/option.py
--rw-r--r--   0        0        0        0 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/py.typed
--rw-r--r--   0        0        0     1809 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/reawaitable.py
--rw-r--r--   0        0        0    53507 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/result.py
--rw-r--r--   0        0        0      853 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/typing.py
--rw-r--r--   0        0        0      604 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/utils.py
--rw-r--r--   0        0        0     9422 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/wraps.py
--rw-r--r--   0        0        0     7769 1970-01-01 00:00:00.000000 wraps-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-21 09:34:54.330970 wraps-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6517 2023-05-21 09:34:54.330970 wraps-0.6.0/README.md
+-rw-r--r--   0        0        0     3331 2023-05-21 09:34:54.330970 wraps-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2566 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/__init__.py
+-rw-r--r--   0        0        0     2854 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/early.py
+-rw-r--r--   0        0        0    15277 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/either.py
+-rw-r--r--   0        0        0     1228 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/errors.py
+-rw-r--r--   0        0        0     4379 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/future.py
+-rw-r--r--   0        0        0     1360 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/future_either.py
+-rw-r--r--   0        0        0    12016 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/future_option.py
+-rw-r--r--   0        0        0    15809 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/future_result.py
+-rw-r--r--   0        0        0      340 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/markers.py
+-rw-r--r--   0        0        0    41151 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/option.py
+-rw-r--r--   0        0        0        0 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/py.typed
+-rw-r--r--   0        0        0     1811 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/reawaitable.py
+-rw-r--r--   0        0        0    53509 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/result.py
+-rw-r--r--   0        0        0      855 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/typing.py
+-rw-r--r--   0        0        0      604 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/utils.py
+-rw-r--r--   0        0        0     9424 2023-05-21 09:34:54.330970 wraps-0.6.0/wraps/wraps.py
+-rw-r--r--   0        0        0     7767 1970-01-01 00:00:00.000000 wraps-0.6.0/PKG-INFO
```

### Comparing `wraps-0.5.0/LICENSE` & `wraps-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wraps-0.5.0/README.md` & `wraps-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add wraps
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-wraps = "^0.5.0"
+wraps = "^0.6.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.wraps]
 git = "https://github.com/nekitdev/wraps.git"
```

### Comparing `wraps-0.5.0/pyproject.toml` & `wraps-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wraps"
-version = "0.5.0"
+version = "0.6.0"
 description = "Meaningful and safe wrapping types."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/wraps"
@@ -31,15 +31,16 @@
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
 attrs = ">= 23.1.0"
 
 funcs = ">= 0.5.1"
-async-extensions = ">= 1.2.3"
+
+typing-aliases = ">= 1.1.0"
 typing-extensions = ">= 4.5.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
 black = "23.3.0"
@@ -69,22 +70,22 @@
 trio = "0.22.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.3"
-mkdocs-material = "9.1.12"
+mkdocs-material = "9.1.14"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
 version = "0.21.2"
 extras = ["python"]
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.2.0"
+changelogging = "1.3.0"
 
 [tool.black]
 line_length = 100
 
 [tool.flake8]
 max_line_length = 100
 ignore = [
@@ -141,15 +142,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "wraps"
-version = "0.5.0"
+version = "0.6.0"
 url = "https://github.com/nekitdev/wraps"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `wraps-0.5.0/wraps/__init__.py` & `wraps-0.6.0/wraps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __description__ = "Meaningful and safe wrapping types."
 __url__ = "https://github.com/nekitdev/wraps"
 
 __title__ = "wraps"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 from wraps.early import early_option, early_option_await, early_result, early_result_await
 from wraps.either import Either, Left, Right, is_left, is_right
 from wraps.errors import Panic, panic
 from wraps.future import Future
 from wraps.future_option import FutureOption
 from wraps.future_result import FutureResult
```

### Comparing `wraps-0.5.0/wraps/early.py` & `wraps-0.6.0/wraps/early.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Early returns."""
 
 from typing import Callable, TypeVar
 
 from funcs.decorators import wraps
-from funcs.typing import AsyncCallable
+from typing_aliases import AsyncCallable
 from typing_extensions import ParamSpec
 
 from wraps.errors import EarlyOption, EarlyResult
 from wraps.option import Null, Option
 from wraps.result import Error, Result
 
 __all__ = ("early_option", "early_option_await", "early_result", "early_result_await")
```

### Comparing `wraps-0.5.0/wraps/either.py` & `wraps-0.6.0/wraps/either.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from __future__ import annotations
 
 from abc import abstractmethod as required
 from typing import AsyncIterator, Iterator, TypeVar, Union
 
 from attrs import frozen
-from funcs.typing import (
+from typing_aliases import (
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
     Predicate,
```

### Comparing `wraps-0.5.0/wraps/errors.py` & `wraps-0.6.0/wraps/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Panics and early return errors."""
 
 from typing import Generic, TypeVar
 
-from funcs.typing import AnyError
+from typing_aliases import AnyError
 from typing_extensions import Never
 
 __all__ = ("Panic", "panic", "EarlyOption", "EarlyResult")
 
 
 class Panic(AnyError):
     """Represents panics as errors.
```

### Comparing `wraps-0.5.0/wraps/future.py` & `wraps-0.6.0/wraps/future.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Asynchronous computation using futures."""
 
 from __future__ import annotations
 
 from typing import AsyncIterator, Awaitable, Generator, TypeVar
 
 from attrs import field, frozen
-from funcs.typing import AsyncUnary, Unary
+from typing_aliases import AsyncUnary, Unary
 
 from wraps.reawaitable import ReAwaitable
 from wraps.utils import async_identity, identity
 
 __all__ = ("Future",)
 
 T = TypeVar("T", covariant=True)
```

### Comparing `wraps-0.5.0/wraps/future_either.py` & `wraps-0.6.0/wraps/future_either.py`

 * *Files identical despite different names*

### Comparing `wraps-0.5.0/wraps/future_option.py` & `wraps-0.6.0/wraps/future_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Future optional values."""
 
 from __future__ import annotations
 
 from typing import Awaitable, Optional, Tuple, TypeVar, final
 
 from attrs import field, frozen
-from funcs.typing import (
+from typing_aliases import (
     AsyncBinary,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Binary,
     Inspect,
```

### Comparing `wraps-0.5.0/wraps/future_result.py` & `wraps-0.6.0/wraps/future_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Future error handling."""
 
 from __future__ import annotations
 
 from typing import Awaitable, TypeVar, final
 
 from attrs import field, frozen
-from funcs.typing import (
+from typing_aliases import (
     AnyError,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
```

### Comparing `wraps-0.5.0/wraps/option.py` & `wraps-0.6.0/wraps/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     TypeVar,
     Union,
     final,
     overload,
 )
 
 from attrs import frozen
-from funcs.typing import (
+from typing_aliases import (
     AsyncBinary,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Binary,
     Inspect,
```

### Comparing `wraps-0.5.0/wraps/reawaitable.py` & `wraps-0.6.0/wraps/reawaitable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Awaitable, Callable, Generator, TypeVar, final
 
 from attrs import define, field
 from funcs.decorators import wraps
-from funcs.typing import AsyncCallable
+from typing_aliases import AsyncCallable
 from typing_extensions import ParamSpec
 
 from wraps.option import Null, Option, Some
 
 __all__ = ("ReAwaitable", "reawaitable")
 
 P = ParamSpec("P")
```

### Comparing `wraps-0.5.0/wraps/result.py` & `wraps-0.6.0/wraps/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 from __future__ import annotations
 
 from abc import abstractmethod as required
 from typing import AsyncIterable, AsyncIterator, Iterable, Iterator, TypeVar, Union, final
 
 from attrs import frozen
-from funcs.typing import (
+from typing_aliases import (
     AnyError,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
```

### Comparing `wraps-0.5.0/wraps/typing.py` & `wraps-0.6.0/wraps/typing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable, TypeVar
 
-from funcs.typing import Binary, Nullary, Quaternary, Ternary, Unary
+from typing_aliases import Binary, Nullary, Quaternary, Ternary, Unary
 from typing_extensions import ParamSpec
 
 from wraps.future import Future
 
 __all__ = (
     "FutureCallable",
     "FutureNullary",
```

### Comparing `wraps-0.5.0/wraps/utils.py` & `wraps-0.6.0/wraps/utils.py`

 * *Files identical despite different names*

### Comparing `wraps-0.5.0/wraps/wraps.py` & `wraps-0.6.0/wraps/wraps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from typing import Callable, Generic, Optional, Type, TypeVar, final
 
 from attrs import frozen
 from funcs.decorators import wraps
-from funcs.typing import AnyError, AsyncCallable, NormalError
+from typing_aliases import AnyError, AsyncCallable, NormalError
 from typing_extensions import ParamSpec
 
 from wraps.either import Either
 from wraps.future import Future
 from wraps.future_either import FutureEither
 from wraps.future_option import FutureOption
 from wraps.future_result import FutureResult
```

### Comparing `wraps-0.5.0/PKG-INFO` & `wraps-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wraps
-Version: 0.5.0
+Version: 0.6.0
 Summary: Meaningful and safe wrapping types.
 Home-page: https://github.com/nekitdev/wraps
 License: MIT
 Keywords: python,future,either,option,result
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: async-extensions (>=1.2.3)
 Requires-Dist: attrs (>=23.1.0)
 Requires-Dist: funcs (>=0.5.1)
+Requires-Dist: typing-aliases (>=1.1.0)
 Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Documentation, https://nekitdev.github.io/wraps
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/wraps/issues
 Project-URL: Repository, https://github.com/nekitdev/wraps
 Description-Content-Type: text/markdown
@@ -72,15 +72,15 @@
 $ poetry add wraps
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-wraps = "^0.5.0"
+wraps = "^0.6.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.wraps]
 git = "https://github.com/nekitdev/wraps.git"
```

