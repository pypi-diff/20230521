# Comparing `tmp/alacorder-80.7.1.tar.gz` & `tmp/alacorder-80.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.7.1.tar", max compression
+gzip compressed data, was "alacorder-80.7.2.tar", max compression
```

## Comparing `alacorder-80.7.1.tar` & `alacorder-80.7.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.1/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.7.1/README.md
--rw-r--r--   0        0        0      746 2023-05-21 21:27:16.536705 alacorder-80.7.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-21 17:23:39.998455 alacorder-80.7.1/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   238419 2023-05-21 21:25:40.237348 alacorder-80.7.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   238419 2023-05-21 21:25:29.913084 alacorder-80.7.1/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.2/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.7.2/README.md
+-rw-r--r--   0        0        0      746 2023-05-21 21:55:38.253512 alacorder-80.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-21 21:31:22.687412 alacorder-80.7.2/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.2/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.2/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   238144 2023-05-21 21:55:17.304226 alacorder-80.7.2/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   238144 2023-05-21 21:55:10.650312 alacorder-80.7.2/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.7.2/PKG-INFO
```

### Comparing `alacorder-80.7.1/LICENSE` & `alacorder-80.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.1/README.md` & `alacorder-80.7.2/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.1/pyproject.toml` & `alacorder-80.7.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.7.1"
+version = "80.7.2"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.7.1/src/alacorder/.DS_Store` & `alacorder-80.7.2/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.1/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.7.2/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.1/src/alacorder/__main__.py` & `alacorder-80.7.2/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.1"
+version = "80.7.2"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -817,25 +817,16 @@
             .alias("AllPagesTextNoNewLine")
         )
         return archive
     elif os.path.isdir(cf):  # directory path input
         queue = glob.glob(cf + "**/*.pdf", recursive=True)
         aptxt = []
         print("Extracting text...", cf=cf)
-        if cf["WINDOW"]:
-            cf["WINDOW"].write_event_value("PROGRESS_TOTAL", len(queue))
-            for i, pp in enumerate(queue):
-                aptxt += [extract_text(pp)]
-                cf["WINDOW"].write_event_value("PROGRESS", i + 1)
-        elif cf["LOG"]:
-            for pp in tqdm(queue):
-                aptxt += [extract_text(pp)]
-        else:
-            for pp in queue:
-                aptxt += [extract_text(pp)]
+        for pp in tqdm(queue):
+            aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
             pl.col("AllPagesText")
             .str.replace_all(r"\n", " ")
             .alias("AllPagesTextNoNewLine")
@@ -1091,27 +1082,30 @@
     Returns:
         DataFrame: Appended archive object
     """
     if not cf:
         cf = {
             'INPUTS': inpath,
             'OUTPUT_PATH': outpath,
-            'WINDOW': window
+            'WINDOW': window,
         }
     if cf and inpath == "":
         inpath = cf["INPUTS"]
 
     if cf and outpath == "":
         outpath = cf["OUTPUT_PATH"]
-
+    cfin = set(inpath, window=window, log=True)
+    cfout = set(outpath, window=window, log=True)
     if not os.path.isfile(inpath) and not os.path.isfile(outpath):
         error("Invalid path.", cf=cf)
 
-    inarc = read(inpath)
-    outarc = read(outpath)
+    inarc = read(cfin)
+    outarc = read(cfout)
+
+    print("Appending archives...")
 
     try:
         inarc = inarc.select("AllPagesText", "Path", "Timestamp")
         outarc = outarc.select("AllPagesText", "Path", "Timestamp")
     except:
         try:
             dlog(inarc, outarc, cf=conf)
@@ -4511,15 +4505,14 @@
         in_path (Path|DataFrame): Path to input archive / PDF directory
         out_path (Path): Path to output archive
         no_write (bool, optional): Do not export to output path
 
     Returns:
         DataFrame: Appended archive
     """
-    print("Appending archives...")
     arc = append_archive(in_path, out_path)
     print("Completed task.")
     return arc
 
 
 
 @main.command(name="fetch", help="Fetch cases from Alacourt.com")
```

### Comparing `alacorder-80.7.1/src/alacorder/alac.py` & `alacorder-80.7.2/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.1"
+version = "80.7.2"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -817,25 +817,16 @@
             .alias("AllPagesTextNoNewLine")
         )
         return archive
     elif os.path.isdir(cf):  # directory path input
         queue = glob.glob(cf + "**/*.pdf", recursive=True)
         aptxt = []
         print("Extracting text...", cf=cf)
-        if cf["WINDOW"]:
-            cf["WINDOW"].write_event_value("PROGRESS_TOTAL", len(queue))
-            for i, pp in enumerate(queue):
-                aptxt += [extract_text(pp)]
-                cf["WINDOW"].write_event_value("PROGRESS", i + 1)
-        elif cf["LOG"]:
-            for pp in tqdm(queue):
-                aptxt += [extract_text(pp)]
-        else:
-            for pp in queue:
-                aptxt += [extract_text(pp)]
+        for pp in tqdm(queue):
+            aptxt += [extract_text(pp)]
         archive = pl.DataFrame(
             {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
         )
         archive = archive.with_columns(
             pl.col("AllPagesText")
             .str.replace_all(r"\n", " ")
             .alias("AllPagesTextNoNewLine")
@@ -1091,27 +1082,30 @@
     Returns:
         DataFrame: Appended archive object
     """
     if not cf:
         cf = {
             'INPUTS': inpath,
             'OUTPUT_PATH': outpath,
-            'WINDOW': window
+            'WINDOW': window,
         }
     if cf and inpath == "":
         inpath = cf["INPUTS"]
 
     if cf and outpath == "":
         outpath = cf["OUTPUT_PATH"]
-
+    cfin = set(inpath, window=window, log=True)
+    cfout = set(outpath, window=window, log=True)
     if not os.path.isfile(inpath) and not os.path.isfile(outpath):
         error("Invalid path.", cf=cf)
 
-    inarc = read(inpath)
-    outarc = read(outpath)
+    inarc = read(cfin)
+    outarc = read(cfout)
+
+    print("Appending archives...")
 
     try:
         inarc = inarc.select("AllPagesText", "Path", "Timestamp")
         outarc = outarc.select("AllPagesText", "Path", "Timestamp")
     except:
         try:
             dlog(inarc, outarc, cf=conf)
@@ -4511,15 +4505,14 @@
         in_path (Path|DataFrame): Path to input archive / PDF directory
         out_path (Path): Path to output archive
         no_write (bool, optional): Do not export to output path
 
     Returns:
         DataFrame: Appended archive
     """
-    print("Appending archives...")
     arc = append_archive(in_path, out_path)
     print("Completed task.")
     return arc
 
 
 
 @main.command(name="fetch", help="Fetch cases from Alacourt.com")
```

### Comparing `alacorder-80.7.1/PKG-INFO` & `alacorder-80.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.7.1
+Version: 80.7.2
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

