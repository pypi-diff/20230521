# Comparing `tmp/std.algorithm-1.1.2.tar.gz` & `tmp/std.algorithm-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std.algorithm-1.1.2.tar", last modified: Wed Apr  5 04:20:16 2023, max compression
+gzip compressed data, was "std.algorithm-1.1.3.tar", last modified: Sun May 21 09:44:04 2023, max compression
```

## Comparing `std.algorithm-1.1.2.tar` & `std.algorithm-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 04:20:16.989740 std.algorithm-1.1.2/
--rw-rw-rw-   0        0        0      324 2023-04-05 04:20:16.989740 std.algorithm-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       47 2022-10-07 01:09:45.000000 std.algorithm-1.1.2/README.md
--rw-rw-rw-   0        0        0      312 2023-04-05 04:20:16.990724 std.algorithm-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      478 2023-02-19 07:05:31.000000 std.algorithm-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 04:20:16.963699 std.algorithm-1.1.2/std/
--rw-rw-rw-   0        0        0    19016 2023-04-05 03:45:33.000000 std.algorithm-1.1.2/std/__init__.py
--rw-rw-rw-   0        0        0      214 2022-10-12 06:19:30.000000 std.algorithm-1.1.2/std/error.py
--rw-rw-rw-   0        0        0     8443 2023-03-24 13:15:51.000000 std.algorithm-1.1.2/std/file.py
--rw-rw-rw-   0        0        0     1467 2022-10-07 01:19:27.000000 std.algorithm-1.1.2/std/heap.py
--rw-rw-rw-   0        0        0     1754 2023-03-04 02:50:47.000000 std.algorithm-1.1.2/std/http.py
-drwxrwxrwx   0        0        0        0 2023-04-05 04:20:16.987703 std.algorithm-1.1.2/std/lib/
--rw-rw-rw-   0        0        0  2220528 2022-10-22 04:21:48.000000 std.algorithm-1.1.2/std/lib/eigen.dll
--rw-rw-rw-   0        0        0    12858 2022-11-01 16:38:35.000000 std.algorithm-1.1.2/std/nlp.py
--rw-rw-rw-   0        0        0     1956 2022-11-05 03:18:44.000000 std.algorithm-1.1.2/std/padding.py
--rw-rw-rw-   0        0        0       89 2023-03-11 01:48:50.000000 std.algorithm-1.1.2/std/regexp.py
--rw-rw-rw-   0        0        0      770 2022-10-12 05:55:17.000000 std.algorithm-1.1.2/std/search.py
--rw-rw-rw-   0        0        0    19454 2023-03-11 01:48:50.000000 std.algorithm-1.1.2/std/sets.py
--rw-rw-rw-   0        0        0     1162 2022-10-07 01:27:48.000000 std.algorithm-1.1.2/std/tree.py
--rw-rw-rw-   0        0        0      443 2023-03-17 14:49:04.000000 std.algorithm-1.1.2/std/unicode.py
--rw-rw-rw-   0        0        0    35286 2023-02-05 04:04:59.000000 std.algorithm-1.1.2/std/xml.py
-drwxrwxrwx   0        0        0        0 2023-04-05 04:20:16.968723 std.algorithm-1.1.2/std.algorithm.egg-info/
--rw-rw-rw-   0        0        0      324 2023-04-05 04:20:16.000000 std.algorithm-1.1.2/std.algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-04-05 04:20:16.000000 std.algorithm-1.1.2/std.algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 04:20:16.000000 std.algorithm-1.1.2/std.algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-05 04:20:16.000000 std.algorithm-1.1.2/std.algorithm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-05 04:20:16.000000 std.algorithm-1.1.2/std.algorithm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 09:44:04.008292 std.algorithm-1.1.3/
+-rw-rw-rw-   0        0        0      324 2023-05-21 09:44:04.008292 std.algorithm-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2022-10-07 01:09:45.000000 std.algorithm-1.1.3/README.md
+-rw-rw-rw-   0        0        0      312 2023-05-21 09:44:04.012309 std.algorithm-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      478 2023-02-19 07:05:31.000000 std.algorithm-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:44:03.958368 std.algorithm-1.1.3/std/
+-rw-rw-rw-   0        0        0    13868 2023-05-18 13:13:28.000000 std.algorithm-1.1.3/std/MySQL.py
+-rw-rw-rw-   0        0        0    20406 2023-04-28 14:40:16.000000 std.algorithm-1.1.3/std/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-04-18 14:54:44.000000 std.algorithm-1.1.3/std/combinatorics.py
+-rw-rw-rw-   0        0        0     2819 2023-05-14 09:54:42.000000 std.algorithm-1.1.3/std/data.py
+-rw-rw-rw-   0        0        0      214 2022-10-12 06:19:30.000000 std.algorithm-1.1.3/std/error.py
+-rw-rw-rw-   0        0        0     8504 2023-05-14 09:57:03.000000 std.algorithm-1.1.3/std/file.py
+-rw-rw-rw-   0        0        0     1754 2023-03-04 02:50:47.000000 std.algorithm-1.1.3/std/http.py
+-rw-rw-rw-   0        0        0    39598 2023-05-20 02:05:20.000000 std.algorithm-1.1.3/std/keras.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:44:04.006296 std.algorithm-1.1.3/std/lib/
+-rw-rw-rw-   0        0        0  2220528 2022-10-22 04:21:48.000000 std.algorithm-1.1.3/std/lib/eigen.dll
+-rw-rw-rw-   0        0        0    12858 2022-11-01 16:38:35.000000 std.algorithm-1.1.3/std/nlp.py
+-rw-rw-rw-   0        0        0       89 2023-03-11 01:48:50.000000 std.algorithm-1.1.3/std/regexp.py
+-rw-rw-rw-   0        0        0      770 2022-10-12 05:55:17.000000 std.algorithm-1.1.3/std/search.py
+-rw-rw-rw-   0        0        0    19454 2023-03-11 01:48:50.000000 std.algorithm-1.1.3/std/sets.py
+-rw-rw-rw-   0        0        0     1162 2022-10-07 01:27:48.000000 std.algorithm-1.1.3/std/tree.py
+-rw-rw-rw-   0        0        0      443 2023-03-17 14:49:04.000000 std.algorithm-1.1.3/std/unicode.py
+-rw-rw-rw-   0        0        0    35286 2023-02-05 04:04:59.000000 std.algorithm-1.1.3/std/xml.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:44:03.964354 std.algorithm-1.1.3/std.algorithm.egg-info/
+-rw-rw-rw-   0        0        0      324 2023-05-21 09:44:03.000000 std.algorithm-1.1.3/std.algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-05-21 09:44:03.000000 std.algorithm-1.1.3/std.algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 09:44:03.000000 std.algorithm-1.1.3/std.algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-21 09:44:03.000000 std.algorithm-1.1.3/std.algorithm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-21 09:44:03.000000 std.algorithm-1.1.3/std.algorithm.egg-info/top_level.txt
```

### Comparing `std.algorithm-1.1.2/std/__init__.py` & `std.algorithm-1.1.3/std/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -739,13 +739,58 @@
     else:
         args, = args
         for key, value in args:
             obj[key] = value
 
     return obj
 
