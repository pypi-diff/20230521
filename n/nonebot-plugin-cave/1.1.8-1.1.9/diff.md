# Comparing `tmp/nonebot_plugin_cave-1.1.8.tar.gz` & `tmp/nonebot_plugin_cave-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cave-1.1.8.tar", last modified: Sat May  6 14:40:24 2023, max compression
+gzip compressed data, was "nonebot_plugin_cave-1.1.9.tar", last modified: Sun May 21 03:30:29 2023, max compression
```

## Comparing `nonebot_plugin_cave-1.1.8.tar` & `nonebot_plugin_cave-1.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 14:40:24.082627 nonebot_plugin_cave-1.1.8/
--rw-rw-rw-   0        0        0     1064 2022-12-29 13:25:04.000000 nonebot_plugin_cave-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     3264 2023-05-06 14:40:24.081626 nonebot_plugin_cave-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2847 2023-05-06 14:13:09.000000 nonebot_plugin_cave-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 14:40:24.068603 nonebot_plugin_cave-1.1.8/nonebot_plugin_cave/
--rw-rw-rw-   0        0        0    19263 2023-05-06 14:13:09.000000 nonebot_plugin_cave-1.1.8/nonebot_plugin_cave/__init__.py
--rw-rw-rw-   0        0        0    17736 2023-05-06 14:13:09.000000 nonebot_plugin_cave-1.1.8/nonebot_plugin_cave/data_source.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:40:24.077626 nonebot_plugin_cave-1.1.8/nonebot_plugin_cave.egg-info/
--rw-rw-rw-   0        0        0     3264 2023-05-06 14:40:23.000000 nonebot_plugin_cave-1.1.8/nonebot_plugin_cave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-06 14:40:23.000000 nonebot_plugin_cave-1.1.8/nonebot_plugin_cave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 14:40:23.000000 nonebot_plugin_cave-1.1.8/nonebot_plugin_cave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-06 14:40:23.000000 nonebot_plugin_cave-1.1.8/nonebot_plugin_cave.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 14:40:23.000000 nonebot_plugin_cave-1.1.8/nonebot_plugin_cave.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 14:40:24.082627 nonebot_plugin_cave-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      819 2023-05-06 14:39:25.000000 nonebot_plugin_cave-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 03:30:29.008601 nonebot_plugin_cave-1.1.9/
+-rw-rw-rw-   0        0        0     1064 2022-12-29 13:25:04.000000 nonebot_plugin_cave-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3264 2023-05-21 03:30:29.007601 nonebot_plugin_cave-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2847 2023-05-06 14:13:09.000000 nonebot_plugin_cave-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 03:30:28.985765 nonebot_plugin_cave-1.1.9/nonebot_plugin_cave/
+-rw-rw-rw-   0        0        0    19263 2023-05-06 14:13:09.000000 nonebot_plugin_cave-1.1.9/nonebot_plugin_cave/__init__.py
+-rw-rw-rw-   0        0        0    17736 2023-05-06 14:13:09.000000 nonebot_plugin_cave-1.1.9/nonebot_plugin_cave/data_source.py
+drwxrwxrwx   0        0        0        0 2023-05-21 03:30:29.005603 nonebot_plugin_cave-1.1.9/nonebot_plugin_cave.egg-info/
+-rw-rw-rw-   0        0        0     3264 2023-05-21 03:30:28.000000 nonebot_plugin_cave-1.1.9/nonebot_plugin_cave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-21 03:30:28.000000 nonebot_plugin_cave-1.1.9/nonebot_plugin_cave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 03:30:28.000000 nonebot_plugin_cave-1.1.9/nonebot_plugin_cave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-21 03:30:28.000000 nonebot_plugin_cave-1.1.9/nonebot_plugin_cave.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-21 03:30:28.000000 nonebot_plugin_cave-1.1.9/nonebot_plugin_cave.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 03:30:29.008601 nonebot_plugin_cave-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      819 2023-05-21 03:30:01.000000 nonebot_plugin_cave-1.1.9/setup.py
```

### Comparing `nonebot_plugin_cave-1.1.8/LICENSE` & `nonebot_plugin_cave-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cave-1.1.8/PKG-INFO` & `nonebot_plugin_cave-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_cave
-Version: 1.1.8
+Version: 1.1.9
 Summary: cave plugin in Nonebot2
 Home-page: https://github.com/hmzz804/nonebot_plugin_cave
 Author: hmzz804
 Author-email: 2166908863@qq.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot_plugin_cave-1.1.8/README.md` & `nonebot_plugin_cave-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cave-1.1.8/nonebot_plugin_cave/__init__.py` & `nonebot_plugin_cave-1.1.9/nonebot_plugin_cave/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cave-1.1.8/nonebot_plugin_cave/data_source.py` & `nonebot_plugin_cave-1.1.9/nonebot_plugin_cave/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cave-1.1.8/nonebot_plugin_cave.egg-info/PKG-INFO` & `nonebot_plugin_cave-1.1.9/nonebot_plugin_cave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cave
-Version: 1.1.8
+Version: 1.1.9
 Summary: cave plugin in Nonebot2
 Home-page: https://github.com/hmzz804/nonebot_plugin_cave
 Author: hmzz804
 Author-email: 2166908863@qq.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot_plugin_cave-1.1.8/setup.py` & `nonebot_plugin_cave-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf-8') as f:
   long_description = f.read()
 
 setuptools.setup(
     name='nonebot_plugin_cave',
-    version='1.1.8',
+    version='1.1.9',
     description='cave plugin in Nonebot2',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='hmzz804',
     author_email='2166908863@qq.com',
     url='https://github.com/hmzz804/nonebot_plugin_cave',
     install_requires=[
```

