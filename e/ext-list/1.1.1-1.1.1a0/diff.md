# Comparing `tmp/ext-list-1.1.1.tar.gz` & `tmp/ext-list-1.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ext-list-1.1.1.tar", last modified: Sun May 21 17:57:00 2023, max compression
+gzip compressed data, was "ext-list-1.1.1a0.tar", last modified: Sun May 21 17:53:22 2023, max compression
```

## Comparing `ext-list-1.1.1.tar` & `ext-list-1.1.1a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:57:00.740163 ext-list-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-03-28 13:29:21.000000 ext-list-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4448 2023-05-21 17:57:00.737162 ext-list-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3326 2023-05-16 13:02:45.000000 ext-list-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:57:00.655892 ext-list-1.1.1/ext_list/
--rwxr-xr-x   0 root         (0) root         (0)    33983 2023-05-21 17:55:18.000000 ext-list-1.1.1/ext_list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-05-21 15:32:55.000000 ext-list-1.1.1/ext_list/base.py
--rw-r--r--   0 root         (0) root         (0)     7947 2023-05-21 17:55:18.000000 ext-list-1.1.1/ext_list/dict_operations.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-05-21 17:55:18.000000 ext-list-1.1.1/ext_list/list_operations.py
--rw-r--r--   0 root         (0) root         (0)     6559 2023-05-21 17:55:18.000000 ext-list-1.1.1/ext_list/operator_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:57:00.721934 ext-list-1.1.1/ext_list.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4448 2023-05-21 17:57:00.000000 ext-list-1.1.1/ext_list.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-21 17:57:00.000000 ext-list-1.1.1/ext_list.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 17:57:00.000000 ext-list-1.1.1/ext_list.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-21 17:57:00.000000 ext-list-1.1.1/ext_list.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-21 17:57:00.000000 ext-list-1.1.1/ext_list.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 17:57:00.740667 ext-list-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1464 2023-05-21 17:54:28.000000 ext-list-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:53:22.010778 ext-list-1.1.1a0/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-03-28 13:29:21.000000 ext-list-1.1.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4450 2023-05-21 17:53:22.010061 ext-list-1.1.1a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3326 2023-05-16 13:02:45.000000 ext-list-1.1.1a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:53:21.947446 ext-list-1.1.1a0/ext_list/
+-rwxr-xr-x   0 root         (0) root         (0)    33983 2023-05-21 17:32:49.000000 ext-list-1.1.1a0/ext_list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-21 15:32:55.000000 ext-list-1.1.1a0/ext_list/base.py
+-rw-r--r--   0 root         (0) root         (0)     7947 2023-05-21 17:32:49.000000 ext-list-1.1.1a0/ext_list/dict_operations.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-05-21 17:32:49.000000 ext-list-1.1.1a0/ext_list/list_operations.py
+-rw-r--r--   0 root         (0) root         (0)     6559 2023-05-21 17:32:49.000000 ext-list-1.1.1a0/ext_list/operator_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 17:53:22.001906 ext-list-1.1.1a0/ext_list.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4450 2023-05-21 17:53:21.000000 ext-list-1.1.1a0/ext_list.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-21 17:53:21.000000 ext-list-1.1.1a0/ext_list.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 17:53:21.000000 ext-list-1.1.1a0/ext_list.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-21 17:53:21.000000 ext-list-1.1.1a0/ext_list.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-21 17:53:21.000000 ext-list-1.1.1a0/ext_list.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 17:53:22.011783 ext-list-1.1.1a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-05-21 17:46:19.000000 ext-list-1.1.1a0/setup.py
```

### Comparing `ext-list-1.1.1/LICENSE` & `ext-list-1.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ext-list-1.1.1/PKG-INFO` & `ext-list-1.1.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ext-list
-Version: 1.1.1
+Version: 1.1.1a0
 Summary: This is a utility library that extends Python's list operations.
 Home-page: https://github.com/sk-guritech/ext-list
 Author: Sakaguchi Ryo
 Author-email: sakaguchi@sk-techfirm.com
 Project-URL: Bug Tracker, https://github.com/sk-guritech/ext-list/issues
 Keywords: list,comprehension,iterable,code quality
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `ext-list-1.1.1/README.md` & `ext-list-1.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `ext-list-1.1.1/ext_list/__init__.py` & `ext-list-1.1.1a0/ext_list/__init__.py`

 * *Files identical despite different names*

### Comparing `ext-list-1.1.1/ext_list/base.py` & `ext-list-1.1.1a0/ext_list/base.py`

 * *Files identical despite different names*

### Comparing `ext-list-1.1.1/ext_list/dict_operations.py` & `ext-list-1.1.1a0/ext_list/dict_operations.py`

 * *Files identical despite different names*

### Comparing `ext-list-1.1.1/ext_list/list_operations.py` & `ext-list-1.1.1a0/ext_list/list_operations.py`

 * *Files identical despite different names*

### Comparing `ext-list-1.1.1/ext_list/operator_operations.py` & `ext-list-1.1.1a0/ext_list/operator_operations.py`

 * *Files identical despite different names*

### Comparing `ext-list-1.1.1/ext_list.egg-info/PKG-INFO` & `ext-list-1.1.1a0/ext_list.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ext-list
-Version: 1.1.1
+Version: 1.1.1a0
 Summary: This is a utility library that extends Python's list operations.
 Home-page: https://github.com/sk-guritech/ext-list
 Author: Sakaguchi Ryo
 Author-email: sakaguchi@sk-techfirm.com
 Project-URL: Bug Tracker, https://github.com/sk-guritech/ext-list/issues
 Keywords: list,comprehension,iterable,code quality
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `ext-list-1.1.1/setup.py` & `ext-list-1.1.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_md:
     long_description = readme_md.read()
 
 setup(
     name='ext-list',
-    version='1.1.1',
+    version='1.1.1a',
     author='Sakaguchi Ryo',
     author_email='sakaguchi@sk-techfirm.com',
     description='This is a utility library that extends Python\'s list operations.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sk-guritech/ext-list',
     project_urls={
```

