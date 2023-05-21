# Comparing `tmp/configzen-0.1.26.tar.gz` & `tmp/configzen-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.26.tar", max compression
+gzip compressed data, was "configzen-0.1.27.tar", max compression
```

## Comparing `configzen-0.1.26.tar` & `configzen-0.1.27.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.26/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.26/configzen/__main__.py
--rw-r--r--   0        0        0    55346 2023-05-21 04:30:24.933672 configzen-0.1.26/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.26/configzen/errors.py
--rw-r--r--   0        0        0    19853 2023-05-21 04:30:24.907677 configzen-0.1.26/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.26/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.26/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.26/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-21 04:20:17.779499 configzen-0.1.26/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.26/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.26/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.27/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.27/configzen/__main__.py
+-rw-r--r--   0        0        0    55460 2023-05-21 04:38:55.177491 configzen-0.1.27/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.27/configzen/errors.py
+-rw-r--r--   0        0        0    19854 2023-05-21 04:35:55.247433 configzen-0.1.27/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.27/configzen/py.typed
+-rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.27/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.27/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-21 04:39:45.359411 configzen-0.1.27/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.27/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.27/PKG-INFO
```

### Comparing `configzen-0.1.26/configzen/__main__.py` & `configzen-0.1.27/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.26/configzen/config.py` & `configzen-0.1.27/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,16 +284,16 @@
     ----------
     obj
     """
     return obj.dict()
 
 
 def with_exporter(
-    func: Callable[[ConfigModelT],
-    dict[str, Any]], cls: type[ConfigModelT] | None = None
+    func: Callable[[ConfigModelT], dict[str, Any]],
+    cls: type[ConfigModelT] | None = None,
 ) -> type[ConfigModelT] | Any:
     """
     Register a custom exporter for a type.
 
     Parameters
     ----------
     func
@@ -304,15 +304,14 @@
     if cls is None:
         return functools.partial(with_exporter, func)
 
     export.register(cls, func)
     return cls
 
 
-
 @pre_serialize.register(list)
 def _ps_list(obj: list[Any]) -> list[Any]:
     """
     Convert a list to safely-serializable form.
 
     Parameters
     ----------
@@ -446,27 +445,40 @@
         "ensure_ascii": False,
         "indent": 2,
     }
 
     predefined_default_kwargs: ClassVar[dict[str, Any]] = {"encoding": "UTF-8"}
     default_allowed_url_schemes: ClassVar[set[str]] = {"file", "http", "https"}
 
-    _OPEN_KWARGS: ClassVar[frozenset[str]] = frozenset(
-        ("mode", "buffering", "encoding", "errors", "newline")
-    )
-    _URLOPEN_KWARGS: ClassVar[frozenset[str]] = frozenset(
-        (
-            "data",
-            "timeout",
-            "cafile",
-            "capath",
-            "cadefault",
-            "context",
-        )
-    )
+    OPEN_KWARGS: ClassVar[set[str]] = {
+        "mode",
+        "buffering",
+        "encoding",
+        "errors",
+        "newline",
+    }
+    URLOPEN_KWARGS: ClassVar[set[str]] = {
+        "data",
+        "timeout",
+        "cafile",
+        "capath",
+        "cadefault",
+        "context",
+    }
+    JSON_KWARGS: ClassVar[set[str]] = {
+        "skipkeys",
+        "ensure_ascii",
+        "check_circular",
+        "allow_nan",
+        "cls",
+        "indent",
+        "separators",
+        "default",
+        "sort_keys",
+    }
 
     def __init__(
         self,
         resource: RawResourceT,
         ac_parser: str | None = None,
         processor_class: type[Processor[ConfigModelT]] | None = None,
         *,
@@ -646,16 +658,15 @@
         Returns
         -------
         The dumped configuration.
         """
         if ac_parser is None:
             ac_parser = self.ac_parser
         if ac_parser == "json" and self.use_pydantic_json:
