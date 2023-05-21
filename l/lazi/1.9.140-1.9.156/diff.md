# Comparing `tmp/lazi-1.9.140.tar.gz` & `tmp/lazi-1.9.156.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.9.140.tar", max compression
+gzip compressed data, was "lazi-1.9.156.tar", max compression
```

## Comparing `lazi-1.9.140.tar` & `lazi-1.9.156.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0      150 2023-05-17 23:57:14.424788 lazi-1.9.140/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.9.140/lazi/conf/auto.py
--rw-r--r--   0        0        0     2036 2023-05-18 08:23:34.697245 lazi-1.9.140/lazi/conf/base.py
--rw-r--r--   0        0        0     4708 2023-05-18 02:24:12.623535 lazi-1.9.140/lazi/conf/conf.py
--rw-r--r--   0        0        0     1330 2023-05-18 02:20:03.676308 lazi-1.9.140/lazi/conf/envs.py
--rw-r--r--   0        0        0      287 2023-05-18 04:13:09.132500 lazi-1.9.140/lazi/core/__init__.py
--rw-r--r--   0        0        0     5135 2023-05-18 08:20:50.135091 lazi-1.9.140/lazi/core/finder.py
--rw-r--r--   0        0        0     5640 2023-05-18 08:05:28.331019 lazi-1.9.140/lazi/core/loader.py
--rw-r--r--   0        0        0     3832 2023-05-18 08:17:17.748313 lazi-1.9.140/lazi/core/module.py
--rw-r--r--   0        0        0     1998 2023-05-18 07:52:43.688996 lazi-1.9.140/lazi/core/spec.py
--rw-r--r--   0        0        0     3571 2023-05-17 06:13:14.860256 lazi-1.9.140/lazi/core/stat.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.9.140/lazi/util/__init__.py
--rw-r--r--   0        0        0      873 2023-05-18 05:48:25.043176 lazi-1.9.140/lazi/util/debug.py
--rw-r--r--   0        0        0      146 2023-05-18 08:04:01.089875 lazi-1.9.140/lazi/util/functional.py
--rw-r--r--   0        0        0       73 2023-05-18 08:06:11.639587 lazi-1.9.140/lazi/util/util.py
--rw-r--r--   0        0        0     1655 2023-05-18 08:29:15.101699 lazi-1.9.140/pyproject.toml
--rw-r--r--   0        0        0     9564 2023-05-18 08:28:28.397087 lazi-1.9.140/readme.md
--rw-r--r--   0        0        0        0 2023-05-17 06:10:55.650459 lazi-1.9.140/tests/__init__.py
--rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.9.140/tests/standalone/sa_array.py
--rw-r--r--   0        0        0      922 2023-05-18 00:51:41.543400 lazi-1.9.140/tests/standalone/sa_nested.py
--rw-r--r--   0        0        0       43 2023-05-18 04:25:44.850316 lazi-1.9.140/tests/standalone/sa_pandas.py
--rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.9.140/tests/standalone/sa_pygments.py
--rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.9.140/tests/test_array.py
--rw-r--r--   0        0        0      378 2023-05-17 06:09:23.165264 lazi-1.9.140/tests/test_asyncio.py
--rw-r--r--   0        0        0     1187 2023-05-18 00:16:22.071819 lazi-1.9.140/tests/test_django.py
--rw-r--r--   0        0        0     1251 2023-05-18 01:33:30.900017 lazi-1.9.140/tests/test_importlib.py
--rw-r--r--   0        0        0      230 2023-05-18 01:11:43.475022 lazi-1.9.140/tests/test_lazy.py
--rw-r--r--   0        0        0      307 2023-05-18 01:33:30.888016 lazi-1.9.140/tests/test_pygments.py
--rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.9.140/tests/test_requests.py
--rw-r--r--   0        0        0     1004 2023-05-17 07:14:47.163887 lazi-1.9.140/tests/test_rich.py
--rw-r--r--   0        0        0     1200 2023-05-18 01:33:30.900017 lazi-1.9.140/tests/test_stat.py
--rw-r--r--   0        0        0    10660 1970-01-01 00:00:00.000000 lazi-1.9.140/PKG-INFO
+-rw-r--r--   0        0        0      150 2023-05-17 23:57:14.424788 lazi-1.9.156/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.9.156/lazi/conf/auto.py
+-rw-r--r--   0        0        0     2426 2023-05-20 16:57:39.763399 lazi-1.9.156/lazi/conf/base.py
+-rw-r--r--   0        0        0     4708 2023-05-18 02:24:12.623535 lazi-1.9.156/lazi/conf/conf.py
+-rw-r--r--   0        0        0     1330 2023-05-18 02:20:03.676308 lazi-1.9.156/lazi/conf/envs.py
+-rw-r--r--   0        0        0      425 2023-05-20 17:42:19.998625 lazi-1.9.156/lazi/conf/lazy.py
+-rw-r--r--   0        0        0      289 2023-05-20 16:53:17.056017 lazi-1.9.156/lazi/core/__init__.py
+-rw-r--r--   0        0        0     5061 2023-05-20 18:03:11.131351 lazi-1.9.156/lazi/core/finder.py
+-rw-r--r--   0        0        0     6549 2023-05-20 16:53:17.068018 lazi-1.9.156/lazi/core/loader.py
+-rw-r--r--   0        0        0     3832 2023-05-18 08:17:17.748313 lazi-1.9.156/lazi/core/module.py
+-rw-r--r--   0        0        0     2765 2023-05-20 17:20:27.169172 lazi-1.9.156/lazi/core/spec.py
+-rw-r--r--   0        0        0     3571 2023-05-17 06:13:14.860256 lazi-1.9.156/lazi/core/stat.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.9.156/lazi/util/__init__.py
+-rw-r--r--   0        0        0      873 2023-05-18 05:48:25.043176 lazi-1.9.156/lazi/util/debug.py
+-rw-r--r--   0        0        0      146 2023-05-18 08:04:01.089875 lazi-1.9.156/lazi/util/functional.py
+-rw-r--r--   0        0        0       73 2023-05-18 08:06:11.639587 lazi-1.9.156/lazi/util/util.py
+-rw-r--r--   0        0        0     2077 2023-05-20 18:16:02.701821 lazi-1.9.156/pyproject.toml
+-rw-r--r--   0        0        0     8937 2023-05-18 16:04:24.075835 lazi-1.9.156/readme.md
+-rw-r--r--   0        0        0        0 2023-05-17 06:10:55.650459 lazi-1.9.156/tests/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.9.156/tests/standalone/sa_array.py
+-rw-r--r--   0        0        0      922 2023-05-18 00:51:41.543400 lazi-1.9.156/tests/standalone/sa_nested.py
+-rw-r--r--   0        0        0       43 2023-05-18 04:25:44.850316 lazi-1.9.156/tests/standalone/sa_pandas.py
+-rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.9.156/tests/standalone/sa_pygments.py
+-rw-r--r--   0        0        0      524 2023-05-20 17:57:16.350542 lazi-1.9.156/tests/test_array.py
+-rw-r--r--   0        0        0      408 2023-05-20 17:46:16.661789 lazi-1.9.156/tests/test_asyncio.py
+-rw-r--r--   0        0        0     1291 2023-05-20 17:46:16.661789 lazi-1.9.156/tests/test_django.py
+-rw-r--r--   0        0        0     1285 2023-05-18 22:58:43.789962 lazi-1.9.156/tests/test_importlib.py
+-rw-r--r--   0        0        0      263 2023-05-20 17:46:16.673789 lazi-1.9.156/tests/test_lazy.py
+-rw-r--r--   0        0        0      337 2023-05-20 17:46:16.673789 lazi-1.9.156/tests/test_pygments.py
+-rw-r--r--   0        0        0      862 2023-05-20 17:46:16.669789 lazi-1.9.156/tests/test_requests.py
+-rw-r--r--   0        0        0     1046 2023-05-20 17:46:16.665789 lazi-1.9.156/tests/test_rich.py
+-rw-r--r--   0        0        0     1259 2023-05-20 18:00:58.413489 lazi-1.9.156/tests/test_stat.py
+-rw-r--r--   0        0        0     9934 1970-01-01 00:00:00.000000 lazi-1.9.156/PKG-INFO
```

### Comparing `lazi-1.9.140/lazi/conf/base.py` & `lazi-1.9.156/lazi/conf/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 """Base project configuration.
 """
 __meta__ = dict(                        # Internal configuration for <root>.conf.conf (cannot override elsewhere).
     root="lazi",                        # - Root namespace package name.
 )                                       # See conf.py for more options.
 #