+def array_split(arr, index):
+    if isinstance(index, int):
+        return arr[:index], arr[index:]
+    
+    if isinstance(index, slice):
+        start, stop, step = index.start, index.stop, index.step
+        if step is None:
+            step = 1
+
+        if step > 0:
+            if start is None:
+                start = 0
+            elif start < 0:
+                start += len(arr)
+
+            if stop is None:
+                stop = len(arr)
+            elif stop < 0:
+                stop += len(arr)
+
+            if step > 1:
+                rest = (arr[i] for i in {*range(start, stop)} - {*range(start, stop, step)})
+                rest = arr[:start] + type(arr)(rest) + arr[stop:]
+            else:
+                rest = arr[:start] + arr[stop:]
+        else:
+            if start is None:
+                start = len(arr) - 1
+            elif start < 0:
+                start += len(arr)
+
+            if stop is None:
+                stop = -1
+            elif stop < -1:
+                stop += len(arr)
+            
+            if step < -1:
+                rest = (arr[i] for i in {*range(start, stop, -1)} - {*range(start, stop, step)})
+                rest = arr[:stop + 1] + type(arr)(rest) + arr[start + 1:]
+            else:
+                rest = arr[:stop + 1] + arr[start + 1:]
+
+        return arr[index], rest
+
 
 if __name__ == '__main__':
