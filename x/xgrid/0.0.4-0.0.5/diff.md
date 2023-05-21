# Comparing `tmp/xgrid-0.0.4.tar.gz` & `tmp/xgrid-0.0.5.tar.gz`

## Comparing `xgrid-0.0.4.tar` & `xgrid-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 xgrid-0.0.4/requirements.txt
--rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 xgrid-0.0.4/test.py
--rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 xgrid-0.0.4/examples/cavity.py
--rw-r--r--   0        0        0   455424 2020-02-02 00:00:00.000000 xgrid-0.0.4/imgs/cavity.gif
--rw-r--r--   0        0        0   181643 2020-02-02 00:00:00.000000 xgrid-0.0.4/imgs/cavity.png
--rw-r--r--   0        0        0   181637 2020-02-02 00:00:00.000000 xgrid-0.0.4/imgs/cavityref.png
--rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 xgrid-0.0.4/imgs/convection_1d.png
--rw-r--r--   0        0        0    14277 2020-02-02 00:00:00.000000 xgrid-0.0.4/imgs/convection_1d_nonlinear.png
--rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 xgrid-0.0.4/imgs/convection_2d.png
--rw-r--r--   0        0        0    16467 2020-02-02 00:00:00.000000 xgrid-0.0.4/imgs/diffusion_1d.png
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/__init__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/lang/__init__.py
--rw-r--r--   0        0        0    18585 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/lang/generator.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/lang/operator.py
--rw-r--r--   0        0        0    27541 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/lang/parser.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/lang/ir/__init__.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/lang/ir/expression.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/lang/ir/statement.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/lang/ir/visitor.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/util/__init__.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/util/console.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/util/ffi.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/util/init.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/util/logging.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/util/typing/__init__.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/util/typing/annotation.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/util/typing/reference.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/util/typing/value.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 xgrid-0.0.4/xgrid/xgrid/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 xgrid-0.0.4/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 xgrid-0.0.4/LICENSE
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 xgrid-0.0.4/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 xgrid-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 xgrid-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 xgrid-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 xgrid-0.0.5/test.py
+-rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 xgrid-0.0.5/examples/cavity.py
+-rw-r--r--   0        0        0   455424 2020-02-02 00:00:00.000000 xgrid-0.0.5/imgs/cavity.gif
+-rw-r--r--   0        0        0   181643 2020-02-02 00:00:00.000000 xgrid-0.0.5/imgs/cavity.png
+-rw-r--r--   0        0        0   181637 2020-02-02 00:00:00.000000 xgrid-0.0.5/imgs/cavityref.png
+-rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 xgrid-0.0.5/imgs/convection_1d.png
+-rw-r--r--   0        0        0    14277 2020-02-02 00:00:00.000000 xgrid-0.0.5/imgs/convection_1d_nonlinear.png
+-rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 xgrid-0.0.5/imgs/convection_2d.png
+-rw-r--r--   0        0        0    16467 2020-02-02 00:00:00.000000 xgrid-0.0.5/imgs/diffusion_1d.png
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/__init__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/lang/__init__.py
+-rw-r--r--   0        0        0    18713 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/lang/generator.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/lang/operator.py
+-rw-r--r--   0        0        0    27541 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/lang/parser.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/lang/ir/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/lang/ir/expression.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/lang/ir/statement.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/lang/ir/visitor.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/util/__init__.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/util/console.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/util/ffi.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/util/init.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/util/logging.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/util/typing/__init__.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/util/typing/annotation.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/util/typing/reference.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/util/typing/value.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 xgrid-0.0.5/xgrid/xgrid/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 xgrid-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 xgrid-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 xgrid-0.0.5/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 xgrid-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 xgrid-0.0.5/PKG-INFO
```

### Comparing `xgrid-0.0.4/requirements.txt` & `xgrid-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/test.py` & `xgrid-0.0.5/test.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/examples/cavity.py` & `xgrid-0.0.5/examples/cavity.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/imgs/cavity.gif` & `xgrid-0.0.5/imgs/cavity.gif`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/imgs/cavity.png` & `xgrid-0.0.5/imgs/cavity.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/imgs/cavityref.png` & `xgrid-0.0.5/imgs/cavityref.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/imgs/convection_1d.png` & `xgrid-0.0.5/imgs/convection_1d.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/imgs/convection_1d_nonlinear.png` & `xgrid-0.0.5/imgs/convection_1d_nonlinear.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/imgs/convection_2d.png` & `xgrid-0.0.5/imgs/convection_2d.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/imgs/diffusion_1d.png` & `xgrid-0.0.5/imgs/diffusion_1d.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/__init__.py` & `xgrid-0.0.5/xgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/lang/generator.py` & `xgrid-0.0.5/xgrid/lang/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
             self.stencil_flag = StencilFlag(ir.variable, ir.boundary_mask)
         elif ir.context == "load":
             if self.stencil_flag is None:
                 self.logger.dead(
                     f"Unable to perform load operation to grid '{ir.variable.name}' without stencil context")
 
-            if ir.time_offset == 0 and self.stencil_flag.variable == ir.variable:
+            if ir.time_offset == 0 and self.stencil_flag.variable == ir.variable and ir.boundary_mask == 0:
                 self.stencil_flag.implicit = True
 
     def visit_Assignment(self, ir: stat.Assignment):
         self.visit(ir.terminal)
         self.visit(ir.value)
 
         setattr(ir, "__stencil_flag", self.stencil_flag)
@@ -215,15 +215,17 @@
 
         with implementation.indent():
             # variable definitions
             for name, var in operator.ir.scope.items():
                 if name not in operator.signature.argnames_map:
                     implementation.println(
                         f"{self.format_type(var.type)} {name};")
-
+            
+            for macro in operator.macro: 
+                implementation.println(macro)
             self.visits(operator.ir.body, implementation)
         implementation.println("}")
 
     def compile(self):
         self.logger.info(
             f"Compiling kernel {self.operator.name}' and retrive interface")
         dynlib = Compiler(cacheroot=self.config.cacheroot, cc=self.config.cc).compile(
```

