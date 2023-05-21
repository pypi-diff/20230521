# Comparing `tmp/changelogging-1.2.0.tar.gz` & `tmp/changelogging-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelogging-1.2.0.tar", max compression
+gzip compressed data, was "changelogging-1.3.0.tar", max compression
```

## Comparing `changelogging-1.2.0.tar` & `changelogging-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1092 2023-05-10 15:46:44.941030 changelogging-1.2.0/LICENSE
--rw-r--r--   0        0        0     3098 2023-05-10 15:46:44.941030 changelogging-1.2.0/README.md
--rw-r--r--   0        0        0      517 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/__init__.py
--rw-r--r--   0        0        0      122 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/__main__.py
--rw-r--r--   0        0        0     9824 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/build.py
--rw-r--r--   0        0        0      810 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/changelogging.toml
--rw-r--r--   0        0        0    13857 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/config.py
--rw-r--r--   0        0        0      645 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/constants.py
--rw-r--r--   0        0        0     6040 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/fragments.py
--rw-r--r--   0        0        0      803 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/git.py
--rw-r--r--   0        0        0     2966 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/main.py
--rw-r--r--   0        0        0        0 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/py.typed
--rw-r--r--   0        0        0      321 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/typing.py
--rw-r--r--   0        0        0     1443 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/utils.py
--rw-r--r--   0        0        0     3545 2023-05-10 15:46:44.941030 changelogging-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4610 1970-01-01 00:00:00.000000 changelogging-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-21 12:44:39.051866 changelogging-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3098 2023-05-21 12:44:39.051866 changelogging-1.3.0/README.md
+-rw-r--r--   0        0        0      517 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/__main__.py
+-rw-r--r--   0        0        0     9826 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/build.py
+-rw-r--r--   0        0        0      810 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/changelogging.toml
+-rw-r--r--   0        0        0    13796 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/config.py
+-rw-r--r--   0        0        0      645 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/constants.py
+-rw-r--r--   0        0        0     6009 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/fragments.py
+-rw-r--r--   0        0        0      797 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/git.py
+-rw-r--r--   0        0        0     2966 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/main.py
+-rw-r--r--   0        0        0        0 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/py.typed
+-rw-r--r--   0        0        0      915 2023-05-21 12:44:39.051866 changelogging-1.3.0/changelogging/utils.py
+-rw-r--r--   0        0        0     3573 2023-05-21 12:44:39.051866 changelogging-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4650 1970-01-01 00:00:00.000000 changelogging-1.3.0/PKG-INFO
```

### Comparing `changelogging-1.2.0/LICENSE` & `changelogging-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `changelogging-1.2.0/README.md` & `changelogging-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add changelogging
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-changelogging = "^1.2.0"
+changelogging = "^1.3.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.changelogging]
 git = "https://github.com/nekitdev/changelogging.git"
```

### Comparing `changelogging-1.2.0/changelogging/__init__.py` & `changelogging-1.3.0/changelogging/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 
 __description__ = "Building changelogs from fragments."
 __url__ = "https://github.com/nekitdev/changelogging"
 
 __title__ = "changelogging"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 from changelogging.build import Builder
 from changelogging.config import Config
 from changelogging.fragments import Display, Fragment, FragmentType, FragmentTypes, Issue
 
 __all__ = ("Builder", "Config", "Display", "Fragment", "FragmentType", "FragmentTypes", "Issue")
```

### Comparing `changelogging-1.2.0/changelogging/build.py` & `changelogging-1.3.0/changelogging/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections import defaultdict as default_dict
 from pathlib import Path
 from textwrap import wrap
 from typing import Dict, Iterable, Iterator, List, Mapping, Tuple, TypeVar
 
 from attrs import define, field
-from funcs.typing import Binary, Unary
 from funcs.unpacking import unpack_binary
 from iters.iters import iter, wrap_iter
 from pendulum import Date
