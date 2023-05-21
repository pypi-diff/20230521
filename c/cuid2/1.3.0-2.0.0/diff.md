# Comparing `tmp/cuid2-1.3.0.tar.gz` & `tmp/cuid2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuid2-1.3.0.tar", last modified: Fri May 19 12:14:23 2023, max compression
+gzip compressed data, was "cuid2-2.0.0.tar", last modified: Sun May 21 15:33:47 2023, max compression
```

## Comparing `cuid2-1.3.0.tar` & `cuid2-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1078 2023-05-19 12:14:08.569073 cuid2-1.3.0/LICENSE
--rw-r--r--   0        0        0     1749 2023-05-19 12:14:08.569073 cuid2-1.3.0/README.md
--rw-r--r--   0        0        0     3783 2023-05-19 12:14:23.285277 cuid2-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      240 2023-05-19 12:14:08.569073 cuid2-1.3.0/src/cuid2/__init__.py
--rw-r--r--   0        0        0     5081 2023-05-19 12:14:08.569073 cuid2-1.3.0/src/cuid2/generator.py
--rw-r--r--   0        0        0        0 2023-05-19 12:14:08.569073 cuid2-1.3.0/src/cuid2/py.typed
--rw-r--r--   0        0        0     5816 2023-05-19 12:14:08.573073 cuid2-1.3.0/src/cuid2/utils.py
--rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 cuid2-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-21 15:33:27.914489 cuid2-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2184 2023-05-21 15:33:27.914489 cuid2-2.0.0/README.md
+-rw-r--r--   0        0        0     3827 2023-05-21 15:33:47.286849 cuid2-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      255 2023-05-21 15:33:27.918489 cuid2-2.0.0/src/cuid2/__init__.py
+-rw-r--r--   0        0        0      231 2023-05-21 15:33:27.918489 cuid2-2.0.0/src/cuid2/cli.py
+-rw-r--r--   0        0        0     4759 2023-05-21 15:33:27.918489 cuid2-2.0.0/src/cuid2/generator.py
+-rw-r--r--   0        0        0        0 2023-05-21 15:33:27.918489 cuid2-2.0.0/src/cuid2/py.typed
+-rw-r--r--   0        0        0     5816 2023-05-21 15:33:27.918489 cuid2-2.0.0/src/cuid2/utils.py
+-rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 cuid2-2.0.0/PKG-INFO
```

### Comparing `cuid2-1.3.0/LICENSE` & `cuid2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cuid2-1.3.0/README.md` & `cuid2-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -35,17 +35,35 @@
 
 ## Install
 ```
 pip install cuid2
 ```
 
 ## Usage
-You can generate CUIDs with the following:
+
+You can generate CUIDs directly in the terminal with the following:
+```bash
+$ cuid2
+```
+
+Or you can rely on a CUID wrapper if you don't need any customizations:
+```python
+from typing import Callable
+from cuid2 import cuid_wrapper
+
+cuid_generator: Callable[[], str] = cuid_wrapper()
+
+def main():
+  my_cuid: str = cuid_generator()
+  next_cuid: str = cuid_generator()
+```
+
+Finally, for more explicit control of the CUID generator, you can instantiate the class directly:
 ```python
 from cuid2 import Cuid
 
-CUID_GENERATOR: Cuid = Cuid()
+CUID_GENERATOR: Cuid = Cuid(length=10)
 
 def main():
   my_cuid: str = CUID_GENERATOR.generate()
   next_cuid: str = CUID_GENERATOR.generate()
 ```
```

### Comparing `cuid2-1.3.0/pyproject.toml` & `cuid2-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -27,22 +27,25 @@
     "crypt",
     "security",
     "uuid",
     "guid",
     "cuid",
     "cryptography",
 ]
-version = "1.3.0"
+version = "2.0.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 repository = "https://github.com/gordon-code/cuid2/"
 
+[project.scripts]
+cuid2 = "cuid2.cli:main"
+
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.scripts]
 black = "black {args:src/ local/tests/}"
 ruff = "ruff check --fix --exit-zero {args:src/ local/tests/}"
 spelling = "codespell {args:src/ local/tests/}"
@@ -69,29 +72,29 @@
 ]
 
 [tool.pdm.dev-dependencies]
 lint = [
     "black~=23.3.0",
     "codespell~=2.2.4",
     "pylint~=2.17.4",
-    "ruff~=0.0.267",
+    "ruff~=0.0.269",
     "safety==2.4.0b1",
 ]
 test = [
     "pytest~=7.3.1",
     "pytest-mock~=3.10.0",
     "pytest-sugar~=0.9.7",
 ]