### Comparing `xgrid-0.0.4/xgrid/lang/operator.py` & `xgrid-0.0.5/xgrid/lang/operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from xgrid.xgrid import Grid as XGrid
 
 
 CustomTypecheck = Callable[[list[BaseType]], BaseType]
 
 
 class Operator:
-    def __init__(self, func, mode: str, name: str | None = None, includes: list[str] | None = None, self_type: BaseType | None = None, typecheck_override: CustomTypecheck | None = None, tick: bool = True) -> None:
+    def __init__(self, func, mode: str, name: str | None = None, includes: list[str] | None = None, self_type: BaseType | None = None, typecheck_override: CustomTypecheck | None = None, tick: bool = True, macro: list[str] | None = None) -> None:
         self.func = func
         self.mode = mode
 
         self.logger = Logger(self)
 
         self.name = func.__name__ if name is None else name
         self.includes = [] if includes is None else includes
+        self.macro = [] if macro is None else macro
 
         self.native = None
         self.self_type = self_type
         self.typecheck_override = typecheck_override
         self.tick = tick
 
     def __call__(self, *args: Any) -> Any:
@@ -48,40 +49,40 @@
     def ir(self) -> Definition:
         _ir = getattr(self, "_ir", None)
         if _ir is None:
             parser = Parser(self.func, self.name, self.mode, self.self_type)
             self._ir = parser.result
             self.includes.extend(parser.includes)
         return self._ir
-    
+
     @property
     def src(self) -> str:
         from xgrid.lang.generator import Generator
         return Generator(self).source
 
     @property
     def signature(self):
         return self.ir.signature
 
 
-def kernel(*, name: str | None = None, includes: list[str] | None = None, tick: bool = True):
+def kernel(*, name: str | None = None, includes: list[str] | None = None, tick: bool = True, macro: list[str] | None = None):
     def aux(func):
-        return Operator(func, "kernel", name, includes, tick=tick)
+        return Operator(func, "kernel", name, includes, tick=tick, macro=macro)
     return aux
 
 
-def function(*, method: bool = False, name: str | None = None, includes: list[str] | None = None):
+def function(*, method: bool = False, name: str | None = None, includes: list[str] | None = None, macro: list[str] | None = None):
     if method:
         def aux_method(func):
             setattr(func, "__xgrid_method", (name, includes))
             return func
         return aux_method
     else:
         def aux(func):
-            return Operator(func, "function", name, includes)
+            return Operator(func, "function", name, includes, macro=macro)
         return aux
 
 
 def external(*, name: str | None = None, includes: list[str] | None = None, typecheck_override: CustomTypecheck):
     def aux(func):
         return Operator(func, "external", name, includes, typecheck_override=typecheck_override)
     return aux
```

### Comparing `xgrid-0.0.4/xgrid/lang/parser.py` & `xgrid-0.0.5/xgrid/lang/parser.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/lang/ir/__init__.py` & `xgrid-0.0.5/xgrid/lang/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/lang/ir/expression.py` & `xgrid-0.0.5/xgrid/lang/ir/expression.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/lang/ir/statement.py` & `xgrid-0.0.5/xgrid/lang/ir/statement.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/lang/ir/visitor.py` & `xgrid-0.0.5/xgrid/lang/ir/visitor.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/util/console.py` & `xgrid-0.0.5/xgrid/util/console.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/util/ffi.py` & `xgrid-0.0.5/xgrid/util/ffi.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/util/init.py` & `xgrid-0.0.5/xgrid/util/init.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/util/logging.py` & `xgrid-0.0.5/xgrid/util/logging.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/util/typing/annotation.py` & `xgrid-0.0.5/xgrid/util/typing/annotation.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/util/typing/reference.py` & `xgrid-0.0.5/xgrid/util/typing/reference.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/util/typing/value.py` & `xgrid-0.0.5/xgrid/util/typing/value.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/xgrid/xgrid/__init__.py` & `xgrid-0.0.5/xgrid/xgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/LICENSE` & `xgrid-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/README.md` & `xgrid-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.4/pyproject.toml` & `xgrid-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xgrid"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="yhl1219", email="yhliu2000@outlook.com" },
 ]
 description = "Domain-specific language for developing partial differential equation solvers"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `xgrid-0.0.4/PKG-INFO` & `xgrid-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgrid
-Version: 0.0.4
+Version: 0.0.5
 Summary: Domain-specific language for developing partial differential equation solvers
 Project-URL: Homepage, https://github.com/yhl1219/xgrid
 Project-URL: Bug Tracker, https://github.com/yhl1219/xgrid/issues
 Author-email: yhl1219 <yhliu2000@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

