# Comparing `tmp/configzen-0.1.24.tar.gz` & `tmp/configzen-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.24.tar", max compression
+gzip compressed data, was "configzen-0.1.25.tar", max compression
```

## Comparing `configzen-0.1.24.tar` & `configzen-0.1.25.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.24/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.24/configzen/__main__.py
--rw-r--r--   0        0        0    53152 2023-05-20 00:12:29.622344 configzen-0.1.24/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.24/configzen/errors.py
--rw-r--r--   0        0        0    19828 2023-05-20 00:04:43.942145 configzen-0.1.24/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.24/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.24/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.24/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-20 00:14:57.999530 configzen-0.1.24/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.24/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.24/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.25/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.25/configzen/__main__.py
+-rw-r--r--   0        0        0    54369 2023-05-21 04:13:06.218438 configzen-0.1.25/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.25/configzen/errors.py
+-rw-r--r--   0        0        0    19841 2023-05-20 00:22:31.783945 configzen-0.1.25/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.25/configzen/py.typed
+-rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.25/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.25/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-21 04:13:25.968387 configzen-0.1.25/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.25/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.25/PKG-INFO
```

### Comparing `configzen-0.1.24/configzen/__main__.py` & `configzen-0.1.25/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.24/configzen/config.py` & `configzen-0.1.25/configzen/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1120,72 +1120,88 @@
         Returns
         -------
         The reloaded configuration or its belonging item.
         """
         return reload(self, **kwargs)
 
 
-def save(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> int:
+def save(
+    section: ConfigModelT | ConfigAt[ConfigModelT],
+    write_kwargs: dict[str, Any] | None = None,
+    **kwargs: Any
+) -> int:
     """
     Save the configuration.
 
     Parameters
     ----------
     section
         The configuration model instance or the configuration item.
+    write_kwargs
+        Keyword arguments to pass to the writing function.
     **kwargs
-        Keyword arguments to pass to the saving function.
+        Keyword arguments to pass to the dumping function.
 
     Returns
     -------
     The number of bytes written.
     """
     if isinstance(section, ConfigModel):
         config = section
-        return config.save()
+        return config.save(write_kwargs=write_kwargs, **kwargs)
+
+    if write_kwargs is None:
+        write_kwargs = {}
 
     config = section.owner
     data = config.initial_state
-    at = ConfigAt(config, data, section.route)
-    data = at.update(section.get())
+    scope = ConfigAt(config, data, section.route)
+    data = scope.update(section.get())
     context = get_context(config)
-    blob = context.loader.dump_config(config.copy(update=data))
-    result = config.write(blob, **kwargs)
+    blob = context.loader.dump_config(config.copy(update=data), **kwargs)
+    result = config.write(blob, **write_kwargs)
     context.initial_state = data
     return result
 
 
 async def save_async(
-    section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any
+    section: ConfigModelT | ConfigAt[ConfigModelT],
+    write_kwargs: dict[str, Any] | None = None,
+    **kwargs: Any
 ) -> int:
     """
     Save the configuration asynchronously.
 
     Parameters
     ----------
     section
         The configuration model instance or the configuration item.
+    write_kwargs
+        Keyword arguments to pass to the writing function.
     **kwargs
-        Keyword arguments to pass to the saving function.
+        Keyword arguments to pass to the dumping function.
 
     Returns
     -------
     The number of bytes written.
     """
     if isinstance(section, ConfigModel):
         config = section
-        return await config.save_async(**kwargs)
+        return await config.save_async(write_kwargs=write_kwargs, **kwargs)
+
+    if write_kwargs is None:
+        write_kwargs = {}
 
     config = section.owner
     data = config.initial_state
-    at = ConfigAt(config, data, section.route)
-    data = at.update(section.get())
+    scope = ConfigAt(config, data, section.route)
+    data = scope.update(section.get())
     context = get_context(config)
-    blob = context.loader.dump_config(config.copy(update=data))
-    result = await config.write_async(blob, **kwargs)
+    blob = context.loader.dump_config(config.copy(update=data), **kwargs)
+    result = await config.write_async(blob, **write_kwargs)
     context.initial_state = data
     return result
 
 
 def reload(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> Any:
     """
     Reload the configuration.
@@ -1489,15 +1505,15 @@
     initial_state_type = type(value)
     converted_value = convert(value)
     if isinstance(converted_value, initial_state_type):
         return model_encoder(value, **kwargs)
     return converted_value
 
 
-class CMBMetaclass(ModelMetaclass):
+class ConfigModelMetaclass(ModelMetaclass):
     def __new__(
         cls,
         name: str,
         bases: tuple[type, ...],
         namespace: dict[str, Any],
         **kwargs: Any,
     ) -> type:
@@ -1511,15 +1527,15 @@
             new_class.__json_encoder__,
         )
         return cast(type, new_class)
 
 
 class ConfigModel(
     pydantic.BaseSettings,
-    metaclass=CMBMetaclass,
+    metaclass=ConfigModelMetaclass,
     root=True,
 ):
     """
     The base class for configuration models.
 
     It is not recommended to inherit from this class directly for basic usage.
     Instead, use either :class:`ConfigModel` or :class:`AsyncConfigModel`.
@@ -1684,36 +1700,51 @@
         context = get_context(self)
         if context.owner is self:
             new_config = context.loader.read(config_class=type(self), **kwargs)
             context.bind_to(new_config)
             context.initial_state = new_config.__dict__
             new_config.rollback()
             return new_config
-        return cast(ConfigModelT, reload(cast(ConfigAt[ConfigModelT], context.at)))
+        return cast(
+            ConfigModelT,
+            reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
+        )
 
-    def save(self: ConfigModelT, **kwargs: Any) -> int:
+    def save(
+        self: ConfigModelT,
+        write_kwargs: dict[str, Any] | None = None,
+        **kwargs: Any
+    ) -> int:
         """
         Save the configuration to the configuration file.
 
         Parameters
         ----------
-        **kwargs
+        write_kwargs
             Keyword arguments to pass to the write method.
+        **kwargs
+            Keyword arguments to pass to the dumping method.
 
         Returns
         -------
         The number of bytes written.
         """
         context = get_context(self)
         if context.owner is self:
-            blob = context.loader.dump_config(self)
-            result = self.write(blob, **kwargs)
+            if write_kwargs is None:
+                write_kwargs = {}
+            blob = context.loader.dump_config(self, **kwargs)
+            result = self.write(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
-        return save(cast(ConfigAt[ConfigModelT], context.at))
+        return save(
+            cast(ConfigAt[ConfigModelT], context.at),
+            write_kwargs=write_kwargs,
+            **kwargs,
+        )
 
     def write(self, blob: str, **kwargs: Any) -> int:
         """
         Overwrite the configuration file with the given string or bytes.
 
         Parameters
         ----------
@@ -1780,37 +1811,50 @@
         if context.owner is self:
             new_async_config = await context.loader.read_async(**kwargs)
             context.bind_to(new_async_config)
             context.initial_state = new_async_config.__dict__
             self.rollback()
             return new_async_config
         return cast(
-            ConfigModelT, await reload_async(cast(ConfigAt[ConfigModelT], context.at))
+            ConfigModelT,
+            await reload_async(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
         )
 
-    async def save_async(self: ConfigModelT, **kwargs: Any) -> int:
+    async def save_async(
+        self: ConfigModelT,
+        write_kwargs: dict[str, Any] | None = None,
+        **kwargs: Any
+    ) -> int:
         """
         Save the configuration to the configuration file asynchronously.
 
         Parameters
         ----------
-        **kwargs
+        write_kwargs
             Keyword arguments to pass to the write method.
+        **kwargs
+            Keyword arguments to pass to the dumping method.
 
         Returns
         -------
         The number of bytes written.
         """
         context = get_context(self)
         if context.owner is self:
-            blob = context.loader.dump_config(self)
-            result = await self.write_async(blob, **kwargs)
+            if write_kwargs is None:
+                write_kwargs = {}
+            blob = context.loader.dump_config(self, **kwargs)
+            result = await self.write_async(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
-        return await save_async(cast(ConfigAt[ConfigModelT], context.at))
+        return await save_async(
+            cast(ConfigAt[ConfigModelT], context.at),
+            write_kwargs=write_kwargs,
+            **kwargs
+        )
 
     async def write_async(self, blob: str, **kwargs: Any) -> int:
         """
         Overwrite the configuration file asynchronously with the given string or bytes.
 
         Parameters
         ----------
```

### Comparing `configzen-0.1.24/configzen/errors.py` & `configzen-0.1.25/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.24/configzen/processor.py` & `configzen-0.1.25/configzen/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -561,15 +561,15 @@
 
         loader_class = type(self.loader)
 
         if len(ctx.arguments) > 1:
             msg = f"{ctx.directive!r} directive can select only one section"
             raise ConfigPreprocessingError(msg)
 
-        if ctx.has_duplicates(require_same_arguments=False):
+        if preserve and ctx.has_duplicates(require_same_arguments=False):
             msg = (
                 f"using more than one {ctx.directive!r} directive "
                 "in the same section is not allowed"
             )
             raise ConfigPreprocessingError(msg)
 
         loader = loader_class.from_directive_context(ctx)
```

### Comparing `configzen-0.1.24/configzen/typedefs.py` & `configzen-0.1.25/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.24/LICENSE` & `configzen-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.24/pyproject.toml` & `configzen-0.1.25/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.24"
+version = "0.1.25"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.24/README.md` & `configzen-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.24/PKG-INFO` & `configzen-0.1.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.24
+Version: 0.1.25
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