+#
 TRACE: int = 0                          # Enable debug traces. Currently using levels 0-4.
-TRACEE: bool = True                     # Enable debug traces for loader exceptions when TRACE is 0.
-#                                       # - Tracing relies on __debug__ and asserts, so -O will disable completely.
-AUTO_AUTO: bool = True                  # Automatically install when importing lazi.auto.
-CORE_AUTO: bool = False                 # Automatically install when importing lazi.core.
+#                                       # - Tracing relies on __debug__ and asserts, so `python -O` will disable completely.
+#
+NO_LAZY: int = 0                        # Hook loaders, but skip lazy loading.
+#                                       # - 0: Lazy load all modules. [NB: New option 0.5 WIP - Unhook mod after lazy attr load.]
+#                                       # - 1: Skip lazy loading.
+#                                       # - 2: Skip lazy loading, and unwrap the module as well.
+#                                       # - 3: Skip lazy loading, and unhook the loader as well.
+#
+LAZY: dict[str, int | str] = {}         # Specify loading behavior for specific modules (regex name -> NO_LAZY level).
+#                                       # - Currently, `conf` does not merge dicts, so this must be set from one module only.
 #
 NO_HOOK: bool = False                   # Disable all spec loader hooks.
-NO_LAZY: bool = False                   # Hook loaders, but skip lazy loading.
 NO_HOOK_STD: bool = False               # Disable spec loader hooking for stdlib modules.
 NO_HOOK_BI: bool = False                # Disable spec loader hooking for built-in modules.
 #
