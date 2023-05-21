# Comparing `tmp/alacorder-80.7.0.tar.gz` & `tmp/alacorder-80.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.7.0.tar", max compression
+gzip compressed data, was "alacorder-80.7.1.tar", max compression
```

## Comparing `alacorder-80.7.0.tar` & `alacorder-80.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.0/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.7.0/README.md
--rw-r--r--   0        0        0      746 2023-05-20 22:21:23.557879 alacorder-80.7.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-20 14:44:20.349040 alacorder-80.7.0/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.0/src/alacorder/__init__.py
--rw-r--r--   0        0        0   238014 2023-05-20 22:21:11.354439 alacorder-80.7.0/src/alacorder/__main__.py
--rw-r--r--   0        0        0   238014 2023-05-20 22:21:02.454254 alacorder-80.7.0/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.1/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.7.1/README.md
+-rw-r--r--   0        0        0      746 2023-05-21 21:27:16.536705 alacorder-80.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-21 17:23:39.998455 alacorder-80.7.1/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.1/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   238419 2023-05-21 21:25:40.237348 alacorder-80.7.1/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   238419 2023-05-21 21:25:29.913084 alacorder-80.7.1/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.7.1/PKG-INFO
```

### Comparing `alacorder-80.7.0/LICENSE` & `alacorder-80.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.0/README.md` & `alacorder-80.7.1/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.0/pyproject.toml` & `alacorder-80.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.7.0"
+version = "80.7.1"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.7.0/src/alacorder/.DS_Store` & `alacorder-80.7.1/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.7.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.0/src/alacorder/__main__.py` & `alacorder-80.7.1/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.0"
+version = "80.7.1"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1075,15 +1075,15 @@
         return ""
     text = " \n ".join(
         x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
     )
     return text
 
 
-def append_archive(inpath="", outpath="", cf=None):
+def append_archive(inpath="", outpath="", cf=None, window=None):
     """
     Append the contents of one archive to another.
 
     Args:
         inpath (str): Input archive
         outpath (str): Output archive
         cf (dict): Configuration object
@@ -1091,15 +1091,15 @@
     Returns:
         DataFrame: Appended archive object
     """
     if not cf:
         cf = {
             'INPUTS': inpath,
             'OUTPUT_PATH': outpath,
-            'WINDOW': None
+            'WINDOW': window
         }
     if cf and inpath == "":
         inpath = cf["INPUTS"]
 
     if cf and outpath == "":
         outpath = cf["OUTPUT_PATH"]
 
@@ -1249,14 +1249,15 @@
                 pl.col("DOB").arr.get(0),
                 pl.col("CaseNumber").arr.lengths().alias("CaseCount"),
                 pl.col("CaseNumber").arr.join(", ").alias("Cases"),
             ]
         )
     )
     names = names.sort("Name")
+    names = names.filter(pl.col("Name") != "")
     return names
 
 
 def _vrr_summary_from_pairs(src, pairs, dest=None, window=None, debug=False):
     if isinstance(src, str):
         cases = cf(src, table="cases", now=True)
         charges = cf(src, table="charges", now=True)
@@ -3729,28 +3730,28 @@
 
     Args:
         path (str): Desired output path (.xls, .xlsx)
 
     """
     success = True
     empty = pl.DataFrame(
-        columns=[
-            "NAME",
-            "PARTY_TYPE",
-            "SSN",
-            "DOB",
-            "COUNTY",
-            "DIVISION",
-            "CASE_YEAR",
-            "NO_RECORDS",
-            "FILED_BEFORE",
-            "FILED_AFTER",
-            "RETRIEVED",
-            "CASES_FOUND",
-        ]
+            {
+                "NAME": [],
+                "PARTY_TYPE": [],
+                "SSN": [],
+                "DOB": [],
+                "COUNTY": [],
+                "DIVISION": [],
+                "CASE_YEAR": [],
+                "NO_RECORDS": [],
+                "FILED_BEFORE": [],
+                "FILED_AFTER": [],
+                "RETRIEVED": [],
+                "CASES_FOUND": []
+            }
     )
     return write(empty, sheet_names="query", path=path, overwrite=True)
 
 
 #   #   #   #      GRAPHICAL USER INTERFACE    #   #   #   #
 
 
@@ -4249,23 +4250,27 @@
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
             window["RN"].update(disabled=False)
+            window["MT"].update(disabled=False)
+            window["NEWQUERY"].update(disabled=False)
         elif "COMPLETE" in event:
             print("Alacorder completed the task.")
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
             window["RN"].update(disabled=False)
+            window["MT"].update(disabled=False)
+            window["NEWQUERY"].update(disabled=False)
             window["PROGRESS"].update(current_count=0, max=100)
             sg.popup("Alacorder completed the task.")
             continue
         elif event == "NEWQUERY":
             if window["SQ-INPUTPATH"].get() == "":
                 sg.popup(
                     "To create empty query template, enter file output path (extension must be .xlsx) in Input Path, then press the New Query button to try again."
@@ -4507,15 +4512,18 @@
         out_path (Path): Path to output archive
         no_write (bool, optional): Do not export to output path
 
     Returns:
         DataFrame: Appended archive
     """
     print("Appending archives...")
