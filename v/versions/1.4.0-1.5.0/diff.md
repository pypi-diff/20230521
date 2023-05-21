# Comparing `tmp/versions-1.4.0.tar.gz` & `tmp/versions-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versions-1.4.0.tar", max compression
+gzip compressed data, was "versions-1.5.0.tar", max compression
```

## Comparing `versions-1.4.0.tar` & `versions-1.5.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     1092 2023-05-17 21:34:32.173164 versions-1.4.0/LICENSE
--rw-r--r--   0        0        0     5452 2023-05-17 21:34:32.173164 versions-1.4.0/README.md
--rw-r--r--   0        0        0     3445 2023-05-17 21:34:32.173164 versions-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3488 2023-05-17 21:34:32.173164 versions-1.4.0/versions/__init__.py
--rw-r--r--   0        0        0      107 2023-05-17 21:34:32.173164 versions-1.4.0/versions/__main__.py
--rw-r--r--   0        0        0     2715 2023-05-17 21:34:32.173164 versions-1.4.0/versions/constants.py
--rw-r--r--   0        0        0      607 2023-05-17 21:34:32.173164 versions-1.4.0/versions/converters.py
--rw-r--r--   0        0        0     3473 2023-05-17 21:34:32.173164 versions-1.4.0/versions/converters_modern.py
--rw-r--r--   0        0        0     3466 2023-05-17 21:34:32.173164 versions-1.4.0/versions/converters_normal.py
--rw-r--r--   0        0        0     2267 2023-05-17 21:34:32.173164 versions-1.4.0/versions/converters_utils.py
--rw-r--r--   0        0        0      520 2023-05-17 21:34:32.173164 versions-1.4.0/versions/errors.py
--rw-r--r--   0        0        0     1934 2023-05-17 21:34:32.173164 versions-1.4.0/versions/functions.py
--rw-r--r--   0        0        0      709 2023-05-17 21:34:32.173164 versions-1.4.0/versions/main.py
--rw-r--r--   0        0        0     1032 2023-05-17 21:34:32.173164 versions-1.4.0/versions/meta.py
--rw-r--r--   0        0        0    28284 2023-05-17 21:34:32.173164 versions-1.4.0/versions/operators.py
--rw-r--r--   0        0        0     7989 2023-05-17 21:34:32.173164 versions-1.4.0/versions/parsers.py
--rw-r--r--   0        0        0     7816 2023-05-17 21:34:32.173164 versions-1.4.0/versions/patterns.py
--rw-r--r--   0        0        0     2602 2023-05-17 21:34:32.173164 versions-1.4.0/versions/phases.py
--rw-r--r--   0        0        0        0 2023-05-17 21:34:32.173164 versions-1.4.0/versions/py.typed
--rw-r--r--   0        0        0      429 2023-05-17 21:34:32.173164 versions-1.4.0/versions/representation.py
--rw-r--r--   0        0        0    21915 2023-05-17 21:34:32.173164 versions-1.4.0/versions/segments.py
--rw-r--r--   0        0        0     1008 2023-05-17 21:34:32.173164 versions-1.4.0/versions/specification.py
--rw-r--r--   0        0        0     7561 2023-05-17 21:34:32.173164 versions-1.4.0/versions/specifiers.py
--rw-r--r--   0        0        0     3656 2023-05-17 21:34:32.173164 versions-1.4.0/versions/string.py
--rw-r--r--   0        0        0     3076 2023-05-17 21:34:32.173164 versions-1.4.0/versions/types.py
--rw-r--r--   0        0        0      704 2023-05-17 21:34:32.177164 versions-1.4.0/versions/typing.py
--rw-r--r--   0        0        0     1288 2023-05-17 21:34:32.177164 versions-1.4.0/versions/utils.py
--rw-r--r--   0        0        0    27967 2023-05-17 21:34:32.177164 versions-1.4.0/versions/version.py
--rw-r--r--   0        0        0    40693 2023-05-17 21:34:32.177164 versions-1.4.0/versions/version_sets.py
--rw-r--r--   0        0        0     2655 2023-05-17 21:34:32.177164 versions-1.4.0/versions/versioned.py
--rw-r--r--   0        0        0     6788 1970-01-01 00:00:00.000000 versions-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-21 12:51:48.266841 versions-1.5.0/LICENSE
+-rw-r--r--   0        0        0     5452 2023-05-21 12:51:48.266841 versions-1.5.0/README.md
+-rw-r--r--   0        0        0     3468 2023-05-21 12:51:48.266841 versions-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3488 2023-05-21 12:51:48.266841 versions-1.5.0/versions/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-21 12:51:48.266841 versions-1.5.0/versions/__main__.py
+-rw-r--r--   0        0        0     2715 2023-05-21 12:51:48.266841 versions-1.5.0/versions/constants.py
+-rw-r--r--   0        0        0      607 2023-05-21 12:51:48.266841 versions-1.5.0/versions/converters.py
+-rw-r--r--   0        0        0     3473 2023-05-21 12:51:48.266841 versions-1.5.0/versions/converters_modern.py
+-rw-r--r--   0        0        0     3466 2023-05-21 12:51:48.266841 versions-1.5.0/versions/converters_normal.py
+-rw-r--r--   0        0        0     2267 2023-05-21 12:51:48.266841 versions-1.5.0/versions/converters_utils.py
+-rw-r--r--   0        0        0      520 2023-05-21 12:51:48.266841 versions-1.5.0/versions/errors.py
+-rw-r--r--   0        0        0     1934 2023-05-21 12:51:48.266841 versions-1.5.0/versions/functions.py
+-rw-r--r--   0        0        0      709 2023-05-21 12:51:48.266841 versions-1.5.0/versions/main.py
+-rw-r--r--   0        0        0     1032 2023-05-21 12:51:48.266841 versions-1.5.0/versions/meta.py
+-rw-r--r--   0        0        0    28283 2023-05-21 12:51:48.266841 versions-1.5.0/versions/operators.py
+-rw-r--r--   0        0        0     7989 2023-05-21 12:51:48.266841 versions-1.5.0/versions/parsers.py
+-rw-r--r--   0        0        0     7816 2023-05-21 12:51:48.266841 versions-1.5.0/versions/patterns.py
+-rw-r--r--   0        0        0     2602 2023-05-21 12:51:48.266841 versions-1.5.0/versions/phases.py
+-rw-r--r--   0        0        0        0 2023-05-21 12:51:48.266841 versions-1.5.0/versions/py.typed
+-rw-r--r--   0        0        0      429 2023-05-21 12:51:48.266841 versions-1.5.0/versions/representation.py
+-rw-r--r--   0        0        0    21914 2023-05-21 12:51:48.266841 versions-1.5.0/versions/segments.py
+-rw-r--r--   0        0        0     1025 2023-05-21 12:51:48.266841 versions-1.5.0/versions/specification.py
+-rw-r--r--   0        0        0     7560 2023-05-21 12:51:48.266841 versions-1.5.0/versions/specifiers.py
+-rw-r--r--   0        0        0     3650 2023-05-21 12:51:48.266841 versions-1.5.0/versions/string.py
+-rw-r--r--   0        0        0     3076 2023-05-21 12:51:48.266841 versions-1.5.0/versions/types.py
+-rw-r--r--   0        0        0     1288 2023-05-21 12:51:48.266841 versions-1.5.0/versions/utils.py
+-rw-r--r--   0        0        0    27967 2023-05-21 12:51:48.270841 versions-1.5.0/versions/version.py
+-rw-r--r--   0        0        0    40692 2023-05-21 12:51:48.270841 versions-1.5.0/versions/version_sets.py
+-rw-r--r--   0        0        0     2654 2023-05-21 12:51:48.270841 versions-1.5.0/versions/versioned.py
+-rw-r--r--   0        0        0     6828 1970-01-01 00:00:00.000000 versions-1.5.0/PKG-INFO
```

### Comparing `versions-1.4.0/LICENSE` & `versions-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/README.md` & `versions-1.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add versions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-versions = "^1.4.0"
+versions = "^1.5.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.versions]
 git = "https://github.com/nekitdev/versions.git"
