# Comparing `tmp/patchparser-0.0.2.tar.gz` & `tmp/patchparser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchparser-0.0.2.tar", last modified: Thu Sep  1 14:04:59 2022, max compression
+gzip compressed data, was "patchparser-0.0.3.tar", last modified: Sun May 21 19:38:16 2023, max compression
```

## Comparing `patchparser-0.0.2.tar` & `patchparser-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 tad       (1000) tad       (1000)        0 2022-09-01 14:04:59.658497 patchparser-0.0.2/
--rw-rw-r--   0 tad       (1000) tad       (1000)     1211 2022-08-18 15:48:38.000000 patchparser-0.0.2/LICENSE
--rw-rw-r--   0 tad       (1000) tad       (1000)     7275 2022-09-01 14:04:59.658497 patchparser-0.0.2/PKG-INFO
--rw-rw-r--   0 tad       (1000) tad       (1000)     6715 2022-09-01 14:00:29.000000 patchparser-0.0.2/README.md
--rw-rw-r--   0 tad       (1000) tad       (1000)      805 2022-09-01 14:04:49.000000 patchparser-0.0.2/pyproject.toml
--rw-rw-r--   0 tad       (1000) tad       (1000)       38 2022-09-01 14:04:59.658497 patchparser-0.0.2/setup.cfg
-drwxrwxr-x   0 tad       (1000) tad       (1000)        0 2022-09-01 14:04:59.658497 patchparser-0.0.2/src/
-drwxrwxr-x   0 tad       (1000) tad       (1000)        0 2022-09-01 14:04:59.658497 patchparser-0.0.2/src/patchparser/
--rw-rw-r--   0 tad       (1000) tad       (1000)        0 2022-08-18 16:52:37.000000 patchparser-0.0.2/src/patchparser/__init__.py
--rw-rw-r--   0 tad       (1000) tad       (1000)    15544 2022-09-01 14:01:38.000000 patchparser-0.0.2/src/patchparser/github_parser.py
-drwxrwxr-x   0 tad       (1000) tad       (1000)        0 2022-09-01 14:04:59.658497 patchparser-0.0.2/src/patchparser.egg-info/
--rw-rw-r--   0 tad       (1000) tad       (1000)     7275 2022-09-01 14:04:59.000000 patchparser-0.0.2/src/patchparser.egg-info/PKG-INFO
--rw-rw-r--   0 tad       (1000) tad       (1000)      287 2022-09-01 14:04:59.000000 patchparser-0.0.2/src/patchparser.egg-info/SOURCES.txt
--rw-rw-r--   0 tad       (1000) tad       (1000)        1 2022-09-01 14:04:59.000000 patchparser-0.0.2/src/patchparser.egg-info/dependency_links.txt
--rw-rw-r--   0 tad       (1000) tad       (1000)        9 2022-09-01 14:04:59.000000 patchparser-0.0.2/src/patchparser.egg-info/requires.txt
--rw-rw-r--   0 tad       (1000) tad       (1000)       12 2022-09-01 14:04:59.000000 patchparser-0.0.2/src/patchparser.egg-info/top_level.txt
+drwxrwxr-x   0 tad       (1000) tad       (1000)        0 2023-05-21 19:38:16.594316 patchparser-0.0.3/
+-rw-rw-r--   0 tad       (1000) tad       (1000)     1211 2022-08-18 15:48:38.000000 patchparser-0.0.3/LICENSE
+-rw-rw-r--   0 tad       (1000) tad       (1000)     7275 2023-05-21 19:38:16.594316 patchparser-0.0.3/PKG-INFO
+-rw-rw-r--   0 tad       (1000) tad       (1000)     6715 2022-09-01 14:15:29.000000 patchparser-0.0.3/README.md
+drwxrwxr-x   0 tad       (1000) tad       (1000)        0 2023-05-21 19:38:16.594316 patchparser-0.0.3/patchparser/
+-rw-rw-r--   0 tad       (1000) tad       (1000)       81 2023-05-21 18:22:58.000000 patchparser-0.0.3/patchparser/__init__.py
+-rw-rw-r--   0 tad       (1000) tad       (1000)    15828 2023-05-21 19:06:54.000000 patchparser-0.0.3/patchparser/github_parser.py
+-rw-rw-r--   0 tad       (1000) tad       (1000)    20075 2023-05-21 19:13:34.000000 patchparser-0.0.3/patchparser/github_parser_local.py
+drwxrwxr-x   0 tad       (1000) tad       (1000)        0 2023-05-21 19:38:16.594316 patchparser-0.0.3/patchparser.egg-info/
+-rw-rw-r--   0 tad       (1000) tad       (1000)     7275 2023-05-21 19:38:16.000000 patchparser-0.0.3/patchparser.egg-info/PKG-INFO
+-rw-rw-r--   0 tad       (1000) tad       (1000)      356 2023-05-21 19:38:16.000000 patchparser-0.0.3/patchparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 tad       (1000) tad       (1000)        1 2023-05-21 19:38:16.000000 patchparser-0.0.3/patchparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 tad       (1000) tad       (1000)       19 2023-05-21 19:38:16.000000 patchparser-0.0.3/patchparser.egg-info/requires.txt
+-rw-rw-r--   0 tad       (1000) tad       (1000)       12 2023-05-21 19:38:16.000000 patchparser-0.0.3/patchparser.egg-info/top_level.txt
+-rw-rw-r--   0 tad       (1000) tad       (1000)      820 2023-05-21 19:38:06.000000 patchparser-0.0.3/pyproject.toml
+-rw-rw-r--   0 tad       (1000) tad       (1000)       38 2023-05-21 19:38:16.594316 patchparser-0.0.3/setup.cfg
+drwxrwxr-x   0 tad       (1000) tad       (1000)        0 2023-05-21 19:38:16.594316 patchparser-0.0.3/tests/
+-rw-rw-r--   0 tad       (1000) tad       (1000)      695 2023-05-21 19:37:21.000000 patchparser-0.0.3/tests/test_github_parser.py
+-rw-rw-r--   0 tad       (1000) tad       (1000)      778 2023-05-21 19:16:24.000000 patchparser-0.0.3/tests/test_github_parser_local.py
```

### Comparing `patchparser-0.0.2/LICENSE` & `patchparser-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `patchparser-0.0.2/PKG-INFO` & `patchparser-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchparser
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package to extract features from a commit patch.
 Author-email: Trevor Dunlap <tdunlap607@gmail.com>
 Project-URL: Homepage, https://github.com/tdunlap607/patchparser
 Project-URL: Bug Tracker, https://github.com/tdunlap607/patchparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
```

