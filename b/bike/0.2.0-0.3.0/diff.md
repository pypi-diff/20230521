# Comparing `tmp/bike-0.2.0.tar.gz` & `tmp/bike-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bike-0.2.0.tar", max compression
+gzip compressed data, was "bike-0.3.0.tar", max compression
```

## Comparing `bike-0.2.0.tar` & `bike-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0     1069 2021-10-30 21:11:18.045026 bike-0.2.0/LICENSE
--rw-r--r--   0        0        0      581 2022-03-11 09:43:39.877138 bike-0.2.0/README.md
--rw-r--r--   0        0        0      616 2022-03-11 09:27:42.199018 bike-0.2.0/bike/CHANGELOG.md
--rw-r--r--   0        0        0      173 2022-03-11 09:27:42.201715 bike-0.2.0/bike/__init__.py
--rw-r--r--   0        0        0     1012 2022-03-11 09:27:42.204715 bike-0.2.0/bike/controllers.py
--rw-r--r--   0        0        0     1778 2022-03-11 09:27:42.205823 bike-0.2.0/bike/fields.py
--rw-r--r--   0        0        0     4282 2022-03-11 09:27:42.207149 bike-0.2.0/bike/models.py
--rw-r--r--   0        0        0      423 2022-03-11 09:27:42.208773 bike-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1205 2022-03-11 09:45:13.522570 bike-0.2.0/setup.py
--rw-r--r--   0        0        0     1141 2022-03-11 09:45:13.522826 bike-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.0/README.md
+-rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.0/bike/__init__.py
+-rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.0/bike/controllers.py
+-rw-r--r--   0        0        0     2780 2023-05-20 11:23:00.413966 bike-0.3.0/bike/fields.py
+-rw-r--r--   0        0        0     8299 2023-05-21 10:46:27.744577 bike-0.3.0/bike/models.py
+-rw-r--r--   0        0        0      534 2023-05-21 11:51:10.827971 bike-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.0/PKG-INFO
```

### Comparing `bike-0.2.0/LICENSE` & `bike-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bike-0.2.0/bike/controllers.py` & `bike-0.3.0/bike/controllers.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,17 @@
             ret = {}
             for k, v in item.items():
                 if k in self.list_fields:
                     ret[k] = v
             return ret
         return item
 
+    def default(self, dct):
+        return "dict"
+
     def json_parser(self, o: Any) -> Any:
         if hasattr(o, "dict"):
             return self.default(o.dict())
         if isinstance(o, datetime.date):
             return o.strftime('%Y-%m-%d')
         if isinstance(o, datetime.datetime):
             return o.isoformat()
```

### Comparing `bike-0.2.0/bike/fields.py` & `bike-0.3.0/bike/fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,87 @@
-import inspect
 import datetime
 from typing import Any
 
 
 class Field:
     def __new__(cls, *args, **kwargs):
-        members = inspect.getmembers(cls)
         obj = super().__new__(cls)
         return obj
 
     def __init__(
             self,
-            default: Any = None,
+            default: ... = None,
             *,
-            field_type=str,
+            field_type: type = str,
             name: str = '',
             null: bool = True,
-            alias: str = ''
+            alias: str = '',
+            prefix: str = ''
     ):
         self.default = default
         self.type = field_type
         self.name = name
         self.null = null
         self.alias = alias
+        self.prefix = prefix
+        self.alias_load = True
         self.required: bool = True
         self.list: bool = False
+        self.list_type = None
         self.object: bool = False
         self.model = None
         self.validators_pre = []
         self.validators_pos = []
 
-    def prepare_value(self, value, instance):
-        if (value is None or value == '') and self.required:
+    def __str__(self):
+        return f'Field:{self.name}({self.type})'
+
+    def __repr__(self):
+        return f'Field:{self.name}({self.type})'
+
+    def __get__(self, obj, owner):
+        value = getattr(obj, f'_{self.name}')
+        return value
+
+    def __set__(self, obj, value):
+        value = self.__prepare_value(value, self)
+        setattr(obj, f'_{self.name}', value)
+
+    def __prepare_value(self, value, instance):
+        if (value is None or str(value) == '') and self.required:
             if self.default is not None:
                 return self.default
             else:
                 raise Exception(f'Field {self.name} required.')
         for validator in self.validators_pre:
-            value = validator(instance, value)
+            value = validator(self.model, value)
         if not value:
             value = self.default or None
-        if self.type == int:
-            value = int(value)
-        if self.type == datetime.datetime:
-            value = datetime.datetime.strptime(value)
-        if self.type == datetime.date:
-            value = datetime.datetime.strptime(value, '%Y-%m-%d').date()
-        if self.type == float:
-            value = float(value)
-        if self.type == bool:
-            value = True if value == 'true' else False
         if self.list:
-            value = [self.type(**item) for item in value]
+            value = [
+                self.list_type(**item) if isinstance(item, dict) else self.list_type(item) for item in value
+            ]
+        elif self.object:
+            value = self.list_type(**value) if isinstance(value, dict) else value
+        else:
+            match self.type:
+                case int():
+                    value = int(value) if value else None
+                case datetime.datetime():
+                    value = datetime.datetime.strptime(value, '')
+                case datetime.date():
+                    value = datetime.datetime.strptime(value, '%Y-%m-%d').date()
+                case float():
+                    value = float(value)
+                case bool():
+                    value = True if value == 'true' else False
+                case str():
+                    value = str(value)
         for validator in self.validators_pos:
             value = validator(instance, value)
         return value
+
+    def set_validators(self, func: callable, pre: bool):
+        if pre:
+            self.validators_pre.append(func)
+        else:
+            self.validators_pos.append(func)
```