-            # xxx: Filter JSON kwargs to ensure safety?
-            kwargs = self.dump_options | kwargs
+            kwargs = filter_options(self.JSON_KWARGS, self.dump_options | kwargs)
             return config.json(**kwargs)
         return self.dump_data(export(config), ac_parser=ac_parser, **kwargs)
 
     def dump_data(
         self,
         data: dict[str, Any],
         ac_parser: str | None = None,
@@ -711,19 +722,19 @@
             url = urllib.parse.urlparse(cast(str, self.resource))
             if url.scheme not in self.allowed_url_schemes:
                 msg = (
                     f"URL scheme {url.scheme!r} is not allowed, "
                     f"must be one of {self.allowed_url_schemes!r}"
                 )
                 raise ValueError(msg)
-            kwds = filter_options(self._URLOPEN_KWARGS, kwds)
+            kwds = filter_options(self.URLOPEN_KWARGS, kwds)
             request = urllib.request.Request(url.geturl())
             return cast(ConfigIO, urllib.request.urlopen(request, **kwds))  # noqa: S310
         if isinstance(self.resource, (str, int, os.PathLike, pathlib.Path)):
-            kwds = filter_options(self._OPEN_KWARGS, kwds)
+            kwds = filter_options(self.OPEN_KWARGS, kwds)
             if isinstance(self.resource, int):
                 return cast(
                     ConfigIO,
                     # We intentionally do not use the context manager here
                     # because we do not want to close the file.
                     # Moreover, we want to allow the file to be opened
                     # from a file descriptor, not supported by Path().
@@ -769,15 +780,15 @@
         if not AIOFILES_AVAILABLE:
             msg = (
                 "aiofiles is not available, cannot open file "
                 "asynchronously (install with `pip install aiofiles`)"
             )
             raise RuntimeError(msg)
         if isinstance(self.resource, (str, int, os.PathLike, pathlib.Path)):
-            kwds = filter_options(self._OPEN_KWARGS, kwds)
+            kwds = filter_options(self.OPEN_KWARGS, kwds)
             return aiofiles.open(self.resource, **kwds)
         raise RuntimeError("cannot open resource asynchronously")
 
     def _get_default_kwargs(
         self,
         method: Literal["read", "write"],
         kwargs: dict[str, Any] | None = None,
@@ -1160,15 +1171,15 @@
         """
         return reload(self, **kwargs)
 
 
 def save(
     section: ConfigModelT | ConfigAt[ConfigModelT],
     write_kwargs: dict[str, Any] | None = None,
-    **kwargs: Any
+    **kwargs: Any,
 ) -> int:
     """
     Save the configuration.
 
     Parameters
     ----------
     section
@@ -1199,15 +1210,15 @@
     context.initial_state = data
     return result
 
 
 async def save_async(
     section: ConfigModelT | ConfigAt[ConfigModelT],
     write_kwargs: dict[str, Any] | None = None,
-    **kwargs: Any
+    **kwargs: Any,
 ) -> int:
     """
     Save the configuration asynchronously.
 
     Parameters
     ----------
     section
@@ -1674,16 +1685,15 @@
             and ConfigModel in type(value).mro()
             and not hasattr(value, CONTEXT)
         ):
             context.enter(name).bind_to(value)
         return value
 
     def __deepcopy__(
-        self: ConfigModelT,
-        memodict: dict[Any, Any] | None = None
+        self: ConfigModelT, memodict: dict[Any, Any] | None = None
     ) -> ConfigModelT:
         return self.parse_obj(export(self))
 
     def __getattribute__(self, attr: str) -> Any:
         value = super().__getattribute__(attr)
         if isinstance(value, ConfigModel):
             return self._ensure_settings_with_context(attr, value)
@@ -1738,22 +1748,19 @@
         if context.owner is self:
             new_config = context.loader.read(config_class=type(self), **kwargs)
             context.bind_to(new_config)
             context.initial_state = new_config.__dict__
             new_config.rollback()
             return new_config
         return cast(
-            ConfigModelT,
-            reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
+            ConfigModelT, reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
         )
 
     def save(
-        self: ConfigModelT,
-        write_kwargs: dict[str, Any] | None = None,
-        **kwargs: Any
+        self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
     ) -> int:
         """
         Save the configuration to the configuration file.
 
         Parameters
         ----------
         write_kwargs
@@ -1849,21 +1856,19 @@
             new_async_config = await context.loader.read_async(**kwargs)
             context.bind_to(new_async_config)
             context.initial_state = new_async_config.__dict__
             self.rollback()
             return new_async_config
         return cast(
             ConfigModelT,
-            await reload_async(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
+            await reload_async(cast(ConfigAt[ConfigModelT], context.at), **kwargs),
         )
 
     async def save_async(
-        self: ConfigModelT,
-        write_kwargs: dict[str, Any] | None = None,
-        **kwargs: Any
+        self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
     ) -> int:
         """
         Save the configuration to the configuration file asynchronously.
 
         Parameters
         ----------
         write_kwargs
@@ -1882,15 +1887,15 @@
             blob = context.loader.dump_config(self, **kwargs)
             result = await self.write_async(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
         return await save_async(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
-            **kwargs
+            **kwargs,
         )
 
     async def write_async(self, blob: str, **kwargs: Any) -> int:
         """
         Overwrite the configuration file asynchronously with the given string or bytes.
 
         Parameters
```

### Comparing `configzen-0.1.26/configzen/errors.py` & `configzen-0.1.27/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.26/configzen/processor.py` & `configzen-0.1.27/configzen/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,15 @@
             The state to export.
         metadata
             The metadata of the substitution.
         """
         if is_dict_like(state):
             if metadata is None:
                 from configzen.config import CONTEXT
+
                 state.pop(CONTEXT, None)
                 metadata = state.pop(SUBST_METADATA, None)
             if metadata:
                 cls._export(state, metadata)
             else:
                 cls.export(list(state.values()), metadata=None)
         elif is_list_like(state):
```

### Comparing `configzen-0.1.26/configzen/typedefs.py` & `configzen-0.1.27/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.26/LICENSE` & `configzen-0.1.27/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.26/pyproject.toml` & `configzen-0.1.27/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.26"
+version = "0.1.27"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.26/README.md` & `configzen-0.1.27/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.26/PKG-INFO` & `configzen-0.1.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.26
+Version: 0.1.27
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

