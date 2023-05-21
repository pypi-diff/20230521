# Comparing `tmp/mach2-0.0.1.tar.gz` & `tmp/mach2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mach2-0.0.1.tar", last modified: Thu May 18 20:52:23 2023, max compression
+gzip compressed data, was "mach2-0.0.2.tar", last modified: Sun May 21 09:38:38 2023, max compression
```

## Comparing `mach2-0.0.1.tar` & `mach2-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1581 2023-05-17 16:26:02.847064 mach2-0.0.1/LICENSE
--rw-r--r--   0        0        0      513 2023-05-15 14:14:08.082067 mach2-0.0.1/README.md
--rw-r--r--   0        0        0      997 2023-05-18 20:52:23.683182 mach2-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-15 12:06:57.622467 mach2-0.0.1/src/mach2/__init__.py
--rw-r--r--   0        0        0    13877 2023-05-15 22:46:48.571251 mach2-0.0.1/src/mach2/clonetree.py
--rw-r--r--   0        0        0    22520 2023-05-18 08:26:20.511578 mach2-0.0.1/src/mach2/mach.py
--rw-r--r--   0        0        0     3043 2023-05-15 22:25:01.101453 mach2-0.0.1/src/mach2/migrationgraph.py
--rw-r--r--   0        0        0     5131 2023-05-15 22:27:26.185860 mach2-0.0.1/src/mach2/solutionset.py
--rw-r--r--   0        0        0      296 2023-05-14 21:09:58.179420 mach2-0.0.1/src/mach2/utils.py
--rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 mach2-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1581 2023-05-17 16:26:02.847064 mach2-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5012 2023-05-21 09:29:39.765450 mach2-0.0.2/README.md
+-rw-r--r--   0        0        0      984 2023-05-21 09:38:38.315606 mach2-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-15 12:06:57.622467 mach2-0.0.2/src/mach2/__init__.py
+-rw-r--r--   0        0        0    13877 2023-05-15 22:46:48.571251 mach2-0.0.2/src/mach2/clonetree.py
+-rw-r--r--   0        0        0    22493 2023-05-21 09:25:29.295937 mach2-0.0.2/src/mach2/mach.py
+-rw-r--r--   0        0        0     3043 2023-05-15 22:25:01.101453 mach2-0.0.2/src/mach2/migrationgraph.py
+-rw-r--r--   0        0        0     5131 2023-05-15 22:27:26.185860 mach2-0.0.2/src/mach2/solutionset.py
+-rw-r--r--   0        0        0      296 2023-05-14 21:09:58.179420 mach2-0.0.2/src/mach2/utils.py
+-rw-r--r--   0        0        0     7644 1970-01-01 00:00:00.000000 mach2-0.0.2/PKG-INFO
```

### Comparing `mach2-0.0.1/LICENSE` & `mach2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mach2-0.0.1/pyproject.toml` & `mach2-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "mach2"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Mrinmoy Saha Roddur", email = "mroddur2@illinois.edu" },
 ]
 description = "Migration Analysis of Clonal History 2"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -26,27 +26,25 @@
     "Phylogeny",
 ]
 dependencies = [
     "numpy",
     "pandas",
     "pyomo",
     "networkx",
+    "gurobi",
 ]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 jupyter = [
     "jupyterlab",
     "python-graphviz",
 ]
-gurobi = [
-    "gurobi",
-]
 
 [project.scripts]
 mach2 = "mach2.mach:main"
 
 [project.urls]
 Homepage = "https://github.com/elkebir-group/MACH2"
 "Bug Tracker" = "https://github.com/elkebir-group/MACH2/issues"
```

### Comparing `mach2-0.0.1/src/mach2/clonetree.py` & `mach2-0.0.2/src/mach2/clonetree.py`

 * *Files identical despite different names*

### Comparing `mach2-0.0.1/src/mach2/mach.py` & `mach2-0.0.2/src/mach2/mach.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
     parser.add_argument('-S', '--seeding_sites', action='store_true', default=False, help='Minimizes the number of seeding sites \
         too (default=False)')
 
     return parser.parse_args()
 
 def main():
     args = process_args()
-    clone_tree = CloneTree.from_file(args.clone_tree, args.leaf_labeling, primary_site=args.primary)
+    clone_tree = CloneTree.from_file(args.clone_tree, args.leaf_labeling)
 
     if args.output is None:
         output_str = '.'
     else:
         output_str = args.output
         if not os.path.exists(output_str):
             os.makedirs(output_str)
```

### Comparing `mach2-0.0.1/src/mach2/migrationgraph.py` & `mach2-0.0.2/src/mach2/migrationgraph.py`

 * *Files identical despite different names*

### Comparing `mach2-0.0.1/src/mach2/solutionset.py` & `mach2-0.0.2/src/mach2/solutionset.py`

 * *Files identical despite different names*

