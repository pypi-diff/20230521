# Comparing `tmp/pteropy-0.1.7.tar.gz` & `tmp/pteropy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pteropy-0.1.7.tar", last modified: Sun Apr  9 13:34:00 2023, max compression
+gzip compressed data, was "pteropy-0.1.8.tar", last modified: Sun May 21 09:12:25 2023, max compression
```

## Comparing `pteropy-0.1.7.tar` & `pteropy-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 13:34:00.773383 pteropy-0.1.7/
--rw-rw-rw-   0        0        0     1083 2023-04-04 14:05:48.000000 pteropy-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     2778 2023-04-09 13:34:00.769214 pteropy-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2308 2023-04-09 13:33:36.000000 pteropy-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 13:34:00.740185 pteropy-0.1.7/pteropy/
--rw-rw-rw-   0        0        0    10648 2023-04-09 13:27:29.000000 pteropy-0.1.7/pteropy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:34:00.765214 pteropy-0.1.7/pteropy.egg-info/
--rw-rw-rw-   0        0        0     2778 2023-04-09 13:34:00.000000 pteropy-0.1.7/pteropy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-04-09 13:34:00.000000 pteropy-0.1.7/pteropy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 13:34:00.000000 pteropy-0.1.7/pteropy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-09 13:34:00.000000 pteropy-0.1.7/pteropy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 13:34:00.774377 pteropy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-04-09 13:26:15.000000 pteropy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:12:25.121054 pteropy-0.1.8/
+-rw-rw-rw-   0        0        0     1083 2023-04-04 14:05:48.000000 pteropy-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2778 2023-05-21 09:12:25.114867 pteropy-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2308 2023-04-09 13:33:36.000000 pteropy-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 09:12:25.086803 pteropy-0.1.8/pteropy/
+-rw-rw-rw-   0        0        0     7477 2023-05-21 09:11:42.000000 pteropy-0.1.8/pteropy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:12:25.109860 pteropy-0.1.8/pteropy.egg-info/
+-rw-rw-rw-   0        0        0     2778 2023-05-21 09:12:24.000000 pteropy-0.1.8/pteropy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-05-21 09:12:24.000000 pteropy-0.1.8/pteropy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 09:12:24.000000 pteropy-0.1.8/pteropy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 09:12:24.000000 pteropy-0.1.8/pteropy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 09:12:25.122074 pteropy-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-05-21 09:12:14.000000 pteropy-0.1.8/setup.py
```

### Comparing `pteropy-0.1.7/LICENSE` & `pteropy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pteropy-0.1.7/PKG-INFO` & `pteropy-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pteropy
-Version: 0.1.7
+Version: 0.1.8
 Summary: 簡單存取Pterodactyl api
 Home-page: https://github.com/HansHans135/pteropy
 Author: Hans
 Author-email: ccoccc14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pteropy-0.1.7/README.md` & `pteropy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pteropy-0.1.7/pteropy.egg-info/PKG-INFO` & `pteropy-0.1.8/pteropy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pteropy
-Version: 0.1.7
+Version: 0.1.8
 Summary: 簡單存取Pterodactyl api
 Home-page: https://github.com/HansHans135/pteropy
 Author: Hans
 Author-email: ccoccc14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

