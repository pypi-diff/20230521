# Comparing `tmp/muutils-0.3.8.tar.gz` & `tmp/muutils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muutils-0.3.8.tar", max compression
+gzip compressed data, was "muutils-0.3.9.tar", max compression
```

## Comparing `muutils-0.3.8.tar` & `muutils-0.3.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.3.8/LICENSE
--rw-r--r--   0        0        0       22 2023-04-10 21:51:10.344133 muutils-0.3.8/muutils/__init__.py
--rw-r--r--   0        0        0     3910 2023-03-24 22:25:29.757321 muutils-0.3.8/muutils/_wip/dataclass_validator.py
--rw-r--r--   0        0        0     4652 2023-02-16 09:10:54.613167 muutils-0.3.8/muutils/_wip/experiments.ipynb
--rw-r--r--   0        0        0     5835 2023-03-24 22:25:29.757321 muutils-0.3.8/muutils/_wip/gptdataset.py
--rw-r--r--   0        0        0    23453 2023-03-24 22:25:29.758323 muutils-0.3.8/muutils/_wip/json_serialize_old.py
--rw-r--r--   0        0        0     3286 2023-03-24 22:25:29.758323 muutils-0.3.8/muutils/_wip/lazy_externals.py
--rw-r--r--   0        0        0     9214 2023-03-24 22:25:29.759320 muutils-0.3.8/muutils/_wip/newargparser.py
--rw-r--r--   0        0        0     7414 2023-03-24 22:25:29.760323 muutils-0.3.8/muutils/_wip/torch_util_old.py
--rw-r--r--   0        0        0     3751 2023-04-10 21:51:10.344133 muutils-0.3.8/muutils/dictmagic.py
--rw-r--r--   0        0        0     1613 2023-03-06 19:25:21.018548 muutils-0.3.8/muutils/group_equiv.py
--rw-r--r--   0        0        0      897 2023-03-24 22:25:29.761326 muutils-0.3.8/muutils/json_serialize/__init__.py
--rw-r--r--   0        0        0     6016 2023-03-30 19:44:39.204722 muutils-0.3.8/muutils/json_serialize/array.py
--rw-r--r--   0        0        0    13391 2023-03-24 22:25:29.762321 muutils-0.3.8/muutils/json_serialize/dataclass_factories.py
--rw-r--r--   0        0        0     8906 2023-04-05 06:39:57.784877 muutils-0.3.8/muutils/json_serialize/json_serialize.py
--rw-r--r--   0        0        0    15663 2023-04-10 21:51:10.345131 muutils-0.3.8/muutils/json_serialize/serializable_dataclass.py
--rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.3.8/muutils/json_serialize/util.py
--rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.3.8/muutils/jsonlines.py
--rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.3.8/muutils/logger/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.3.8/muutils/logger/exception_context.py
--rw-r--r--   0        0        0     1667 2023-03-24 22:25:29.765321 muutils-0.3.8/muutils/logger/headerfuncs.py
--rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.3.8/muutils/logger/log_util.py
--rw-r--r--   0        0        0    10669 2023-03-24 22:25:29.766326 muutils-0.3.8/muutils/logger/logger.py
--rw-r--r--   0        0        0     3796 2023-03-24 22:25:29.767323 muutils-0.3.8/muutils/logger/loggingstream.py
--rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.3.8/muutils/logger/simplelogger.py
--rw-r--r--   0        0        0     2488 2023-03-24 22:25:29.769322 muutils-0.3.8/muutils/logger/timing.py
--rw-r--r--   0        0        0     2231 2023-03-24 22:25:29.770322 muutils-0.3.8/muutils/misc.py
--rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.3.8/muutils/py.typed
--rw-r--r--   0        0        0     8778 2023-03-24 22:25:29.771346 muutils-0.3.8/muutils/statcounter.py
--rw-r--r--   0        0        0     6322 2023-03-30 07:34:00.609964 muutils-0.3.8/muutils/sysinfo.py
--rw-r--r--   0        0        0    10013 2023-04-02 02:41:11.904089 muutils-0.3.8/muutils/tensor_utils.py
--rw-r--r--   0        0        0      139 2023-03-24 22:25:29.773320 muutils-0.3.8/muutils/zanj/__init__.py
--rw-r--r--   0        0        0     1469 2023-03-25 05:30:53.722117 muutils-0.3.8/muutils/zanj/externals.py
--rw-r--r--   0        0        0    11113 2023-03-30 19:44:39.207720 muutils-0.3.8/muutils/zanj/loading.py
--rw-r--r--   0        0        0     4151 2023-03-30 19:44:39.207720 muutils-0.3.8/muutils/zanj/readme.md
--rw-r--r--   0        0        0     8121 2023-03-30 19:44:39.208721 muutils-0.3.8/muutils/zanj/serializing.py
--rw-r--r--   0        0        0     8681 2023-04-06 20:15:44.284139 muutils-0.3.8/muutils/zanj/torchutil.py
--rw-r--r--   0        0        0     7520 2023-04-04 06:14:55.119640 muutils-0.3.8/muutils/zanj/zanj.py
--rw-r--r--   0        0        0      967 2023-04-10 21:51:10.346130 muutils-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1575 2023-02-16 09:10:54.612163 muutils-0.3.8/README.md
--rw-r--r--   0        0        0     2405 1970-01-01 00:00:00.000000 muutils-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.3.9/LICENSE
+-rw-r--r--   0        0        0       22 2023-04-18 18:13:20.205838 muutils-0.3.9/muutils/__init__.py
+-rw-r--r--   0        0        0     3910 2023-03-24 22:25:29.757321 muutils-0.3.9/muutils/_wip/dataclass_validator.py
+-rw-r--r--   0        0        0     4652 2023-02-16 09:10:54.613167 muutils-0.3.9/muutils/_wip/experiments.ipynb
+-rw-r--r--   0        0        0     5835 2023-03-24 22:25:29.757321 muutils-0.3.9/muutils/_wip/gptdataset.py
+-rw-r--r--   0        0        0    23453 2023-03-24 22:25:29.758323 muutils-0.3.9/muutils/_wip/json_serialize_old.py
+-rw-r--r--   0        0        0     3286 2023-03-24 22:25:29.758323 muutils-0.3.9/muutils/_wip/lazy_externals.py
+-rw-r--r--   0        0        0     9214 2023-03-24 22:25:29.759320 muutils-0.3.9/muutils/_wip/newargparser.py
+-rw-r--r--   0        0        0     7414 2023-03-24 22:25:29.760323 muutils-0.3.9/muutils/_wip/torch_util_old.py
+-rw-r--r--   0        0        0     3751 2023-04-10 21:51:10.344133 muutils-0.3.9/muutils/dictmagic.py
+-rw-r--r--   0        0        0     1613 2023-03-06 19:25:21.018548 muutils-0.3.9/muutils/group_equiv.py
+-rw-r--r--   0        0        0      897 2023-03-24 22:25:29.761326 muutils-0.3.9/muutils/json_serialize/__init__.py
+-rw-r--r--   0        0        0     6090 2023-04-18 18:13:20.206840 muutils-0.3.9/muutils/json_serialize/array.py
+-rw-r--r--   0        0        0    10989 2023-04-18 18:13:20.207837 muutils-0.3.9/muutils/json_serialize/dataclass_factories.py
+-rw-r--r--   0        0        0     8906 2023-04-15 04:06:05.294628 muutils-0.3.9/muutils/json_serialize/json_serialize.py
+-rw-r--r--   0        0        0    15787 2023-04-18 18:13:20.209838 muutils-0.3.9/muutils/json_serialize/serializable_dataclass.py
+-rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.3.9/muutils/json_serialize/util.py
+-rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.3.9/muutils/jsonlines.py
+-rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.3.9/muutils/logger/__init__.py
+-rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.3.9/muutils/logger/exception_context.py
+-rw-r--r--   0        0        0     1667 2023-03-24 22:25:29.765321 muutils-0.3.9/muutils/logger/headerfuncs.py
+-rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.3.9/muutils/logger/log_util.py
+-rw-r--r--   0        0        0    10669 2023-03-24 22:25:29.766326 muutils-0.3.9/muutils/logger/logger.py
+-rw-r--r--   0        0        0     3796 2023-03-24 22:25:29.767323 muutils-0.3.9/muutils/logger/loggingstream.py
+-rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.3.9/muutils/logger/simplelogger.py
+-rw-r--r--   0        0        0     2488 2023-03-24 22:25:29.769322 muutils-0.3.9/muutils/logger/timing.py
+-rw-r--r--   0        0        0     2231 2023-03-24 22:25:29.770322 muutils-0.3.9/muutils/misc.py
+-rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.3.9/muutils/py.typed
+-rw-r--r--   0        0        0     8778 2023-03-24 22:25:29.771346 muutils-0.3.9/muutils/statcounter.py
+-rw-r--r--   0        0        0     6322 2023-03-30 07:34:00.609964 muutils-0.3.9/muutils/sysinfo.py
+-rw-r--r--   0        0        0    10118 2023-04-18 18:13:20.210838 muutils-0.3.9/muutils/tensor_utils.py
+-rw-r--r--   0        0        0      139 2023-03-24 22:25:29.773320 muutils-0.3.9/muutils/zanj/__init__.py
+-rw-r--r--   0        0        0     1469 2023-03-25 05:30:53.722117 muutils-0.3.9/muutils/zanj/externals.py
+-rw-r--r--   0        0        0    12685 2023-04-18 18:13:20.211838 muutils-0.3.9/muutils/zanj/loading.py
+-rw-r--r--   0        0        0     4151 2023-03-30 19:44:39.207720 muutils-0.3.9/muutils/zanj/readme.md
+-rw-r--r--   0        0        0     8153 2023-04-18 18:13:20.212838 muutils-0.3.9/muutils/zanj/serializing.py
+-rw-r--r--   0        0        0     8681 2023-04-06 20:15:44.284139 muutils-0.3.9/muutils/zanj/torchutil.py
+-rw-r--r--   0        0        0     7755 2023-04-18 18:13:20.213837 muutils-0.3.9/muutils/zanj/zanj.py
+-rw-r--r--   0        0        0      967 2023-04-18 18:13:20.214835 muutils-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1575 2023-02-16 09:10:54.612163 muutils-0.3.9/README.md
+-rw-r--r--   0        0        0     2405 1970-01-01 00:00:00.000000 muutils-0.3.9/PKG-INFO
```

### Comparing `muutils-0.3.8/LICENSE` & `muutils-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/_wip/dataclass_validator.py` & `muutils-0.3.9/muutils/_wip/dataclass_validator.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/_wip/experiments.ipynb` & `muutils-0.3.9/muutils/_wip/experiments.ipynb`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/_wip/gptdataset.py` & `muutils-0.3.9/muutils/_wip/gptdataset.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/_wip/json_serialize_old.py` & `muutils-0.3.9/muutils/_wip/json_serialize_old.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/_wip/lazy_externals.py` & `muutils-0.3.9/muutils/_wip/lazy_externals.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/_wip/newargparser.py` & `muutils-0.3.9/muutils/_wip/newargparser.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/_wip/torch_util_old.py` & `muutils-0.3.9/muutils/_wip/torch_util_old.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/dictmagic.py` & `muutils-0.3.9/muutils/dictmagic.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/group_equiv.py` & `muutils-0.3.9/muutils/group_equiv.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/json_serialize/__init__.py` & `muutils-0.3.9/muutils/json_serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/json_serialize/array.py` & `muutils-0.3.9/muutils/json_serialize/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,17 @@
         raise TypeError(f"invalid type: {type(arr)}")
 
 
 def arr_metadata(arr) -> dict[str, list[int] | str | int]:
     """get metadata for a numpy array"""
     return {
         "shape": list(arr.shape),
-        "dtype": str(arr.dtype),
+        "dtype": arr.dtype.__name__
+        if hasattr(arr.dtype, "__name__")
+        else str(arr.dtype),
         "n_elements": array_n_elements(arr),
     }
 
 
 def serialize_array(
     jser: "JsonSerializer",  # type: ignore[name-defined]
     arr: np.ndarray,
```

