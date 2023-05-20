# Comparing `tmp/sampling-constraints-0.0.8.tar.gz` & `tmp/sampling-constraints-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampling-constraints-0.0.8.tar", last modified: Tue May  9 03:12:03 2023, max compression
+gzip compressed data, was "sampling-constraints-0.0.9.tar", last modified: Wed May 10 04:14:06 2023, max compression
```

## Comparing `sampling-constraints-0.0.8.tar` & `sampling-constraints-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.8/LICENSE
--rw-r--r--   0 isaac     (1000) isaac     (1000)      625 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)      115 2023-05-08 23:11:28.000000 sampling-constraints-0.0.8/README.md
--rw-r--r--   0 isaac     (1000) isaac     (1000)      723 2023-05-09 03:11:57.000000 sampling-constraints-0.0.8/pyproject.toml
--rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/setup.cfg
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.472585 sampling-constraints-0.0.8/src/
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/src/sampling_constraints.egg-info/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      625 2023-05-09 03:12:03.000000 sampling-constraints-0.0.8/src/sampling_constraints.egg-info/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)      393 2023-05-09 03:12:03.000000 sampling-constraints-0.0.8/src/sampling_constraints.egg-info/SOURCES.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-09 03:12:03.000000 sampling-constraints-0.0.8/src/sampling_constraints.egg-info/dependency_links.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        4 2023-05-09 03:12:03.000000 sampling-constraints-0.0.8/src/sampling_constraints.egg-info/top_level.txt
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/src/scs/
--rw-r--r--   0 isaac     (1000) isaac     (1000)        0 2023-05-07 20:06:06.000000 sampling-constraints-0.0.8/src/scs/__init__.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/src/scs/constraint/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.8/src/scs/constraint/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.8/src/scs/constraint/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/src/scs/incremental_parse/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.8/src/scs/incremental_parse/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)    11908 2023-05-09 02:43:26.000000 sampling-constraints-0.0.8/src/scs/incremental_parse/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/tests/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     6133 2023-05-09 02:41:23.000000 sampling-constraints-0.0.8/tests/test_json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-10 04:14:06.373123 sampling-constraints-0.0.9/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.9/LICENSE
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      625 2023-05-10 04:14:06.373123 sampling-constraints-0.0.9/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      115 2023-05-08 23:11:28.000000 sampling-constraints-0.0.9/README.md
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      723 2023-05-10 04:13:36.000000 sampling-constraints-0.0.9/pyproject.toml
+-rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-10 04:14:06.373123 sampling-constraints-0.0.9/setup.cfg
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-10 04:14:06.373123 sampling-constraints-0.0.9/src/
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-10 04:14:06.373123 sampling-constraints-0.0.9/src/sampling_constraints.egg-info/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      625 2023-05-10 04:14:06.000000 sampling-constraints-0.0.9/src/sampling_constraints.egg-info/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      393 2023-05-10 04:14:06.000000 sampling-constraints-0.0.9/src/sampling_constraints.egg-info/SOURCES.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-10 04:14:06.000000 sampling-constraints-0.0.9/src/sampling_constraints.egg-info/dependency_links.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        4 2023-05-10 04:14:06.000000 sampling-constraints-0.0.9/src/sampling_constraints.egg-info/top_level.txt
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-10 04:14:06.373123 sampling-constraints-0.0.9/src/scs/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        0 2023-05-07 20:06:06.000000 sampling-constraints-0.0.9/src/scs/__init__.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-10 04:14:06.373123 sampling-constraints-0.0.9/src/scs/constraint/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.9/src/scs/constraint/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.9/src/scs/constraint/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-10 04:14:06.373123 sampling-constraints-0.0.9/src/scs/incremental_parse/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.9/src/scs/incremental_parse/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)    11979 2023-05-10 04:10:19.000000 sampling-constraints-0.0.9/src/scs/incremental_parse/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-10 04:14:06.373123 sampling-constraints-0.0.9/tests/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     6133 2023-05-09 02:41:23.000000 sampling-constraints-0.0.9/tests/test_json.py
```

### Comparing `sampling-constraints-0.0.8/LICENSE` & `sampling-constraints-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.8/PKG-INFO` & `sampling-constraints-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampling-constraints
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library of incremental parsers used to force syntax constraints on next-token predictions during language model generation
 Author-email: Isaac Rehg <isaacrehg@gmail.com>
 Project-URL: Homepage, https://github.com/IsaacRe/Syntactically-Constrained-Sampling
 Project-URL: Bug Tracker, https://github.com/IsaacRe/Syntactically-Constrained-Sampling/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sampling-constraints-0.0.8/pyproject.toml` & `sampling-constraints-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sampling-constraints"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name = "Isaac Rehg", email = "isaacrehg@gmail.com" },
 ]
 description = "Library of incremental parsers used to force syntax constraints on next-token predictions during language model generation"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `sampling-constraints-0.0.8/src/sampling_constraints.egg-info/PKG-INFO` & `sampling-constraints-0.0.9/src/sampling_constraints.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampling-constraints
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library of incremental parsers used to force syntax constraints on next-token predictions during language model generation
 Author-email: Isaac Rehg <isaacrehg@gmail.com>
 Project-URL: Homepage, https://github.com/IsaacRe/Syntactically-Constrained-Sampling
 Project-URL: Bug Tracker, https://github.com/IsaacRe/Syntactically-Constrained-Sampling/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sampling-constraints-0.0.8/src/scs/constraint/__init__.py` & `sampling-constraints-0.0.9/src/scs/constraint/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.8/src/scs/incremental_parse/__init__.py` & `sampling-constraints-0.0.9/src/scs/incremental_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.8/src/scs/incremental_parse/json.py` & `sampling-constraints-0.0.9/src/scs/incremental_parse/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
         if other._subparser:
             self._subparser = other._subparser.copy()
         self._complete = other._complete
     
     def _append(self, char: Union[str, SpecialToken]) -> bool:
         if self._subparser is None:
             if char == SpecialChar.OPEN_ARRAY.value:
-                self._subparser = ArrayParser()
+                #self._subparser = ArrayParser()
+                raise ParseFailure("Only allow object in outer JSON")
             elif char == SpecialChar.OPEN_OBJECT.value:
                 self._subparser = ObjectParser()
             elif not (isinstance(char, str) and char.isspace()):
                 raise ParseFailure(f"Expected '{{' or '[', got {char}")
             return False
         if self._complete:
             if char == SpecialToken.EOS:
```

### Comparing `sampling-constraints-0.0.8/tests/test_json.py` & `sampling-constraints-0.0.9/tests/test_json.py`

 * *Files identical despite different names*

