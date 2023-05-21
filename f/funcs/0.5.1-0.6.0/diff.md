# Comparing `tmp/funcs-0.5.1.tar.gz` & `tmp/funcs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs-0.5.1.tar", max compression
+gzip compressed data, was "funcs-0.6.0.tar", max compression
```

## Comparing `funcs-0.5.1.tar` & `funcs-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1092 2023-04-24 11:39:50.864242 funcs-0.5.1/LICENSE
--rw-r--r--   0        0        0     2872 2023-04-24 11:39:50.864242 funcs-0.5.1/README.md
--rw-r--r--   0        0        0     1714 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/__init__.py
--rw-r--r--   0        0        0      883 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/application.py
--rw-r--r--   0        0        0      856 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/callers.py
--rw-r--r--   0        0        0     5467 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/composition.py
--rw-r--r--   0        0        0      830 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/debug.py
--rw-r--r--   0        0        0      166 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/decorators.py
--rw-r--r--   0        0        0     6337 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/flow.py
--rw-r--r--   0        0        0     2259 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/functions.py
--rw-r--r--   0        0        0      418 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/getters.py
--rw-r--r--   0        0        0      782 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/primitives.py
--rw-r--r--   0        0        0        0 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/py.typed
--rw-r--r--   0        0        0     1111 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/reduction.py
--rw-r--r--   0        0        0     1031 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/types.py
--rw-r--r--   0        0        0     6633 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/typing.py
--rw-r--r--   0        0        0     2344 2023-04-24 11:39:50.864242 funcs-0.5.1/funcs/unpacking.py
--rw-r--r--   0        0        0     3022 2023-04-24 11:39:50.864242 funcs-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 funcs-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-21 12:34:46.585748 funcs-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2872 2023-05-21 12:34:46.585748 funcs-0.6.0/README.md
+-rw-r--r--   0        0        0     1714 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/__init__.py
+-rw-r--r--   0        0        0      883 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/application.py
+-rw-r--r--   0        0        0      857 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/callers.py
+-rw-r--r--   0        0        0     5470 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/composition.py
+-rw-r--r--   0        0        0      832 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/debug.py
+-rw-r--r--   0        0        0      166 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/decorators.py
+-rw-r--r--   0        0        0     6369 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/flow.py
+-rw-r--r--   0        0        0     2260 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/functions.py
+-rw-r--r--   0        0        0      418 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/getters.py
+-rw-r--r--   0        0        0      782 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/primitives.py
+-rw-r--r--   0        0        0        0 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/py.typed
+-rw-r--r--   0        0        0     1113 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/reduction.py
+-rw-r--r--   0        0        0     1031 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/types.py
+-rw-r--r--   0        0        0     2346 2023-05-21 12:34:46.589748 funcs-0.6.0/funcs/unpacking.py
+-rw-r--r--   0        0        0     3175 2023-05-21 12:34:46.589748 funcs-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 funcs-0.6.0/PKG-INFO
```

### Comparing `funcs-0.5.1/LICENSE` & `funcs-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs-0.5.1/README.md` & `funcs-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.5.1"
+funcs = "^0.6.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

### Comparing `funcs-0.5.1/funcs/__init__.py` & `funcs-0.6.0/funcs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Functional programming in Python."
 __url__ = "https://github.com/nekitdev/funcs"
 
 __title__ = "funcs"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 
 from funcs.application import apply, partial
 from funcs.callers import caller, method_caller
 from funcs.composition import compose, compose_once, pipe, pipe_once
 from funcs.debug import inspect, tap
 from funcs.decorators import wraps
 from funcs.flow import once, post_processing, reraise, reraise_with, suppress, wrap_with
```

### Comparing `funcs-0.5.1/funcs/application.py` & `funcs-0.6.0/funcs/application.py`

 * *Files identical despite different names*

### Comparing `funcs-0.5.1/funcs/callers.py` & `funcs-0.6.0/funcs/callers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from operator import methodcaller as standard_method_caller
 from typing import Any, TypeVar
 
+from typing_aliases import DynamicCallable, Unary
 from typing_extensions import ParamSpec
 
-from funcs.typing import DynamicCallable, Unary
-
 __all__ = ("caller", "method_caller")
 
 method_caller = standard_method_caller
 """An alias of the standard `method_caller` type that implements method calling."""
 
 P = ParamSpec("P")
```

### Comparing `funcs-0.5.1/funcs/composition.py` & `funcs-0.6.0/funcs/composition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, TypeVar, overload
 
+from typing_aliases import Unary
+
 from funcs.reduction import fold
-from funcs.typing import Unary
 
 __all__ = ("compose", "compose_once", "pipe", "pipe_once")
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 R = TypeVar("R")
```

### Comparing `funcs-0.5.1/funcs/debug.py` & `funcs-0.6.0/funcs/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, TypeVar
 
-from funcs.typing import Inspect
+from typing_aliases import Inspect
 
 __all__ = ("tap", "inspect")
 
 T = TypeVar("T")
 
 LABEL_STRING = "{}: {}"
 label_string = LABEL_STRING.format