### Comparing `muutils-0.3.8/muutils/json_serialize/dataclass_factories.py` & `muutils-0.3.9/muutils/json_serialize/dataclass_factories.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,84 +6,14 @@
 
 from muutils.json_serialize.json_serialize import JsonSerializer
 from muutils.json_serialize.util import JSONdict, JSONitem, MonoTuple, TypeErrorMode
 
 # pylint: disable=pointless-string-statement, unreachable, import-outside-toplevel, consider-using-dict-items
 
 
-# TODO: this is implemented in ZANJ now, I think -- remove this?
-# def serialize_torch_module(
-#     obj: "torch.nn.Module", # type: ignore[name-defined]
-#     *,
-#     member_typecasts: dict[str, Callable],
-#     array_mode: ArrayMode = "array_list_meta",
-# ) -> JSONitem:
-#     """serialize an instance of `torch.nn.Module`
-
-#     you'll need to specify `member_typecasts`, which is a dict mapping
-#     member names to functions to call on the member value before serializing it
-
-#     the state dict will be saved separately under `state_dict`
-#     """
-#     # TODO: add paths to serializer
-#     raise NotImplementedError()
-#     return {
-#         "__format__": "torch_module",
-#         "name": obj.__class__.__name__,
-#         "state_dict": {
-#             k: serialize_array(v.cpu().numpy(), array_mode=array_mode)
-#             for k, v in obj.state_dict().items()
-#         },
-#         "members_dict": {
-#             k: (
-#                 json_serialize(v)
-#                 if k not in member_typecasts
-#                 else json_serialize(member_typecasts[k](v))
-#             )
-#             for k, v in obj.__dict__.items()
-#             if not k.startswith("_")
-#         },
-#     }
-
-
-# def load_torch_module_factory(
-#     cls,
-#     *,
-#     members_exclude: list[str],
-#     typecasts: dict[str, Callable],
-# ) -> Callable[[Any, JSONitem], "torch.nn.Module"]: # type: ignore[name-defined]
-#     """create a function which allows for loading a torch module from `JSONitem`
-
-#     - everything from the `members_dict` not in `members_exclude` will be passed to the `__init__` method of the module
-#     - everything from the `state_dict` will be passed to the `load_state_dict` method of the module
-#     """
-#     raise NotImplementedError()
-
-#     import torch
-
-#     @classmethod
-#     def load(cls, item: JSONitem) -> "torch.nn.Module":
-#         assert item["__format__"] == "torch_module"
-#         assert item["name"] == cls.__name__
-
-#         module_obj = cls(
-#             **{
-#                 k: (v if k not in typecasts else typecasts[k](v))
-#                 for k, v in item["members_dict"].items()
-#                 if k not in members_exclude
-#             }
-#         )
-#         module_obj.load_state_dict(
-#             {k: torch.from_numpy(load_array(v)) for k, v in item["state_dict"].items()},
-#         )
-#         return module_obj
-
-#     return load
-
-
 def dataclass_serializer_factory(
     cls,
     special_serializers: Optional[dict[str, Callable]] = None,
     fields_exclude: Optional[Sequence[str]] = None,
 ) -> Callable[[Any], JSONitem]:
     """outputs a `.serialize` method for a dataclass,
     where fields present in `special_serializers` are serialized using the corresponding function.
```

### Comparing `muutils-0.3.8/muutils/json_serialize/json_serialize.py` & `muutils-0.3.9/muutils/json_serialize/json_serialize.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/json_serialize/serializable_dataclass.py` & `muutils-0.3.9/muutils/json_serialize/serializable_dataclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import dataclasses
+import json
 import types
 import typing
 import warnings
 from typing import Any, Callable, Optional, Type, TypeVar
 
 # pylint: disable=bad-mcs-classmethod-argument, too-many-arguments, protected-access
 
@@ -149,17 +150,17 @@
     if isinstance(a, (dict, typing.Mapping)) and isinstance(b, (dict, typing.Mapping)):
         return len(a) == len(b) and all(
             array_safe_eq(k1, k2) and array_safe_eq(a[k1], b[k2])
             for k1, k2 in zip(a.keys(), b.keys())
         )
 
     try:
-        return a == b
-    except TypeError:
-        warnings.warn(f"Cannot compare {a} and {b} for equality")
+        return bool(a == b)
+    except (TypeError, ValueError) as e:
+        warnings.warn(f"Cannot compare {a} and {b} for equality\n{e}")
         return NotImplemented  # type: ignore[return-value]
 
 
 def dc_eq(dc1, dc2) -> bool:
     """checks if two dataclasses which hold numpy arrays are equal"""
     if dc1 is dc2:
         return True
@@ -223,14 +224,17 @@
     @classmethod
     def load(cls: Type[T], data: dict[str, Any] | T) -> T:
         raise NotImplementedError
 
     def __eq__(self, other: Any) -> bool:
         return dc_eq(self, other)
 
+    def __hash__(self) -> int:
+        return hash(json.dumps(self.serialize()))
+
     def diff(self, other: "SerializableDataclass") -> dict[str, Any]:
         if type(self) != type(other):
             raise ValueError(
                 f"Instances must be of the same type, but got {type(self)} and {type(other)}"
             )
 
         diff_result: dict = {}
```

### Comparing `muutils-0.3.8/muutils/json_serialize/util.py` & `muutils-0.3.9/muutils/json_serialize/util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/jsonlines.py` & `muutils-0.3.9/muutils/jsonlines.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/logger/exception_context.py` & `muutils-0.3.9/muutils/logger/exception_context.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/logger/headerfuncs.py` & `muutils-0.3.9/muutils/logger/headerfuncs.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/logger/log_util.py` & `muutils-0.3.9/muutils/logger/log_util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/logger/logger.py` & `muutils-0.3.9/muutils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/logger/loggingstream.py` & `muutils-0.3.9/muutils/logger/loggingstream.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/logger/simplelogger.py` & `muutils-0.3.9/muutils/logger/simplelogger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/logger/timing.py` & `muutils-0.3.9/muutils/logger/timing.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/misc.py` & `muutils-0.3.9/muutils/misc.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/statcounter.py` & `muutils-0.3.9/muutils/statcounter.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/sysinfo.py` & `muutils-0.3.9/muutils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/tensor_utils.py` & `muutils-0.3.9/muutils/tensor_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,18 @@
     **{dtype.__name__: dtype for dtype in DTYPE_LIST if dtype.__module__ == "numpy"},
 }
 
 TORCH_DTYPE_MAP: dict = {
     key: numpy_to_torch_dtype(dtype) for key, dtype in DTYPE_MAP.items()
 }
 
+# no idea why we have to do this, smh
+DTYPE_MAP["bool"] = np.bool_
+TORCH_DTYPE_MAP["bool"] = torch.bool
+
 
 TORCH_OPTIMIZERS_MAP: dict[str, typing.Type[torch.optim.Optimizer]] = {
     "Adagrad": torch.optim.Adagrad,
     "Adam": torch.optim.Adam,
     "AdamW": torch.optim.AdamW,
     "SparseAdam": torch.optim.SparseAdam,
     "Adamax": torch.optim.Adamax,
```

### Comparing `muutils-0.3.8/muutils/zanj/externals.py` & `muutils-0.3.9/muutils/zanj/externals.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/zanj/loading.py` & `muutils-0.3.9/muutils/zanj/loading.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,14 +136,45 @@
                 and isinstance(json_item["data"], typing.Sequence)
             ),
             load=lambda json_item, path=None, z=None: pd.DataFrame(json_item["data"]),  # type: ignore[misc]
             uid="pandas.DataFrame",
             source_pckg="muutils.zanj",
             desc="pandas.DataFrame loader",
         ),
+        # list/tuple external
+        LoaderHandler(
+            check=lambda json_item, path=None, z=None: (  # type: ignore[misc]
+                isinstance(json_item, typing.Mapping)
+                and "__format__" in json_item
+                and json_item["__format__"].startswith("list")
+                and "data" in json_item
+                and isinstance(json_item["data"], typing.Sequence)
+            ),
+            load=lambda json_item, path=None, z=None: [
+                load_item_recursive(x, path, z) for x in json_item["data"]
+            ],
+            uid="list",
+            source_pckg="muutils.zanj",
+            desc="list loader, for externals",
+        ),
+        LoaderHandler(
+            check=lambda json_item, path=None, z=None: (  # type: ignore[misc]
+                isinstance(json_item, typing.Mapping)
+                and "__format__" in json_item
+                and json_item["__format__"].startswith("tuple")
+                and "data" in json_item
+                and isinstance(json_item["data"], typing.Sequence)
+            ),
+            load=lambda json_item, path=None, z=None: tuple(
+                [load_item_recursive(x, path, z) for x in json_item["data"]]
+            ),
+            uid="tuple",
+            source_pckg="muutils.zanj",
+            desc="tuple loader, for externals",
+        ),
     ]
 }
 
 
 def register_loader_handler(handler: LoaderHandler):
     """register a custom loader handler"""
     global LOADER_MAP, LOADER_MAP_LOCK
@@ -159,14 +190,18 @@
     # lh_map: dict[str, LoaderHandler] = LOADER_MAP,
 ) -> LoaderHandler | None:
     """get the loader for a json item"""
     global LOADER_MAP
 
     # check if we recognize the format
     if isinstance(json_item, typing.Mapping) and "__format__" in json_item:
+        if not isinstance(json_item["__format__"], str):
+            raise TypeError(
+                f"invalid __format__ type '{type(json_item['__format__'])}' in '{path=}': '{json_item['__format__'] = }'"
+            )
         if json_item["__format__"] in LOADER_MAP:
             return LOADER_MAP[json_item["__format__"]]
 
     # if we dont recognize the format, try to find a loader that can handle it
     for key, lh in LOADER_MAP.items():
         if lh.check(json_item, path, zanj):
             return lh
```

### Comparing `muutils-0.3.8/muutils/zanj/readme.md` & `muutils-0.3.9/muutils/zanj/readme.md`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/zanj/serializing.py` & `muutils-0.3.9/muutils/zanj/serializing.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             col: {
                 "types": list(
                     set([type(item[col]).__name__ for item in data if col in item])
                 ),
                 "len": len([item[col] for item in data if col in item]),
             }
             for col in all_cols
+            if col != "__format__"
         },
     }
 
 
 def store_npy(self: _ZANJ_pre, fp: IO[bytes], data: NDArray) -> None:
     """store numpy array to given file as .npy"""
     np.lib.format.write_array(
@@ -180,35 +181,35 @@
             ),
             uid="torch.Tensor:external",
             source_pckg="muutils.zanj",
             desc="external torch tensor",
         ),
         ZANJSerializerHandler(
             check=lambda self, obj, path: isinstance(obj, list)
-            and len(obj) >= self.external_table_threshold,
+            and len(obj) >= self.external_list_threshold,
             serialize_func=lambda self, obj, path: zanj_external_serialize(
                 self, obj, path, item_type="jsonl", _format="list:external"
             ),
             uid="list:external",
             source_pckg="muutils.zanj",
             desc="external list",
         ),
         ZANJSerializerHandler(
             check=lambda self, obj, path: isinstance(obj, tuple)
-            and len(obj) >= self.external_table_threshold,
+            and len(obj) >= self.external_list_threshold,
             serialize_func=lambda self, obj, path: zanj_external_serialize(
                 self, obj, path, item_type="jsonl", _format="tuple:external"
             ),
             uid="tuple:external",
             source_pckg="muutils.zanj",
             desc="external tuple",
         ),
         ZANJSerializerHandler(
             check=lambda self, obj, path: isinstance(obj, pd.DataFrame)
-            and len(obj) >= self.external_table_threshold,
+            and len(obj) >= self.external_list_threshold,
             serialize_func=lambda self, obj, path: zanj_external_serialize(
                 self, obj, path, item_type="jsonl", _format="pandas.DataFrame:external"
             ),
             uid="pandas.DataFrame:external",
             source_pckg="muutils.zanj",
             desc="external pandas DataFrame",
         ),
```

### Comparing `muutils-0.3.8/muutils/zanj/torchutil.py` & `muutils-0.3.9/muutils/zanj/torchutil.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/muutils/zanj/zanj.py` & `muutils-0.3.9/muutils/zanj/zanj.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
 
     def __init__(
         self,
         error_mode: ErrorMode = "except",
         internal_array_mode: ArrayMode = "array_list_meta",
         external_array_threshold: int = 64,
-        external_table_threshold: int = 64,
+        external_list_threshold: int = 64,
         custom_settings: dict[str, Any] | None = None,
         compress: bool | int = True,
         handlers_pre: MonoTuple[SerializerHandler] = tuple(),
         handlers_default: MonoTuple[
             SerializerHandler
         ] = DEFAULT_SERIALIZER_HANDLERS_ZANJ,
     ) -> None:
@@ -77,15 +77,15 @@
             array_mode=internal_array_mode,
             error_mode=error_mode,
             handlers_pre=handlers_pre,
             handlers_default=handlers_default,
         )
 
         self.external_array_threshold: int = external_array_threshold
-        self.external_table_threshold: int = external_table_threshold
+        self.external_list_threshold: int = external_list_threshold
         self.custom_settings: dict = (
             custom_settings if custom_settings is not None else dict()
         )
 
         # process compression to int if bool given
         self.compress = compress
         if isinstance(compress, bool):
@@ -127,15 +127,15 @@
 
         return dict(
             # configuration of this ZANJ instance
             zanj_cfg=dict(
                 error_mode=str(self.error_mode),
                 array_mode=str(self.array_mode),
                 external_array_threshold=self.external_array_threshold,
-                external_table_threshold=self.external_table_threshold,
+                external_list_threshold=self.external_list_threshold,
                 compress=self.compress,
                 serialization_handlers=serialization_handlers,
                 load_handlers=load_handlers,
             ),
             # system info (python, pip packages, torch & cuda, platform info, git info)
             sysinfo=json_serialize(SysInfo.get_all(include=("python", "pytorch"))),
             externals_info=self.externals_info(),
@@ -197,14 +197,20 @@
     def read(
         self,
         file_path: Union[str, Path],
     ) -> JSONitem:
         """load the object from a ZANJ archive
         # TODO: load only some part of the zanj file by passing an ObjectPath
         """
+        file_path = Path(file_path)
+        if not file_path.exists():
+            raise FileNotFoundError(f"file not found: {file_path}")
+        if not file_path.is_file():
+            raise FileNotFoundError(f"not a file: {file_path}")
+
         loaded_zanj: LoadedZANJ = LoadedZANJ(
             path=file_path,
             zanj=self,
         )
 
         loaded_zanj.populate_externals()
```

### Comparing `muutils-0.3.8/pyproject.toml` & `muutils-0.3.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muutils"
-version = "0.3.8"
+version = "0.3.9"
 description = "A collection of miscellaneous python utilities"
 license = "GPL-3.0-only"
 authors = ["mivanit <mivanits@umich.edu>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `muutils-0.3.8/README.md` & `muutils-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `muutils-0.3.8/PKG-INFO` & `muutils-0.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muutils
-Version: 0.3.8
+Version: 0.3.9
 Summary: A collection of miscellaneous python utilities
 Home-page: https://github.com/mivanit/muutils
 License: GPL-3.0-only
 Author: mivanit
 Author-email: mivanits@umich.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

