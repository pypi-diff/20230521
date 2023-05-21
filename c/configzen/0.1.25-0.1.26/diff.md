# Comparing `tmp/configzen-0.1.25.tar.gz` & `tmp/configzen-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.25.tar", max compression
+gzip compressed data, was "configzen-0.1.26.tar", max compression
```

## Comparing `configzen-0.1.25.tar` & `configzen-0.1.26.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.25/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.25/configzen/__main__.py
--rw-r--r--   0        0        0    54369 2023-05-21 04:13:06.218438 configzen-0.1.25/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.25/configzen/errors.py
--rw-r--r--   0        0        0    19841 2023-05-20 00:22:31.783945 configzen-0.1.25/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.25/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.25/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.25/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-21 04:13:25.968387 configzen-0.1.25/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.25/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.25/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.26/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.26/configzen/__main__.py
+-rw-r--r--   0        0        0    55346 2023-05-21 04:30:24.933672 configzen-0.1.26/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.26/configzen/errors.py
+-rw-r--r--   0        0        0    19853 2023-05-21 04:30:24.907677 configzen-0.1.26/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.26/configzen/py.typed
+-rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.26/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.26/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-21 04:20:17.779499 configzen-0.1.26/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.26/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.26/PKG-INFO
```

### Comparing `configzen-0.1.25/configzen/__main__.py` & `configzen-0.1.26/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.25/configzen/config.py` & `configzen-0.1.26/configzen/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -105,20 +105,18 @@
     "ConfigLoader",
     "ConfigModel",
     "ConfigMeta",
     "save",
     "save_async",
     "reload",
     "reload_async",
-    "convert",
-    "converter",
-    "convert_namedtuple",
-    "convert_mapping",
-    "generic_validate",
-    "generic_validator",
+    "pre_serialize",
+    "with_pre_serialize",
+    "post_deserialize",
+    "with_post_deserialize",
 )
 
 _URL_SCHEMES: set[str] = set(
     urllib.parse.uses_relative + urllib.parse.uses_netloc + urllib.parse.uses_params,
 ) - {""}
 CONTEXT: str = "__configzen_context__"
 
@@ -148,15 +146,15 @@
 ) -> bool:
     return (
         isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields")
     )
 
 
 @functools.singledispatch
-def convert(obj: Any) -> Any:
+def pre_serialize(obj: Any) -> Any:
     """
     Convert a value to a format that can be safely serialized.
 
     This function is used to convert values that are not supported by
     `anyconfig` to a format that can be safely serialized. It is used
     internally by `ConfigModel` and `AsyncConfigModel` to convert
     values before saving them to a file.
@@ -167,27 +165,29 @@
         The value to convert.
 
     Returns
     -------
     Any
     """
     if dataclasses.is_dataclass(obj):
-        return convert(dataclasses.asdict(obj))
+        return pre_serialize(dataclasses.asdict(obj))
     if _is_namedtuple(obj):
-        return convert_namedtuple(obj)
+        return _ps_namedtuple(obj)
     return obj
 
 
 for obj_type, encoder in ENCODERS_BY_TYPE.items():
-    convert.register(obj_type, encoder)
+    pre_serialize.register(obj_type, encoder)
 
 
-def converter(func: Callable[[T], Any], cls: type[T] | None = None) -> type[T] | Any:
+def with_pre_serialize(
+    func: Callable[[T], Any], cls: type[T] | None = None
+) -> type[T] | Any:
     """
-    Register a converter function for a type.
+    Register a pre-serialization converter function for a type.
 
     Parameters
     ----------
     func
         The converter function.
 
     cls
@@ -198,38 +198,38 @@
     -------
     The conversion result class.
 
     Usage
     -----
     .. code-block:: python
 
-        @converter(converter_func)
+        @with_pre_serialize(converter_func)
         class MyClass:
             ...
 
     """
     if cls is None:
-        return functools.partial(converter, func)
+        return functools.partial(with_pre_serialize, func)
 
