# Comparing `tmp/serial_deserial_lib-0.1.tar.gz` & `tmp/serial_deserial_lib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serial_deserial_lib-0.1.tar", last modified: Sun May 14 17:21:26 2023, max compression
+gzip compressed data, was "serial_deserial_lib-0.2.tar", last modified: Sun May 21 13:43:37 2023, max compression
```

## Comparing `serial_deserial_lib-0.1.tar` & `serial_deserial_lib-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 17:21:26.108416 serial_deserial_lib-0.1/
--rw-rw-rw-   0        0        0      153 2023-05-14 17:21:26.108416 serial_deserial_lib-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 17:21:26.102414 serial_deserial_lib-0.1/serial_deserial_lib/
--rw-rw-rw-   0        0        0     1279 2023-05-14 17:00:59.000000 serial_deserial_lib-0.1/serial_deserial_lib/__init__.py
--rw-rw-rw-   0        0        0    25627 2023-05-13 21:59:32.000000 serial_deserial_lib-0.1/serial_deserial_lib/ser_deser_class.py
--rw-rw-rw-   0        0        0     8192 2023-05-14 17:01:59.000000 serial_deserial_lib-0.1/serial_deserial_lib/ser_deser_class_test.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:21:26.107414 serial_deserial_lib-0.1/serial_deserial_lib.egg-info/
--rw-rw-rw-   0        0        0      153 2023-05-14 17:21:26.000000 serial_deserial_lib-0.1/serial_deserial_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-05-14 17:21:26.000000 serial_deserial_lib-0.1/serial_deserial_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 17:21:26.000000 serial_deserial_lib-0.1/serial_deserial_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 17:21:26.000000 serial_deserial_lib-0.1/serial_deserial_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-14 17:21:26.000000 serial_deserial_lib-0.1/serial_deserial_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 17:21:26.108416 serial_deserial_lib-0.1/setup.cfg
--rw-rw-rw-   0        0        0      264 2023-05-14 17:21:22.000000 serial_deserial_lib-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:43:37.489991 serial_deserial_lib-0.2/
+-rw-rw-rw-   0        0        0      152 2023-05-21 13:43:37.489991 serial_deserial_lib-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-21 13:43:37.483989 serial_deserial_lib-0.2/serial_deserial_lib/
+-rw-rw-rw-   0        0        0     1279 2023-05-21 13:40:08.000000 serial_deserial_lib-0.2/serial_deserial_lib/__init__.py
+-rw-rw-rw-   0        0        0    26681 2023-05-21 13:25:35.000000 serial_deserial_lib-0.2/serial_deserial_lib/ser_deser_class.py
+-rw-rw-rw-   0        0        0     9887 2023-05-21 13:40:20.000000 serial_deserial_lib-0.2/serial_deserial_lib/ser_deser_class_test.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:43:37.488991 serial_deserial_lib-0.2/serial_deserial_lib.egg-info/
+-rw-rw-rw-   0        0        0      152 2023-05-21 13:43:37.000000 serial_deserial_lib-0.2/serial_deserial_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-05-21 13:43:37.000000 serial_deserial_lib-0.2/serial_deserial_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 13:43:37.000000 serial_deserial_lib-0.2/serial_deserial_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 17:21:26.000000 serial_deserial_lib-0.2/serial_deserial_lib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-05-21 13:43:37.000000 serial_deserial_lib-0.2/serial_deserial_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 13:43:37.489991 serial_deserial_lib-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      263 2023-05-21 13:36:12.000000 serial_deserial_lib-0.2/setup.py
```

### Comparing `serial_deserial_lib-0.1/serial_deserial_lib/__init__.py` & `serial_deserial_lib-0.2/serial_deserial_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `serial_deserial_lib-0.1/serial_deserial_lib/ser_deser_class.py` & `serial_deserial_lib-0.2/serial_deserial_lib/ser_deser_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,15 +275,23 @@
             val for key, val in inspect.getmembers(obj) if key == "__name__"
         ][0]
 
         val_dict["code"] = obj.__code__
 
         return self.basic.format(type="function", val=self.dict_to_obj(val_dict))
     
+    def serialize_iter(self, obj, obj_type)->str:
+        ser_list = []
+        for item in obj:
+            ser_list.append(item)
+        ans_str = self.serialize(ser_list)
+        return self.basic.format(type=obj_type, val=ans_str)
+
     def serialize_object(self, obj) -> str:
+
         type_dict = self.type_to_dict(type(obj))
         # print(obj)
         val = obj.__dict__
         val["type properties"] = type_dict
 
         return self.basic.format(type="object", val=self.dict_to_obj(val))
     
@@ -297,26 +305,29 @@
             float,
             list,
             set,
             bool,
             type,
             types.FunctionType,
             types.ModuleType,
+            types.GeneratorType,
             type,
             types.CodeType,
             bytes,
             property,
             classmethod,
             staticmethod,
             types.MethodType,
             types.BuiltinFunctionType,
         ]
         res = ""
         if type(obj) in default_types:
             res = self.basic_serailize(obj)
+        elif hasattr(obj, '__iter__'):
+            res = self.serialize_iter(obj,'iterator')
         elif type(obj) is not types.NoneType:
             res = self.serialize_object(obj)
         else:
             res = self.serialize_none()
 
         if self.__mode == "json":
             return "{" + res + "}"
@@ -342,14 +353,16 @@
             return self.serialize_tuple(obj)
         elif type(obj) == types.FunctionType:
             return self.serialize_func(obj)
         elif type(obj) == type:
             return self.serialize_type(obj)
         elif type(obj) == types.CodeType:
             return self.serialize_code(obj)
+        elif type(obj) == types.GeneratorType:
+            return self.serialize_iter(obj,'generator')
         elif type(obj) == bytes:
             return self.serialize_bytes(obj)
         elif type(obj) == property:
             return self.serialize_property(obj)
         elif type(obj) == staticmethod:
             return self.serialize_staticmethod(obj)
         elif type(obj) == classmethod:
@@ -593,14 +606,18 @@
             return self.deserialize_dict(v)
         elif t == "function":
             return self.deserialize_function(v)
         elif t == "module":
             return self.deserialize_module(v)
         elif t == "type":
             return self.deserialize_type(v)
+        elif t == "generator":
+            return self.deserialize_generator(v)
+        elif t == "iterator":
+            return self.deserialize_iterator(v)
         elif t == "code":
             return self.deserialize_code(v)
         elif t == "bytes":
             return self.deserialize_bytes(v)
         elif t == "property":
             return self.deserialize_property(v)
         elif t == "staticmethod":
@@ -623,14 +640,16 @@
             "bool",
             "set",
             "int",
             "float",
             "type",
             "list",
             "function",
+            "iterator",
+            "generator",
             "module",
             "type",
             "none",
             "code",
             "bytes",
             "property",
             "classmethod",
@@ -732,14 +751,29 @@
 
 
         if func.__globals__.get(func.__name__):
             func.__globals__.update({func.__name__:func})
 
         return func
 
+    def deserialize_generator(self, val):
+        des_list = self.deserialize(val)
+
+        def generator():
+            for item in des_list:
+                yield item
+
+        f = generator()
+        return f
+    
+    def deserialize_iterator(self, val):
+        des_list = self.deserialize(val)
+                
+        return iter(des_list)
+
     def deserialize_string(self, val) -> str:
         if self.__mode == "json":
             return self.deshield_str(val[1:-1])
         else:
             return self.deshield_str(val[2:-2])
 
     def deserialize_int(self, val) -> int:
```

