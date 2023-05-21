# Comparing `tmp/leuci-xyz-0.0.8.tar.gz` & `tmp/leuci-xyz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leuci-xyz-0.0.8.tar", last modified: Tue Feb 28 17:02:38 2023, max compression
+gzip compressed data, was "leuci-xyz-0.0.9.tar", last modified: Mon Mar  6 07:11:46 2023, max compression
```

## Comparing `leuci-xyz-0.0.8.tar` & `leuci-xyz-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-02-28 17:02:38.322676 leuci-xyz-0.0.8/
--rw-r--r--   0 rachel    (1000) rachel    (1000)      777 2023-02-28 17:02:38.322676 leuci-xyz-0.0.8/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)      296 2023-02-27 11:01:25.000000 leuci-xyz-0.0.8/README.md
--rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-xyz-0.0.8/pyproject.toml
--rw-r--r--   0 rachel    (1000) rachel    (1000)      628 2023-02-28 17:02:38.322676 leuci-xyz-0.0.8/setup.cfg
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-02-28 17:02:38.322676 leuci-xyz-0.0.8/src/
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-02-28 17:02:38.322676 leuci-xyz-0.0.8/src/leuci_xyz/
--rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-xyz-0.0.8/src/leuci_xyz/__init__.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)      909 2023-02-28 12:52:09.000000 leuci-xyz-0.0.8/src/leuci_xyz/axestransform.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     6075 2023-02-28 17:01:44.000000 leuci-xyz-0.0.8/src/leuci_xyz/crstransform.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)      660 2023-02-27 17:42:08.000000 leuci-xyz-0.0.8/src/leuci_xyz/gridmaker.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     4171 2023-02-28 15:43:34.000000 leuci-xyz-0.0.8/src/leuci_xyz/matrixthree.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)    10120 2023-02-28 16:34:51.000000 leuci-xyz-0.0.8/src/leuci_xyz/spacetransform.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     3463 2023-02-28 15:42:37.000000 leuci-xyz-0.0.8/src/leuci_xyz/vectorthree.py
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-02-28 17:02:38.322676 leuci-xyz-0.0.8/src/leuci_xyz.egg-info/
--rw-r--r--   0 rachel    (1000) rachel    (1000)      777 2023-02-28 17:02:38.000000 leuci-xyz-0.0.8/src/leuci_xyz.egg-info/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)      386 2023-02-28 17:02:38.000000 leuci-xyz-0.0.8/src/leuci_xyz.egg-info/SOURCES.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-02-28 17:02:38.000000 leuci-xyz-0.0.8/src/leuci_xyz.egg-info/dependency_links.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-02-28 17:02:38.000000 leuci-xyz-0.0.8/src/leuci_xyz.egg-info/top_level.txt
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-03-06 07:11:45.988424 leuci-xyz-0.0.9/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      777 2023-03-06 07:11:45.988424 leuci-xyz-0.0.9/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      296 2023-02-27 11:01:25.000000 leuci-xyz-0.0.9/README.md
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-xyz-0.0.9/pyproject.toml
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      628 2023-03-06 07:11:45.998424 leuci-xyz-0.0.9/setup.cfg
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-03-06 07:11:45.988424 leuci-xyz-0.0.9/src/
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-03-06 07:11:45.988424 leuci-xyz-0.0.9/src/leuci_xyz/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-xyz-0.0.9/src/leuci_xyz/__init__.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      909 2023-02-28 12:52:09.000000 leuci-xyz-0.0.9/src/leuci_xyz/axestransform.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     6107 2023-03-06 07:09:47.000000 leuci-xyz-0.0.9/src/leuci_xyz/crstransform.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      659 2023-03-01 11:09:37.000000 leuci-xyz-0.0.9/src/leuci_xyz/gridmaker.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     6176 2023-03-06 07:08:40.000000 leuci-xyz-0.0.9/src/leuci_xyz/matrixthree.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    10120 2023-02-28 16:34:51.000000 leuci-xyz-0.0.9/src/leuci_xyz/spacetransform.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     3584 2023-03-05 16:06:12.000000 leuci-xyz-0.0.9/src/leuci_xyz/vectorthree.py
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-03-06 07:11:45.988424 leuci-xyz-0.0.9/src/leuci_xyz.egg-info/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      777 2023-03-06 07:11:45.000000 leuci-xyz-0.0.9/src/leuci_xyz.egg-info/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      386 2023-03-06 07:11:45.000000 leuci-xyz-0.0.9/src/leuci_xyz.egg-info/SOURCES.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-03-06 07:11:45.000000 leuci-xyz-0.0.9/src/leuci_xyz.egg-info/dependency_links.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-03-06 07:11:45.000000 leuci-xyz-0.0.9/src/leuci_xyz.egg-info/top_level.txt
```

### Comparing `leuci-xyz-0.0.8/PKG-INFO` & `leuci-xyz-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-xyz
-Version: 0.0.8
+Version: 0.0.9
 Summary: objects in 3d space library
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `leuci-xyz-0.0.8/setup.cfg` & `leuci-xyz-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = leuci-xyz
-version = 0.0.8
+version = 0.0.9
 author = Rachel Alcraft
 author_email = rachelalcraft@gmail.com
 description = objects in 3d space library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `leuci-xyz-0.0.8/src/leuci_xyz/axestransform.py` & `leuci-xyz-0.0.9/src/leuci_xyz/axestransform.py`

 * *Files identical despite different names*

### Comparing `leuci-xyz-0.0.8/src/leuci_xyz/crstransform.py` & `leuci-xyz-0.0.9/src/leuci_xyz/crstransform.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 class CrsTransform(object):
     def __init__(self,  dim_order,
                         crs_starts,
                         axis_sampling,
                         map2crs,
                         cell_dims,
-                        angles):
+                        angles                        ):
         
         self.M_PI = 3.14159265358979323846
