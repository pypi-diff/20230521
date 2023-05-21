# Comparing `tmp/khloraascaf_utils-0.8.1.tar.gz` & `tmp/khloraascaf_utils-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf_utils-0.8.1.tar", last modified: Wed May 17 16:50:34 2023, max compression
+gzip compressed data, was "khloraascaf_utils-0.8.2.tar", last modified: Sun May 21 21:20:44 2023, max compression
```

## Comparing `khloraascaf_utils-0.8.1.tar` & `khloraascaf_utils-0.8.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:50:34.667677 khloraascaf_utils-0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/LICENCE
--rw-r--r--   0 root         (0) root         (0)    43838 2023-05-17 16:50:34.666679 khloraascaf_utils-0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 16:50:34.667677 khloraascaf_utils-0.8.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:50:34.659686 khloraascaf_utils-0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:50:34.663682 khloraascaf_utils-0.8.1/src/khloraascaf_utils/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9489 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils/artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7285 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils/asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils/contigs_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    13859 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils/to_networkx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:50:34.665680 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43838 2023-05-17 16:50:34.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-17 16:50:34.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 16:50:34.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-17 16:50:34.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-17 16:50:34.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:50:34.666679 khloraascaf_utils-0.8.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4112 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/tests/test_artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/tests/test_asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     1806 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/tests/test_contigs_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:20:44.974427 khloraascaf_utils-0.8.2/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-21 21:20:44.974427 khloraascaf_utils-0.8.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 21:20:44.974427 khloraascaf_utils-0.8.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:20:44.970427 khloraascaf_utils-0.8.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:20:44.972427 khloraascaf_utils-0.8.2/src/khloraascaf_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9489 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils/artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7243 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils/asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils/contigs_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    13859 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils/to_networkx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:20:44.973427 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-21 21:20:44.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-21 21:20:44.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 21:20:44.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-21 21:20:44.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-21 21:20:44.000000 khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:20:44.973427 khloraascaf_utils-0.8.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4112 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/tests/test_artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/tests/test_asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2023-05-21 21:20:23.000000 khloraascaf_utils-0.8.2/tests/test_contigs_attributes.py
```

### Comparing `khloraascaf_utils-0.8.1/LICENCE` & `khloraascaf_utils-0.8.2/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.1/PKG-INFO` & `khloraascaf_utils-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf_utils
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.8.1/README.md` & `khloraascaf_utils-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.1/pyproject.toml` & `khloraascaf_utils-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf_utils"
-version = "0.8.1"
+version = "0.8.2"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "Python utilities for khloraascaf python package."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `khloraascaf_utils-0.8.1/src/khloraascaf_utils/artificial_data.py` & `khloraascaf_utils-0.8.2/src/khloraascaf_utils/artificial_data.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.1/src/khloraascaf_utils/asm_graph_to_fasta.py` & `khloraascaf_utils-0.8.2/src/khloraascaf_utils/asm_graph_to_fasta.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,16 @@
 
         for link_id, c_id, c_or, d_id, d_or in read_contig_links_file(
                 contig_links_file):
             self.__orc_link_to_id[(c_id, c_or), (d_id, d_or)] = link_id
             self.__link_sequences[link_id] = Seq.Seq('')
 
         for record in SeqIO.parse(link_sequences_file, 'fasta'):
-            if record.id not in self.__link_sequences:
-                raise KeyError(record.id)
-            self.__link_sequences[record.id] = record.seq
+            if record.id in self.__link_sequences:
+                self.__link_sequences[record.id] = record.seq
         #
         # Sequence for each forward region
         #
         # OPTIMIZE stop keeping in hard memory: index method?
         self.__region_sequences: list[Seq.Seq] = []
         #
         # For each region (forward) gives its oriented contig extremities
```

### Comparing `khloraascaf_utils-0.8.1/src/khloraascaf_utils/contigs_attributes.py` & `khloraascaf_utils-0.8.2/src/khloraascaf_utils/contigs_attributes.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.1/src/khloraascaf_utils/to_networkx.py` & `khloraascaf_utils-0.8.2/src/khloraascaf_utils/to_networkx.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/PKG-INFO` & `khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf-utils
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/SOURCES.txt` & `khloraascaf_utils-0.8.2/src/khloraascaf_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.1/tests/test_artificial_data.py` & `khloraascaf_utils-0.8.2/tests/test_artificial_data.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.1/tests/test_asm_graph_to_fasta.py` & `khloraascaf_utils-0.8.2/tests/test_asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.1/tests/test_contigs_attributes.py` & `khloraascaf_utils-0.8.2/tests/test_contigs_attributes.py`

 * *Files identical despite different names*