-    convert.register(cls, func)
+    pre_serialize.register(cls, func)
 
     if not hasattr(cls, "__get_validators__"):
 
         def validator_gen() -> Generator[Callable[[Any], Any], None, None]:
-            yield lambda value: generic_validate.dispatch(cls)(cls, value)
+            yield lambda value: post_deserialize.dispatch(cls)(cls, value)
 
         cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
 
     return cls
 
 
 @functools.singledispatch
-def generic_validate(cls: Any, value: Any) -> Any:
+def post_deserialize(cls: Any, value: Any) -> Any:
     """
-    Load a value into a type.
+    Load a value into a type after deserialization.
 
     This function is used to load values that are not supported by
     `anyconfig` to a format that can be used at runtime. It is used
     by pydantic while performing validation.
 
     Parameters
     ----------
@@ -244,15 +244,15 @@
     The loaded value.
     """
     if isinstance(value, cls):
         return value
     return cls(value)
 
 
-def generic_validator(
+def with_post_deserialize(
     func: Callable[[Any], T], cls: type[T] | None = None
 ) -> type[T] | Any:
     """
     Register a loader function for a type.
 
     Parameters
     ----------
@@ -263,71 +263,107 @@
 
     Returns
     -------
     The loading result class.
     """
 
     if cls is None:
-        return functools.partial(generic_validator, func)
+        return functools.partial(with_post_deserialize, func)
 
-    generic_validate.register(cls, func)
+    post_deserialize.register(cls, func)
     return cls
 
 
-@convert.register(list)
-def convert_list(obj: list[Any]) -> list[Any]:
+@functools.singledispatch
+def export(obj: ConfigModelT) -> dict[str, Any]:
+    """
+    Export a ConfigModel to a safely-serializable format.
+    Register a custom exporter for a type using the `with_exporter` decorator,
+    which can help to exclude particular values from the export if needed.
+
+    Parameters
+    ----------
+    obj
+    """
+    return obj.dict()
+
+
+def with_exporter(
+    func: Callable[[ConfigModelT],
+    dict[str, Any]], cls: type[ConfigModelT] | None = None
+) -> type[ConfigModelT] | Any:
+    """
+    Register a custom exporter for a type.
+
+    Parameters
+    ----------
+    func
+        The exporter function.
+    cls
+        The type to register the exporter for.
+    """
+    if cls is None:
+        return functools.partial(with_exporter, func)
+
+    export.register(cls, func)
+    return cls
+
+
+
+@pre_serialize.register(list)
+def _ps_list(obj: list[Any]) -> list[Any]:
     """
     Convert a list to safely-serializable form.
 
     Parameters
     ----------
     obj
         The list to convert.
 
     Returns
     -------
     The converted list.
     """
-    return [convert(item) for item in obj]
+    return [pre_serialize(item) for item in obj]
 
 
-@convert.register(collections.abc.Mapping)
-def convert_mapping(obj: collections.abc.Mapping[Any, Any]) -> dict[Any, Any]:
+@pre_serialize.register(collections.abc.Mapping)
+def _ps_mapping(obj: collections.abc.Mapping[Any, Any]) -> dict[Any, Any]:
     """
     Convert a mapping to safely-serializable form.
 
     Parameters
     ----------
     obj
         The mapping to convert.
 
     Returns
     -------
     The converted mapping.
     """
-    return {k: convert(v) for k, v in obj.items()}
+    return {k: pre_serialize(v) for k, v in obj.items()}
 
 
 @functools.singledispatch
-def convert_namedtuple(obj: tuple[Any, ...]) -> Any:
+def _ps_namedtuple(obj: tuple[Any, ...]) -> Any:
     """
     Convert a namedtuple to safely-serializable form.
 
     Parameters
     ----------
     obj
         The namedtuple to convert.
 
     Returns
     -------
     The converted namedtuple (likely a list).
     """
-    # Initially I wanted it to be convert(obj._asdict()), but
-    # pydantic doesn't seem to be friends with custom NamedTuples.
-    return convert(list(obj))
+    # Initially I wanted it to be pre_serialize(obj._asdict()), but
+    # pydantic doesn't seem to be friends with custom NamedTuple-s.
+    return pre_serialize(list(obj))
 
 
 def _delegate_ac_options(
     load_options: dict[str, Any], dump_options: dict[str, Any], options: dict[str, Any]
 ) -> None:
     for key, value in options.items():
         if key.startswith("dump_"):
@@ -611,16 +647,17 @@
         -------
         The dumped configuration.
         """
         if ac_parser is None:
             ac_parser = self.ac_parser
         if ac_parser == "json" and self.use_pydantic_json:
             # xxx: Filter JSON kwargs to ensure safety?
+            kwargs = self.dump_options | kwargs
             return config.json(**kwargs)
-        return self.dump_data(config.dict(), ac_parser=ac_parser, **kwargs)
+        return self.dump_data(export(config), ac_parser=ac_parser, **kwargs)
 
     def dump_data(
         self,
         data: dict[str, Any],
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> str:
@@ -639,15 +676,15 @@
         Returns
         -------
         The dumped configuration.
         """
         if ac_parser is None:
             ac_parser = self.ac_parser
         kwargs = self.dump_options | kwargs
-        return anyconfig.dumps(convert(data), ac_parser=ac_parser, **kwargs)
+        return anyconfig.dumps(pre_serialize(data), ac_parser=ac_parser, **kwargs)
 
     @property
     def is_url(self) -> bool:
         """Whether the resource is a URL."""
         return (
             isinstance(self.resource, str)
             and urllib.parse.urlparse(self.resource).scheme in _URL_SCHEMES
@@ -1499,15 +1536,15 @@
     except RuntimeError:
         context = None
     return context
 
 
 def _json_encoder(model_encoder: Callable[..., Any], value: Any, **kwargs: Any) -> Any:
     initial_state_type = type(value)
-    converted_value = convert(value)
+    converted_value = pre_serialize(value)
     if isinstance(converted_value, initial_state_type):
         return model_encoder(value, **kwargs)
     return converted_value
 
 
 class ConfigModelMetaclass(ModelMetaclass):
     def __new__(
@@ -1640,15 +1677,15 @@
             context.enter(name).bind_to(value)
         return value
 
     def __deepcopy__(
         self: ConfigModelT,
         memodict: dict[Any, Any] | None = None
     ) -> ConfigModelT:
-        return self.parse_obj(self.dict())
+        return self.parse_obj(export(self))
 
     def __getattribute__(self, attr: str) -> Any:
         value = super().__getattribute__(attr)
         if isinstance(value, ConfigModel):
             return self._ensure_settings_with_context(attr, value)
         return value
```

### Comparing `configzen-0.1.25/configzen/errors.py` & `configzen-0.1.26/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.25/configzen/processor.py` & `configzen-0.1.26/configzen/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -611,15 +611,15 @@
         Exports model state preserving substition directive calls in the model state.
 
         Parameters
         ----------
         metadata
         state
         """
-        from configzen.config import at, convert, CONTEXT
+        from configzen.config import at, pre_serialize, CONTEXT
 
         overrides = {}
 
         route = metadata["route"]
         context = metadata["context"]
         loader = context.loader
 
@@ -634,15 +634,15 @@
 
         missing = object()
 
         for key, value in loaded.items():
             counterpart_value = state.pop(key, missing)
             if counterpart_value is missing:
                 continue
-            counterpart_value = convert(counterpart_value)
+            counterpart_value = pre_serialize(counterpart_value)
 
             if is_dict_like(value):
                 if SUBST_METADATA in value:
                     value.pop(CONTEXT, None)
                     cls.export(value, metadata=value.pop(SUBST_METADATA))
                 overrides_for_key = {
                     sub_key: comp
```

### Comparing `configzen-0.1.25/configzen/typedefs.py` & `configzen-0.1.26/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.25/LICENSE` & `configzen-0.1.26/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.25/pyproject.toml` & `configzen-0.1.26/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.25"
+version = "0.1.26"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.25/README.md` & `configzen-0.1.26/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.25/PKG-INFO` & `configzen-0.1.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.25
+Version: 0.1.26
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