-
+        
         # PUBLIC INTERFACE
         self.dim_order = dim_order
         self.crs_starts = crs_starts
         self.axis_sampling = axis_sampling        
         self.map2crs = map2crs
         self.cell_dims = cell_dims
         self.angles = angles
```

### Comparing `leuci-xyz-0.0.8/src/leuci_xyz/gridmaker.py` & `leuci-xyz-0.0.9/src/leuci_xyz/gridmaker.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,13 +18,12 @@
         coords = []
         for i in range(samples):
             row = []            
             for j in range(samples):
                 row.append(((i-offset)*gap,(j-offset)*gap))
             coords.append(row)        
         return coords
-                        
-
 
-
-        
+    
+    
+
```

### Comparing `leuci-xyz-0.0.8/src/leuci_xyz/spacetransform.py` & `leuci-xyz-0.0.9/src/leuci_xyz/spacetransform.py`

 * *Files identical despite different names*

### Comparing `leuci-xyz-0.0.8/src/leuci_xyz/vectorthree.py` & `leuci-xyz-0.0.9/src/leuci_xyz/vectorthree.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """
 RSA 25/2/23
 
 This class handles 3d vectors
 """
 
 import math
+import numpy
 
 # class interface
 
 class VectorThree(object):
     def __init__(self, a=0,b=0,c=0):    
         self.A = a
         self.B = b
         self.C = c        
         self.Valid = True
+        self.npy = numpy.zeros((3))
+        self.npy[0] = a
+        self.npy[1] = b
+        self.npy[2] = c
 
     def from_coords(self, coords):    
         coords = coords.strip()
         if coords[0] == "(":
             coords = coords[1:]
         if coords[-1] == ")":
             coords = coords[:-1]
```

### Comparing `leuci-xyz-0.0.8/src/leuci_xyz.egg-info/PKG-INFO` & `leuci-xyz-0.0.9/src/leuci_xyz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-xyz
-Version: 0.0.8
+Version: 0.0.9
 Summary: objects in 3d space library
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

