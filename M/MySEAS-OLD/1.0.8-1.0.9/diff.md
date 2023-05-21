# Comparing `tmp/MySEAS_OLD-1.0.8.tar.gz` & `tmp/MySEAS_OLD-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MySEAS_OLD-1.0.8.tar", last modified: Fri Nov 18 09:12:48 2022, max compression
+gzip compressed data, was "MySEAS_OLD-1.0.9.tar", last modified: Sun May 21 09:25:54 2023, max compression
```

## Comparing `MySEAS_OLD-1.0.8.tar` & `MySEAS_OLD-1.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.073385 MySEAS_OLD-1.0.8/
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.055424 MySEAS_OLD-1.0.8/MySEAS_OLD.egg-info/
--rw-r--r--   0 Siggbo     (502) staff       (20)      656 2022-11-18 09:12:48.000000 MySEAS_OLD-1.0.8/MySEAS_OLD.egg-info/PKG-INFO
--rw-r--r--   0 Siggbo     (502) staff       (20)     1135 2022-11-18 09:12:48.000000 MySEAS_OLD-1.0.8/MySEAS_OLD.egg-info/SOURCES.txt
--rw-r--r--   0 Siggbo     (502) staff       (20)        1 2022-11-18 09:12:48.000000 MySEAS_OLD-1.0.8/MySEAS_OLD.egg-info/dependency_links.txt
--rw-r--r--   0 Siggbo     (502) staff       (20)        7 2022-11-18 09:12:48.000000 MySEAS_OLD-1.0.8/MySEAS_OLD.egg-info/requires.txt
--rw-r--r--   0 Siggbo     (502) staff       (20)        5 2022-11-18 09:12:48.000000 MySEAS_OLD-1.0.8/MySEAS_OLD.egg-info/top_level.txt
--rw-r--r--   0 Siggbo     (502) staff       (20)      656 2022-11-18 09:12:48.072984 MySEAS_OLD-1.0.8/PKG-INFO
--rw-r--r--   0 Siggbo     (502) staff       (20)      972 2022-11-17 15:22:36.000000 MySEAS_OLD-1.0.8/README.md
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.055918 MySEAS_OLD-1.0.8/SEAS/
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.056393 MySEAS_OLD-1.0.8/SEAS/Assets/
--rw-r--r--   0 Siggbo     (502) staff       (20)        0 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Assets/__init__.py
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.056731 MySEAS_OLD-1.0.8/SEAS/Engine/
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.061910 MySEAS_OLD-1.0.8/SEAS/Engine/Components/
--rw-r--r--   0 Siggbo     (502) staff       (20)      433 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Components/__init__.py
--rw-r--r--   0 Siggbo     (502) staff       (20)     2814 2022-11-17 14:47:24.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Components/characterPolyControllerComp.py
--rw-r--r--   0 Siggbo     (502) staff       (20)     6690 2022-11-14 12:12:51.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Components/collidePolyComp.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      505 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Components/gravityComp.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      580 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Components/hitboxPolyComp.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      419 2022-11-17 09:45:19.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Components/renderPolyComp.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      529 2022-11-17 09:45:26.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Components/renderRectComp.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      936 2022-11-11 09:31:17.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Components/transformPolyComp.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      269 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Components/transformRectComp.py
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.065391 MySEAS_OLD-1.0.8/SEAS/Engine/Core/
--rw-r--r--   0 Siggbo     (502) staff       (20)      110 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Core/__init__.py
--rw-r--r--   0 Siggbo     (502) staff       (20)     8690 2022-11-18 09:10:11.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Core/core.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      245 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Core/event.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      164 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Core/filePreset.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      459 2022-11-14 13:54:45.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Core/font.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      187 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Core/input.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      570 2022-11-15 12:19:41.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Core/screen.py
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.066523 MySEAS_OLD-1.0.8/SEAS/Engine/Game/
--rw-r--r--   0 Siggbo     (502) staff       (20)       35 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Game/__init__.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      289 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Game/run.py
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.069210 MySEAS_OLD-1.0.8/SEAS/Engine/Maths/
--rw-r--r--   0 Siggbo     (502) staff       (20)       38 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Maths/__init__.py
--rw-r--r--   0 Siggbo     (502) staff       (20)        0 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Maths/maths.py
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.070228 MySEAS_OLD-1.0.8/SEAS/Engine/Models/
--rw-r--r--   0 Siggbo     (502) staff       (20)       44 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Models/__init__.py
--rw-r--r--   0 Siggbo     (502) staff       (20)     1009 2022-11-15 12:16:01.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Models/emptyModel.py
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.071042 MySEAS_OLD-1.0.8/SEAS/Engine/Scene/
--rw-r--r--   0 Siggbo     (502) staff       (20)       38 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Scene/__init__.py
--rw-r--r--   0 Siggbo     (502) staff       (20)     7510 2022-11-18 09:02:44.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Scene/scene.py
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.072048 MySEAS_OLD-1.0.8/SEAS/Engine/Setup/
--rw-r--r--   0 Siggbo     (502) staff       (20)       44 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Setup/__init__.py
--rw-r--r--   0 Siggbo     (502) staff       (20)       28 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/Setup/pygameSetup.py
--rw-r--r--   0 Siggbo     (502) staff       (20)      202 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/Engine/__init__.py
-drwxr-xr-x   0 Siggbo     (502) staff       (20)        0 2022-11-18 09:12:48.072478 MySEAS_OLD-1.0.8/SEAS/UI/
--rw-r--r--   0 Siggbo     (502) staff       (20)        0 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/UI/__init__.py
--rw-r--r--   0 Siggbo     (502) staff       (20)       74 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.8/SEAS/__init__.py
--rw-r--r--   0 Siggbo     (502) staff       (20)       38 2022-11-18 09:12:48.073533 MySEAS_OLD-1.0.8/setup.cfg
--rw-r--r--   0 Siggbo     (502) staff       (20)     1136 2022-11-18 09:12:44.000000 MySEAS_OLD-1.0.8/setup.py
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.063363 MySEAS_OLD-1.0.9/
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.043314 MySEAS_OLD-1.0.9/MySEAS_OLD.egg-info/
+-rw-r--r--   0 primary    (502) staff       (20)      601 2023-05-21 09:25:53.000000 MySEAS_OLD-1.0.9/MySEAS_OLD.egg-info/PKG-INFO
+-rw-r--r--   0 primary    (502) staff       (20)     1135 2023-05-21 09:25:54.000000 MySEAS_OLD-1.0.9/MySEAS_OLD.egg-info/SOURCES.txt
+-rw-r--r--   0 primary    (502) staff       (20)        1 2023-05-21 09:25:53.000000 MySEAS_OLD-1.0.9/MySEAS_OLD.egg-info/dependency_links.txt
+-rw-r--r--   0 primary    (502) staff       (20)        7 2023-05-21 09:25:53.000000 MySEAS_OLD-1.0.9/MySEAS_OLD.egg-info/requires.txt
+-rw-r--r--   0 primary    (502) staff       (20)        5 2023-05-21 09:25:53.000000 MySEAS_OLD-1.0.9/MySEAS_OLD.egg-info/top_level.txt
+-rw-r--r--   0 primary    (502) staff       (20)      601 2023-05-21 09:25:54.062927 MySEAS_OLD-1.0.9/PKG-INFO
+-rw-r--r--   0 primary    (502) staff       (20)      972 2022-11-17 15:22:36.000000 MySEAS_OLD-1.0.9/README.md
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.043939 MySEAS_OLD-1.0.9/SEAS/
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.045373 MySEAS_OLD-1.0.9/SEAS/Assets/
+-rw-r--r--   0 primary    (502) staff       (20)        0 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Assets/__init__.py
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.045766 MySEAS_OLD-1.0.9/SEAS/Engine/
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.050505 MySEAS_OLD-1.0.9/SEAS/Engine/Components/
+-rw-r--r--   0 primary    (502) staff       (20)      433 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Components/__init__.py
+-rw-r--r--   0 primary    (502) staff       (20)     2814 2022-11-17 14:47:24.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Components/characterPolyControllerComp.py
+-rw-r--r--   0 primary    (502) staff       (20)     6690 2022-11-14 12:12:51.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Components/collidePolyComp.py
+-rw-r--r--   0 primary    (502) staff       (20)      505 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Components/gravityComp.py
+-rw-r--r--   0 primary    (502) staff       (20)      580 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Components/hitboxPolyComp.py
+-rw-r--r--   0 primary    (502) staff       (20)      419 2022-11-17 09:45:19.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Components/renderPolyComp.py
+-rw-r--r--   0 primary    (502) staff       (20)      529 2022-11-17 09:45:26.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Components/renderRectComp.py
+-rw-r--r--   0 primary    (502) staff       (20)      936 2022-11-11 09:31:17.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Components/transformPolyComp.py
+-rw-r--r--   0 primary    (502) staff       (20)      269 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Components/transformRectComp.py
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.054160 MySEAS_OLD-1.0.9/SEAS/Engine/Core/
+-rw-r--r--   0 primary    (502) staff       (20)      110 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Core/__init__.py
+-rw-r--r--   0 primary    (502) staff       (20)     8690 2023-05-06 09:41:49.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Core/core.py
+-rw-r--r--   0 primary    (502) staff       (20)      245 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Core/event.py
+-rw-r--r--   0 primary    (502) staff       (20)      164 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Core/filePreset.py
+-rw-r--r--   0 primary    (502) staff       (20)      459 2022-11-14 13:54:45.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Core/font.py
+-rw-r--r--   0 primary    (502) staff       (20)      187 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Core/input.py
+-rw-r--r--   0 primary    (502) staff       (20)      570 2022-11-15 12:19:41.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Core/screen.py
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.055263 MySEAS_OLD-1.0.9/SEAS/Engine/Game/
+-rw-r--r--   0 primary    (502) staff       (20)       35 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Game/__init__.py
+-rw-r--r--   0 primary    (502) staff       (20)      289 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Game/run.py
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.056664 MySEAS_OLD-1.0.9/SEAS/Engine/Maths/
+-rw-r--r--   0 primary    (502) staff       (20)       38 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Maths/__init__.py
+-rw-r--r--   0 primary    (502) staff       (20)        0 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Maths/maths.py
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.057778 MySEAS_OLD-1.0.9/SEAS/Engine/Models/
+-rw-r--r--   0 primary    (502) staff       (20)       44 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Models/__init__.py
+-rw-r--r--   0 primary    (502) staff       (20)     1009 2022-11-15 12:16:01.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Models/emptyModel.py
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.059547 MySEAS_OLD-1.0.9/SEAS/Engine/Scene/
+-rw-r--r--   0 primary    (502) staff       (20)       38 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Scene/__init__.py
+-rw-r--r--   0 primary    (502) staff       (20)     7510 2022-11-18 09:02:44.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Scene/scene.py
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.061740 MySEAS_OLD-1.0.9/SEAS/Engine/Setup/
+-rw-r--r--   0 primary    (502) staff       (20)       44 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Setup/__init__.py
+-rw-r--r--   0 primary    (502) staff       (20)       28 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/Setup/pygameSetup.py
+-rw-r--r--   0 primary    (502) staff       (20)      202 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/Engine/__init__.py
+drwxr-xr-x   0 primary    (502) staff       (20)        0 2023-05-21 09:25:54.062378 MySEAS_OLD-1.0.9/SEAS/UI/
+-rw-r--r--   0 primary    (502) staff       (20)        0 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/UI/__init__.py
+-rw-r--r--   0 primary    (502) staff       (20)       74 2022-11-10 08:21:16.000000 MySEAS_OLD-1.0.9/SEAS/__init__.py
+-rw-r--r--   0 primary    (502) staff       (20)       38 2023-05-21 09:25:54.063488 MySEAS_OLD-1.0.9/setup.cfg
+-rw-r--r--   0 primary    (502) staff       (20)     1136 2023-05-21 09:25:25.000000 MySEAS_OLD-1.0.9/setup.py
```

### Comparing `MySEAS_OLD-1.0.8/MySEAS_OLD.egg-info/SOURCES.txt` & `MySEAS_OLD-1.0.9/MySEAS_OLD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/README.md` & `MySEAS_OLD-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/SEAS/Engine/Components/characterPolyControllerComp.py` & `MySEAS_OLD-1.0.9/SEAS/Engine/Components/characterPolyControllerComp.py`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/SEAS/Engine/Components/collidePolyComp.py` & `MySEAS_OLD-1.0.9/SEAS/Engine/Components/collidePolyComp.py`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/SEAS/Engine/Components/hitboxPolyComp.py` & `MySEAS_OLD-1.0.9/SEAS/Engine/Components/hitboxPolyComp.py`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/SEAS/Engine/Components/renderRectComp.py` & `MySEAS_OLD-1.0.9/SEAS/Engine/Components/renderRectComp.py`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/SEAS/Engine/Components/transformPolyComp.py` & `MySEAS_OLD-1.0.9/SEAS/Engine/Components/transformPolyComp.py`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/SEAS/Engine/Core/core.py` & `MySEAS_OLD-1.0.9/SEAS/Engine/Core/core.py`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/SEAS/Engine/Core/screen.py` & `MySEAS_OLD-1.0.9/SEAS/Engine/Core/screen.py`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/SEAS/Engine/Models/emptyModel.py` & `MySEAS_OLD-1.0.9/SEAS/Engine/Models/emptyModel.py`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/SEAS/Engine/Scene/scene.py` & `MySEAS_OLD-1.0.9/SEAS/Engine/Scene/scene.py`

 * *Files identical despite different names*

### Comparing `MySEAS_OLD-1.0.8/setup.py` & `MySEAS_OLD-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ########SAVE THIS UNVALUABLE INFORMATION#########
 #      python3 setup.py sdist bdist_wheel       #
 #        twine upload dist/* --verbose          #
 ########SAVE THIS UNVALUABLE INFORMATION#########
 
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 DESCRIPTION = 'A Simple Game Engine Libary'
 LONG_DESCRIPTION = 'Chech github: https://github.com/coding610/SEAS/tree/master'
 
 
 # Setting up
 setup(
     name="MySEAS_OLD",
```