-INVAL_SOFT: bool = False                # Keep modules in sys.modules after cache invalidation.
-INVAL_GC: bool = (not INVAL_SOFT)       # Enable garbage collection on cache invalidation.
-#                                       # - Only makes sense if INVAL_SOFT is False.
+AUTO_AUTO: bool = True                  # Automatically install when importing lazi.auto.
+CORE_AUTO: bool = False                 # Automatically install when importing lazi.core.
+#
+CONTEXT_INVALIDATION: bool = False      # Call invalidate_caches() when exiting a `with Finder()` statement.
+#
 #
 #
 CONF_NO_CACHING: bool | None = None     # Disable caching of conf vars.
 #                                         - None: Use the default caching behavior, which will disable
 #                                                 caching if `lazi.core` is already present in sys.modules
 #                                                 when lazi.conf.conf is imported.
 #
```

### Comparing `lazi-1.9.140/lazi/conf/conf.py` & `lazi-1.9.156/lazi/conf/conf.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.140/lazi/conf/envs.py` & `lazi-1.9.156/lazi/conf/envs.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.140/lazi/core/finder.py` & `lazi-1.9.156/lazi/core/finder.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,149 +4,145 @@
 - https://github.com/facebookincubator/cinder/blob/cinder/3.8/CinderDoc/lazy_imports.rst
 - https://snarky.ca/lazy-importing-in-python-3-7/
 - https://pypi.org/project/demandimport/
 - https://github.com/facebookincubator/cinder (CPython implementation)
 """
 from __future__ import annotations
 
-import gc
 import sys
 import atexit
 from types import ModuleType
 from importlib.abc import MetaPathFinder
 from importlib.machinery import ModuleSpec
 from importlib import import_module
 from pathlib import Path
+import re
 
 from lazi.conf import conf
 from lazi.util import classproperty, debug, oid
 
 from .spec import Spec
 from .loader import Loader
 from .module import Module
 
 __all__ = "Finder", "__finder__"
 
-INVAL_SOFT = conf.INVAL_SOFT
-INVAL_GC = conf.INVAL_GC
-
 
 class Finder(MetaPathFinder):
     Spec: type[Spec] = Spec
     Loader: type[Loader] = Loader
     Module: type[Module] = Module
 
+    NO_LAZY: int = conf.NO_LAZY
+    LAZY: dict[str, int | str] = conf.LAZY
+    CONTEXT_INVALIDATION: bool = conf.CONTEXT_INVALIDATION
+
+    meta_path = classproperty(lambda cls: (_ for _ in sys.meta_path if isinstance(_, cls)))
     __finders__: list[Finder] = []
-    __stack__: list[Finder] = []
 
+    __refs: int = 0
+    refs = property(lambda self: self.__refs)
     specs: dict[str, Spec]
-    __busy: bool = False
-    __refs: int = 0; refs = property(lambda self: self.__refs)  # noqa
 
-    meta_path = classproperty(lambda cls: (_ for _ in sys.meta_path if isinstance(_, cls)))
-
-    def __init__(self):
+    def __init__(self, **CONF):
         assert None is debug.traced(3, f"[{oid(self)}] INIT {self.__class__.__name__} count:{len(self.__finders__)}")
-        self.__finders__.append(self)
+
+        for k, v in CONF.items():
+            if not k.isupper() or k.startswith("_"):
+                raise ValueError(f"Invalid configuration key: {k}")
+            setattr(self, k, v)
+
         self.specs = {}
+        self.__finders__.append(self)
 
     def __del__(self):
+        if self in self.__finders__:
+            self.__finders__.remove(self)
         try:
-            if self in self.__finders__:
-                self.__finders__.remove(self)
-                self.invalidate_caches()
+            self.invalidate_caches()
         except Exception as e:
-            assert None is debug.info(
+            self.specs.clear()
+            assert None is debug.exception(
                 f"[{oid(self)}] DEL! {self.__class__.__name__} !!!! {type(e).__name__}: {e}"
             )
 
     def __enter__(self) -> Finder:
-        if self not in sys.meta_path:
-            assert self.__refs == 0, self.__refs
+        if self.__refs == 0:
             assert None is debug.traced(
                 2,
                 f"[{oid(self)}] HOOK {self.__class__.__name__} refs:{self.__refs} "
                 f"inst:{len(list(self.meta_path))} sys:{len(sys.meta_path)} "
             )
             sys.meta_path.insert(0, self)
-            self.__stack__.append(self)
 
         self.__refs += 1
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.__refs = max(self.__refs - 1, 0)
 
         if self.__refs == 0 and self in sys.meta_path:
-            pop = self.__stack__.pop()
-            assert pop is self, (pop, self)
             sys.meta_path.remove(self)
+            if self.CONTEXT_INVALIDATION:
+                self.invalidate_caches()
 
         assert None is debug.traced(
             2,
             f"[{oid(self)}] EXIT {self.__class__.__name__} refs:{self.__refs} "
             f"inst:{len(list(self.meta_path))} sys:{len(sys.meta_path)} "
         )
 
-    def lazy(self, name: str, package: str | None = None) -> ModuleType:
-        with self:
+    @classmethod
+    def lazy(cls, name: str, package: str | None = None, **CONF) -> ModuleType:
+        if CONF:
+            with cls(**CONF):
+                return import_module(name, package)
+
+        with __finder__:
             return import_module(name, package)
 
     def find_spec(self, name: str, path: list[str] | None = None, target: ModuleType | None = None) -> Spec | None:
-        assert self in self.__stack__, (self, self.__stack__)
-
-        if self.__busy or self.__stack__[-1] != self:
-            return None
-
         assert None is debug.traced(
             4 if target is None else 1,
-            f"[{oid(self)}] SPEC FIND {name} {'' if path is not None else '*'}"
+            f"[{oid(self)}] SPEC FIND {name}"
         )
 
         if (spec := self.specs.get(name)) is not None:
-            assert spec.finder is self, (spec.finder, self)
-            if path is not None:
-                spec.path = path
-            if target is not None:
-                spec.target = target
+            assert None is debug.traced(
+                4 if target is None else 1,
+                f"[{oid(self)}] SPEC FOUN {name}"
+            )
             return spec
 
         if (spec := self._find_spec(name, path, target)) is not None:
-
-            if not isinstance(spec, self.Spec):
-                spec = self.specs[name] = self.Spec(self, spec, path, target)
-            else:
-                if path is not None:
-                    spec.path = path
-                if target is not None:
-                    spec.target = target
+            spec = self.specs[name] = self.Spec(self, spec, path, target)
 
             assert None is debug.traced(
                 1,
                 f"[{oid(self)}] FIND " +
                 ((Path(c).suffix[1:] if (c := spec.cached) else Path(o).suffix[1:] if (o := spec.origin) else '?') +
                     f"{'S' if spec.stdlib else ''}{'B' if spec.builtin else ''}").ljust(5) +
-                f"{spec.f_name} {'*' if path is None else ''}"
+                f"{spec.f_name} {'?' if spec.loader is None else ''}"
             )
 
-            return spec
+        return spec
 
     def _find_spec(self, name: str, path: list[str] | None, target: ModuleType | None) -> ModuleSpec | None:
-        for finder in (_ for _ in sys.meta_path if _ is not self):
+        for finder in (_ for _ in sys.meta_path if not isinstance(_, self.__class__)):
             if (spec := finder.find_spec(name, path, target)) is not None:
                 return spec
 
-    def invalidate_caches(self) -> None:
-        if not INVAL_SOFT:
-            while self.specs and (spec := self.specs.popitem()[1]):
-                if hasattr(spec.loader, "invalidate_caches"):
-                    spec.loader.invalidate_caches()
-        else:
-            self.specs.clear()
+    def get_level(self, full_name: str) -> Spec.Level:
+        for name, level in self.LAZY.items():
+            if re.match(name, full_name):
+                return Spec.Level.get(level)
+        return Spec.Level(self.NO_LAZY)
 
-        if INVAL_GC:
-            gc.collect()
+    def invalidate_caches(self) -> None:
+        while self.specs:
+            if hasattr(loader := self.specs.popitem()[1].loader, "invalidate_caches"):
+                loader.invalidate_caches()
 
 
 __finder__: Finder = Finder()
 
 atexit.register(lambda: [finder.invalidate_caches() for finder in Finder.__finders__])
```

### Comparing `lazi-1.9.140/lazi/core/loader.py` & `lazi-1.9.156/lazi/core/loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,41 +8,51 @@
 
 from sys import modules
 from types import ModuleType
 from typing import ForwardRef
 from enum import IntEnum
 from importlib.abc import Loader as _Loader
 
-from lazi.conf import conf
 from lazi.util import debug, oid
 
 __all__ = "Loader",
 
 Spec = ForwardRef("Spec")
 Module = ForwardRef("Module")
 
-NO_LAZY = conf.NO_LAZY
-TRACE = conf.TRACE
-TRACEE = conf.TRACEE
-
 
 class Loader(_Loader):
     spec: Spec
     loader: _Loader
+    module: Module | None = None
+
     __busy: bool = False
     __forc: bool = False
 
     class State(IntEnum):
         __str__ = lambda self: self.name
         INIT = 0
         CREA = 1
         LAZY = 2
-        EXEC = 3
-        LOAD = 4
-        DEAD = 5
+        PART = 3
+        EXEC = 4
+        LOAD = 5
+        DEAD = 6
+
+    class Exception(ImportError):
+        pass
+
+    class Error(Exception):
+        ldr: Loader
+        exc: BaseException
+
+        def __init__(self, ldr: Loader, exc: BaseException, msg: str, /):
+            self.ldr = ldr
+            self.exc = exc
+            super().__init__(msg)
 
     def __init__(self, spec: Spec):
         self.spec = spec
         self.loader = spec.loader
         spec.loader_state = Loader.State.INIT
 
     def create_module(self, spec: Spec | None = None):
@@ -51,26 +61,35 @@
 
         if self.__busy:
             return None
 
         self.__busy = True
 
         try:
-            target = spec.target if spec.target is not None else self.loader.create_module(spec)
-            target = ModuleType(spec.name) if target is None else target
-            target = spec.finder.Module(spec, target) if not isinstance(target, spec.finder.Module) else target
+            module = spec.target if spec.target is not None else self.loader.create_module(spec)
+            # module = self.module if module is None else module
+            module = ModuleType(spec.name) if module is None else module
+            module = spec.finder.Module(spec, module) if not isinstance(module, spec.finder.Module) else module
 
             spec.loader_state = Loader.State.CREA
 
-            if NO_LAZY:  # or spec.s_path is None:  # Consider whether spec is a package?
+            if spec.level > 0:
                 self.__forc = True
 
-            modules[spec.name] = target
+                if spec.level >= 2:
+                    module = spec.target
+
+                if spec.level >= 3:
+                    spec.loader_state = None
+                    module.__loader__ = self.loader
+                    spec.loader = self.loader
+                    spec.target = None
 
-            return target
+            self.module = module
+            return module
 
         finally:
             self.__busy = False
 
     def exec_module(self, module: Module, force: bool | None = None, /):
         spec = self.spec
         lazy = not ((force or self.__forc) if force is not None else self.__forc)
@@ -79,14 +98,15 @@
         name_ = spec.f_name
         state = spec.loader_state
         nexts = Loader.State.LAZY if lazy else Loader.State.EXEC
         target = spec.target
         in_sys = name in modules
 
         assert state in (Loader.State.CREA, Loader.State.LAZY), state
+        assert module is self.module, (module, self.module)
 
         if (mod := modules.get(name)) is not module:
             if in_sys:
                 assert None is debug.trace(
                     f"[{oid(module)}] {state} {nexts} [{oid(target) if target is not None else '*'*15}] {name_} "
                     f"::[{oid(mod) if mod is not target else 'same' if mod is not None else '-'}] "
                     "(before)"
@@ -99,43 +119,46 @@
 
         assert None is debug.traced(
             1,  # if nexts is Loader.State.EXEC else 2,
             f"[{oid(module)}] {state} {nexts} [{oid(target) if target is not None else '*'*15}] {name_} "
             f"{'>>>> ' if nexts is Loader.State.EXEC else '.... '}"
         )
 
-        if nexts < Loader.State.EXEC:
-            spec.loader_state = nexts
+        spec.loader_state = nexts
+
+        if nexts <= Loader.State.LAZY:
             return
 
         try:
-            spec.loader_state = state = nexts
-
             self.loader.exec_module(target if target is not None else module)
 
             state = nexts
             spec.loader_state = nexts = Loader.State.LOAD
             target = spec.target
 
             assert None is debug.traced(
                 1,  # if nexts is Loader.State.LOAD else 2,
                 f"[{oid(module)}] {state} {nexts} [{oid(target) if target is not None else '*'*15}] {name_} "
                 f"++++ "
             )
 
         except Exception as e:
-            spec.loader_state = nexts = Loader.State.DEAD
-            assert None is getattr(
-                debug,
-                "exception" if not isinstance(e, ImportError) and (TRACEE or TRACE > 0) else
-                "trace" if not TRACEE else "info"
-            )(
-                f"[{oid(module)}] {state} {nexts} [{oid(target) if target is not None else '*'*15}] {name_} !!!! " +
-                (('\n' + " " * 18 + f"!!!! {type(e).__name__}: {e}") if not isinstance(e, ImportError) else e.name)
+            spec.loader_state = nexts = Loader.State.DEAD if not isinstance(e, Loader.Exception) else Loader.State.PART
+
+            assert None is debug.traced(
+                0 if not isinstance(e, ImportError) else 1,
+                msg :=
+                f"[{oid(module)}] {state} {nexts} [{oid(target) if target is not None else '*'*15}] {name_} !!!! "
+                f"{type(e).__name__ if not isinstance(e, ImportError) else ''}"
             )
+
+            if nexts is Loader.State.DEAD:
+                modules.pop(name, None)
+                raise Loader.Error(self, e, f"Error loading {name_}" if not __debug__ else msg) from e
+
             raise
 
         if (mod := modules.get(name)) is not module:
             if in_sys:
                 assert None is debug.trace(
                     f"[{oid(module)}] {state} {nexts} [{oid(target) if target is not None else '*'*15}] {name_} "
                     f"::[{oid(mod) if mod is not target else 'same' if mod is not None else '-'}] "
@@ -143,25 +166,29 @@
                 ), "module was replaced in sys.modules after exec_module"
 
                 modules[name] = module
 
             if mod is not None and mod is not spec.target:
                 spec.target = mod
 
-    def invalidate_caches(self) -> None:
+    def invalidate_caches(self, keep: bool = False) -> None:
         spec = self.spec
+        mod = self.module
 
-        if (mod := modules.get(spec.name)) is spec.target and mod is not None:
-            del modules[spec.name]
+        if (mod_sys := modules.get(spec.name, object())) is mod or mod_sys is spec.target:
+            modules.pop(spec.name)
+            if keep:
+                modules[spec.name] = spec.target if spec.target is not None else mod if mod is not None else mod_sys
 
         assert None is debug.traced(
             2,
             f"[{oid(mod) if mod is not None else '*'*15}] "
-            f"{spec.loader_state} DEAD [{oid(spec.target) if spec.target else '*'*15}] {spec.f_name}"
+            f"{spec.loader_state} DEAD [{oid(spec.target) if spec.target is not None else '*'*15}] {spec.f_name} "
         )
 
         spec.loader = self.loader
         spec.loader_state = None  # type: ignore
         spec.target = None
         self.__forc = False
+        self.module = None
         self.spec = None  # type: ignore
         self.loader = None  # type: ignore
```

### Comparing `lazi-1.9.140/lazi/core/module.py` & `lazi-1.9.156/lazi/core/module.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.140/lazi/core/stat.py` & `lazi-1.9.156/lazi/core/stat.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.140/lazi/util/debug.py` & `lazi-1.9.156/lazi/util/debug.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.140/pyproject.toml` & `lazi-1.9.156/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.9.140"
+version = "1.9.156"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "readme.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
@@ -24,30 +24,47 @@
     { include = "lazi" }
 ]
 
 include = [
     { path = "tests", format = "sdist" }
 ]
 
+[tool.poe.tasks]
+
+git_commit_num.cmd = "git rev-list --count HEAD"
+git_commit_sha.cmd = "git show --pretty=format:'%H' --no-patch"
+pkg_version.cmd = "poetry version -s"
+
+commit-info.sequence = [
+    { ref = "pkg_version" },
+    { ref = "git_commit_num" },
+    { ref = "git_commit_sha" },
+]
+
+build.sequence = [
+    { ref = "commit-info" },
+    { cmd = "poetry build" },
+    { shell = "sha512sum dist/lazi-$(poetry version -s).tar.gz" },
+]
+
 [tool.poetry.dependencies]
 python = "^3.11"
 
 
-[tool.poetry.group.dev]
-optional = true
 [tool.poetry.group.dev.dependencies]
 django = "^4"
 requests = "^2"
 toolz = "^0"
 rich = "^13"
 setuptools = "^67"
 pandas = "^2"
 pytest = "^7"
 wagtail = "^5.0"
 presto-requests = "^1.3.6"
+poethepoet = "^0.20.0"
 
 [tool.poetry.group.direct]
 optional = true
 [tool.poetry.group.direct.dependencies]
 presto-requests = {git = "https://github.com/sitbon/presto"}
```

### Comparing `lazi-1.9.140/readme.md` & `lazi-1.9.156/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -101,26 +101,22 @@
 
 ## Tricky Situations
 
 ### Expected global state is not there.
 
 This is the most common issue when using `lazi.auto`, and can be difficult to debug.
 
-Fortunately, Lazi will show some useful tracebacks including the original exception before
-it was transformed into an `ImportError` (by CPython, thowing away the original traceback).
+Fortunately, Lazi wraps the original exception before it poetentially gets transformed into an `ImportError`.
 
-Example (with `TRACE=0` and `TRACEE=1`):
+Example (with `TRACE=0`):
 ```pycon
 >>> import lazi.auto
 >>> import pandas.core.nanops
-[7FABA3D89300] EXEC DEAD [7FABA3D89350] dateutil.tz|win !!!! six.moves  # This is an unrelated error that a module handled.
-[7FABA30D6B10] EXEC DEAD [7FABA30D5B70] pandas.core|nanops !!!! 
-                  !!!! OptionError: No such keys(s): 'compute.use_bottleneck'
 Traceback (most recent call last):
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<frozen importlib._bootstrap_external>", line 940, in exec_module
   File "<frozen importlib._bootstrap>", line 241, in _call_with_frames_removed
   File "<site-packages>/pandas/core/nanops.py", line 74, in <module>
     set_use_bottleneck(get_option("compute.use_bottleneck"))
                        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
   File "<site-packages>/pandas/_config/config.py", line 261, in __call__
@@ -128,59 +124,60 @@
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
   File "<site-packages>/pandas/_config/config.py", line 135, in _get_option
     key = _get_single_key(pat, silent)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
   File "<site-packages>/pandas/_config/config.py", line 121, in _get_single_key
     raise OptionError(f"No such keys(s): {repr(pat)}")
 pandas._config.config.OptionError: No such keys(s): 'compute.use_bottleneck'
-[7FABA2FCAE30] EXEC DEAD [7FABA2FCAED0] pandas.core.arrays.sparse|array !!!! pandas.core.nanops
-[7FABA2FCA480] EXEC DEAD [7FABA2FCA570] pandas.core.arrays.sparse|accessor !!!! pandas.core.nanops
-[7FABA2FCA390] EXEC DEAD [7FABA2FCA2A0] pandas.core.arrays.sparse !!!! pandas.core.nanops
-[7FABA3395440] EXEC DEAD [7FABA33953F0] pandas.core.arrays !!!! pandas.core.nanops # These lines without tracebacks
-[7FABA3342250] EXEC DEAD [7FABA33422A0] pandas.core|api !!!! pandas.core.nanops    #  are ImportErrors passed up
-[7FABF4F4D8A0] EXEC DEAD [7FABF4F4CE00] pandas !!!! pandas.core.nanops             #  in the load stack.
+
+The above exception was the direct cause of the following exception:
+
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
   File "/home/jq/pr/lazi/lazi/core/module.py", line 102, in __setattr__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/__init__.py", line 48, in <module>
     from pandas.core.api import (
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/core/api.py", line 27, in <module>
     from pandas.core.arrays import Categorical
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/core/arrays/__init__.py", line 19, in <module>
     from pandas.core.arrays.sparse import SparseArray
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/core/arrays/sparse/__init__.py", line 1, in <module>
     from pandas.core.arrays.sparse.accessor import (
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/core/arrays/sparse/accessor.py", line 16, in <module>
     from pandas.core.arrays.sparse.array import SparseArray
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/core/arrays/sparse/array.py", line 101, in <module>
     from pandas.core.nanops import check_below_min_count
-ImportError: cannot import name 'check_below_min_count' from 'pandas.core.nanops' (unknown location)
+  File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
+    spec.loader.exec_module(self, True)
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 136, in exec_module
+    raise Loader.Error(f"Error loading {name_}" if not __debug__ else msg) from e
+lazi.core.loader.Loader.Error: [7F899C139260] EXEC DEAD [7F899C1382C0] pandas.core|nanops !!!! OptionError
 >>> _
 ```
 
 _Unforunately_... This isn't something that can be worked around without outer dependency tracking, which
 generally results in entire packages getting loaded anyway.
 
 If you're more interested in just tracking imports with Lazi, use the `NO_HOOK` config variable (see below).
```

### Comparing `lazi-1.9.140/tests/standalone/sa_nested.py` & `lazi-1.9.156/tests/standalone/sa_nested.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.140/tests/test_django.py` & `lazi-1.9.156/tests/test_django.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,29 +8,35 @@
         debug.trace("test_django_version_lazy: finder.lazy ->")
         django = finder.lazy("django")
         debug.trace("test_django_version_lazy: ^- finder.lazy")
         version = django.VERSION
         debug.trace(f"test_django_version_lazy: ^- VERSION: {version}")
         assert isinstance(version, tuple), version
 
+    finder.invalidate_caches()
+
 
 def test_django_version_import():
     from lazi.util import debug
     from lazi.core.finder import Finder
 
-    with Finder():
+    with Finder() as finder:
         debug.trace("test_django_version_import: import django ->")
         import django
         debug.trace("test_django_version_import: ^- import django")
         version = django.VERSION
         debug.trace(f"test_django_version_import: ^- VERSION: {version}")
         assert isinstance(version, tuple), version
 
+    finder.invalidate_caches()
+
 
 def test_asgiref():
     from lazi.util import debug
     from lazi.core import lazi
 
     with lazi:
         debug.trace("-> from asgiref.sync import sync_to_async ->")
         from asgiref.sync import sync_to_async
         debug.trace("^- from asgiref.sync import sync_to_async -^")
+
+    lazi.invalidate_caches()
```

### Comparing `lazi-1.9.140/tests/test_importlib.py` & `lazi-1.9.156/tests/test_importlib.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,7 +25,9 @@
         else:
             module = importlib.import_module(name, package)
             if attr is not None:
                 with track(f"getattr({name}, {attr})"):
                     value = getattr(module, attr)
                     info(f"value: {repr(value)}")
             assert issubclass(type(module), expected_type)
+
+        lazi.invalidate_caches()
```

### Comparing `lazi-1.9.140/tests/test_requests.py` & `lazi-1.9.156/tests/test_requests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 
 
 def test_requests_parse_dict_header():
     from lazi.util import debug
     from lazi.core.finder import Finder
 
-    with Finder():
+    with Finder() as finder:
         debug.trace("-> from requests.utils import parse_dict_header ->")
         from requests.utils import parse_dict_header
         debug.trace("^- from requests.utils import parse_dict_header -^")
 
+    finder.invalidate_caches()
+
 
 def test_requests_presto_import():
     from lazi.util import debug
     from lazi.core.finder import Finder
 
-    with Finder():
+    with Finder() as finder:
         debug.trace("-> from presto import Presto ->")
         from presto import Presto
         debug.trace("^- from presto import Presto -^")
         debug.trace("-> p = Presto('https://httpbin.org') ->")
         p = Presto("https://httpbin.org")
         debug.trace("^- p = Presto('https://httpbin.org') -^")
+        finder.invalidate_caches()
```

### Comparing `lazi-1.9.140/tests/test_rich.py` & `lazi-1.9.156/tests/test_rich.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 def test_rich_fn_import_ctx():
     from lazi.util import debug
     from lazi.core.finder import Finder
 
-    with Finder():
+    with Finder() as finder:
         debug.trace("-> setup() ->")
 
         def setup():
             from rich import console as rc, pretty, traceback
             debug.trace("^- from rich import console as rc, pretty, traceback -^")
             debug.trace("-> console = rc.Console(color_system='256', force_terminal=True) ->")
             console = rc.Console(color_system="256", force_terminal=True)
@@ -18,7 +18,9 @@
             debug.trace("^- pretty.install(console=console) -^")
             debug.trace("-> traceback.install(console=console) ->")
             traceback.install(console=console)
             debug.trace("^- traceback.install(console=console) -^")
 
         setup()
         debug.trace("^- setup() -^")
+
+    finder.invalidate_caches()
```

### Comparing `lazi-1.9.140/tests/test_stat.py` & `lazi-1.9.156/tests/test_stat.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,32 +13,37 @@
             import django.test as dt
             info(Stat())
 
         with track("TestCase = dt.TestCase"):
             TestCase = dt.TestCase
             info(Stat())
 
+    lazi.invalidate_caches()
+
 
 # @pytest.mark.skip(reason="not working")
 def test_stat_presto():
     from lazi.util.debug import track, info
 
     from lazi.core.stat import Stat
     from lazi.core import lazi
 
     with lazi:
+        info(Stat())
+
         with track("import presto"):
-            info(Stat())
-            from presto import Presto
+            import presto
             info(Stat())
 
-        with track("p = Presto('https://httpbin.org')"):
-            p = Presto("https://httpbin.org")
+        with track("p = presto.Presto('https://httpbin.org')"):
+            p = presto.Presto("https://httpbin.org")
             info(Stat())
 
+    lazi.invalidate_caches()
+
 
 def test_stat_nolazi_presto():
     from lazi.util.debug import track, info
 
     from lazi.core.stat import Stat
 
     with track("import presto"):
```

### Comparing `lazi-1.9.140/PKG-INFO` & `lazi-1.9.156/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.9.140
+Version: 1.9.156
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Web Environment
@@ -12,18 +12,16 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Project-URL: Repository, https://github.com/sitbon/lazi
 Description-Content-Type: text/markdown
 
 # Lazi: Lazy Imports Everywhere
 
 An easy way to implement and track lazy imports globally.
@@ -127,26 +125,22 @@
 
 ## Tricky Situations
 
 ### Expected global state is not there.
 
 This is the most common issue when using `lazi.auto`, and can be difficult to debug.
 
-Fortunately, Lazi will show some useful tracebacks including the original exception before
-it was transformed into an `ImportError` (by CPython, thowing away the original traceback).
+Fortunately, Lazi wraps the original exception before it poetentially gets transformed into an `ImportError`.
 
-Example (with `TRACE=0` and `TRACEE=1`):
+Example (with `TRACE=0`):
 ```pycon
 >>> import lazi.auto
 >>> import pandas.core.nanops
-[7FABA3D89300] EXEC DEAD [7FABA3D89350] dateutil.tz|win !!!! six.moves  # This is an unrelated error that a module handled.
-[7FABA30D6B10] EXEC DEAD [7FABA30D5B70] pandas.core|nanops !!!! 
-                  !!!! OptionError: No such keys(s): 'compute.use_bottleneck'
 Traceback (most recent call last):
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<frozen importlib._bootstrap_external>", line 940, in exec_module
   File "<frozen importlib._bootstrap>", line 241, in _call_with_frames_removed
   File "<site-packages>/pandas/core/nanops.py", line 74, in <module>
     set_use_bottleneck(get_option("compute.use_bottleneck"))
                        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
   File "<site-packages>/pandas/_config/config.py", line 261, in __call__
@@ -154,59 +148,60 @@
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
   File "<site-packages>/pandas/_config/config.py", line 135, in _get_option
     key = _get_single_key(pat, silent)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
   File "<site-packages>/pandas/_config/config.py", line 121, in _get_single_key
     raise OptionError(f"No such keys(s): {repr(pat)}")
 pandas._config.config.OptionError: No such keys(s): 'compute.use_bottleneck'
-[7FABA2FCAE30] EXEC DEAD [7FABA2FCAED0] pandas.core.arrays.sparse|array !!!! pandas.core.nanops
-[7FABA2FCA480] EXEC DEAD [7FABA2FCA570] pandas.core.arrays.sparse|accessor !!!! pandas.core.nanops
-[7FABA2FCA390] EXEC DEAD [7FABA2FCA2A0] pandas.core.arrays.sparse !!!! pandas.core.nanops
-[7FABA3395440] EXEC DEAD [7FABA33953F0] pandas.core.arrays !!!! pandas.core.nanops # These lines without tracebacks
-[7FABA3342250] EXEC DEAD [7FABA33422A0] pandas.core|api !!!! pandas.core.nanops    #  are ImportErrors passed up
-[7FABF4F4D8A0] EXEC DEAD [7FABF4F4CE00] pandas !!!! pandas.core.nanops             #  in the load stack.
+
+The above exception was the direct cause of the following exception:
+
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
   File "/home/jq/pr/lazi/lazi/core/module.py", line 102, in __setattr__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/__init__.py", line 48, in <module>
     from pandas.core.api import (
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/core/api.py", line 27, in <module>
     from pandas.core.arrays import Categorical
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/core/arrays/__init__.py", line 19, in <module>
     from pandas.core.arrays.sparse import SparseArray
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/core/arrays/sparse/__init__.py", line 1, in <module>
     from pandas.core.arrays.sparse.accessor import (
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/core/arrays/sparse/accessor.py", line 16, in <module>
     from pandas.core.arrays.sparse.array import SparseArray
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
-  File "/home/jq/pr/lazi/lazi/core/loader.py", line 113, in exec_module
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 115, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<site-packages>/pandas/core/arrays/sparse/array.py", line 101, in <module>
     from pandas.core.nanops import check_below_min_count
-ImportError: cannot import name 'check_below_min_count' from 'pandas.core.nanops' (unknown location)
+  File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
+    spec.loader.exec_module(self, True)
+  File "/home/jq/pr/lazi/lazi/core/loader.py", line 136, in exec_module
+    raise Loader.Error(f"Error loading {name_}" if not __debug__ else msg) from e
+lazi.core.loader.Loader.Error: [7F899C139260] EXEC DEAD [7F899C1382C0] pandas.core|nanops !!!! OptionError
 >>> _
 ```
 
 _Unforunately_... This isn't something that can be worked around without outer dependency tracking, which
 generally results in entire packages getting loaded anyway.
 
 If you're more interested in just tracking imports with Lazi, use the `NO_HOOK` config variable (see below).
```

