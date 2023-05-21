# Comparing `tmp/tiktokget-1.0.3.tar.gz` & `tmp/tiktokget-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktokget-1.0.3.tar", last modified: Wed Mar 22 06:22:42 2023, max compression
+gzip compressed data, was "tiktokget-1.0.4.tar", last modified: Sun May 21 00:45:59 2023, max compression
```

## Comparing `tiktokget-1.0.3.tar` & `tiktokget-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-22 06:22:42.944107 tiktokget-1.0.3/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1458 2022-11-28 03:26:45.000000 tiktokget-1.0.3/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)       30 2021-01-23 07:23:28.000000 tiktokget-1.0.3/MANIFEST.in
--rw-rw-r--   0 rob       (1000) rob       (1000)     1256 2023-03-22 06:22:42.944107 tiktokget-1.0.3/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      942 2023-03-22 06:21:21.000000 tiktokget-1.0.3/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-22 06:22:42.940107 tiktokget-1.0.3/bin/
--rwxr-xr-x   0 rob       (1000) rob       (1000)     6676 2023-03-22 06:20:06.000000 tiktokget-1.0.3/bin/tiktokget
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-03-22 06:22:42.944107 tiktokget-1.0.3/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)      531 2023-03-22 06:22:30.000000 tiktokget-1.0.3/setup.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-03-22 06:22:42.944107 tiktokget-1.0.3/tiktokget.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1256 2023-03-22 06:22:42.000000 tiktokget-1.0.3/tiktokget.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      216 2023-03-22 06:22:42.000000 tiktokget-1.0.3/tiktokget.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-03-22 06:22:42.000000 tiktokget-1.0.3/tiktokget.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       25 2023-03-22 06:22:42.000000 tiktokget-1.0.3/tiktokget.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-03-22 06:22:42.000000 tiktokget-1.0.3/tiktokget.egg-info/top_level.txt
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-21 00:45:59.205393 tiktokget-1.0.4/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1458 2022-11-28 03:26:45.000000 tiktokget-1.0.4/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)       30 2021-01-23 07:23:28.000000 tiktokget-1.0.4/MANIFEST.in
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1682 2023-05-21 00:45:59.205393 tiktokget-1.0.4/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1368 2023-05-21 00:43:39.000000 tiktokget-1.0.4/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-21 00:45:59.201393 tiktokget-1.0.4/bin/
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     4955 2023-05-21 00:43:29.000000 tiktokget-1.0.4/bin/tiktokget
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-21 00:45:59.205393 tiktokget-1.0.4/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)      531 2023-05-21 00:45:47.000000 tiktokget-1.0.4/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-21 00:45:59.205393 tiktokget-1.0.4/tiktokget.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1682 2023-05-21 00:45:59.000000 tiktokget-1.0.4/tiktokget.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      216 2023-05-21 00:45:59.000000 tiktokget-1.0.4/tiktokget.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-21 00:45:59.000000 tiktokget-1.0.4/tiktokget.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       25 2023-05-21 00:45:59.000000 tiktokget-1.0.4/tiktokget.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-21 00:45:59.000000 tiktokget-1.0.4/tiktokget.egg-info/top_level.txt
```

### Comparing `tiktokget-1.0.3/LICENSE` & `tiktokget-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktokget-1.0.3/setup.py` & `tiktokget-1.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tiktokget',
-    version='1.0.3',
+    version='1.0.4',
     author='github.com/charmparticle',
     scripts=['bin/tiktokget'],
     url='https://github.com/charmparticle/tiktokget',
     license='BSD 3-Clause License',
     description='A tiktok getter.',
     long_description=open('README.md').read(),
     install_requires=[
```

