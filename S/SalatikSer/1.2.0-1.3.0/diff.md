# Comparing `tmp/SalatikSer-1.2.0.tar.gz` & `tmp/SalatikSer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SalatikSer-1.2.0.tar", last modified: Tue May 16 13:48:26 2023, max compression
+gzip compressed data, was "SalatikSer-1.3.0.tar", last modified: Sun May 21 14:51:13 2023, max compression
```

## Comparing `SalatikSer-1.2.0.tar` & `SalatikSer-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:48:26.384767 SalatikSer-1.2.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:48:26.384767 SalatikSer-1.2.0/MySerializer/
--rw-r--r--   0 root         (0) root         (0)      341 2023-05-14 10:53:12.000000 SalatikSer-1.2.0/MySerializer/MySerializer.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-14 10:44:05.000000 SalatikSer-1.2.0/MySerializer/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 13:27:44.000000 SalatikSer-1.2.0/MySerializer/constants.py
--rw-r--r--   0 root         (0) root         (0)     6796 2023-05-15 18:46:48.000000 SalatikSer-1.2.0/MySerializer/json_utils.py
--rw-r--r--   0 root         (0) root         (0)     4709 2023-05-16 13:44:11.000000 SalatikSer-1.2.0/MySerializer/pack_utils.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-05-14 14:36:25.000000 SalatikSer-1.2.0/MySerializer/serializer.py
--rw-r--r--   0 root         (0) root         (0)     6179 2023-05-16 13:44:13.000000 SalatikSer-1.2.0/MySerializer/unpack_utils.py
--rw-r--r--   0 root         (0) root         (0)     6793 2023-05-14 13:32:11.000000 SalatikSer-1.2.0/MySerializer/xml_utils.py
--rw-r--r--   0 root         (0) root         (0)      212 2023-05-16 13:48:26.384767 SalatikSer-1.2.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:48:26.384767 SalatikSer-1.2.0/SalatikSer.egg-info/
--rw-r--r--   0 root         (0) root         (0)      212 2023-05-16 13:48:26.000000 SalatikSer-1.2.0/SalatikSer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-16 13:48:26.000000 SalatikSer-1.2.0/SalatikSer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 13:48:26.000000 SalatikSer-1.2.0/SalatikSer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-16 13:48:26.000000 SalatikSer-1.2.0/SalatikSer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 13:48:26.000000 SalatikSer-1.2.0/SalatikSer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 13:48:26.384767 SalatikSer-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-16 13:40:19.000000 SalatikSer-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:22:18.767994 SalatikSer-1.3.0/
+drwxrwxrwx   0        0        0        0 2023-05-20 13:22:18.659661 SalatikSer-1.3.0/MySerializer/
+-rw-rw-rw-   0        0        0      341 2023-05-20 11:29:42.000000 SalatikSer-1.3.0/MySerializer/MySerializer.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 11:29:42.000000 SalatikSer-1.3.0/MySerializer/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-05-20 11:29:42.000000 SalatikSer-1.3.0/MySerializer/constants.py
+-rw-rw-rw-   0        0        0     6775 2023-05-20 11:29:42.000000 SalatikSer-1.3.0/MySerializer/json_utils.py
+-rw-rw-rw-   0        0        0     4680 2023-05-20 13:21:16.000000 SalatikSer-1.3.0/MySerializer/pack_utils.py
+-rw-rw-rw-   0        0        0     1339 2023-05-20 11:29:42.000000 SalatikSer-1.3.0/MySerializer/serializer.py
+-rw-rw-rw-   0        0        0     6359 2023-05-20 13:21:03.000000 SalatikSer-1.3.0/MySerializer/unpack_utils.py
+-rw-rw-rw-   0        0        0     6789 2023-05-20 11:29:42.000000 SalatikSer-1.3.0/MySerializer/xml_utils.py
+-rw-rw-rw-   0        0        0      154 2023-05-20 13:22:18.767994 SalatikSer-1.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 13:22:18.735494 SalatikSer-1.3.0/SalatikSer.egg-info/
+-rw-rw-rw-   0        0        0      154 2023-05-20 13:22:18.000000 SalatikSer-1.3.0/SalatikSer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-05-20 13:22:18.000000 SalatikSer-1.3.0/SalatikSer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 13:22:18.000000 SalatikSer-1.3.0/SalatikSer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-20 13:22:18.000000 SalatikSer-1.3.0/SalatikSer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-05-20 13:22:18.000000 SalatikSer-1.3.0/SalatikSer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 13:22:18.767994 SalatikSer-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      399 2023-05-20 13:21:46.000000 SalatikSer-1.3.0/setup.py
```

### Comparing `SalatikSer-1.2.0/MySerializer/json_utils.py` & `SalatikSer-1.3.0/MySerializer/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def load(self, file):
         return self.loads(file.read())
     
     def deserialize_from_str(self, string):
         self.pos = string.find('"type":', self.pos)
 
         if self.pos != -1:
