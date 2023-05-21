# Comparing `tmp/filedbm-0.0.5.tar.gz` & `tmp/filedbm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedbm-0.0.5.tar", last modified: Sun May 14 20:38:05 2023, max compression
+gzip compressed data, was "filedbm-0.0.6.tar", last modified: Sun May 21 21:18:43 2023, max compression
```

## Comparing `filedbm-0.0.5.tar` & `filedbm-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 20:38:05.356268 filedbm-0.0.5/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-08 01:46:02.000000 filedbm-0.0.5/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-14 20:38:05.356268 filedbm-0.0.5/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      152 2023-05-08 01:50:12.000000 filedbm-0.0.5/README.rst
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 20:38:05.356268 filedbm-0.0.5/filedbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)       70 2023-05-08 05:12:10.000000 filedbm-0.0.5/filedbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     8341 2023-05-14 20:37:19.000000 filedbm-0.0.5/filedbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 20:38:05.356268 filedbm-0.0.5/filedbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-08 01:48:21.000000 filedbm-0.0.5/filedbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5306 2023-05-14 08:48:26.000000 filedbm-0.0.5/filedbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 20:38:05.356268 filedbm-0.0.5/filedbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-14 20:38:05.000000 filedbm-0.0.5/filedbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      255 2023-05-14 20:38:05.000000 filedbm-0.0.5/filedbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-14 20:38:05.000000 filedbm-0.0.5/filedbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-14 20:38:05.000000 filedbm-0.0.5/filedbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-08 01:48:21.000000 filedbm-0.0.5/pyproject.toml
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-14 20:38:05.356268 filedbm-0.0.5/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7116 2023-05-14 20:37:47.000000 filedbm-0.0.5/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-21 21:18:43.831107 filedbm-0.0.6/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-08 01:46:02.000000 filedbm-0.0.6/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-21 21:18:43.831107 filedbm-0.0.6/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      152 2023-05-08 01:50:12.000000 filedbm-0.0.6/README.rst
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-21 21:18:43.831107 filedbm-0.0.6/filedbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       70 2023-05-08 05:12:10.000000 filedbm-0.0.6/filedbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7975 2023-05-21 21:18:01.000000 filedbm-0.0.6/filedbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-21 21:18:43.831107 filedbm-0.0.6/filedbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-08 01:48:21.000000 filedbm-0.0.6/filedbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5675 2023-05-21 21:12:59.000000 filedbm-0.0.6/filedbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-21 21:18:43.831107 filedbm-0.0.6/filedbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-21 21:18:43.000000 filedbm-0.0.6/filedbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      255 2023-05-21 21:18:43.000000 filedbm-0.0.6/filedbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-21 21:18:43.000000 filedbm-0.0.6/filedbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-21 21:18:43.000000 filedbm-0.0.6/filedbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-08 01:48:21.000000 filedbm-0.0.6/pyproject.toml
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-21 21:18:43.831107 filedbm-0.0.6/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7116 2023-05-21 21:18:10.000000 filedbm-0.0.6/setup.py
```

### Comparing `filedbm-0.0.5/LICENSE` & `filedbm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `filedbm-0.0.5/PKG-INFO` & `filedbm-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedbm
-Version: 0.0.5
+Version: 0.0.6
 Summary: A persistent key-value database
 Home-page: https://github.com/mullenkamp/filedbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `filedbm-0.0.5/filedbm/main.py` & `filedbm-0.0.6/filedbm/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,24 +176,14 @@
 
     def close(self):
         pass
 
     # def __del__(self):
     #     self.close()
 
-    # def sync(self):
-    #     if self._write:
-    #         if self._buffer_index:
-    #             utils.flush_write_buffer(self._mm, self._write_buffer)
-    #             self._sync_index()
-    #         self._mm.seek(n_keys_pos)
-    #         self._mm.write(utils.int_to_bytes(self._n_keys, 4))
-    #         self._mm.flush()
-    #         self._file.flush()
-
 
 
 def open(
     db_path: str, flag: str = "r", buffer_size: int=512000, n_bytes_key: int=2, n_bytes_value: int=4, ttl: int=None):
     """
     Open a persistent dictionary for reading and writing. All keys and values are stored in individual files within the db_path. Keys must be strings and values must be either bytes or file-objects. In the future, I might add more flexibility for inputs and outputs.
```

### Comparing `filedbm-0.0.5/filedbm/utils.py` & `filedbm-0.0.6/filedbm/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jan  5 11:04:13 2023
 
 @author: mike
 """
