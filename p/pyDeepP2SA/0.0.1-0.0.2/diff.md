# Comparing `tmp/pyDeepP2SA-0.0.1.tar.gz` & `tmp/pyDeepP2SA-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDeepP2SA-0.0.1.tar", last modified: Fri May 19 15:59:50 2023, max compression
+gzip compressed data, was "pyDeepP2SA-0.0.2.tar", last modified: Sun May 21 03:07:32 2023, max compression
```

## Comparing `pyDeepP2SA-0.0.1.tar` & `pyDeepP2SA-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 15:59:50.974593 pyDeepP2SA-0.0.1/
--rw-rw-rw-   0        0        0      108 2023-05-17 08:19:42.000000 pyDeepP2SA-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-05-17 06:46:46.000000 pyDeepP2SA-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-05-17 07:18:28.000000 pyDeepP2SA-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      763 2023-05-19 15:59:50.958598 pyDeepP2SA-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-17 06:46:43.000000 pyDeepP2SA-0.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 15:59:50.982589 pyDeepP2SA-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1004 2023-05-19 15:56:58.000000 pyDeepP2SA-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 15:59:50.696603 pyDeepP2SA-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 15:59:50.958598 pyDeepP2SA-0.0.1/src/pyDeepP2SA.egg-info/
--rw-rw-rw-   0        0        0      763 2023-05-19 15:59:50.000000 pyDeepP2SA-0.0.1/src/pyDeepP2SA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-19 15:59:50.000000 pyDeepP2SA-0.0.1/src/pyDeepP2SA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 15:59:50.000000 pyDeepP2SA-0.0.1/src/pyDeepP2SA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-19 15:59:50.000000 pyDeepP2SA-0.0.1/src/pyDeepP2SA.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-19 15:59:50.000000 pyDeepP2SA-0.0.1/src/pyDeepP2SA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11374 2023-05-18 14:22:48.000000 pyDeepP2SA-0.0.1/src/pyDeepP2SA.py
+drwxrwxrwx   0        0        0        0 2023-05-21 03:07:32.181343 pyDeepP2SA-0.0.2/
+-rw-rw-rw-   0        0        0      108 2023-05-17 08:19:42.000000 pyDeepP2SA-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-05-17 06:46:46.000000 pyDeepP2SA-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-17 07:18:28.000000 pyDeepP2SA-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9366 2023-05-21 03:07:32.173324 pyDeepP2SA-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8575 2023-05-21 02:59:54.000000 pyDeepP2SA-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 03:07:32.181343 pyDeepP2SA-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2023-05-21 03:06:18.000000 pyDeepP2SA-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 03:07:31.944855 pyDeepP2SA-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 03:07:32.165327 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/
+-rw-rw-rw-   0        0        0     9366 2023-05-21 03:07:31.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-05-21 03:07:31.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 03:07:31.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-21 03:07:31.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-21 03:07:31.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11374 2023-05-18 14:22:48.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.py
```

### Comparing `pyDeepP2SA-0.0.1/LICENCE.txt` & `pyDeepP2SA-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pyDeepP2SA-0.0.1/setup.py` & `pyDeepP2SA-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     'matplotlib',
     'pandas',
     'seaborn'
 ]
 
 setup(
     name='pyDeepP2SA',
-    version='0.0.1',
+    version='0.0.2',
     description='A python package for particle size and shape analysis using deep learning',
     py_modules=["pyDeepP2SA"],
     package_dir={'': 'src'},
-    long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
-    url='',
+    long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
+    url='https://github.com/BrinthanK/pyDeepP2SA',
     author='Brinthan K',
     author_email='kanesalingambrinthan187@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='Particle shape analyser, PSD, Deep learning, Image processing, Circularity',
     install_requires=install_requires
     )
```

### Comparing `pyDeepP2SA-0.0.1/src/pyDeepP2SA.py` & `pyDeepP2SA-0.0.2/src/pyDeepP2SA.py`

 * *Files identical despite different names*

