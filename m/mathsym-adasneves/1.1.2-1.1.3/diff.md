# Comparing `tmp/mathsym_adasneves-1.1.2.tar.gz` & `tmp/mathsym_adasneves-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathsym_adasneves-1.1.2.tar", last modified: Sat May 20 22:10:54 2023, max compression
+gzip compressed data, was "mathsym_adasneves-1.1.3.tar", last modified: Sat May 20 22:13:33 2023, max compression
```

## Comparing `mathsym_adasneves-1.1.2.tar` & `mathsym_adasneves-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:10:54.527135 mathsym_adasneves-1.1.2/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-1.1.2/LICENSE
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1744 2023-05-20 22:10:54.527135 mathsym_adasneves-1.1.2/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1226 2023-05-19 00:28:33.000000 mathsym_adasneves-1.1.2/README.md
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      591 2023-05-20 22:10:43.000000 mathsym_adasneves-1.1.2/pyproject.toml
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-20 22:10:54.527135 mathsym_adasneves-1.1.2/setup.cfg
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:10:54.523136 mathsym_adasneves-1.1.2/src/
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:10:54.527135 mathsym_adasneves-1.1.2/src/mathsym_adasneves.egg-info/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1744 2023-05-20 22:10:54.000000 mathsym_adasneves-1.1.2/src/mathsym_adasneves.egg-info/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      437 2023-05-20 22:10:54.000000 mathsym_adasneves-1.1.2/src/mathsym_adasneves.egg-info/SOURCES.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-20 22:10:54.000000 mathsym_adasneves-1.1.2/src/mathsym_adasneves.egg-info/dependency_links.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-20 22:10:54.000000 mathsym_adasneves-1.1.2/src/mathsym_adasneves.egg-info/top_level.txt
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:10:54.527135 mathsym_adasneves-1.1.2/src/symMath_adasneves127/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:08:33.000000 mathsym_adasneves-1.1.2/src/symMath_adasneves127/__init__.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-19 00:54:00.000000 mathsym_adasneves-1.1.2/src/symMath_adasneves127/equation.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-19 00:13:51.000000 mathsym_adasneves-1.1.2/src/symMath_adasneves127/token.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     2084 2023-05-19 00:57:25.000000 mathsym_adasneves-1.1.2/src/symMath_adasneves127/token_maker.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     3438 2023-05-19 00:09:20.000000 mathsym_adasneves-1.1.2/src/symMath_adasneves127/tree_maker.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     2620 2023-05-20 22:09:51.000000 mathsym_adasneves-1.1.2/src/symMath_adasneves127/tree_node.py
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:13:33.617088 mathsym_adasneves-1.1.3/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-1.1.3/LICENSE
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1744 2023-05-20 22:13:33.617088 mathsym_adasneves-1.1.3/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1226 2023-05-19 00:28:33.000000 mathsym_adasneves-1.1.3/README.md
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      591 2023-05-20 22:13:15.000000 mathsym_adasneves-1.1.3/pyproject.toml
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-20 22:13:33.617088 mathsym_adasneves-1.1.3/setup.cfg
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:13:33.613089 mathsym_adasneves-1.1.3/src/
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:13:33.613089 mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1744 2023-05-20 22:13:33.000000 mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      437 2023-05-20 22:13:33.000000 mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/SOURCES.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-20 22:13:33.000000 mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/dependency_links.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-20 22:13:33.000000 mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/top_level.txt
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:13:33.617088 mathsym_adasneves-1.1.3/src/symMath_adasneves127/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:08:33.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/__init__.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-19 00:54:00.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/equation.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-19 00:13:51.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/token.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     2084 2023-05-19 00:57:25.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/token_maker.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     3438 2023-05-19 00:09:20.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/tree_maker.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     2621 2023-05-20 22:13:21.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/tree_node.py
```

### Comparing `mathsym_adasneves-1.1.2/LICENSE` & `mathsym_adasneves-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.1.2/PKG-INFO` & `mathsym_adasneves-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym_adasneves
-Version: 1.1.2
+Version: 1.1.3
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathsym_adasneves-1.1.2/README.md` & `mathsym_adasneves-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.1.2/pyproject.toml` & `mathsym_adasneves-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mathsym_adasneves"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Alex Dasneves", email="adasneves@adasneves.info" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mathsym_adasneves-1.1.2/src/mathsym_adasneves.egg-info/PKG-INFO` & `mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym-adasneves
-Version: 1.1.2
+Version: 1.1.3
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathsym_adasneves-1.1.2/src/symMath_adasneves127/equation.py` & `mathsym_adasneves-1.1.3/src/symMath_adasneves127/equation.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.1.2/src/symMath_adasneves127/token_maker.py` & `mathsym_adasneves-1.1.3/src/symMath_adasneves127/token_maker.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.1.2/src/symMath_adasneves127/tree_maker.py` & `mathsym_adasneves-1.1.3/src/symMath_adasneves127/tree_maker.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.1.2/src/symMath_adasneves127/tree_node.py` & `mathsym_adasneves-1.1.3/src/symMath_adasneves127/tree_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,11 +54,11 @@
                     return 0
                 
     def instantaneous_slope(self, x):
         y_1 = self.evaluate(x + 0.0000000001) # Evaluate the function at a x value to the right.
         y_2 = self.evaluate(x) # Evaluate the function at the current X pos
         
         if y_2 is not None and y_1 is not None:
-            return (y_2 - y_1)/(0.0000000001)
+            return (y_2 - y_1)/(-0.0000000001)
         else:
             return None
```

