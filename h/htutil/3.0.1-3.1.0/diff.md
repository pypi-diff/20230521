# Comparing `tmp/htutil-3.0.1.tar.gz` & `tmp/htutil-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/htutil/htutil/dist/.tmp-viilr2b8/htutil-3.0.1.tar", last modified: Tue May  9 07:16:38 2023, max compression
+gzip compressed data, was "/home/runner/work/htutil/htutil/dist/.tmp-5oj0ya71/htutil-3.1.0.tar", last modified: Sun May 21 03:04:20 2023, max compression
```

## Comparing `htutil-3.0.1.tar` & `htutil-3.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:16:38.000000 htutil-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-09 07:16:26.000000 htutil-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-09 07:16:38.000000 htutil-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-09 07:16:26.000000 htutil-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:16:26.000000 htutil-3.0.1/htutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-09 07:16:26.000000 htutil-3.0.1/htutil/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-09 07:16:26.000000 htutil-3.0.1/htutil/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-09 07:16:26.000000 htutil-3.0.1/htutil/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:16:38.000000 htutil-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-09 07:16:26.000000 htutil-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:04:20.000000 htutil-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-21 03:04:08.000000 htutil-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-21 03:04:20.000000 htutil-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-21 03:04:08.000000 htutil-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 03:04:08.000000 htutil-3.1.0/htutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-21 03:04:08.000000 htutil-3.1.0/htutil/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-21 03:04:08.000000 htutil-3.1.0/htutil/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-21 03:04:08.000000 htutil-3.1.0/htutil/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 03:04:20.000000 htutil-3.1.0/htutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 03:04:20.000000 htutil-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-21 03:04:08.000000 htutil-3.1.0/setup.py
```

### Comparing `htutil-3.0.1/LICENSE` & `htutil-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htutil-3.0.1/PKG-INFO` & `htutil-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htutil
-Version: 3.0.1
+Version: 3.1.0
 Summary: HaoTian's Python Util
 Home-page: https://github.com/117503445/htutil
 Author: 117503445
 Author-email: t117503445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `htutil-3.0.1/README.md` & `htutil-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `htutil-3.0.1/htutil/cache.py` & `htutil-3.1.0/htutil/cache.py`

 * *Files identical despite different names*

### Comparing `htutil-3.0.1/htutil/file.py` & `htutil-3.1.0/htutil/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 def read_pkl(path: str| Path):
     with open(path, 'rb') as f:
         result = pkl.load(f)
     return result
 
 
 def write_json(path: str| Path, content, indent=4) -> None:
-    write_text(path, json.dumps(content, indent=indent, ensure_ascii=False))
+    write_text(path, json.dumps(content, indent=indent, ensure_ascii=False, default=lambda x: x.__dict__))
 
 
 def read_json(path: str| Path):
     return json.loads(read_text(path))
 
 
 def main():
```

### Comparing `htutil-3.0.1/htutil.egg-info/PKG-INFO` & `htutil-3.1.0/htutil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htutil
-Version: 3.0.1
+Version: 3.1.0
 Summary: HaoTian's Python Util
 Home-page: https://github.com/117503445/htutil
 Author: 117503445
 Author-email: t117503445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `htutil-3.0.1/setup.py` & `htutil-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="htutil",
-    version="3.0.1",
+    version="3.1.0",
     author="117503445",
     author_email="t117503445@gmail.com",
     description="HaoTian's Python Util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/117503445/htutil",
     packages=setuptools.find_packages(),
```