### Comparing `serial_deserial_lib-0.1/serial_deserial_lib/ser_deser_class_test.py` & `serial_deserial_lib-0.2/serial_deserial_lib/ser_deser_class_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,37 @@
         return cls.class_variable + e
 
 
 class MySubclass(MyClass):
     def method(self, c):
         return 2 * self.a + 2 * self.b + c
 
+class Bass:
+    def bass(self):
+        return("раз раз раз")
+
+
+class Hard:
+    def hard(self):
+        return("yeah")
+
+
+class Based(Hard, Bass):
+    def __init__(self, a: str, b: int):
+        self.a = a
+        self.b = b
+        self.__hop = "hop" + a
+        self.__hey = "hey" + str(b)
+
+    def method(self):
+        return self.a + str(self.b)
+    
+    def __add__(self, other):
+        return 1
+
 
 class ClassSerDeser(unittest.TestCase):
     def test_class_serialization(self):
         my_class = MyClass(1, 2)
         deserialized = SerDeser.deserialize(SerDeser.serialize(my_class))
         deserialized_xml = SerDeserXML.deserialize(SerDeserXML.serialize(my_class))
 
@@ -70,14 +93,32 @@
         self.assertEqual(deserialized_xml.a, 1)
         self.assertEqual(deserialized_xml.b, 2)
         self.assertEqual(deserialized_xml.method(4), my_subclass.method(4))
         self.assertEqual(
             deserialized_xml.method2(2, 3, 4), my_subclass.method2(2, 3, 4)
         )
 
+    def test_multiinheritance(self):
+        test = Based('1', 2)
+
+        deserialized = SerDeser.deserialize(SerDeser.serialize(test))
+        deserialized_xml = SerDeserXML.deserialize(SerDeserXML.serialize(test))
+
+        self.assertEqual(deserialized.a, '1')
+        self.assertEqual(deserialized.b, 2)
+        self.assertEqual(deserialized.method(), test.method())
+        self.assertEqual(deserialized.hard(), test.hard())
+        self.assertEqual(deserialized.bass(), test.bass())
+
+        self.assertEqual(deserialized_xml.a, '1')
+        self.assertEqual(deserialized_xml.b, 2)
+        self.assertEqual(deserialized_xml.method(), test.method())
+        self.assertEqual(deserialized_xml.hard(), test.hard())
+        self.assertEqual(deserialized_xml.bass(), test.bass())
+
     def test_static_method_serialization(self):
         my_class = MyClass(1, 2)
         func = SerDeser.deserialize(SerDeser.serialize(my_class.static_method))
         self.assertEqual(func(5), MyClass.static_method(5))
         self.assertEqual(func(6), MyClass.static_method(6))
         self.assertEqual(func(7), MyClass.static_method(7))
 
@@ -224,15 +265,31 @@
         def my_function(x):
             return x + 1
 
         self.assertEqual(SerDeser.deserialize(SerDeser.serialize(my_function))(3), 8)
         self.assertEqual(
             SerDeserXML.deserialize(SerDeserXML.serialize(my_function))(3), 8
         )
+    
+    def test_generator(self):
+        def foo(a):
+            for _ in a:
+                yield _
+
+        q = foo([1,2,3])
+        des = SerDeser.loads(SerDeser.dumps(q))
+        self.assertEqual(next(des), 1)
+        self.assertEqual(next(des), 2)
+
+    def test_iterator(self):
+        q = iter([1,2,3])
+        des = SerDeser.loads(SerDeser.dumps(q))
+        self.assertEqual(next(des), 1)
+        self.assertEqual(next(des), 2)
 
 
 def do_test():
-    unittest.main("serdeser_test")
+    unittest.main("ser_deser_class_test")
 
 
 if __name__ == "__main__":
     do_test()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

