# Comparing `tmp/configzen-0.1.29.tar.gz` & `tmp/configzen-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.29.tar", max compression
+gzip compressed data, was "configzen-0.1.30.tar", max compression
```

## Comparing `configzen-0.1.29.tar` & `configzen-0.1.30.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.29/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.29/configzen/__main__.py
--rw-r--r--   0        0        0    55527 2023-05-21 05:27:05.631245 configzen-0.1.29/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.29/configzen/errors.py
--rw-r--r--   0        0        0    19854 2023-05-21 04:35:55.247433 configzen-0.1.29/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.29/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.29/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.29/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-21 05:30:21.377497 configzen-0.1.29/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.29/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.29/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.30/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.30/configzen/__main__.py
+-rw-r--r--   0        0        0    56508 2023-05-21 13:26:11.847024 configzen-0.1.30/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.30/configzen/errors.py
+-rw-r--r--   0        0        0    19939 2023-05-21 13:23:41.824893 configzen-0.1.30/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.30/configzen/py.typed
+-rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.30/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.30/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-21 13:23:24.640346 configzen-0.1.30/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.30/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.30/PKG-INFO
```

### Comparing `configzen-0.1.29/configzen/__main__.py` & `configzen-0.1.30/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.29/configzen/config.py` & `configzen-0.1.30/configzen/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -921,87 +921,102 @@
         """
         kwargs = self._get_default_kwargs("write", kwargs=kwargs)
         async with self.open_resource_async(**kwargs) as fp:
             return await fp.write(blob)
 
     @classmethod
     def from_directive_context(
-        cls, ctx: DirectiveContext, /
-    ) -> ConfigLoader[ConfigModelT]:
+        cls,
+        ctx: DirectiveContext,
+        /,
+        route_separator: str = ":",
+        route_class: type[Route] | None = None,
+    ) -> tuple[ConfigLoader[ConfigModelT], SupportsRoute | None]:
         """
         Create a configuration loader from a preprocessor directive context.
+        Return an optional scope that the context points to.
 
         Parameters
         ----------
+        route_class
+        route_separator
         ctx
 
         Returns
         -------
         The configuration loader.
         """
+        if route_class is None:
+            route_class = Route
+        route: SupportsRoute | None = None
         args: list[Any] = []
         kwargs: dict[str, Any] = {}
-        if isinstance(ctx.snippet, (str, int)):
+        if isinstance(ctx.snippet, str):
+            path, _, route = ctx.snippet.partition(route_separator)
+            route = Route(route.strip().replace(route_separator, route_class.TOK_DOT))
+            args.append(path)
+        elif isinstance(ctx.snippet, int):
             args.append(ctx.snippet)
         elif is_dict_like(ctx.snippet):
             kwargs |= ctx.snippet
         elif is_list_like(ctx.snippet):
             args += list(ctx.snippet)
         else:
             msg = (
                 f"invalid snippet for the {ctx.directive!r} directive: {ctx.snippet!r}"
             )
             raise ValueError(msg)
-        return cls(*args, **kwargs)
+        return cls(*args, **kwargs), str(route)
 
 
 class Route:
-    _TOK_DOT = "."
-    _TOK_DOTLIST_ESCAPE_LEFT = "["
-    _TOK_DOTLIST_ESCAPE_RIGHT = "]"
+    TOK_DOT = "."
+    TOK_DOTLIST_ESCAPE_ENTER = "["
+    TOK_DOTLIST_ESCAPE_EXIT = "]"
 
     def __init__(self, route: SupportsRoute) -> None:
         self.list_route = self.parse(route)
 
     @classmethod
     def parse(cls, route: SupportsRoute) -> list[str]:
         if isinstance(route, Route):
             return route.list_route
         if isinstance(route, list):
             return route
         if isinstance(route, str):
-            return cls._decompose(route)
+            with format_syntax_error(route):
+                return cls._decompose(route)
         raise TypeError(f"invalid route type {type(route)!r}")
 
     @classmethod
     def _decompose(cls, route: str) -> list[str]:
-        route = route.removesuffix(cls._TOK_DOT) + cls._TOK_DOT[0]
+        route = route.removesuffix(cls.TOK_DOT) + cls.TOK_DOT[0]
         argument = ""
         escape_ctx = False
         prev_char = None
         list_route = []
         for char_no, char in enumerate(route, start=1):
-            if char in cls._TOK_DOT:
+            if char in cls.TOK_DOT:
                 if escape_ctx:
                     argument += char
                 else:
                     list_route.append(argument)
                     argument = ""
-            elif char in cls._TOK_DOTLIST_ESCAPE_LEFT:
-                if prev_char and prev_char in cls._TOK_DOTLIST_ESCAPE_RIGHT:
+            elif char in cls.TOK_DOTLIST_ESCAPE_ENTER:
+                if prev_char and prev_char in cls.TOK_DOTLIST_ESCAPE_EXIT:
                     raise InternalConfigError(
                         "invalid escape sequence "
-                        f"(expected {cls._TOK_DOT[0]} between escape sequences)",
+                        f"(expected {cls.TOK_DOT[0]} between escape sequences)",
                         extra=char_no,
                     )
                 if escape_ctx:
                     msg = "invalid escape sequence"
                     raise InternalConfigError(msg, extra=char_no)
                 escape_ctx = True
-            elif char in cls._TOK_DOTLIST_ESCAPE_RIGHT:
+            elif char in cls.TOK_DOTLIST_ESCAPE_EXIT:
                 if not escape_ctx:
                     msg = "invalid escape sequence"
                     raise InternalConfigError(msg, extra=char_no)
                 escape_ctx = False
                 list_route.append(argument)
                 argument = ""
             else:
@@ -1010,14 +1025,25 @@
         return list_route
 
     @classmethod
     def decompose(cls, route: str) -> list[str]:
         with format_syntax_error(route):
             return cls._decompose(route)
 
+    def compose(self) -> str:
+        escape = (self.TOK_DOTLIST_ESCAPE_ENTER, self.TOK_DOTLIST_ESCAPE_EXIT)
+        raw = ("", "")
+        return self.TOK_DOT.join(
+            fragment.join(escape) if self.TOK_DOT in fragment else fragment.join(raw)
+            for fragment in self.list_route
+        )
+
+    def __str__(self) -> str:
+        return self.compose()
+
     def __iter__(self) -> Generator[str, None, None]:
         yield from self.list_route
 
 
 def at(
     mapping: Any,
     route: SupportsRoute,
```

### Comparing `configzen-0.1.29/configzen/errors.py` & `configzen-0.1.30/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.29/configzen/processor.py` & `configzen-0.1.30/configzen/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,14 +435,15 @@
     PROCESSOR = "processor"
     DEFINE = "define"
 
 
 class Processor(BaseProcessor[ConfigModelT]):
     directive_prefix = "^"
     extension_prefix = "+"
+    route_separator: ClassVar[str] = ":"
 
     @directive(Directives.EXTEND)
     def extend(self, ctx: DirectiveContext) -> None:
         """
         extend a configuration with another configuration.
         Recursively preprocess the referenced configuration.
         Preserve information about the referenced configuration.