```

### Comparing `funcs-0.5.1/funcs/flow.py` & `funcs-0.6.0/funcs/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+from types import TracebackType as Traceback
 from typing import Callable, Generic, Optional, Type, TypeVar, final, overload
 
 from attrs import frozen
-from typing_extensions import Literal, ParamSpec
-
-from funcs.decorators import wraps
-from funcs.types import MarkerOr, is_not_marker, marker
-from funcs.typing import (
+from typing_aliases import (
     AnyContextManager,
     AnyError,
     AnyErrorType,
     AnyErrorTypes,
     SimpleContextManager,
-    Traceback,
     Unary,
     is_subclass,
 )
+from typing_extensions import Literal, ParamSpec
+
+from funcs.decorators import wraps
+from funcs.types import MarkerOr, is_not_marker, marker
 
 __all__ = ("once", "reraise", "reraise_with", "suppress", "post_processing", "wrap_with")
 
 P = ParamSpec("P")
 
 R = TypeVar("R")
 S = TypeVar("S")
```

### Comparing `funcs-0.5.1/funcs/functions.py` & `funcs-0.6.0/funcs/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Callable, TypeVar
 
+from typing_aliases import AnyError, AsyncCallable, Binary, GenericPredicate, Nullary
 from typing_extensions import Never, ParamSpec
 
-from funcs.typing import AnyError, AsyncCallable, Binary, GenericPredicate, Nullary
-
 __all__ = ("asyncify", "identity", "always", "raises", "flip", "complement")
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 R = TypeVar("R")
```

### Comparing `funcs-0.5.1/funcs/primitives.py` & `funcs-0.6.0/funcs/primitives.py`

 * *Files identical despite different names*

### Comparing `funcs-0.5.1/funcs/reduction.py` & `funcs-0.6.0/funcs/reduction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import reduce as standard_reduce
 from typing import Iterable, TypeVar
 
-from funcs.typing import Binary
+from typing_aliases import Binary
 
 __all__ = ("reduce", "fold")
 
 T = TypeVar("T")
 U = TypeVar("U")
```

### Comparing `funcs-0.5.1/funcs/types.py` & `funcs-0.6.0/funcs/types.py`

 * *Files identical despite different names*

### Comparing `funcs-0.5.1/funcs/unpacking.py` & `funcs-0.6.0/funcs/unpacking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Tuple, TypeVar
 
-from funcs.typing import (
+from typing_aliases import (
     Binary,
     EmptyTuple,
     Nullary,
     Quaternary,
     Ternary,
     Unary,
     UnpackBinary,
```

### Comparing `funcs-0.5.1/pyproject.toml` & `funcs-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcs"
-version = "0.5.1"
+version = "0.6.0"
 description = "Functional programming in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/funcs"
@@ -28,54 +28,61 @@
 
 [[tool.poetry.packages]]
 include = "funcs"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
+typing-aliases = ">= 1.1.1"
 typing-extensions = ">= 4.5.0"
 
 solus = ">= 1.1.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
-black = "22.12.0"
+black = "23.3.0"
+flake8-pyproject = "1.2.3"
+
+[tool.poetry.group.format.dependencies.flake8]
+version = "6.0.0"
+python = ">= 3.8.1"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.11.4"
+version = "5.12.0"
+python = ">= 3.8"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "1.2.0"
+mypy = "1.3.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.1.3"
-pytest-cov = "3.0.0"
-hypothesis = "6.71.0"
+pytest = "7.3.1"
+pytest-cov = "4.0.0"
+hypothesis = "6.75.3"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.3.1"
-mkdocs-material = "8.5.3"
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.14"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
-version = "0.19.0"
+version = "0.21.2"
 extras = ["python"]
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.1.0"
+changelogging = "1.3.0"
 
 [tool.black]
 line_length = 100
 
 [tool.isort]
 line_length = 100
 profile = "black"
@@ -90,15 +97,15 @@
 [tool.coverage.report]
 ignore_errors = true
 exclude_lines = [
     "pragma: never",
     "pragma: no cover",
     "if TYPE_CHECKING",
     "@overload",
-    "@abstractmethod",
+    "@required",
     "raise NotImplementedError",
     "raise AssertionError",
     "def __repr__",
 ]
 
 [tool.coverage.html]
 directory = "coverage"
@@ -126,15 +133,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "funcs"
-version = "0.5.1"
+version = "0.6.0"
 url = "https://github.com/nekitdev/funcs"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `funcs-0.5.1/PKG-INFO` & `funcs-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs
-Version: 0.5.1
+Version: 0.6.0
 Summary: Functional programming in Python.
 Home-page: https://github.com/nekitdev/funcs
 License: MIT
 Keywords: python,function,functional,paradigm
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: solus (>=1.1.0)
+Requires-Dist: typing-aliases (>=1.1.1)
 Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Documentation, https://nekitdev.github.io/funcs
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/funcs/issues
 Project-URL: Repository, https://github.com/nekitdev/funcs
 Description-Content-Type: text/markdown
@@ -70,15 +71,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.5.1"
+funcs = "^0.6.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