+from typing_aliases import Binary, Unary
 
 from changelogging.config import Config
 from changelogging.constants import (
     DEFAULT_ENCODING,
     DEFAULT_ERRORS,
     DOT,
     DOUBLE_NEW_LINE,
```

### Comparing `changelogging-1.2.0/changelogging/changelogging.toml` & `changelogging-1.3.0/changelogging/changelogging.toml`

 * *Files identical despite different names*

### Comparing `changelogging-1.2.0/changelogging/config.py` & `changelogging-1.3.0/changelogging/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from pathlib import Path
 from typing import Any, Iterable, Optional, Type, TypeVar, cast, overload
 
 import toml
 from attrs import define
-from funcs.typing import Unary
 from iters.iters import iter
-from iters.utils import empty
+from iters.utils import contains_only_item, empty
+from typing_aliases import IntoPath, StringDict, Unary
 from versions.functions import parse_version
 from versions.version import Version
 from wraps.option import Option, Some
 from wraps.wraps import wrap_optional
 from yarl import URL
 
 from changelogging.constants import (
     DEFAULT_ENCODING,
     DEFAULT_ERRORS,
     DEFAULT_IGNORE_REQUIRED,
     EMPTY,
     ROOT,
 )
 from changelogging.fragments import AnyFragmentTypes, Display, FragmentType
-from changelogging.typing import IntoPath, StringDict
-from changelogging.utils import contains_only_item
 
 __all__ = ("Config", "ConfigData", "AnyConfigData")
 
 CHANGELOGGING = "changelogging.toml"
 PYPROJECT = "pyproject.toml"
 
 SEARCH = (CHANGELOGGING, PYPROJECT)
```

### Comparing `changelogging-1.2.0/changelogging/constants.py` & `changelogging-1.3.0/changelogging/constants.py`

 * *Files identical despite different names*

### Comparing `changelogging-1.2.0/changelogging/fragments.py` & `changelogging-1.3.0/changelogging/fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Any, Generic, Iterable, Iterator, Type, TypeVar
 
 from attrs import field, frozen
-from funcs.typing import DynamicTuple
 from iters.mappings import merge
-
-from changelogging.typing import StringDict
+from typing_aliases import DynamicTuple, StringDict
 
 __all__ = ("Display", "Fragment", "FragmentType", "FragmentTypes", "AnyFragmentTypes", "Issue")
 
 SUFFIX = ".{}"
 suffix = SUFFIX.format
```

### Comparing `changelogging-1.2.0/changelogging/git.py` & `changelogging-1.3.0/changelogging/git.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from subprocess import call
 from typing import Iterable, Sequence
 
-from funcs.typing import DynamicTuple
+from iters.utils import unary_tuple
+from typing_aliases import DynamicTuple
 
 from changelogging.constants import DEFAULT_QUIET
-from changelogging.utils import unary_tuple
 
 __all__ = ("remove_command", "remove_paths")
 
 GIT = "git"
 REMOVE = "rm"
 QUIET = "-q"
 FORCE = "-f"
```

### Comparing `changelogging-1.2.0/changelogging/main.py` & `changelogging-1.3.0/changelogging/main.py`

 * *Files identical despite different names*

### Comparing `changelogging-1.2.0/changelogging/utils.py` & `changelogging-1.3.0/changelogging/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-from typing import Sized, Tuple, TypeVar
-
 from pendulum import Date, now, parse
 
 __all__ = (
     "left_strip",
     "right_strip",
     "split_lines",
     "starts_with",
-    "unary_tuple",
-    "contains_only_item",
     "parse_date",
     "today",
 )
 
 left_strip = str.lstrip
 """An alias of [`str.lstrip`][str.lstrip]."""
 right_strip = str.rstrip
@@ -20,37 +16,14 @@
 
 split_lines = str.splitlines
 """An alias of [`str.splitlines`][str.splitlines]."""
 starts_with = str.startswith
 """An alias of [`str.startswith`][str.startswith]."""
 
 
-T = TypeVar("T")
-
-
-def unary_tuple(item: T) -> Tuple[T]:
-    """Creates an unary tuple containing the `item`.
-
-    Returns:
-        An unary tuple containing the `item`.
-    """
-    return (item,)  # pragma: no cover  # used in CLI
-
-
-ONE = 1
-
-
-def contains_only_item(items: Sized) -> bool:
-    """Checks if there is only one item in `items`.
-
-    Returns:
-        Whether there is only one item in `items`."""
-    return len(items) == ONE
-
-
 def parse_date(string: str) -> Date:
     """Parses `YYYY-MM-DD` strings into dates.
 
     Arguments:
         string: The string to parse.
 
     Returns:
```

### Comparing `changelogging-1.2.0/pyproject.toml` & `changelogging-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "changelogging"
-version = "1.2.0"
+version = "1.3.0"
 description = "Building changelogs from fragments."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/changelogging"
@@ -36,23 +36,24 @@
 python = ">= 3.7"
 
 attrs = ">= 23.1.0"
 click = ">= 8.1.3"
 toml = ">= 0.10.2"
 yarl = ">= 1.9.2"
 
+typing-aliases = ">= 1.1.1"
 typing-extensions = ">= 4.5.0"
 
 pendulum = ">= 2.1.2"
 
 entrypoint = ">= 1.4.0"
 versions = ">= 1.4.0"
-funcs = ">= 0.5.1"
-wraps = ">= 0.4.0"
-iters = ">= 0.12.0"
+funcs = ">= 0.6.0"
+wraps = ">= 0.5.0"
+iters = ">= 0.13.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
 black = "23.3.0"
 flake8-pyproject = "1.2.3"
@@ -65,15 +66,15 @@
 version = "6.0.0"
 python = ">= 3.8.1"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "1.2.0"
+mypy = "1.3.0"
 
 types-toml = "0.10.8.6"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
@@ -81,15 +82,15 @@
 pytest-cov = "4.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.3"
-mkdocs-material = "9.1.11"
+mkdocs-material = "9.1.14"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
 version = "0.21.2"
 extras = ["python"]
 
 [tool.black]
 line_length = 100
@@ -149,15 +150,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "changelogging"
-version = "1.2.0"
+version = "1.3.0"
 url = "https://github.com/nekitdev/changelogging"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `changelogging-1.2.0/PKG-INFO` & `changelogging-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelogging
-Version: 1.2.0
+Version: 1.3.0
 Summary: Building changelogs from fragments.
 Home-page: https://github.com/nekitdev/changelogging
 License: MIT
 Keywords: python,changelog,changes
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,21 +18,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: attrs (>=23.1.0)
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: entrypoint (>=1.4.0)
-Requires-Dist: funcs (>=0.5.1)
-Requires-Dist: iters (>=0.12.0)
+Requires-Dist: funcs (>=0.6.0)
+Requires-Dist: iters (>=0.13.0)
 Requires-Dist: pendulum (>=2.1.2)
 Requires-Dist: toml (>=0.10.2)
+Requires-Dist: typing-aliases (>=1.1.1)
 Requires-Dist: typing-extensions (>=4.5.0)
 Requires-Dist: versions (>=1.4.0)
-Requires-Dist: wraps (>=0.4.0)
+Requires-Dist: wraps (>=0.5.0)
 Requires-Dist: yarl (>=1.9.2)
 Project-URL: Documentation, https://nekitdev.github.io/changelogging
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/changelogging/issues
 Project-URL: Repository, https://github.com/nekitdev/changelogging
 Description-Content-Type: text/markdown
@@ -79,15 +80,15 @@
 $ poetry add changelogging
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-changelogging = "^1.2.0"
+changelogging = "^1.3.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.changelogging]
 git = "https://github.com/nekitdev/changelogging.git"
```