### Comparing `patchparser-0.0.2/README.md` & `patchparser-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `patchparser-0.0.2/pyproject.toml` & `patchparser-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "patchparser"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Trevor Dunlap", email="tdunlap607@gmail.com" },
 ]
 description = "A python package to extract features from a commit patch."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: The Unlicense (Unlicense)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'requests'
+  'requests',
+  'GitPython'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/tdunlap607/patchparser"
 "Bug Tracker" = "https://github.com/tdunlap607/patchparser/issues"
```

### Comparing `patchparser-0.0.2/src/patchparser/github_parser.py` & `patchparser-0.0.3/patchparser/github_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,19 @@
             """Find patch headers (e.g., @@ @@)"""
             headers_search = re.findall(r"@@(.*?)@@", raw_file_patch) 
             
             """Cleaning the headers, found @@REPLACE_ME@@ in some random code"""
             headers = []
             for head_row in headers_search:
                 if '-' in head_row and '+' in head_row:
-                    headers.append(f"@@{head_row}@@")
+                    # get the original line headers
+                    original_header_lines = re.search(f"@@ -(.*?) \+", f"@@{head_row}@@").group(1)
+                    # make sure the header is of type int
+                    if original_header_lines.split(',')[-1].isdigit():
+                        headers.append(f"@@{head_row}@@")
             total_patches = len(headers)
             
             for index, header in enumerate(headers):
                 patch_number = index
                 """Get line numbers changed for original code"""
                 original_lines = re.search(f"@@ -(.*?) \+", header).group(1)
                 if "," in original_lines:
```

### Comparing `patchparser-0.0.2/src/patchparser.egg-info/PKG-INFO` & `patchparser-0.0.3/patchparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchparser
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package to extract features from a commit patch.
 Author-email: Trevor Dunlap <tdunlap607@gmail.com>
 Project-URL: Homepage, https://github.com/tdunlap607/patchparser
 Project-URL: Bug Tracker, https://github.com/tdunlap607/patchparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
```

