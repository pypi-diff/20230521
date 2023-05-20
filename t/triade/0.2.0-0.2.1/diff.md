# Comparing `tmp/triade-0.2.0.tar.gz` & `tmp/triade-0.2.1.tar.gz`

## Comparing `triade-0.2.0.tar` & `triade-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 triade-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triade-0.2.0/triade/__init__.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 triade-0.2.0/triade/cli.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 triade-0.2.0/triade/lib.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 triade-0.2.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 triade-0.2.0/LICENSE
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 triade-0.2.0/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 triade-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 triade-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 triade-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triade-0.2.1/triade/__init__.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 triade-0.2.1/triade/cli.py
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 triade-0.2.1/triade/element.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 triade-0.2.1/triade/lib.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 triade-0.2.1/triade/xml_formatter.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 triade-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 triade-0.2.1/LICENSE
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 triade-0.2.1/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 triade-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 triade-0.2.1/PKG-INFO
```

### Comparing `triade-0.2.0/triade/cli.py` & `triade-0.2.1/triade/cli.py`

 * *Files identical despite different names*

### Comparing `triade-0.2.0/triade/lib.py` & `triade-0.2.1/triade/lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 parsers = {
     "json": json.loads,
     "yaml": yaml.safe_load,
     "toml": toml.loads,
 }
 
 writers = {
-    "json": json.dumps,
+    "json": lambda data: json.dumps(data, ensure_ascii=False),
     "yaml": lambda data: yaml.dump(data, Dumper=yaml.SafeDumper,
                                    allow_unicode=True),
     "toml": write_toml,
 }
 
 
 def parse(input_data: str, data_format: str) -> object:
```

### Comparing `triade-0.2.0/LICENSE` & `triade-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `triade-0.2.0/pyproject.toml` & `triade-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Makefile",
     "dev_requirements.txt",
     ".?*",
 ]
 
 [project]
 name = "triade"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Lucas L. S. Haine", email="lucaslshaine@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -24,14 +24,16 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: POSIX",
 ]
 
 dependencies = [
   "PyYAML",
   "toml",
+  "lxml",
+  "beautifulsoup4",
 ]
 
 [project.scripts]
 triade = "triade.cli:main"
 
 [project.urls]
 "Homepage" = "https://github.com/llucasls/triade"
```

### Comparing `triade-0.2.0/PKG-INFO` & `triade-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: triade
-Version: 0.2.0
+Version: 0.2.1
 Project-URL: Homepage, https://github.com/llucasls/triade
 Author-email: "Lucas L. S. Haine" <lucaslshaine@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
 Requires-Dist: pyyaml
 Requires-Dist: toml
 Description-Content-Type: text/markdown
 
 # Triade
 
 ## About
```

