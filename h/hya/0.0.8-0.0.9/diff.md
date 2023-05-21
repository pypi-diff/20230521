# Comparing `tmp/hya-0.0.8.tar.gz` & `tmp/hya-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hya-0.0.8.tar", max compression
+gzip compressed data, was "hya-0.0.9.tar", max compression
```

## Comparing `hya-0.0.8.tar` & `hya-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1501 2023-03-23 01:34:32.016499 hya-0.0.8/LICENSE
--rw-r--r--   0        0        0     3144 2023-03-23 01:34:32.016499 hya-0.0.8/README.md
--rw-r--r--   0        0        0     2354 2023-03-23 01:34:32.016499 hya-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      206 2023-03-23 01:34:32.016499 hya-0.0.8/src/hya/__init__.py
--rw-r--r--   0        0        0      212 2023-03-23 01:34:32.016499 hya-0.0.8/src/hya/import_utils.py
--rw-r--r--   0        0        0     1559 2023-03-23 01:34:32.016499 hya-0.0.8/src/hya/pytorch.py
--rw-r--r--   0        0        0     2117 2023-03-23 01:34:32.016499 hya-0.0.8/src/hya/registry.py
--rw-r--r--   0        0        0     7385 2023-03-23 01:34:32.016499 hya-0.0.8/src/hya/resolvers.py
--rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 hya-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-04-04 14:12:33.650071 hya-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3144 2023-04-04 14:12:33.650071 hya-0.0.9/README.md
+-rw-r--r--   0        0        0     3968 2023-04-04 14:12:33.650071 hya-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      234 2023-04-04 14:12:33.650071 hya-0.0.9/src/hya/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-04 14:12:33.650071 hya-0.0.9/src/hya/import_utils.py
+-rw-r--r--   0        0        0     1559 2023-04-04 14:12:33.650071 hya-0.0.9/src/hya/pytorch.py
+-rw-r--r--   0        0        0     2133 2023-04-04 14:12:33.650071 hya-0.0.9/src/hya/registry.py
+-rw-r--r--   0        0        0     7645 2023-04-04 14:12:33.650071 hya-0.0.9/src/hya/resolvers.py
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 hya-0.0.9/PKG-INFO
```

### Comparing `hya-0.0.8/LICENSE` & `hya-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hya-0.0.8/README.md` & `hya-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hya-0.0.8/src/hya/pytorch.py` & `hya-0.0.9/src/hya/pytorch.py`

 * *Files identical despite different names*

### Comparing `hya-0.0.8/src/hya/registry.py` & `hya-0.0.9/src/hya/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from omegaconf import OmegaConf
 
 
 class ResolverRegistry:
     r"""Implementation of a resolver registry."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._state: dict[str, Callable] = dict()
 
     @property
     def state(self) -> dict[str, Callable]:
         r"""dict: The state of the registry."""
         return self._state
 
@@ -52,15 +52,15 @@
 
         return wrap
 
 
 registry = ResolverRegistry()
 
 
-def register_resolvers():
+def register_resolvers() -> None:
     r"""Registers the resolvers.
 
     Example usage:
 
     .. code-block:: python
 
         >>> from hya import register_resolvers
```

### Comparing `hya-0.0.8/src/hya/resolvers.py` & `hya-0.0.9/src/hya/resolvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,27 @@
 
     Returns:
         int: ``dividend // divisor``
     """
     return dividend // divisor
 
 
+@registry.register("hya.len")
+def len_resolver(obj: Any) -> int:
+    r"""Implements a resolver to compute the length of an object.
+
+    Args:
+        obj: Specifies the object.
+
+    Returns:
+        int: The length of the object.
+    """
+    return len(obj)
+
+
 @registry.register("hya.log")
 def log_resolver(number: Union[int, float], base: float = math.e) -> float:
     r"""Implements a resolver to compute logarithm of the input value to the
     given base.
 
     Args:
         number (int or float): Specifies the number.
```

### Comparing `hya-0.0.8/PKG-INFO` & `hya-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hya
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library of custom OmegaConf resolvers
 Home-page: https://github.com/durandtibo/hya
 License: BSD-3-Clause
 Keywords: omegaconf,resolver
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hya Version: 0.0.8 Summary: A library of custom
+Metadata-Version: 2.1 Name: hya Version: 0.0.9 Summary: A library of custom
 OmegaConf resolvers Home-page: https://github.com/durandtibo/hya License: BSD-
 3-Clause Keywords: omegaconf,resolver Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