@@ -148,15 +148,15 @@
 
 `versions` allows users to access versions of items that have the `__version__` attribute:
 
 ```python
 >>> from versions import get_version
 >>> import versions
 >>> get_version(versions)
-<Version (1.4.0)>
+<Version (1.5.0)>
 ```
 
 ## Documentation
 
 You can find the documentation [here][Documentation].
 
 ## Support
```

### Comparing `versions-1.4.0/pyproject.toml` & `versions-1.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "versions"
-version = "1.4.0"
+version = "1.5.0"
 description = "Parsing, inspecting and specifying versions."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/versions"
@@ -29,14 +29,16 @@
 [[tool.poetry.packages]]
 include = "versions"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
 attrs = ">= 23.1.0"
+
+typing-aliases = ">= 1.1.1"
 typing-extensions = ">= 4.5.0"
 
 click = ">= 8.1.3"
 
 orderings = ">= 1.1.0"
 solus = ">= 1.1.0"
 entrypoint = ">= 1.4.0"
@@ -71,22 +73,22 @@
 hypothesis = "6.75.3"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.3"
-mkdocs-material = "9.1.13"
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
@@ -108,15 +110,15 @@
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
     "raise InternalError",
     "def __repr__",
 ]
 
 [tool.coverage.html]
@@ -145,15 +147,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "versions"
-version = "1.4.0"
+version = "1.5.0"
 url = "https://github.com/nekitdev/versions"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `versions-1.4.0/versions/__init__.py` & `versions-1.5.0/versions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 __description__ = "Parsing, inspecting and specifying versions."
 __url__ = "https://github.com/nekitdev/versions"
 
 __title__ = "versions"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.3.0"
+__version__ = "1.5.0"
 
 from versions.converters import (
     simplify,
     specifier_from_version_set,
     specifier_to_version_set,
     version_set_from_specifier,
     version_set_to_specifier,
```