-    obj = Object(a=1, b=2, c=3)
-    dic = {**obj}
-    print(dic)
+    arr = [*range(10)]
+    former, latter = array_split(arr, slice(-2, -8, -2))
+    print(former)
+    print(latter)
```

### Comparing `std.algorithm-1.1.2/std/file.py` & `std.algorithm-1.1.3/std/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,22 +99,22 @@
                     assert _offset == offset
                     char = self.file.read(1)
 #                     print('char =', char)
                     if char[0] == '\n' or char[0] == '\r':
                         break
         else:
             self.rewind()
-            offset = self.f.tell()
+            offset = self.file.tell()
             while index > 0:
                 index -= 1
                 while True:
                     offset += 1
-                    _offset = self.f.seek(offset, os.SEEK_SET)
+                    _offset = self.file.seek(offset, os.SEEK_SET)
                     assert _offset == offset
-                    char = self.f.read(1)
+                    char = self.file.read(1)
 #                     print('char =', char)
                     if char[0] == '\n' or char[0] == '\r':
                         break
 
         current_pos = self.file.tell()
         assert current_pos == offset + 1
 
@@ -131,44 +131,44 @@
 
         self.file.flush()
 
     def __getitem__(self, index):
         if index < 0:
             self.end()
             index = -index
-            offset = self.f.tell() - 1
+            offset = self.file.tell() - 1
             while index > 0:
                 index -= 1
                 offset -= 1
                 while True:
                     offset -= 1
-                    _offset = self.f.seek(offset, os.SEEK_SET)
+                    _offset = self.file.seek(offset, os.SEEK_SET)
                     assert _offset == offset
-                    char = self.f.read(1)
+                    char = self.file.read(1)
     #                     print('char =', char)
                     if char == '\n' or char == '\r':
                         break
         else:
             self.rewind()
-            offset = self.f.tell()
+            offset = self.file.tell()
             while index > 0:
                 index -= 1
                 while True:
                     offset += 1
-                    _offset = self.f.seek(offset, os.SEEK_SET)
+                    _offset = self.file.seek(offset, os.SEEK_SET)
                     assert _offset == offset
-                    char = self.f.read(1)
+                    char = self.file.read(1)
 #                     print('char =', char)
                     if char == '\n' or char == '\r':
                         break
-        current_pos = self.f.tell()
+        current_pos = self.file.tell()
 
-        self.f.seek(current_pos, os.SEEK_SET)
+        self.file.seek(current_pos, os.SEEK_SET)
 
-        return self.f.readline().strip()
+        return self.file.readline().strip()
 
     def write(self, s):
         self.rewind()
 
         if type(s) == str:
             self.file.write(s + '\n')
         else:
@@ -184,15 +184,15 @@
         self.file.flush()
 
     def rewind(self):
 #         skip_byte_order_mark
         self.file.seek(0, os.SEEK_SET)
         byteOrderMark = self.file.read(1)
         if byteOrderMark and ord(byteOrderMark) != 0xFEFF:
-            self.file.seek(0, os.SEEK_SET)        
+            self.file.seek(0, os.SEEK_SET)
 
     def end(self):
         self.file.seek(0, os.SEEK_END)
 
     def collect(self):
         self.rewind()
 
@@ -243,15 +243,16 @@
             return False
         
         _offset = self.file.seek(offset, os.SEEK_SET)
         assert _offset == offset
         char = self.file.read(size)        
         return char == end
 
-    def readlines(self): 
+    def readlines(self):
+        self.rewind()
         return [s for s in self]
     
     def readline(self):
         try: 
             return next(self)
         except StopIteration:
             return ''
@@ -297,15 +298,16 @@
     def close(self):
         self.file.close()
         
     def __iter__(self):  # Get iterator object on iter
         return self
 
     def __next__(self):
-        if line := self.file.readline():
+        line = self.file.readline()
+        if line:
             return json.loads(line) if self.json else line
 
         raise StopIteration
 
     def append(self, s):
         if not isinstance(s, str):
             s = json.dumps(s)
```

### Comparing `std.algorithm-1.1.2/std/http.py` & `std.algorithm-1.1.3/std/http.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.2/std/lib/eigen.dll` & `std.algorithm-1.1.3/std/lib/eigen.dll`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.2/std/nlp.py` & `std.algorithm-1.1.3/std/nlp.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.2/std/search.py` & `std.algorithm-1.1.3/std/search.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.2/std/sets.py` & `std.algorithm-1.1.3/std/sets.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.2/std/tree.py` & `std.algorithm-1.1.3/std/tree.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.2/std/xml.py` & `std.algorithm-1.1.3/std/xml.py`

 * *Files identical despite different names*

