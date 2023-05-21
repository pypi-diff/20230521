# Comparing `tmp/cm2py-0.0.3.tar.gz` & `tmp/cm2py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.0.3.tar", last modified: Sat May  6 12:31:06 2023, max compression
+gzip compressed data, was "cm2py-0.1.0.tar", last modified: Sun May 21 06:02:21 2023, max compression
```

## Comparing `cm2py-0.0.3.tar` & `cm2py-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 12:31:06.416536 cm2py-0.0.3/
--rw-rw-rw-   0        0        0    35921 2023-05-06 09:53:00.000000 cm2py-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    43012 2023-05-06 12:31:06.415786 cm2py-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1087 2023-05-06 10:42:35.000000 cm2py-0.0.3/README.md
--rw-rw-rw-   0        0        0      709 2023-05-06 12:30:49.000000 cm2py-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 12:31:06.416536 cm2py-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 12:31:06.374385 cm2py-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 12:31:06.388247 cm2py-0.0.3/src/cm2py/
--rw-rw-rw-   0        0        0      149 2023-05-06 12:25:04.000000 cm2py-0.0.3/src/cm2py/__init__.py
--rw-rw-rw-   0        0        0     4207 2023-05-06 12:30:46.000000 cm2py-0.0.3/src/cm2py/cm2py.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:31:06.412037 cm2py-0.0.3/src/cm2py.egg-info/
--rw-rw-rw-   0        0        0    43012 2023-05-06 12:31:06.000000 cm2py-0.0.3/src/cm2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-06 12:31:06.000000 cm2py-0.0.3/src/cm2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 12:31:06.000000 cm2py-0.0.3/src/cm2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-06 12:31:06.000000 cm2py-0.0.3/src/cm2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-06 12:31:06.000000 cm2py-0.0.3/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 06:02:21.295195 cm2py-0.1.0/
+-rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3012 2023-05-21 06:02:21.294191 cm2py-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1189 2023-05-09 09:48:28.000000 cm2py-0.1.0/README.md
+-rw-rw-rw-   0        0        0      687 2023-05-21 06:01:41.000000 cm2py-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 06:02:21.296192 cm2py-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 06:02:21.233193 cm2py-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 06:02:21.253189 cm2py-0.1.0/src/cm2py/
+-rw-rw-rw-   0        0        0      213 2023-05-21 06:01:41.000000 cm2py-0.1.0/src/cm2py/__init__.py
+-rw-rw-rw-   0        0        0     5804 2023-05-21 06:01:41.000000 cm2py-0.1.0/src/cm2py/cm2py.py
+drwxrwxrwx   0        0        0        0 2023-05-21 06:02:21.288198 cm2py-0.1.0/src/cm2py.egg-info/
+-rw-rw-rw-   0        0        0     3012 2023-05-21 06:02:21.000000 cm2py-0.1.0/src/cm2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-05-21 06:02:21.000000 cm2py-0.1.0/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 06:02:21.000000 cm2py-0.1.0/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-21 06:02:21.000000 cm2py-0.1.0/src/cm2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-21 06:02:21.000000 cm2py-0.1.0/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 06:02:21.290189 cm2py-0.1.0/tests/
+-rw-rw-rw-   0        0        0     1525 2023-05-21 06:01:41.000000 cm2py-0.1.0/tests/test_app.py
```

### Comparing `cm2py-0.0.3/README.md` & `cm2py-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,32 +13,35 @@
 ## Usage
 
 Basic program to generate a line of 8 looping OR gates:
 
 ```python
 import cm2py as cm2
 
+length = 8
+
 save = cm2.save()
 
 blocks = []
 
-for i in range(8):
+for i in range(length):
     blocks.append(save.addBlock(cm2.OR, (i, 0, 0)))
 
 ### Commented out for clarity. 
 ### You should store connections in a list if you want to modify them later.
 # connections = []  
 
-for i in range(8):
+for i in range(length):
     # connections.append(save.addConnection(blocks[i-1], blocks[i]))
     save.addConnection(blocks[i-1], blocks[i])  # Directly add the connections to the save object
 
-save.exportSave()
-
+saveString = save.exportSave()
+print(saveString)
 ```
+(from [the loop.py example](examples/loop.py))
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 ## License
```

### Comparing `cm2py-0.0.3/pyproject.toml` & `cm2py-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cm2py"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
-  { name="SKM GEK", email="qestudios17@gmail.com" },
+  { name="SKM GEEK", email="qestudios17@gmail.com" },
 ]
 description = "Circuit Maker 2 save generation and manipulation package"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+    "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "uuid",
+  "numpy"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/QEStudios/cm2py"
 "Bug Tracker" = "https://github.com/QEStudios/cm2py/issues"
```