+import pathlib
 import os
 import io
 from hashlib import blake2b, blake2s
 # from time import time
 from typing import Any, Generic, Iterator, Union
 import mmap
 from time import time
@@ -19,43 +20,49 @@
 key_hash_len = 13
 
 
 ############################################
 ### Classes
 
 
-class FileObjectSlice(io.IOBase):
-    def __init__(self, file: Union[io.IOBase, mmap.mmap], offset: int, length: int):
-        self.f = file
+class FileObjectReadSlice(io.IOBase):
+    def __init__(self, file_path: Union[pathlib.Path, str], offset: int, length: int):
+        self.f = file_path
         self.f_offset = offset
         self.offset = 0
         self.length = length
 
     def seek(self, offset, whence=0):
         if whence == os.SEEK_SET:
             self.offset = offset
         elif whence == os.SEEK_CUR:
             self.offset += offset
         elif whence == os.SEEK_END:
-            self.offset = self.length+offset
+            self.offset = self.length + offset
         else:
             # Other values of whence should raise an IOError
-            return self.f.seek(offset, whence)
-        return self.f.seek(self.offset+self.f_offset, os.SEEK_SET)
+            raise IOError(offset, whence)
+        return self.offset
+        # return self.f.seek(self.offset + self.f_offset, os.SEEK_SET)
 
     def tell(self):
         return self.offset
 
     def read(self, size=-1):
-        self.seek(self.offset)
-        if size<0:
-            size = self.length-self.offset
-        size = max(0, min(size, self.length-self.offset))
-        self.offset += size
-        return self.f.read(size)
+        if size < 0:
+            size = self.length - self.offset
+        size = max(0, min(size, self.length - self.offset))
+        with io.open(self.f, 'rb', buffering=0) as file:
+            with mmap.mmap(file.fileno(), 0, access=mmap.ACCESS_READ) as mm:
+                mm.seek(self.offset + self.f_offset)
+                b1 = mm.read(size)
+                mm.close()
+                file.close()
+                self.offset += size
+                return b1
 
 
 ############################################
 ### Functions
 
 
 def bytes_to_int(b, signed=False):
@@ -86,46 +93,46 @@
     pos = file_obj.tell()
     size = file_obj.seek(0, io.SEEK_END)
     file_obj.seek(pos)
 
     return size
 
 
-def get_data_block(mm, key, value, n_bytes_key, n_bytes_value):
+def get_data_block(file_path, key, value, n_bytes_key, n_bytes_value):
     """
     Function to get either the key or the value or both from a data block.
     """
-
-    if key and value:
-        key_len_value_len = mm.read(n_bytes_key + n_bytes_value)
-        key_len = bytes_to_int(key_len_value_len[:n_bytes_key])
-        value_len = bytes_to_int(key_len_value_len[n_bytes_key:])
-        key_value = mm.read(key_len + value_len)
-        key = key_value[:key_len]
-        value = FileObjectSlice(mm, n_bytes_key + n_bytes_value + key_len, value_len)
-
-        # value = key_value[key_len:]
-        return key.decode(), value
-
-    elif key:
-        key_len = bytes_to_int(mm.read(n_bytes_key))
-        mm.seek(n_bytes_value, 1)
-        key = mm.read(key_len)
-        return key.decode()
-
-    elif value:
-        key_len_value_len = mm.read(n_bytes_key + n_bytes_value)
-        key_len = bytes_to_int(key_len_value_len[:n_bytes_key])
-        value_len = bytes_to_int(key_len_value_len[n_bytes_key:])
-        value = FileObjectSlice(mm, n_bytes_key + n_bytes_value + key_len, value_len)
-        # mm.seek(key_len, 1)
-        # value = mm.read(value_len)
-        return value
-    else:
-        raise ValueError('One or both key and value must be True.')
+    with io.open(file_path, 'rb', buffering=0) as file:
+        with mmap.mmap(file.fileno(), 0, access=mmap.ACCESS_READ) as mm:
+            if key and value:
+                key_len_value_len = mm.read(n_bytes_key + n_bytes_value)
+                key_len = bytes_to_int(key_len_value_len[:n_bytes_key])
+                value_len = bytes_to_int(key_len_value_len[n_bytes_key:])
+                key_value = mm.read(key_len + value_len)
+                key = key_value[:key_len]
+                value = FileObjectReadSlice(file_path, n_bytes_key + n_bytes_value + key_len, value_len)
+
+                return key.decode(), value
+
+            elif key:
+                key_len = bytes_to_int(mm.read(n_bytes_key))
+                mm.seek(n_bytes_value, 1)
+                key = mm.read(key_len)
+
+                return key.decode()
+
+            elif value:
+                key_len_value_len = mm.read(n_bytes_key + n_bytes_value)
+                key_len = bytes_to_int(key_len_value_len[:n_bytes_key])
+                value_len = bytes_to_int(key_len_value_len[n_bytes_key:])
+                value = FileObjectReadSlice(file_path, n_bytes_key + n_bytes_value + key_len, value_len)
+
+                return value
+            else:
+                raise ValueError('One or both key and value must be True.')
 
 
 def get_value(db_path, key, n_bytes_key, n_bytes_value, ttl=None):
     """
 
     """
     key_bytes_len = len(key)