@@ -558,51 +559,55 @@
     def _substitute(
         self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
     ) -> None:
         from configzen.config import CONTEXT, Context, at
 
         loader_class = type(self.loader)
 
-        if len(ctx.arguments) > 1:
-            msg = f"{ctx.directive!r} directive can select only one section"
+        if len(ctx.arguments):
+            msg = f"{ctx.directive!r} directive takes no () arguments"
             raise ConfigPreprocessingError(msg)
 
         if preserve and ctx.has_duplicates(require_same_arguments=False):
             msg = (
                 f"using more than one {ctx.directive!r} directive "
                 "in the same section is not allowed"
             )
             raise ConfigPreprocessingError(msg)
 
-        loader = loader_class.from_directive_context(ctx)
+        loader, substitution_route = loader_class.from_directive_context(
+            ctx, route_separator=self.route_separator
+        )
 
         if loader.resource == self.loader.resource:
             raise ConfigPreprocessingError(
                 f"{loader.resource} tried to {ctx.directive!r} on itself"
             )
 
         with loader.processor_open_resource() as reader:
             substituted = loader.load_into_dict(reader.read(), preprocess=preprocess)
 
-        substitution_route = ctx.arguments[0] if ctx.arguments else None
         if substitution_route:
             substituted = at(substituted, substitution_route, loader=loader)
             if not is_dict_like(substituted):
                 raise ConfigPreprocessingError(
                     f"imported item {substitution_route!r} "
                     f"from {loader.resource} is not a dictionary"
                 )
+
         context: Context[ConfigModelT] = Context(loader)
         ctx.container = substituted | ctx.container
 
         if preserve:
             ctx.container |= {
                 CONTEXT: context,
                 SUBST_METADATA: SubstitutionMetadata(
-                    route=substitution_route, context=context, preprocess=preprocess
+                    route=str(substitution_route),
+                    context=context,
+                    preprocess=preprocess,
                 ),
             }
 
     @classmethod
     def _export(
         cls,
         state: dict[str, Any],
```

### Comparing `configzen-0.1.29/configzen/typedefs.py` & `configzen-0.1.30/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.29/LICENSE` & `configzen-0.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.29/pyproject.toml` & `configzen-0.1.30/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.29"
+version = "0.1.30"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.29/README.md` & `configzen-0.1.30/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.29/PKG-INFO` & `configzen-0.1.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.29
+Version: 0.1.30
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