-    return append_archive(in_path, out_path)
+    arc = append_archive(in_path, out_path)
+    print("Completed task.")
+    return arc
+
 
 
 @main.command(name="fetch", help="Fetch cases from Alacourt.com")
 @click.option(
     "--input-path",
     "-in",
     "querypath",
```

### Comparing `alacorder-80.7.0/src/alacorder/alac.py` & `alacorder-80.7.1/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.0"
+version = "80.7.1"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1075,15 +1075,15 @@
         return ""
     text = " \n ".join(
         x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
     )
     return text
 
 
-def append_archive(inpath="", outpath="", cf=None):
+def append_archive(inpath="", outpath="", cf=None, window=None):
     """
     Append the contents of one archive to another.
 
     Args:
         inpath (str): Input archive
         outpath (str): Output archive
         cf (dict): Configuration object
@@ -1091,15 +1091,15 @@
     Returns:
         DataFrame: Appended archive object
     """
     if not cf:
         cf = {
             'INPUTS': inpath,
             'OUTPUT_PATH': outpath,
-            'WINDOW': None
+            'WINDOW': window
         }
     if cf and inpath == "":
         inpath = cf["INPUTS"]
 
     if cf and outpath == "":
         outpath = cf["OUTPUT_PATH"]
 
@@ -1249,14 +1249,15 @@
                 pl.col("DOB").arr.get(0),
                 pl.col("CaseNumber").arr.lengths().alias("CaseCount"),
                 pl.col("CaseNumber").arr.join(", ").alias("Cases"),
             ]
         )
     )
     names = names.sort("Name")
+    names = names.filter(pl.col("Name") != "")
     return names
 
 
 def _vrr_summary_from_pairs(src, pairs, dest=None, window=None, debug=False):
     if isinstance(src, str):
         cases = cf(src, table="cases", now=True)
         charges = cf(src, table="charges", now=True)
@@ -3729,28 +3730,28 @@
 
     Args:
         path (str): Desired output path (.xls, .xlsx)
 
     """
     success = True
     empty = pl.DataFrame(
-        columns=[
-            "NAME",
-            "PARTY_TYPE",
-            "SSN",
-            "DOB",
-            "COUNTY",
-            "DIVISION",
-            "CASE_YEAR",
-            "NO_RECORDS",
-            "FILED_BEFORE",
-            "FILED_AFTER",
-            "RETRIEVED",
-            "CASES_FOUND",
-        ]
+            {
+                "NAME": [],
+                "PARTY_TYPE": [],
+                "SSN": [],
+                "DOB": [],
+                "COUNTY": [],
+                "DIVISION": [],
+                "CASE_YEAR": [],
+                "NO_RECORDS": [],
+                "FILED_BEFORE": [],
+                "FILED_AFTER": [],
+                "RETRIEVED": [],
+                "CASES_FOUND": []
+            }
     )
     return write(empty, sheet_names="query", path=path, overwrite=True)
 
 
 #   #   #   #      GRAPHICAL USER INTERFACE    #   #   #   #
 
 
@@ -4249,23 +4250,27 @@
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
             window["RN"].update(disabled=False)
+            window["MT"].update(disabled=False)
+            window["NEWQUERY"].update(disabled=False)
         elif "COMPLETE" in event:
             print("Alacorder completed the task.")
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
             window["RN"].update(disabled=False)
+            window["MT"].update(disabled=False)
+            window["NEWQUERY"].update(disabled=False)
             window["PROGRESS"].update(current_count=0, max=100)
             sg.popup("Alacorder completed the task.")
             continue
         elif event == "NEWQUERY":
             if window["SQ-INPUTPATH"].get() == "":
                 sg.popup(
                     "To create empty query template, enter file output path (extension must be .xlsx) in Input Path, then press the New Query button to try again."
@@ -4507,15 +4512,18 @@
         out_path (Path): Path to output archive
         no_write (bool, optional): Do not export to output path
 
     Returns:
         DataFrame: Appended archive
     """
     print("Appending archives...")
-    return append_archive(in_path, out_path)
+    arc = append_archive(in_path, out_path)
+    print("Completed task.")
+    return arc
+
 
 
 @main.command(name="fetch", help="Fetch cases from Alacourt.com")
 @click.option(
     "--input-path",
     "-in",
     "querypath",
```

### Comparing `alacorder-80.7.0/PKG-INFO` & `alacorder-80.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.7.0
+Version: 80.7.1
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