-typing = [
-    "mypy~=1.3.0",
-]
 tox = [
     "tox~=4.4.12",
     "tox-pdm~=0.6.1",
 ]
+typing = [
+    "mypy~=1.3.0",
+]
 
 [tool.tox]
 legacy_tox_ini = "    [tox]\n    min_version = 4\n    env_list = py3{8,9,10,11}, check\n    work_dir = local/.tox\n    isolated_build = True\n\n    [testenv]\n    description = run unit tests\n    groups = test\n    commands = testing\n\n    [testenv:check]\n    description = run linters and typing\n    skip_install = true\n    groups = lint, typing, test\n    commands = lint-full\n"
 
 [tool.black]
 line-length = 120
 target_version = [
```

### Comparing `cuid2-1.3.0/src/cuid2/generator.py` & `cuid2-2.0.0/src/cuid2/generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import time
-import warnings
 from math import floor
 from secrets import SystemRandom
-from typing import TYPE_CHECKING, Any, Callable, Dict, Final, Optional, Protocol, Tuple, Type
+from typing import TYPE_CHECKING, Callable, Final, Optional, Protocol
 
 from cuid2 import utils
 
 if TYPE_CHECKING:
     from _random import Random
 
     class FingerprintCallable(Protocol):  # pylint: disable=too-few-public-methods
@@ -95,17 +94,21 @@
 
         salt: str = utils.create_entropy(length=length, random_generator=self._random)
         hash_input: str = base36_time + salt + base36_count + self._fingerprint
 
         return first_letter + utils.create_hash(hash_input)[1 : length or self._length]
 
 
-class CUID(Cuid):  # pylint: disable=too-few-public-methods
-    def __init_subclass__(cls: Type["CUID"], **kwargs: Dict[str, Any]) -> None:
-        """Deprecated class CUID. Use Cuid instead."""
-        warnings.warn("CUID is deprecated, use Cuid instead", DeprecationWarning, stacklevel=1)
-        super().__init_subclass__(**kwargs)
-
-    def __new__(cls: Type["CUID"], *args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> "CUID":
-        """Deprecated class CUID. Use Cuid instead."""
-        warnings.warn("CUID is deprecated, use Cuid instead", DeprecationWarning, stacklevel=1)
-        return super().__new__(cls, *args, **kwargs)
+def cuid_wrapper() -> Callable[[], str]:
+    """Wrap a single Cuid class instance and return a callable that generates a CUID string.
+
+    Returns
+    -------
+    Callable[[], str]
+        A callable that generates a CUID string.
+    """
+    cuid_generator: Cuid = Cuid()
+
+    def cuid() -> str:
+        return cuid_generator.generate()
+
+    return cuid
```

### Comparing `cuid2-1.3.0/src/cuid2/utils.py` & `cuid2-2.0.0/src/cuid2/utils.py`

 * *Files identical despite different names*

### Comparing `cuid2-1.3.0/PKG-INFO` & `cuid2-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuid2
-Version: 1.3.0
+Version: 2.0.0
 Summary: Next generation GUIDs. Collision-resistant ids optimized for horizontal scaling and performance.
 Keywords: crypt security uuid guid cuid cryptography
 Author-Email: Will Gordon <wgordon@redhat.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Gordon Code
         
@@ -74,17 +74,35 @@
 
 ## Install
 ```
 pip install cuid2
 ```
 
 ## Usage
-You can generate CUIDs with the following:
+
+You can generate CUIDs directly in the terminal with the following:
+```bash
+$ cuid2
+```
+
+Or you can rely on a CUID wrapper if you don't need any customizations:
+```python
+from typing import Callable
+from cuid2 import cuid_wrapper
+
+cuid_generator: Callable[[], str] = cuid_wrapper()
+
+def main():
+  my_cuid: str = cuid_generator()
+  next_cuid: str = cuid_generator()
+```
+
+Finally, for more explicit control of the CUID generator, you can instantiate the class directly:
 ```python
 from cuid2 import Cuid
 
-CUID_GENERATOR: Cuid = Cuid()
+CUID_GENERATOR: Cuid = Cuid(length=10)
 
 def main():
   my_cuid: str = CUID_GENERATOR.generate()
   next_cuid: str = CUID_GENERATOR.generate()
 ```
```

