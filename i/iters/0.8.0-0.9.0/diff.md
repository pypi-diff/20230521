# Comparing `tmp/iters-0.8.0.tar.gz` & `tmp/iters-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iters-0.8.0.tar", max compression
+gzip compressed data, was "iters-0.9.0.tar", max compression
```

## Comparing `iters-0.8.0.tar` & `iters-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1092 2022-12-22 12:40:18.993079 iters-0.8.0/LICENSE
--rw-r--r--   0        0        0     3633 2022-12-22 12:40:18.997079 iters-0.8.0/README.md
--rw-r--r--   0        0        0     1613 2022-12-22 12:40:18.997079 iters-0.8.0/iters/__init__.py
--rw-r--r--   0        0        0    92726 2022-12-22 12:40:18.997079 iters-0.8.0/iters/async_iters.py
--rw-r--r--   0        0        0   122039 2022-12-22 12:40:18.997079 iters-0.8.0/iters/async_utils.py
--rw-r--r--   0        0        0     8192 2022-12-22 12:40:18.997079 iters-0.8.0/iters/concurrent.py
--rw-r--r--   0        0        0    98193 2022-12-22 12:40:18.997079 iters-0.8.0/iters/iters.py
--rw-r--r--   0        0        0     8027 2022-12-22 12:40:18.997079 iters-0.8.0/iters/ordered_set.py
--rw-r--r--   0        0        0        0 2022-12-22 12:40:18.997079 iters-0.8.0/iters/py.typed
--rw-r--r--   0        0        0      461 2022-12-22 12:40:18.997079 iters-0.8.0/iters/types.py
--rw-r--r--   0        0        0     4121 2022-12-22 12:40:18.997079 iters-0.8.0/iters/typing.py
--rw-r--r--   0        0        0    63340 2022-12-22 12:40:18.997079 iters-0.8.0/iters/utils.py
--rw-r--r--   0        0        0     3076 2022-12-22 12:40:18.997079 iters-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4540 1970-01-01 00:00:00.000000 iters-0.8.0/setup.py
--rw-r--r--   0        0        0     4940 1970-01-01 00:00:00.000000 iters-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-01-07 16:49:39.410964 iters-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3633 2023-01-07 16:49:39.410964 iters-0.9.0/README.md
+-rw-r--r--   0        0        0     1613 2023-01-07 16:49:39.410964 iters-0.9.0/iters/__init__.py
+-rw-r--r--   0        0        0    92873 2023-01-07 16:49:39.410964 iters-0.9.0/iters/async_iters.py
+-rw-r--r--   0        0        0   121980 2023-01-07 16:49:39.410964 iters-0.9.0/iters/async_utils.py
+-rw-r--r--   0        0        0     8244 2023-01-07 16:49:39.410964 iters-0.9.0/iters/concurrent.py
+-rw-r--r--   0        0        0    98999 2023-01-07 16:49:39.410964 iters-0.9.0/iters/iters.py
+-rw-r--r--   0        0        0     8027 2023-01-07 16:49:39.410964 iters-0.9.0/iters/ordered_set.py
+-rw-r--r--   0        0        0        0 2023-01-07 16:49:39.410964 iters-0.9.0/iters/py.typed
+-rw-r--r--   0        0        0      461 2023-01-07 16:49:39.410964 iters-0.9.0/iters/types.py
+-rw-r--r--   0        0        0     4165 2023-01-07 16:49:39.410964 iters-0.9.0/iters/typing.py
+-rw-r--r--   0        0        0    63376 2023-01-07 16:49:39.410964 iters-0.9.0/iters/utils.py
+-rw-r--r--   0        0        0     3076 2023-01-07 16:49:39.410964 iters-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4540 1970-01-01 00:00:00.000000 iters-0.9.0/setup.py
+-rw-r--r--   0        0        0     4940 1970-01-01 00:00:00.000000 iters-0.9.0/PKG-INFO
```

### Comparing `iters-0.8.0/LICENSE` & `iters-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iters-0.8.0/README.md` & `iters-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 $ poetry add iters
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-iters = "^0.8.0"
+iters = "^0.9.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.iters]
 git = "https://github.com/nekitdev/iters.git"