### Comparing `versions-1.4.0/versions/constants.py` & `versions-1.5.0/versions/constants.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/converters.py` & `versions-1.5.0/versions/converters.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/converters_modern.py` & `versions-1.5.0/versions/converters_modern.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/converters_normal.py` & `versions-1.5.0/versions/converters_normal.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/converters_utils.py` & `versions-1.5.0/versions/converters_utils.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/errors.py` & `versions-1.5.0/versions/errors.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/functions.py` & `versions-1.5.0/versions/functions.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/main.py` & `versions-1.5.0/versions/main.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/meta.py` & `versions-1.5.0/versions/meta.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/operators.py` & `versions-1.5.0/versions/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from enum import Enum
 from string import digits
 from typing import TYPE_CHECKING, Any, Mapping, Optional, Tuple, Type, TypeVar, Union
 
 from attrs import frozen
+from typing_aliases import Binary, Unary, is_same_type
 
 from versions.constants import (
     CARET,
     DOUBLE_EQUAL,
     EQUAL,
     GREATER,
     GREATER_OR_EQUAL,
@@ -21,15 +22,14 @@
     WILDCARD_DOUBLE_EQUAL,
     WILDCARD_EQUAL,
     WILDCARD_NOT_EQUAL,
 )
 from versions.errors import InternalError
 from versions.representation import Representation
 from versions.string import ToString, concat_empty_args, concat_space_args
-from versions.typing import Binary, Unary, is_same_type
 
 if TYPE_CHECKING:
     from versions.version import Version
     from versions.version_sets import VersionSet
 
     Matches = Binary[Version, Version, bool]
     """The `(version, against) -> bool` function."""
```

### Comparing `versions-1.4.0/versions/parsers.py` & `versions-1.5.0/versions/parsers.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/patterns.py` & `versions-1.5.0/versions/patterns.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/phases.py` & `versions-1.5.0/versions/phases.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/segments.py` & `versions-1.5.0/versions/segments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import ClassVar, Iterable, Optional, Set, Tuple, Type, TypeVar, Union
 
 from attrs import Attribute, evolve, field, frozen
 from named import get_type_name
+from typing_aliases import DynamicTuple, is_int
 
 from versions.constants import EMPTY
 from versions.parsers import TagParser
 from versions.phases import (
     PHASE_ALL_DEFAULT,
     PHASE_ALL_SET,
     PHASE_DEV_DEFAULT,
@@ -28,15 +29,14 @@
     concat_dot,
     concat_dot_args,
     concat_empty_args,
     split_dot,
     split_separators,
 )
 from versions.types import NegativeInfinity, negative_infinity
