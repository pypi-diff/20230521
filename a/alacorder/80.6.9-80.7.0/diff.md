# Comparing `tmp/alacorder-80.6.9.tar.gz` & `tmp/alacorder-80.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.6.9.tar", max compression
+gzip compressed data, was "alacorder-80.7.0.tar", max compression
```

## Comparing `alacorder-80.6.9.tar` & `alacorder-80.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.9/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.9/README.md
--rw-r--r--   0        0        0      746 2023-05-20 14:44:29.028389 alacorder-80.6.9/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-20 14:44:20.349040 alacorder-80.6.9/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.6.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.9/src/alacorder/__init__.py
--rw-r--r--   0        0        0   237390 2023-05-20 14:44:03.709218 alacorder-80.6.9/src/alacorder/__main__.py
--rw-r--r--   0        0        0   237390 2023-05-20 14:43:32.982677 alacorder-80.6.9/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.0/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.7.0/README.md
+-rw-r--r--   0        0        0      746 2023-05-20 22:21:23.557879 alacorder-80.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-20 14:44:20.349040 alacorder-80.7.0/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.0/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   238014 2023-05-20 22:21:11.354439 alacorder-80.7.0/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   238014 2023-05-20 22:21:02.454254 alacorder-80.7.0/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.7.0/PKG-INFO
```

### Comparing `alacorder-80.6.9/LICENSE` & `alacorder-80.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.9/README.md` & `alacorder-80.7.0/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.9/pyproject.toml` & `alacorder-80.7.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.6.9"
+version = "80.7.0"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.6.9/src/alacorder/.DS_Store` & `alacorder-80.7.0/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.7.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.9/src/alacorder/__main__.py` & `alacorder-80.7.0/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.9"
+version = "80.7.0"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1087,14 +1087,20 @@
         inpath (str): Input archive
         outpath (str): Output archive
         cf (dict): Configuration object
 
     Returns:
         DataFrame: Appended archive object
     """
+    if not cf:
+        cf = {
+            'INPUTS': inpath,
+            'OUTPUT_PATH': outpath,
+            'WINDOW': None
+        }
     if cf and inpath == "":
         inpath = cf["INPUTS"]
 
     if cf and outpath == "":
         outpath = cf["OUTPUT_PATH"]
 
     if not os.path.isfile(inpath) and not os.path.isfile(outpath):
@@ -1115,17 +1121,30 @@
         except:
             dlog(inarc, outarc, cf=conf)
             print("Warning! Could not find column Path in archive.")
             inarc = inarc.select("AllPagesText")
             outarc = outarc.select("AllPagesText")
 
     out = pl.concat([inarc, outarc])
-
-    if window:
-        window.write_event_value("COMPLETE-AA", True)
+    out = out.with_columns(
+        [
+            pl.concat_str(
+                [
+                    pl.col("AllPagesText").str.extract(
+                        r"(County: )(\d{2})", group_index=2
+                    ),
+                    pl.lit("-"),
+                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                ]
+            ).alias("CaseNumber")
+        ]
+    )
+    out = out.unique("CaseNumber").select(pl.exclude("CaseNumber"))
+    if cf['WINDOW']:
+        cf['WINDOW'].write_event_value("COMPLETE-AA", True)
     write(out, path=outpath, overwrite=True)
     return out
 
 
 def rename_pdfs(cf):
     if isinstance(cf, dict):
         q = cf["QUEUE"]
```

### Comparing `alacorder-80.6.9/src/alacorder/alac.py` & `alacorder-80.7.0/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.9"
+version = "80.7.0"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1087,14 +1087,20 @@
         inpath (str): Input archive
         outpath (str): Output archive
         cf (dict): Configuration object
 
     Returns:
         DataFrame: Appended archive object
     """
+    if not cf:
+        cf = {
+            'INPUTS': inpath,
+            'OUTPUT_PATH': outpath,
+            'WINDOW': None
+        }
     if cf and inpath == "":
         inpath = cf["INPUTS"]
 
     if cf and outpath == "":
         outpath = cf["OUTPUT_PATH"]
 
     if not os.path.isfile(inpath) and not os.path.isfile(outpath):
@@ -1115,17 +1121,30 @@
         except:
             dlog(inarc, outarc, cf=conf)
             print("Warning! Could not find column Path in archive.")
             inarc = inarc.select("AllPagesText")
             outarc = outarc.select("AllPagesText")
 
     out = pl.concat([inarc, outarc])
-
-    if window:
-        window.write_event_value("COMPLETE-AA", True)
+    out = out.with_columns(
+        [
+            pl.concat_str(
+                [
+                    pl.col("AllPagesText").str.extract(
+                        r"(County: )(\d{2})", group_index=2
+                    ),
+                    pl.lit("-"),
+                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                ]
+            ).alias("CaseNumber")
+        ]
+    )
+    out = out.unique("CaseNumber").select(pl.exclude("CaseNumber"))
+    if cf['WINDOW']:
+        cf['WINDOW'].write_event_value("COMPLETE-AA", True)
     write(out, path=outpath, overwrite=True)
     return out
 
 
 def rename_pdfs(cf):
     if isinstance(cf, dict):
         q = cf["QUEUE"]
```

### Comparing `alacorder-80.6.9/PKG-INFO` & `alacorder-80.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.6.9
+Version: 80.7.0
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