```

### Comparing `iters-0.8.0/iters/__init__.py` & `iters-0.9.0/iters/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 __description__ = "Composable external iteration."
 __url__ = "https://github.com/nekitdev/iters"
 
 __title__ = "iters"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 from iters.async_iters import (
     AsyncIter,
     async_iter,
     async_next,
     async_next_unchecked,
     standard_async_iter,
```

### Comparing `iters-0.8.0/iters/async_iters.py` & `iters-0.9.0/iters/async_iters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1156,14 +1156,17 @@
 
     def collect(self, function: Unary[AsyncIterable[T], U]) -> U:
         return function(self.iterator)
 
     async def collect_await(self, function: AsyncUnary[AsyncIterable[T], U]) -> U:
         return await function(self.iterator)
 
+    def collect_iter(self, function: Unary[AsyncIterable[T], AnyIterable[U]]) -> AsyncIter[U]:
+        return self.create(self.collect(function))
+
     async def list(self) -> List[T]:
         return await async_list(self.iterator)
 
     async def set(self: AsyncIter[Q]) -> Set[Q]:
         return await async_set(self.iterator)
 
     async def ordered_set(self: AsyncIter[Q]) -> OrderedSet[Q]:
```

### Comparing `iters-0.8.0/iters/async_utils.py` & `iters-0.9.0/iters/async_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from builtins import next as standard_next
 from collections import Counter as counter_dict
 from collections import deque
 from itertools import cycle
 from operator import add, mul
 from typing import (
     Any,
@@ -4844,15 +4846,15 @@
 async def async_cartesian_product_step(
     stack: AnyIterable[Tuple[Unpack[Ts]]], iterable: AnyIterable[T]  # type: ignore
 ) -> AsyncIterator[Tuple[Unpack[Ts], T]]:  # type: ignore
     array = await async_list(iterable)
 
     async for items in async_iter(stack):
         for item in array:
-            yield items + tuple_args(item)
+            yield items + unary_tuple(item)
 
 
 @overload
 def async_cartesian_power(power: Literal[0], iterable: AnyIterable[T]) -> AsyncIterator[EmptyTuple]:
     ...
 
 
@@ -4910,22 +4912,19 @@
         nonlocal state
 
         if state is None:
             state = await async_list(iterable)
 
         async for items in async_iter(stack):
             for item in state:
-                yield items + tuple_args(item)
+                yield items + unary_tuple(item)
 
     stack = async_once(())
 
     for _ in range(power):
         stack = async_cartesian_power_step(stack)  # type: ignore
 
     return stack
 
 
-Args = TypeVarTuple("Args")  # type: ignore
-
-
-def tuple_args(*args: Unpack[Args]) -> Tuple[Unpack[Args]]:  # type: ignore
-    return args  # type: ignore
+def unary_tuple(item: T) -> Tuple[T]:
+    return (item,)
```

### Comparing `iters-0.8.0/iters/concurrent.py` & `iters-0.9.0/iters/concurrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import partial
 from typing import Any, Awaitable, Callable, Iterable, List, Tuple, TypeVar, Union, overload
 
 from typing_extensions import ParamSpec
 
 try:
     from anyio import create_task_group
@@ -9,15 +11,15 @@
 
 except ImportError:
     CONCURRENT = False
 
 else:
     CONCURRENT = True
 
-from iters.typing import AnyException, DynamicTuple, EmptyTuple, is_error
+from iters.typing import AnyException, DynamicTuple, EmptyTuple, is_any_exception
 
 __all__ = (
     "CONCURRENT",
     "collect",
     "collect_with_errors",
     "collect_iterable",
     "collect_iterable_with_errors",
@@ -71,15 +73,15 @@
     except AnyException as error:
         result = error
 
     array.append((tag, result))
 
 
 def unwrap_result(result: AnyResult[T]) -> T:
-    if is_error(result):
+    if is_any_exception(result):
         raise result
 
     return result  # type: ignore
 
 
 if CONCURRENT:
```

### Comparing `iters-0.8.0/iters/iters.py` & `iters-0.9.0/iters/iters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1849,14 +1849,47 @@
             function: The function to use.
 
         Returns:
             The result of the `function` call.
         """
         return function(self.iterator)
 
+    def collect_iter(self, function: Unary[Iterable[T], Iterable[U]]) -> Iter[U]:
+        """Collects the iterator with the `function`.
+
+        This is equivalent to:
+
+        ```python
+        iterator.create(iterator.collect(function))
+        ```
+
+        Example:
+            ```python
+            from typing import TypeVar
+
+            T = TypeVar("T")
+
+            def identity(item: T) -> T:
+                return item
+
+            array = [13, 25, 34]
+
+            iterator = iter(array).collect_iter(identity)
+
+            assert iterator.list() == array
+            ```
+
+        Arguments:
+            function: The function to use.
+
+        Returns:
+            The result of the `function` call, wrapped back into an iterator.
+        """
+        return self.create(self.collect(function))
+
     def list(self) -> List[T]:
         """Collects the iterator into the [`List[T]`][list].
 
         This is equivalent to:
 
         ```python
         list(iterator.unwrap())
```

### Comparing `iters-0.8.0/iters/ordered_set.py` & `iters-0.9.0/iters/ordered_set.py`

 * *Files identical despite different names*

### Comparing `iters-0.8.0/iters/typing.py` & `iters-0.9.0/iters/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import abstractmethod
 from builtins import isinstance as is_instance
 from builtins import issubclass as is_subclass
 from typing import (
     Any,
     AsyncIterable,
     AsyncIterator,
@@ -155,15 +157,15 @@
     return is_instance(item, str)
 
 
 def is_bytes(item: Any) -> TypeGuard[bytes]:
     return is_instance(item, bytes)
 
 
-def is_error(item: Any) -> TypeGuard[AnyException]:
+def is_any_exception(item: Any) -> TypeGuard[AnyException]:
     return is_instance(item, AnyException)
 
 
 RecursiveIterable: TypeAlias = Union[T, Iterable[Any]]
 RecursiveAsyncIterable: TypeAlias = Union[T, AsyncIterable[Any]]
 RecursiveAnyIterable: TypeAlias = Union[T, AnyIterable[Any]]
```

### Comparing `iters-0.8.0/iters/utils.py` & `iters-0.9.0/iters/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from builtins import zip as standard_zip
 from collections import Counter as counter_dict
 from collections import deque
 from functools import reduce as standard_reduce
 from itertools import accumulate as standard_accumulate
 from itertools import chain, compress
 from itertools import count as standard_count
```

### Comparing `iters-0.8.0/pyproject.toml` & `iters-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iters"
-version = "0.8.0"
+version = "0.9.0"
 description = "Composable external iteration."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/iters"
@@ -131,15 +131,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "iters"
-version = "0.8.0"
+version = "0.9.0"
 url = "https://github.com/nekitdev/iters"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `iters-0.8.0/setup.py` & `iters-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['named>=1.1.0', 'orderings>=1.1.0', 'solus>=1.1.0', 'typing-extensions>=4.3.0']
 
 extras_require = \
 {'concurrent': ['anyio>=3.6.1']}
 
 setup_kwargs = {
     'name': 'iters',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Composable external iteration.',
-    'long_description': '# `iters`\n\n[![License][License Badge]][License]\n[![Version][Version Badge]][Package]\n[![Downloads][Downloads Badge]][Package]\n[![Discord][Discord Badge]][Discord]\n\n[![Documentation][Documentation Badge]][Documentation]\n[![Check][Check Badge]][Actions]\n[![Test][Test Badge]][Actions]\n[![Coverage][Coverage Badge]][Coverage]\n\n> *Composable external iteration.*\n\nIf you have found yourself with a *collection* of some kind, and needed to perform\nan operation on the elements of said collection, you will quickly run into *iterators*.\nIterators are heavily used in idiomatic Python code, so becoming familiar with them is essential.\n\n## Installing\n\n**Python 3.7 or above is required.**\n\n### pip\n\nInstalling the library with `pip` is quite simple:\n\n```console\n$ pip install iters\n```\n\nAlternatively, the library can be installed from source:\n\n```console\n$ git clone https://github.com/nekitdev/iters.git\n$ cd iters\n$ python -m pip install .\n```\n\n### poetry\n\nYou can add `iters` as a dependency with the following command:\n\n```console\n$ poetry add iters\n```\n\nOr by directly specifying it in the configuration like so:\n\n```toml\n[tool.poetry.dependencies]\niters = "^0.8.0"\n```\n\nAlternatively, you can add it directly from the source:\n\n```toml\n[tool.poetry.dependencies.iters]\ngit = "https://github.com/nekitdev/iters.git"\n```\n\n## Examples\n\n### Simple\n\nSquaring only even numbers in some sequence:\n\n```python\nfrom iters import iter\n\n\ndef is_even(value: int) -> bool:\n    return not value % 2\n\n\ndef square(value: int) -> int:\n    return value * value\n\n\nnumbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n\nresult = iter(numbers).filter(is_even).map(square).list()\n\nprint(result)  # [0, 4, 16, 36, 64]\n```\n\n### Asynchronous\n\nAsynchronous iteration is fully supported by `iters`, and its API is similar to its\nsynchronous counterpart.\n\n## Documentation\n\nYou can find the documentation [here][Documentation].\n\n## Support\n\nIf you need support with the library, you can send an [email][Email]\nor refer to the official [Discord server][Discord].\n\n## Changelog\n\nYou can find the changelog [here][Changelog].\n\n## Security Policy\n\nYou can find the Security Policy of `iters` [here][Security].\n\n## Contributing\n\nIf you are interested in contributing to `iters`, make sure to take a look at the\n[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].\n\n## License\n\n`iters` is licensed under the MIT License terms. See [License][License] for details.\n\n[Email]: mailto:support@nekit.dev\n\n[Discord]: https://nekit.dev/discord\n\n[Actions]: https://github.com/nekitdev/iters/actions\n\n[Changelog]: https://github.com/nekitdev/iters/blob/main/CHANGELOG.md\n[Code of Conduct]: https://github.com/nekitdev/iters/blob/main/CODE_OF_CONDUCT.md\n[Contributing Guide]: https://github.com/nekitdev/iters/blob/main/CONTRIBUTING.md\n[Security]: https://github.com/nekitdev/iters/blob/main/SECURITY.md\n\n[License]: https://github.com/nekitdev/iters/blob/main/LICENSE\n\n[Package]: https://pypi.org/project/iters\n[Coverage]: https://codecov.io/gh/nekitdev/iters\n[Documentation]: https://nekitdev.github.io/iters\n\n[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2\n[License Badge]: https://img.shields.io/pypi/l/iters\n[Version Badge]: https://img.shields.io/pypi/v/iters\n[Downloads Badge]: https://img.shields.io/pypi/dm/iters\n\n[Documentation Badge]: https://github.com/nekitdev/iters/workflows/docs/badge.svg\n[Check Badge]: https://github.com/nekitdev/iters/workflows/check/badge.svg\n[Test Badge]: https://github.com/nekitdev/iters/workflows/test/badge.svg\n[Coverage Badge]: https://codecov.io/gh/nekitdev/iters/branch/main/graph/badge.svg\n',
+    'long_description': '# `iters`\n\n[![License][License Badge]][License]\n[![Version][Version Badge]][Package]\n[![Downloads][Downloads Badge]][Package]\n[![Discord][Discord Badge]][Discord]\n\n[![Documentation][Documentation Badge]][Documentation]\n[![Check][Check Badge]][Actions]\n[![Test][Test Badge]][Actions]\n[![Coverage][Coverage Badge]][Coverage]\n\n> *Composable external iteration.*\n\nIf you have found yourself with a *collection* of some kind, and needed to perform\nan operation on the elements of said collection, you will quickly run into *iterators*.\nIterators are heavily used in idiomatic Python code, so becoming familiar with them is essential.\n\n## Installing\n\n**Python 3.7 or above is required.**\n\n### pip\n\nInstalling the library with `pip` is quite simple:\n\n```console\n$ pip install iters\n```\n\nAlternatively, the library can be installed from source:\n\n```console\n$ git clone https://github.com/nekitdev/iters.git\n$ cd iters\n$ python -m pip install .\n```\n\n### poetry\n\nYou can add `iters` as a dependency with the following command:\n\n```console\n$ poetry add iters\n```\n\nOr by directly specifying it in the configuration like so:\n\n```toml\n[tool.poetry.dependencies]\niters = "^0.9.0"\n```\n\nAlternatively, you can add it directly from the source:\n\n```toml\n[tool.poetry.dependencies.iters]\ngit = "https://github.com/nekitdev/iters.git"\n```\n\n## Examples\n\n### Simple\n\nSquaring only even numbers in some sequence:\n\n```python\nfrom iters import iter\n\n\ndef is_even(value: int) -> bool:\n    return not value % 2\n\n\ndef square(value: int) -> int:\n    return value * value\n\n\nnumbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n\nresult = iter(numbers).filter(is_even).map(square).list()\n\nprint(result)  # [0, 4, 16, 36, 64]\n```\n\n### Asynchronous\n\nAsynchronous iteration is fully supported by `iters`, and its API is similar to its\nsynchronous counterpart.\n\n## Documentation\n\nYou can find the documentation [here][Documentation].\n\n## Support\n\nIf you need support with the library, you can send an [email][Email]\nor refer to the official [Discord server][Discord].\n\n## Changelog\n\nYou can find the changelog [here][Changelog].\n\n## Security Policy\n\nYou can find the Security Policy of `iters` [here][Security].\n\n## Contributing\n\nIf you are interested in contributing to `iters`, make sure to take a look at the\n[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].\n\n## License\n\n`iters` is licensed under the MIT License terms. See [License][License] for details.\n\n[Email]: mailto:support@nekit.dev\n\n[Discord]: https://nekit.dev/discord\n\n[Actions]: https://github.com/nekitdev/iters/actions\n\n[Changelog]: https://github.com/nekitdev/iters/blob/main/CHANGELOG.md\n[Code of Conduct]: https://github.com/nekitdev/iters/blob/main/CODE_OF_CONDUCT.md\n[Contributing Guide]: https://github.com/nekitdev/iters/blob/main/CONTRIBUTING.md\n[Security]: https://github.com/nekitdev/iters/blob/main/SECURITY.md\n\n[License]: https://github.com/nekitdev/iters/blob/main/LICENSE\n\n[Package]: https://pypi.org/project/iters\n[Coverage]: https://codecov.io/gh/nekitdev/iters\n[Documentation]: https://nekitdev.github.io/iters\n\n[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2\n[License Badge]: https://img.shields.io/pypi/l/iters\n[Version Badge]: https://img.shields.io/pypi/v/iters\n[Downloads Badge]: https://img.shields.io/pypi/dm/iters\n\n[Documentation Badge]: https://github.com/nekitdev/iters/workflows/docs/badge.svg\n[Check Badge]: https://github.com/nekitdev/iters/workflows/check/badge.svg\n[Test Badge]: https://github.com/nekitdev/iters/workflows/test/badge.svg\n[Coverage Badge]: https://codecov.io/gh/nekitdev/iters/branch/main/graph/badge.svg\n',
     'author': 'nekitdev',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nekitdev/iters',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `iters-0.8.0/PKG-INFO` & `iters-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iters
-Version: 0.8.0
+Version: 0.9.0
 Summary: Composable external iteration.
 Home-page: https://github.com/nekitdev/iters
 License: MIT
 Keywords: python,iter,iterator
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
@@ -78,15 +78,15 @@
 $ poetry add iters
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-iters = "^0.8.0"
+iters = "^0.9.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.iters]
 git = "https://github.com/nekitdev/iters.git"
```