-            self.pos += len('"type": ')  # add "type" length
+            self.pos += len('"type": ')
 
         if self.pos >= len(string) or self.pos == -1:
             return
 
         if string[self.pos:self.pos + len('"int"')] == '"int"':
             self.pos += len('"int"\n')
```

### Comparing `SalatikSer-1.2.0/MySerializer/pack_utils.py` & `SalatikSer-1.3.0/MySerializer/pack_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,13 +158,12 @@
 
     result["__bases__"] = [pack_class(base) for base in obj.__bases__ if base != object]
 
     return result
 
 def pack_object(obj):
     result = {"__type__": "object", "__class__": pack_class(obj.__class__), "attr": {}}
-
     for key, value in inspect.getmembers(obj):
-        if not key.startswith("__") and not is_function(value):
+        if not key.startswith("__"):
             result["attr"][key] = pack(value)
 
     return result
```

### Comparing `SalatikSer-1.2.0/MySerializer/serializer.py` & `SalatikSer-1.3.0/MySerializer/serializer.py`

 * *Files identical despite different names*

### Comparing `SalatikSer-1.2.0/MySerializer/unpack_utils.py` & `SalatikSer-1.3.0/MySerializer/unpack_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,19 +77,24 @@
 
     return result
 
 def unpack_object(obj):
     obj_class = unpack(obj["__class__"])
     attrs = {}
 
+
     for key, value in obj["attr"].items():
         attrs[key] = unpack(value)
 
-    result = object.__new__(obj_class)
-    result.__dict__ = attrs
+    if "property" in obj_class.__name__:
+        obj_class = property
+        result = property(fget=attrs["fget"],fset=attrs["fset"],fdel=attrs["fdel"])
+    else:
+        result = object.__new__(obj_class)
+        result.__dict__ = attrs
 
     return result
 
 def unpack_function(src):
     arguments = src["__args__"]
     globs = src["__globals__"]
     globs["__builtins__"] = __builtins__
@@ -99,14 +104,15 @@
             try:
                 globs[key] = __import__(src["__globals__"][key])
 
             except:
                 if globs[key] != src["__name__"]:
                     globs[key] = unpack(src["__globals__"][key])
 
+
     coded = CodeType(arguments['co_argcount'],
                      arguments['co_posonlyargcount'],
                      arguments['co_kwonlyargcount'],
                      arguments['co_nlocals'],
                      arguments['co_stacksize'],
                      arguments['co_flags'],
                      bytes(arguments['co_code']),
```

### Comparing `SalatikSer-1.2.0/MySerializer/xml_utils.py` & `SalatikSer-1.3.0/MySerializer/xml_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     def load(self, file):
         return self.loads(file.read())
 
     def deserialize_from_str(self, string):
         self.pos = string.find('<"', self.pos)
 
         if self.pos != -1:
-            self.pos += len('<')  # add "type" length
+            self.pos += len('<')  
 
         if self.pos >= len(string) or self.pos == -1:
             return None
 
         if string[self.pos:self.pos + len('"int"')] == '"int"':
             self.pos += len('"int"')
 
@@ -116,15 +116,14 @@
         if string[self.pos:self.pos + len('"str"')] == '"str"':
             self.pos += len('"str"')
 
             return self.deserialize_str(string)
 
         if string[self.pos:self.pos + len('"dict"')] == '"dict"':
             self.pos += len('"dict"')
-
             return self.deserialize_dict(string)
 
         if string[self.pos:self.pos + len('"list"')] == '"list"' or \
                 string[self.pos:self.pos + len('"tuple"')] == '"tuple"' or \
                 string[self.pos:self.pos + len('"set"')] == '"set"':
 
             self.pos += 1
@@ -167,29 +166,30 @@
         else:
             self.pos += 1
             return res
 
     def deserialize_dict(self, s):
         res = {}
 
-        while self.pos < len(s) and s[self.pos:self.pos+9] != '</"dict">':
+        while self.pos < len(s) and s[self.pos:self.pos+len('</"dict">')] != '</"dict">':
             self.pos = s.find('<', self.pos)
 
             while s[self.pos+1] == '/' and s[self.pos:self.pos+9] != '</"dict">':
                 self.pos = s.find('<', self.pos+1)
             if s[self.pos+1] == '/' and s[self.pos:self.pos+9] == '</"dict">':
                 self.pos = s.find('<', self.pos + 1)
                 return res
             k = self.deserialize_from_str(s)
             v = self.deserialize_from_str(s)
 
             res[k] = v
 
             if self.pos == -1:
                 return res
+
         return res
 
     def deserialize_str(self, s):
         res = ''
         self.pos = s.find('>', self.pos) + 1
 
         while self.pos < len(s) and s[self.pos] != '<':
```

