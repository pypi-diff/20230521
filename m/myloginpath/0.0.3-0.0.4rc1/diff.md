# Comparing `tmp/myloginpath-0.0.3.tar.gz` & `tmp/myloginpath-0.0.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myloginpath-0.0.3.tar", last modified: Wed Sep 15 07:48:47 2021, max compression
+gzip compressed data, was "myloginpath-0.0.4rc1.tar", last modified: Sun May 21 10:07:53 2023, max compression
```

## Comparing `myloginpath-0.0.3.tar` & `myloginpath-0.0.4rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2021-09-15 07:48:47.190509 myloginpath-0.0.3/
--rw-r--r--   0 inada-n    (502) staff       (20)       31 2018-05-08 09:21:49.000000 myloginpath-0.0.3/AUTHORS
--rw-r--r--   0 inada-n    (502) staff       (20)     1068 2018-05-08 09:19:28.000000 myloginpath-0.0.3/LICENSE.txt
--rw-r--r--   0 inada-n    (502) staff       (20)      950 2021-09-15 07:48:47.190065 myloginpath-0.0.3/PKG-INFO
--rw-r--r--   0 inada-n    (502) staff       (20)      645 2018-05-08 10:57:00.000000 myloginpath-0.0.3/README.md
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2021-09-15 07:48:47.188522 myloginpath-0.0.3/myloginpath.egg-info/
--rw-r--r--   0 inada-n    (502) staff       (20)      950 2021-09-15 07:48:47.000000 myloginpath-0.0.3/myloginpath.egg-info/PKG-INFO
--rw-r--r--   0 inada-n    (502) staff       (20)      267 2021-09-15 07:48:47.000000 myloginpath-0.0.3/myloginpath.egg-info/SOURCES.txt
--rw-r--r--   0 inada-n    (502) staff       (20)        1 2021-09-15 07:48:47.000000 myloginpath-0.0.3/myloginpath.egg-info/dependency_links.txt
--rw-r--r--   0 inada-n    (502) staff       (20)       13 2021-09-15 07:48:47.000000 myloginpath-0.0.3/myloginpath.egg-info/requires.txt
--rw-r--r--   0 inada-n    (502) staff       (20)       12 2021-09-15 07:48:47.000000 myloginpath-0.0.3/myloginpath.egg-info/top_level.txt
--rw-r--r--   0 inada-n    (502) staff       (20)     3867 2021-09-09 07:34:55.000000 myloginpath-0.0.3/myloginpath.py
--rw-r--r--   0 inada-n    (502) staff       (20)       38 2021-09-15 07:48:47.190642 myloginpath-0.0.3/setup.cfg
--rw-r--r--   0 inada-n    (502) staff       (20)      474 2021-09-15 07:46:57.000000 myloginpath-0.0.3/setup.py
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2021-09-15 07:48:47.189441 myloginpath-0.0.3/test/
--rw-r--r--   0 inada-n    (502) staff       (20)      716 2021-09-09 07:34:55.000000 myloginpath-0.0.3/test/test_decrypt.py
--rw-r--r--   0 inada-n    (502) staff       (20)      826 2021-09-09 07:34:55.000000 myloginpath-0.0.3/test/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:53.839763 myloginpath-0.0.4rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-21 10:07:53.839763 myloginpath-0.0.4rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:53.839763 myloginpath-0.0.4rc1/myloginpath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-21 10:07:53.000000 myloginpath-0.0.4rc1/myloginpath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-21 10:07:53.000000 myloginpath-0.0.4rc1/myloginpath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 10:07:53.000000 myloginpath-0.0.4rc1/myloginpath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 10:07:53.000000 myloginpath-0.0.4rc1/myloginpath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 10:07:53.000000 myloginpath-0.0.4rc1/myloginpath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/myloginpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 10:07:53.839763 myloginpath-0.0.4rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:53.839763 myloginpath-0.0.4rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/test/test_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-21 10:07:31.000000 myloginpath-0.0.4rc1/test/test_parse.py
```

### Comparing `myloginpath-0.0.3/LICENSE.txt` & `myloginpath-0.0.4rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `myloginpath-0.0.3/README.md` & `myloginpath-0.0.4rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 
 Use it from Python:
 
 ```python
 import myloginpath, MySQLdb
 conf = myloginpath.parse('client')
 print(conf)  # {'host': 'localhost', 'user': 'localuser', 'password': 'secretstring'}
-conn = MySQLdb.connect(**conf, db="myapp")
+conn = MySQLdb.connect(**conf, database="myapp")
 ```
```

### Comparing `myloginpath-0.0.3/myloginpath.py` & `myloginpath-0.0.4rc1/myloginpath.py`

 * *Files identical despite different names*

### Comparing `myloginpath-0.0.3/test/test_decrypt.py` & `myloginpath-0.0.4rc1/test/test_decrypt.py`

 * *Files identical despite different names*

### Comparing `myloginpath-0.0.3/test/test_parse.py` & `myloginpath-0.0.4rc1/test/test_parse.py`

 * *Files identical despite different names*

