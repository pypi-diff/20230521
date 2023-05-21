# Comparing `tmp/smartdict-0.0.5.tar.gz` & `tmp/smartdict-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdict-0.0.5.tar", last modified: Wed Nov  2 06:21:02 2022, max compression
+gzip compressed data, was "smartdict-0.0.6.tar", last modified: Sun May 21 15:01:21 2023, max compression
```

## Comparing `smartdict-0.0.5.tar` & `smartdict-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2022-11-02 06:21:02.120410 smartdict-0.0.5/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     2556 2022-11-02 06:21:02.120318 smartdict-0.0.5/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)     2284 2022-11-02 06:20:42.000000 smartdict-0.0.5/README.md
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2022-11-02 06:21:02.120438 smartdict-0.0.5/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      591 2022-11-02 06:20:54.000000 smartdict-0.0.5/setup.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2022-11-02 06:21:02.119615 smartdict-0.0.5/smartdict/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       89 2022-10-20 00:56:59.000000 smartdict-0.0.5/smartdict/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     4590 2022-11-01 12:33:12.000000 smartdict-0.0.5/smartdict/dict_compiler.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2022-11-02 06:21:02.120177 smartdict-0.0.5/smartdict.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     2556 2022-11-02 06:21:02.000000 smartdict-0.0.5/smartdict.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      199 2022-11-02 06:21:02.000000 smartdict-0.0.5/smartdict.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2022-11-02 06:21:02.000000 smartdict-0.0.5/smartdict.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       10 2022-11-02 06:21:02.000000 smartdict-0.0.5/smartdict.egg-info/top_level.txt
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-21 15:01:21.966395 smartdict-0.0.6/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     2556 2023-05-21 15:01:21.966298 smartdict-0.0.6/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     2284 2022-11-02 06:20:42.000000 smartdict-0.0.6/README.md
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-05-21 15:01:21.966423 smartdict-0.0.6/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      591 2023-05-21 15:01:08.000000 smartdict-0.0.6/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-21 15:01:21.965734 smartdict-0.0.6/smartdict/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       89 2022-10-20 00:56:59.000000 smartdict-0.0.6/smartdict/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     4606 2023-05-21 15:01:03.000000 smartdict-0.0.6/smartdict/dict_compiler.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-21 15:01:21.966148 smartdict-0.0.6/smartdict.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     2556 2023-05-21 15:01:21.000000 smartdict-0.0.6/smartdict.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      199 2023-05-21 15:01:21.000000 smartdict-0.0.6/smartdict.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-05-21 15:01:21.000000 smartdict-0.0.6/smartdict.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       10 2023-05-21 15:01:21.000000 smartdict-0.0.6/smartdict.egg-info/top_level.txt
```

### Comparing `smartdict-0.0.5/PKG-INFO` & `smartdict-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdict
-Version: 0.0.5
+Version: 0.0.6
 Summary: a string-based refdict
 Home-page: https://github.com/Jyonn/SmartDict
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: dict,refer
 Platform: any
```

### Comparing `smartdict-0.0.5/README.md` & `smartdict-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `smartdict-0.0.5/setup.py` & `smartdict-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='smartdict',
-    version='0.0.5',
+    version='0.0.6',
     keywords=['dict', 'refer'],
     description='a string-based refdict',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/SmartDict',
     author='Jyonn Liu',
```

### Comparing `smartdict-0.0.5/smartdict/dict_compiler.py` & `smartdict-0.0.6/smartdict/dict_compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     def _process_item(self, path: str, s: str):
         if not isinstance(s, str):
             return s
 
         if path in self.circle:
             v = self.circle[path]
             if isinstance(v, self.InCircle):
-                raise ValueError('Dict references are in circle')
+                raise ValueError(f'Dict references are in circle, path = {path}')
             return v
 
         full_value = self._process_full_ref(path, s)
         if full_value is not self.NotFound:
             return full_value
 
         refs = self._get_refs(s)
```

### Comparing `smartdict-0.0.5/smartdict.egg-info/PKG-INFO` & `smartdict-0.0.6/smartdict.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdict
-Version: 0.0.5
+Version: 0.0.6
 Summary: a string-based refdict
 Home-page: https://github.com/Jyonn/SmartDict
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: dict,refer
 Platform: any
```