@@ -133,22 +140,19 @@
     file_path = db_path.joinpath(key_hash)
     if file_path.exists():
         if ttl is not None:
             if (time() - os.path.getmtime(file_path)) > ttl:
                 file_path.unlink()
                 return None
 
-        file = io.open(file_path, 'rb')
-        mm = mmap.mmap(file.fileno(), 0, access=mmap.ACCESS_READ)
-
-        file_len = len(mm)
+        file_len = file_path.stat().st_size
 
         value_pos = n_bytes_key + n_bytes_value + key_bytes_len
 
-        out = FileObjectSlice(mm, value_pos, file_len - value_pos)
+        out = FileObjectReadSlice(file_path, value_pos, file_len - value_pos)
 
         return out
     else:
         return None
 
 
 def iter_keys_values(db_path, key=False, value=False, n_bytes_key=2, n_bytes_value=4, ttl=None):
@@ -156,18 +160,16 @@
 
     """
     for file_path in db_path.iterdir():
         if ttl is not None:
             if (time() - os.path.getmtime(file_path)) > ttl:
                 file_path.unlink()
                 continue
-        file = io.open(file_path, 'rb')
-        mm = mmap.mmap(file.fileno(), 0, access=mmap.ACCESS_READ)
 
-        yield get_data_block(mm, key, value, n_bytes_key, n_bytes_value)
+        yield get_data_block(file_path, key, value, n_bytes_key, n_bytes_value)
 
 
 def write_data_block(db_path, key, value, n_bytes_key, n_bytes_value, buffer_size):
     """
 
     """
     key_bytes_len = len(key)
@@ -178,26 +180,24 @@
 
     value_bytes_len = determine_obj_size(value)
 
     write_init_bytes = int_to_bytes(key_bytes_len, n_bytes_key) + int_to_bytes(value_bytes_len, n_bytes_value) + key
 
     file_path = db_path.joinpath(key_hash)
 
-    file = io.open(file_path, 'w+b')
-    _ = file.write(write_init_bytes)
+    with io.open(file_path, 'w+b') as file:
+        _ = file.write(write_init_bytes)
 
-    if hasattr(value, '_buffer_size'):
-        buffer_size = value._buffer_size
+        if hasattr(value, '_buffer_size'):
+            buffer_size = value._buffer_size
 
-    chunk = value.read(buffer_size)
-    while chunk:
-        file.write(chunk)
         chunk = value.read(buffer_size)
-
-    file.close()
+        while chunk:
+            file.write(chunk)
+            chunk = value.read(buffer_size)
```

### Comparing `filedbm-0.0.5/filedbm.egg-info/PKG-INFO` & `filedbm-0.0.6/filedbm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedbm
-Version: 0.0.5
+Version: 0.0.6
 Summary: A persistent key-value database
 Home-page: https://github.com/mullenkamp/filedbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `filedbm-0.0.5/setup.py` & `filedbm-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 'filedbm'
 main_package = 'filedbm'
-version = '0.0.5'
+version = '0.0.6'
 descrip = 'A persistent key-value database'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

