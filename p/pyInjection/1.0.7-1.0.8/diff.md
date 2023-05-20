# Comparing `tmp/pyInjection-1.0.7.tar.gz` & `tmp/pyInjection-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyInjection-1.0.7.tar", last modified: Sat Mar 18 17:57:41 2023, max compression
+gzip compressed data, was "pyInjection-1.0.8.tar", last modified: Sat May 20 22:19:06 2023, max compression
```

## Comparing `pyInjection-1.0.7.tar` & `pyInjection-1.0.8.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.577366 pyInjection-1.0.7/
--rw-r--r--   0 root         (0) root         (0)     4139 2023-03-18 17:57:41.577366 pyInjection-1.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3874 2023-03-18 17:57:25.000000 pyInjection-1.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-18 17:57:41.577366 pyInjection-1.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-03-18 17:57:25.000000 pyInjection-1.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.566365 pyInjection-1.0.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.570032 pyInjection-1.0.7/src/pyInjection/
--rwxrwxrwx   0 root         (0) root         (0)       43 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.571866 pyInjection-1.0.7/src/pyInjection/container/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/container/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2565 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/container/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3536 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/container/container_instance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.571866 pyInjection-1.0.7/src/pyInjection/dtos/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/dtos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/dtos/registration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.572782 pyInjection-1.0.7/src/pyInjection/enums/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/enums/scope.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.574616 pyInjection-1.0.7/src/pyInjection/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/helpers/type_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.575533 pyInjection-1.0.7/src/pyInjection/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/interfaces/iscope_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/interfaces/ivalidator.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.576449 pyInjection-1.0.7/src/pyInjection/scope_managers/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/scope_managers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4786 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/scope_managers/singleton_scope_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4065 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/scope_managers/transient_scope_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.577366 pyInjection-1.0.7/src/pyInjection/validators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/validators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/validators/decorator_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-03-18 17:57:25.000000 pyInjection-1.0.7/src/pyInjection/validators/primitive_dependency_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 17:57:41.570949 pyInjection-1.0.7/src/pyInjection.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4139 2023-03-18 17:57:41.000000 pyInjection-1.0.7/src/pyInjection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      997 2023-03-18 17:57:41.000000 pyInjection-1.0.7/src/pyInjection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-18 17:57:41.000000 pyInjection-1.0.7/src/pyInjection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-18 17:57:41.000000 pyInjection-1.0.7/src/pyInjection.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.902705 pyInjection-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-05-20 22:19:06.902705 pyInjection-1.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3874 2023-05-20 22:18:55.000000 pyInjection-1.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 22:19:06.902705 pyInjection-1.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-05-20 22:18:55.000000 pyInjection-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.895705 pyInjection-1.0.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.897705 pyInjection-1.0.8/src/pyInjection/
+-rwxrwxrwx   0 root         (0) root         (0)       43 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.899705 pyInjection-1.0.8/src/pyInjection/container/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/container/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/container/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3515 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/container/container_instance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.899705 pyInjection-1.0.8/src/pyInjection/dtos/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/dtos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/dtos/registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.900705 pyInjection-1.0.8/src/pyInjection/enums/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/enums/scope.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.900705 pyInjection-1.0.8/src/pyInjection/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4266 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/helpers/container_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/helpers/type_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.901705 pyInjection-1.0.8/src/pyInjection/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/interfaces/iscope_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/interfaces/ivalidator.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.901705 pyInjection-1.0.8/src/pyInjection/scope_managers/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/scope_managers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/scope_managers/singleton_scope_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/scope_managers/transient_scope_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.902705 pyInjection-1.0.8/src/pyInjection/validators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/validators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/validators/decorator_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/validators/primitive_dependency_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.898705 pyInjection-1.0.8/src/pyInjection.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-05-20 22:19:06.000000 pyInjection-1.0.8/src/pyInjection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-20 22:19:06.000000 pyInjection-1.0.8/src/pyInjection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 22:19:06.000000 pyInjection-1.0.8/src/pyInjection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-20 22:19:06.000000 pyInjection-1.0.8/src/pyInjection.egg-info/top_level.txt
```

### Comparing `pyInjection-1.0.7/PKG-INFO` & `pyInjection-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyInjection
-Version: 1.0.7
+Version: 1.0.8
 Summary: Dependency injection container for Python3
 Author: Joshua Loader
 Author-email: pyInjection@joshloader.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyInjection-1.0.7/README.md` & `pyInjection-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyInjection-1.0.7/setup.py` & `pyInjection-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 long_description: str = ""
 root_path: str = path.abspath(path.dirname(__file__))
 with open(path.join(root_path, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pyInjection",
-    version="1.0.7",
+    version="1.0.8",
     author="Joshua Loader",
     author_email="pyInjection@joshloader.com",
     description="Dependency injection container for Python3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `pyInjection-1.0.7/src/pyInjection/container/container.py` & `pyInjection-1.0.8/src/pyInjection/container/container.py`

 * *Files identical despite different names*

### Comparing `pyInjection-1.0.7/src/pyInjection/container/container_instance.py` & `pyInjection-1.0.8/src/pyInjection/container/container_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from inspect import Signature, signature
 from typing import Any, Dict, List, Type
 
 from ..dtos import Registration
 from ..enums import Scope
+from ..helpers import TypeHelpers
 from ..interfaces import IScopeManager, IValidator
 
 
 class ContainerInstance:
     __container: Dict[Type, Registration]
     __validators: List[IValidator]
     __scope_managers: List[IScopeManager]
@@ -37,20 +38,18 @@
         error_message: str = ""
         if not interface in self.__container.keys():
             if self.__is_valid(interface=interface, implementation=implementation):
                 self.__container[interface] = Registration(
                     implementation=implementation, scope=scope
                 )
             else:
-                error_message = f"Failed to add mapping '{interface.__name__} -> {implementation.__name__}' to the container"
+                error_message = f"Failed to add mapping '{TypeHelpers.to_string(interface)} -> {TypeHelpers.to_string(implementation)}' to the container"
                 raise Exception(error_message)
         else:
-            error_message = (
-                f"Cannot register a duplicate implementation for '{interface.__name__}'"
-            )
+            error_message = f"Cannot register a duplicate implementation for '{TypeHelpers.to_string(interface)}'"
             raise Exception(error_message)
 
     def add_transient(self, interface: Type, implementation: Any) -> None:
         self.__add(
             interface=interface, implementation=implementation, scope=Scope.TRANSIENT
         )
 
@@ -76,11 +75,9 @@
             if type(registration.implementation) in self.__base_types:
                 sig: Signature = signature(registration.implementation)
                 for p in sig.parameters:
                     if p not in self.__ignore_parameters:
                         annotation: Any = sig.parameters[p].annotation
                         if not annotation in self.__container.keys():
                             raise Exception(
-                                "Missing registration for: '{0}'".format(
-                                    annotation.__name__
-                                )
+                                f"Missing registration for: '{TypeHelpers.to_string(annotation)}'"
                             )
```

### Comparing `pyInjection-1.0.7/src/pyInjection/helpers/type_helpers.py` & `pyInjection-1.0.8/src/pyInjection/helpers/type_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,8 +19,8 @@
                 if index == max_generic_index - 1:
                     closing_brackets: str = "]" * (max_generic_index - 1)
                     return_string = f"{return_string}{class_string}{closing_brackets}"
                 else:
                     return_string = f"{return_string}{class_string}["
             else:
                 return_string = class_string
-        return f"[{return_string}]"
+        return f"{return_string}"
```

### Comparing `pyInjection-1.0.7/src/pyInjection/scope_managers/transient_scope_manager.py` & `pyInjection-1.0.8/src/pyInjection/helpers/container_helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,102 @@
 from inspect import Signature, signature
-from typing import Any, Dict, List, Type, TypeVar, _GenericAlias  # type: ignore
+from typing import (  # type: ignore
+    Any,
+    Callable,
+    Dict,
+    List,
+    Type,
+    TypeVar,
+    _GenericAlias,
+)
 
 from ..dtos import Registration
-from ..enums import Scope
-from ..helpers import TypeHelpers
-from ..interfaces import IScopeManager
+from .type_helpers import TypeHelpers
 
 
-class TransientScopeManager(IScopeManager):
-    __base_types: List[Type]
-    __ignore_parameters: List[str]
+class ContainerHelpers:
+    ignore_parameters: List[str] = ["self", "args", "kwargs"]
 
-    def __init__(self, base_types: List[Type]) -> None:
-        self.__base_types = base_types
-        self.__ignore_parameters = ["self", "args", "kwargs"]
-
-    def can_resolve(self, scope: Scope) -> bool:
-        return scope == Scope.TRANSIENT
-
-    def is_same_registration_scope(
-        self, interface: Type, container: Dict[Type, Registration]
-    ) -> bool:
-        registration: Registration = container[interface]
-        return registration.scope == Scope.TRANSIENT
-
-    def resolve(self, interface: Type, container: Dict[Type, Registration]) -> Any:
+    @staticmethod
+    def resolve(
+        interface: Type,
+        container: Dict[Type, Registration],
+        is_same_registration_scope: Callable,
+        base_types: List[Type],
+    ) -> Any:
         error_message: str = ""
         if interface in container.keys():
             implementation: Any = container[interface].implementation
-            if type(implementation) in self.__base_types:
+            if type(implementation) in base_types:
                 if type(implementation) == _GenericAlias:  # type: ignore
-                    return self.resolve_generic(
-                        interface=interface, container=container
+                    return ContainerHelpers.resolve_generic(
+                        interface=interface,
+                        container=container,
+                        is_same_registration_scope=is_same_registration_scope,
+                        base_types=base_types,
                     )
                 else:
                     kwargs: Any = {}
                     sig: Signature = signature(implementation)
                     for p in sig.parameters:
-                        if p not in self.__ignore_parameters:
+                        if p not in ContainerHelpers.ignore_parameters:
                             child_interface: Type = sig.parameters[p].annotation
-                            if not self.is_same_registration_scope(
-                                interface=child_interface, container=container
-                            ):
-                                error_message = f"Error Transient type: {TypeHelpers.to_string(interface)} registered with Singleton dependency: {TypeHelpers.to_string(child_interface)}"
-                                raise Exception(error_message)
-                            instance = self.resolve(
-                                interface=child_interface, container=container
+                            is_same_registration_scope(
+                                interface=interface,
+                                child_interface=child_interface,
+                                container=container,
+                            )
+                            instance = ContainerHelpers.resolve(
+                                interface=child_interface,
+                                container=container,
+                                is_same_registration_scope=is_same_registration_scope,
+                                base_types=base_types,
                             )
                             kwargs[p] = instance
                     return implementation(**kwargs)
             elif type(implementation) == type(lambda: ""):
                 return implementation()
             else:
                 return implementation
         else:
             error_message = f"Cannot resolve type: {TypeHelpers.to_string(interface)}"
             raise Exception(error_message)
 
+    @staticmethod
     def resolve_generic(
-        self, interface: Type, container: Dict[Type, Registration]
+        interface: Type,
+        container: Dict[Type, Registration],
+        is_same_registration_scope: Callable,
+        base_types: List[Type],
     ) -> Any:
+        replace_child_type: bool = False
         implementation: Any = container[interface].implementation
         implementation_type: Type = implementation.__origin__
         generic_class: Type = implementation.__args__[0]
         kwargs: Any = {}
         sig: Signature = signature(implementation_type)
         for p in sig.parameters:
-            if p not in self.__ignore_parameters:
+            if p not in ContainerHelpers.ignore_parameters:
                 child_interface: Type = sig.parameters[p].annotation
                 if type(child_interface) == _GenericAlias:  # type: ignore
                     child_interface_generic_type = child_interface.__args__[0]
                     if type(child_interface_generic_type) == TypeVar:
                         ## Generic type needs to be passed down from parent
                         child_interface.__args__ = (generic_class,)
-                if not self.is_same_registration_scope(
-                    interface=child_interface, container=container
-                ):
-                    error_message = f"Error Transient type: {TypeHelpers.to_string(interface)} registered with Singleton dependency: {TypeHelpers.to_string(child_interface)}"
-                    raise Exception(error_message)
-                instance = self.resolve(interface=child_interface, container=container)
+                        replace_child_type = True
+                is_same_registration_scope(
+                    interface=interface,
+                    child_interface=child_interface,
+                    container=container,
+                )
+                instance = ContainerHelpers.resolve(
+                    interface=child_interface,
+                    container=container,
+                    is_same_registration_scope=is_same_registration_scope,
+                    base_types=base_types,
+                )
                 kwargs[p] = instance
+                ## Place TypeVar back into child_interface for later resolves
+                if replace_child_type:
+                    T = TypeVar("T")
+                    child_interface.__args__ = (T,)
         return implementation(**kwargs)
```

### Comparing `pyInjection-1.0.7/src/pyInjection/validators/decorator_validator.py` & `pyInjection-1.0.8/src/pyInjection/validators/decorator_validator.py`

 * *Files identical despite different names*

### Comparing `pyInjection-1.0.7/src/pyInjection/validators/primitive_dependency_validator.py` & `pyInjection-1.0.8/src/pyInjection/validators/primitive_dependency_validator.py`

 * *Files identical despite different names*

### Comparing `pyInjection-1.0.7/src/pyInjection.egg-info/PKG-INFO` & `pyInjection-1.0.8/src/pyInjection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyInjection
-Version: 1.0.7
+Version: 1.0.8
 Summary: Dependency injection container for Python3
 Author: Joshua Loader
 Author-email: pyInjection@joshloader.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyInjection-1.0.7/src/pyInjection.egg-info/SOURCES.txt` & `pyInjection-1.0.8/src/pyInjection.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/pyInjection/container/container.py
 src/pyInjection/container/container_instance.py
 src/pyInjection/dtos/__init__.py
 src/pyInjection/dtos/registration.py
 src/pyInjection/enums/__init__.py
 src/pyInjection/enums/scope.py
 src/pyInjection/helpers/__init__.py
+src/pyInjection/helpers/container_helpers.py
 src/pyInjection/helpers/type_helpers.py
 src/pyInjection/interfaces/__init__.py
 src/pyInjection/interfaces/iscope_manager.py
 src/pyInjection/interfaces/ivalidator.py
 src/pyInjection/scope_managers/__init__.py
 src/pyInjection/scope_managers/singleton_scope_manager.py
 src/pyInjection/scope_managers/transient_scope_manager.py
```