-from versions.typing import DynamicTuple, is_int
 from versions.utils import count_leading_zeros, fix_to_length
 
 __all__ = (
     # default values
     "DEFAULT_PARTS",
     "DEFAULT_VALUE",
     "DEFAULT_PADDING",
```

### Comparing `versions-1.4.0/versions/specification.py` & `versions-1.5.0/versions/specification.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
 
 from abc import abstractmethod as required
 from typing import TYPE_CHECKING, Any
 
+from typing_aliases import is_instance
 from typing_extensions import Protocol, TypeGuard, runtime_checkable
 
-from versions.typing import is_instance
-
 if TYPE_CHECKING:
     from versions.version import Version
 
-__all__ = ("Specification",)
+__all__ = ("Specification", "is_specification")
 
 EXPECTED_METHOD = "expected `{}` to define `{}` method"
 expected_method = EXPECTED_METHOD.format
 
 ACCEPTS = "accepts"
```

### Comparing `versions-1.4.0/versions/specifiers.py` & `versions-1.5.0/versions/specifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, ClassVar, Iterable
 
 from attrs import Attribute, field, frozen
+from typing_aliases import DynamicTuple, is_instance
 from typing_extensions import Literal, TypeGuard
 
 from versions.constants import EMPTY_VERSION, UNIVERSE_VERSION
 from versions.operators import Operator
 from versions.representation import Representation
 from versions.specification import Specification
 from versions.string import (
     ToString,
     concat_comma,
     concat_comma_space,
     concat_pipes,
     concat_pipes_spaced,
     create_wrap_around,
 )
-from versions.typing import DynamicTuple, is_instance
 from versions.utils import contains_only_item, first
 
 if TYPE_CHECKING:
     from versions.version import Version
 
 __all__ = (
     "NEVER",
```

### Comparing `versions-1.4.0/versions/string.py` & `versions-1.5.0/versions/string.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import abstractmethod as required
 from typing import Iterable, List, Type, TypeVar
 
+from typing_aliases import Parse
 from typing_extensions import Protocol, runtime_checkable
 
 from versions.constants import (
     BRACKETS,
     COMMA,
     COMMA_SPACE,
     DASH,
@@ -13,15 +14,14 @@
     DOUBLE_PIPE_SPACED,
     EMPTY,
     PIPE,
     SEPARATORS,
     SPACE,
     UNDER,
 )
-from versions.typing import Unary
 
 __all__ = (
     # simple from_string() and to_string() protocols
     "FromString",
     "ToString",
     "String",
     # checks
@@ -138,15 +138,15 @@
 
     return left + string + right
 
 
 create_translation = str.maketrans
 dict_from_keys = dict.fromkeys
 
-Split = Unary[str, List[str]]
+Split = Parse[List[str]]
 
 
 def create_split_multiple(main: str, *rest: str) -> Split:
     # the following implementation is faster than `re.split`
     # and it is fully suitable for parsing in this library
 
     table = create_translation(dict_from_keys(rest, main))
```

### Comparing `versions-1.4.0/versions/types.py` & `versions-1.5.0/versions/types.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/utils.py` & `versions-1.5.0/versions/utils.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/version.py` & `versions-1.5.0/versions/version.py`

 * *Files identical despite different names*

### Comparing `versions-1.4.0/versions/version_sets.py` & `versions-1.5.0/versions/version_sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Type,
     TypeVar,
     Union,
 )
 
 from attrs import Attribute, define, evolve, field, frozen
 from orderings import Ordering
+from typing_aliases import DynamicTuple, is_instance
 from typing_extensions import Literal, Protocol, TypeGuard, runtime_checkable
 
 from versions.constants import EMPTY_VERSION, UNIVERSE_VERSION
 from versions.errors import InternalError
 from versions.operators import Operator, OperatorType
 from versions.representation import Representation
 from versions.specification import Specification
@@ -27,15 +28,14 @@
     ToString,
     concat_comma,
     concat_comma_space,
     concat_pipes,
     concat_pipes_spaced,
 )
 from versions.types import Infinity, NegativeInfinity, infinity, negative_infinity
-from versions.typing import DynamicTuple, is_instance
 from versions.utils import contains_only_item, first, flatten, last, next_or_none, set_last
 
 if TYPE_CHECKING:
     from versions.version import Version
 
 __all__ = (
     "VersionEmpty",
```

### Comparing `versions-1.4.0/versions/versioned.py` & `versions-1.5.0/versions/versioned.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from builtins import hasattr as has_attribute
 from typing import Any, Optional, Type, TypeVar, overload
 
+from typing_aliases import is_string
 from typing_extensions import Protocol, TypeGuard, runtime_checkable
 
 from versions.functions import parse_version
-from versions.typing import is_string
 from versions.version import Version
 
 __all__ = (
     "VERSION",
     "Versioned",
     "is_versioned",
     "has_version",
```

### Comparing `versions-1.4.0/PKG-INFO` & `versions-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versions
-Version: 1.4.0
+Version: 1.5.0
 Summary: Parsing, inspecting and specifying versions.
 Home-page: https://github.com/nekitdev/versions
 License: MIT
 Keywords: python,semver,version
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,15 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: attrs (>=23.1.0)
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: entrypoint (>=1.4.0)
 Requires-Dist: orderings (>=1.1.0)
 Requires-Dist: solus (>=1.1.0)
+Requires-Dist: typing-aliases (>=1.1.1)
 Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Documentation, https://nekitdev.github.io/versions
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/versions/issues
 Project-URL: Repository, https://github.com/nekitdev/versions
 Description-Content-Type: text/markdown
@@ -74,15 +75,15 @@
 $ poetry add versions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-versions = "^1.4.0"
+versions = "^1.5.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.versions]
 git = "https://github.com/nekitdev/versions.git"
@@ -182,15 +183,15 @@
 
 `versions` allows users to access versions of items that have the `__version__` attribute:
 
 ```python
 >>> from versions import get_version
 >>> import versions
 >>> get_version(versions)
-<Version (1.4.0)>
+<Version (1.5.0)>
 ```
 
 ## Documentation
 
 You can find the documentation [here][Documentation].
 
 ## Support
```

