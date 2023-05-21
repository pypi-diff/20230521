# Comparing `tmp/esterdb-0.3.8.tar.gz` & `tmp/esterdb-0.4.0.tar.gz`

## Comparing `esterdb-0.3.8.tar` & `esterdb-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esterdb-0.3.8/Makefile
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 esterdb-0.3.8/esterdb/__about__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 esterdb-0.3.8/esterdb/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 esterdb-0.3.8/esterdb/_env.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 esterdb-0.3.8/esterdb/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esterdb-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 esterdb-0.3.8/tests/test_load.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 esterdb-0.3.8/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 esterdb-0.3.8/LICENSE.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 esterdb-0.3.8/README.md
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 esterdb-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esterdb-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esterdb-0.4.0/Makefile
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 esterdb-0.4.0/esterdb/__about__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 esterdb-0.4.0/esterdb/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 esterdb-0.4.0/esterdb/_env.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 esterdb-0.4.0/esterdb/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esterdb-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 esterdb-0.4.0/tests/test_load.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 esterdb-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 esterdb-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 esterdb-0.4.0/README.md
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 esterdb-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esterdb-0.4.0/PKG-INFO
```

### Comparing `esterdb-0.3.8/esterdb/main.py` & `esterdb-0.4.0/esterdb/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 duckdb_arch = "linux_amd64_gcc4"
             else:
                 raise WTTException(
                     f"Unable to find extension for {operating_system} {architecture}"
                 )
 
             filename = f"{name}.duckdb_extension.gz"
-            url = f"https://dbe.wheretrue.com/{name}/{version}/v0.7.1/{duckdb_arch}/{filename}"
+            url = f"https://dbe.wheretrue.com/{name}/{version}/v0.8.0/{duckdb_arch}/{filename}"
             logger.info("Downloading extension from %s", url)
 
             with tempfile.TemporaryDirectory() as temp_dir:
                 temp_dir_path = Path(temp_dir)
                 temp_file_name = temp_dir_path / filename
 
                 try:
```

### Comparing `esterdb-0.3.8/tests/test_load.py` & `esterdb-0.4.0/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `esterdb-0.3.8/LICENSE.txt` & `esterdb-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `esterdb-0.3.8/pyproject.toml` & `esterdb-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-  "duckdb==0.7.1",
+  "duckdb==0.8.0",
 ]
 description = ''
 dynamic = ["version"]
 keywords = []
 license = "MIT"
 name = "esterdb"
 readme = "README.md"
```

### Comparing `esterdb-0.3.8/PKG-INFO` & `esterdb-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: esterdb
-Version: 0.3.8
+Version: 0.4.0
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: duckdb==0.7.1
+Requires-Dist: duckdb==0.8.0
 Description-Content-Type: text/markdown
 
-# WTT 02
+# EsterDB
 
 **Table of Contents**
 
 - [Installation](#installation)
 
 ## Installation
 
 ```console
-pip install wtt02
+pip install esterdb
 ```
```

