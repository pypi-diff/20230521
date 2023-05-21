# Comparing `tmp/arulespy-0.0.2.tar.gz` & `tmp/arulespy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arulespy-0.0.2.tar", last modified: Tue May 16 17:32:07 2023, max compression
+gzip compressed data, was "arulespy-0.1.0.tar", last modified: Sun May 21 01:35:21 2023, max compression
```

## Comparing `arulespy-0.0.2.tar` & `arulespy-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:32:07.760475 arulespy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-16 17:31:58.000000 arulespy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 17:31:58.000000 arulespy-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-16 17:32:07.760475 arulespy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-16 17:31:58.000000 arulespy-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 17:31:58.000000 arulespy-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 17:32:07.760475 arulespy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-16 17:31:58.000000 arulespy-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:32:07.760475 arulespy-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:32:07.760475 arulespy-0.0.2/src/arulespy/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-16 17:31:58.000000 arulespy-0.0.2/src/arulespy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-16 17:31:58.000000 arulespy-0.0.2/src/arulespy/arules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-16 17:31:58.000000 arulespy-0.0.2/src/arulespy/arulesViz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:32:07.760475 arulespy-0.0.2/src/arulespy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-16 17:32:07.000000 arulespy-0.0.2/src/arulespy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-16 17:32:07.000000 arulespy-0.0.2/src/arulespy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:32:07.000000 arulespy-0.0.2/src/arulespy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 17:32:07.000000 arulespy-0.0.2/src/arulespy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 17:32:07.000000 arulespy-0.0.2/src/arulespy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:32:07.760475 arulespy-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-16 17:31:58.000000 arulespy-0.0.2/tests/test_arules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:35:21.281930 arulespy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-21 01:35:07.000000 arulespy-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-21 01:35:07.000000 arulespy-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-05-21 01:35:21.281930 arulespy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-05-21 01:35:07.000000 arulespy-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 01:35:07.000000 arulespy-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-21 01:35:21.281930 arulespy-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-21 01:35:07.000000 arulespy-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:35:21.273930 arulespy-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:35:21.277930 arulespy-0.1.0/src/arulespy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-21 01:35:07.000000 arulespy-0.1.0/src/arulespy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-05-21 01:35:07.000000 arulespy-0.1.0/src/arulespy/arules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-21 01:35:07.000000 arulespy-0.1.0/src/arulespy/arulesViz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:35:21.281930 arulespy-0.1.0/src/arulespy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-05-21 01:35:21.000000 arulespy-0.1.0/src/arulespy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-21 01:35:21.000000 arulespy-0.1.0/src/arulespy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 01:35:21.000000 arulespy-0.1.0/src/arulespy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-21 01:35:21.000000 arulespy-0.1.0/src/arulespy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 01:35:21.000000 arulespy-0.1.0/src/arulespy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:35:21.281930 arulespy-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-21 01:35:07.000000 arulespy-0.1.0/tests/test_arules.py
```

### Comparing `arulespy-0.0.2/LICENSE` & `arulespy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arulespy-0.0.2/PKG-INFO` & `arulespy-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arulespy
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python interface to the R package arules
 Home-page: https://github.com/mhahsler/arulespy
 Author: Michael Hahsler
 Author-email: mhahsler@lyle.smu.edu
 Project-URL: Documentation, https://github.com/mhahsler/arulespy
 Project-URL: Bug Reports, https://github.com/mhahsler/arulespy/issues
 Project-URL: Source Code, https://github.com/mhahsler/arulespy
@@ -50,14 +50,15 @@
 
 `arulespy` provides Python classes
 for
 
 -   `Transactions`: Convert pandas dataframes into transaction data
 -   `Rules`: Association rules
 -   `Itemsets`: Itemsets
+-   `ItemMatrix`: sparse matrix representation of sets of items.
 
 with Phyton-style slicing and `len()`. 
 
 Most arules functions are
 interfaced with conversion from the R data structures to Python.
 Documentation is avaialible in Python via `help()`. Detailed online documentation
 for the R package is available [here](https://mhahsler.r-universe.dev/arules/doc/manual.html). 
@@ -74,36 +75,42 @@
 1. Install the latest version of R from https://www.r-project.org/
 
 2. Install required libraries/set path depending on your OS:
    - libcurl is needed by R package [curl](https://cran.r-project.org/web/packages/curl/index.html).
       - Ubuntu: `sudo apt-get install libcurl4-openssl-dev`
       - MacOS: `brew install curl`
       - Windows: no installation necessary
-   - Environment variable `R_HOME` needs to be set for Windows
+   - Environment variable `R_HOME` may need to be set for Windows
 
 3. Install `arulespy` which will automatically install `rpy2` and `pandas`.
     ``` sh
     pip install arulespy
     ```
 
-4. Optional: Set the environment variable `R_LIBS` to decide where R packages are stored. If not set then 
-  R will determine a suitable location.
+4. Optional: Set the environment variable `R_LIBS_USER` to decide where R packages are stored 
+    (see [libPaths()](https://stat.ethz.ch/R-manual/R-devel/library/base/html/libPaths.html) for details). If not set then R will determine a suitable location.
 
+5. Optional: `arulespy` will install the needed R packages when it is imported for the first time.
+    This may take a while. R packages can also be preinstalled. Start R and run 
+    `install.packages(c("arules", "arulesViz"))`
 
-The most likely issue is `rpy2`. Check `python -m rpy2.situation` to see if R and R's libraries are found.
+
+The most likely issue is that `rpy2` does not find R. 
+This will lead the python kernel to die or exit without explanation when the package `arulespy` is imported.
+Check `python -m rpy2.situation` to see if R and R's libraries are found.
 Details can be found [here](https://pypi.org/project/rpy2/).
 
 
 ## Example
 
 ``` python
 from arulespy import arules
-
 import pandas as pd
 
+# define the data as a pandas dataframe
 df = pd.DataFrame (
     [
         [True,True, True],
         [True, False,False],
         [True, True, True],
         [True, False, False],
         [True, True, True]
@@ -114,15 +121,15 @@
 trans = arules.transactions(df)
 
 # mine association rules
 rules = arules.apriori(trans,
                     parameter = arules.parameters({"supp": 0.1, "conf": 0.8}), 
                     control = arules.parameters({"verbose": False}))  
 
-# display the rules
+# display the rules as a pandas dataframe
 rules.as_df()
 ```
 
 ```
 	LHS	    RHS     support	confidence	coverage	lift	count
 1	{}      {A}	    1.0     1.0	        1.0	        1.000000	5
 2	{B}     {C}	    0.6	    1.0	        0.6	        1.666667	3
```

### Comparing `arulespy-0.0.2/README.md` & `arulespy-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 `arulespy` provides Python classes
 for
 
 -   `Transactions`: Convert pandas dataframes into transaction data
 -   `Rules`: Association rules
 -   `Itemsets`: Itemsets
+-   `ItemMatrix`: sparse matrix representation of sets of items.
 
 with Phyton-style slicing and `len()`. 
 
 Most arules functions are
 interfaced with conversion from the R data structures to Python.
 Documentation is avaialible in Python via `help()`. Detailed online documentation
 for the R package is available [here](https://mhahsler.r-universe.dev/arules/doc/manual.html). 
@@ -49,36 +50,42 @@
 1. Install the latest version of R from https://www.r-project.org/
 
 2. Install required libraries/set path depending on your OS:
    - libcurl is needed by R package [curl](https://cran.r-project.org/web/packages/curl/index.html).
       - Ubuntu: `sudo apt-get install libcurl4-openssl-dev`
       - MacOS: `brew install curl`
       - Windows: no installation necessary
-   - Environment variable `R_HOME` needs to be set for Windows
+   - Environment variable `R_HOME` may need to be set for Windows
 
 3. Install `arulespy` which will automatically install `rpy2` and `pandas`.
     ``` sh
     pip install arulespy
     ```
 
-4. Optional: Set the environment variable `R_LIBS` to decide where R packages are stored. If not set then 
-  R will determine a suitable location.
+4. Optional: Set the environment variable `R_LIBS_USER` to decide where R packages are stored 
+    (see [libPaths()](https://stat.ethz.ch/R-manual/R-devel/library/base/html/libPaths.html) for details). If not set then R will determine a suitable location.
 
+5. Optional: `arulespy` will install the needed R packages when it is imported for the first time.
+    This may take a while. R packages can also be preinstalled. Start R and run 
+    `install.packages(c("arules", "arulesViz"))`
 
-The most likely issue is `rpy2`. Check `python -m rpy2.situation` to see if R and R's libraries are found.
+
+The most likely issue is that `rpy2` does not find R. 
+This will lead the python kernel to die or exit without explanation when the package `arulespy` is imported.
+Check `python -m rpy2.situation` to see if R and R's libraries are found.
 Details can be found [here](https://pypi.org/project/rpy2/).
 
 
 ## Example
 
 ``` python
 from arulespy import arules
-
 import pandas as pd
 
+# define the data as a pandas dataframe
 df = pd.DataFrame (
     [
         [True,True, True],
         [True, False,False],
         [True, True, True],
         [True, False, False],
         [True, True, True]
@@ -89,15 +96,15 @@
 trans = arules.transactions(df)
 
 # mine association rules
 rules = arules.apriori(trans,
                     parameter = arules.parameters({"supp": 0.1, "conf": 0.8}), 
                     control = arules.parameters({"verbose": False}))  
 
-# display the rules
+# display the rules as a pandas dataframe
 rules.as_df()
 ```
 
 ```
 	LHS	    RHS     support	confidence	coverage	lift	count
 1	{}      {A}	    1.0     1.0	        1.0	        1.000000	5
 2	{B}     {C}	    0.6	    1.0	        0.6	        1.666667	3
```

### Comparing `arulespy-0.0.2/setup.py` & `arulespy-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `arulespy-0.0.2/src/arulespy/arulesViz.py` & `arulespy-0.1.0/src/arulespy/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-"""The arules module provides an interface to R's arules package."""
-
-import pandas as pd
-import numpy as np
+__version__ = '0.1.0'
 
 import rpy2.robjects as ro
 import rpy2.robjects.packages as packages
-from rpy2.robjects import pandas2ri
-
-### activate automatic conversion of pandas dataframes to R dataframes
-#pandas2ri.activate()
-
-
-
-
-# install arules if necessary. Note: the system path is probably not writable for the user.
 import os
+
 os.makedirs(ro.r('Sys.getenv("R_LIBS_USER")')[0], exist_ok=True)
 ro.r('.libPaths(c(Sys.getenv("R_LIBS_USER"), .libPaths()))')
 
 utils = packages.importr('utils')
+if not ro.packages.isinstalled('arules'):
+    print("Installing R package arules.")
+    utils.install_packages('arules', 
+                           repos='https://cloud.r-project.org/',
+                           lib = ro.r('Sys.getenv("R_LIBS_USER")[1]'))
+    
+
 if not ro.packages.isinstalled('arulesViz'):
-    print("Installing R package arulesViz.")
+    print("Installing R package arulesViz (plus dependencies).")
     utils.install_packages('arulesViz', 
                            repos='https://cloud.r-project.org/',
                            lib = ro.r('Sys.getenv("R_LIBS_USER")[1]'))
 
-r = packages.importr('arulesViz')
-
-# get the generic for plot
-base = packages.importr('base')
-plot = base.plot
-#plot.__doc__ = r.plot.__doc__
-
-inspectDT = r.inspectDT
-#inspectDT.__doc__ = r.inspectDT.__doc__
-
 
+from .arules import parameters, set, Associations, ItemMatrix, Rules, Itemsets, Transactions, R, a2p, encode, concat, apriori, eclat, discretizeDF, random_transactions                 
+from .arulesViz import plot, inspectDT
```

### Comparing `arulespy-0.0.2/src/arulespy.egg-info/PKG-INFO` & `arulespy-0.1.0/src/arulespy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arulespy
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python interface to the R package arules
 Home-page: https://github.com/mhahsler/arulespy
 Author: Michael Hahsler
 Author-email: mhahsler@lyle.smu.edu
 Project-URL: Documentation, https://github.com/mhahsler/arulespy
 Project-URL: Bug Reports, https://github.com/mhahsler/arulespy/issues
 Project-URL: Source Code, https://github.com/mhahsler/arulespy
@@ -50,14 +50,15 @@
 
 `arulespy` provides Python classes
 for
 
 -   `Transactions`: Convert pandas dataframes into transaction data
 -   `Rules`: Association rules
 -   `Itemsets`: Itemsets
+-   `ItemMatrix`: sparse matrix representation of sets of items.
 
 with Phyton-style slicing and `len()`. 
 
 Most arules functions are
 interfaced with conversion from the R data structures to Python.
 Documentation is avaialible in Python via `help()`. Detailed online documentation
 for the R package is available [here](https://mhahsler.r-universe.dev/arules/doc/manual.html). 
@@ -74,36 +75,42 @@
 1. Install the latest version of R from https://www.r-project.org/
 
 2. Install required libraries/set path depending on your OS:
    - libcurl is needed by R package [curl](https://cran.r-project.org/web/packages/curl/index.html).
       - Ubuntu: `sudo apt-get install libcurl4-openssl-dev`
       - MacOS: `brew install curl`
       - Windows: no installation necessary
-   - Environment variable `R_HOME` needs to be set for Windows
+   - Environment variable `R_HOME` may need to be set for Windows
 
 3. Install `arulespy` which will automatically install `rpy2` and `pandas`.
     ``` sh
     pip install arulespy
     ```
 
-4. Optional: Set the environment variable `R_LIBS` to decide where R packages are stored. If not set then 
-  R will determine a suitable location.
+4. Optional: Set the environment variable `R_LIBS_USER` to decide where R packages are stored 
+    (see [libPaths()](https://stat.ethz.ch/R-manual/R-devel/library/base/html/libPaths.html) for details). If not set then R will determine a suitable location.
 
+5. Optional: `arulespy` will install the needed R packages when it is imported for the first time.
+    This may take a while. R packages can also be preinstalled. Start R and run 
+    `install.packages(c("arules", "arulesViz"))`
 
-The most likely issue is `rpy2`. Check `python -m rpy2.situation` to see if R and R's libraries are found.
+
+The most likely issue is that `rpy2` does not find R. 
+This will lead the python kernel to die or exit without explanation when the package `arulespy` is imported.
+Check `python -m rpy2.situation` to see if R and R's libraries are found.
 Details can be found [here](https://pypi.org/project/rpy2/).
 
 
 ## Example
 
 ``` python
 from arulespy import arules
-
 import pandas as pd
 
+# define the data as a pandas dataframe
 df = pd.DataFrame (
     [
         [True,True, True],
         [True, False,False],
         [True, True, True],
         [True, False, False],
         [True, True, True]
@@ -114,15 +121,15 @@
 trans = arules.transactions(df)
 
 # mine association rules
 rules = arules.apriori(trans,
                     parameter = arules.parameters({"supp": 0.1, "conf": 0.8}), 
                     control = arules.parameters({"verbose": False}))  
 
-# display the rules
+# display the rules as a pandas dataframe
 rules.as_df()
 ```
 
 ```
 	LHS	    RHS     support	confidence	coverage	lift	count
 1	{}      {A}	    1.0     1.0	        1.0	        1.000000	5
 2	{B}     {C}	    0.6	    1.0	        0.6	        1.666667	3
```

### Comparing `arulespy-0.0.2/tests/test_arules.py` & `arulespy-0.1.0/tests/test_arules.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import pandas as pd
-from arulespy import arules
 
+from arulespy.arules import Transactions, apriori, parameters
 
 class TestArules(unittest.TestCase):
 
     def test_transactions(self):       
         df = pd.DataFrame (
             [
                 [True,True, True],
@@ -18,22 +18,22 @@
                 [True, True, True],
                 [False, False, True],
                 [False, True, True],
                 [True, False, True],
             ],
         columns=list ('ABC')) 
         
-        trans = arules.transactions(df)
+        trans = Transactions.from_df(df)
         self.assertEqual(len(trans), 10)
 
-        self.assertEqual(len(arules.unique(trans)), 5)
+        self.assertEqual(len(trans.unique()), 5)
 
-        rules = arules.apriori(trans,
-                    parameter = arules.parameters({"supp": 0.1, "conf": 0.8}), 
-                    control = arules.parameters({"verbose": False})) 
+        rules = apriori(trans,
+                    parameter = parameters({"supp": 0.1, "conf": 0.8}), 
+                    control = parameters({"verbose": False})) 
         self.assertEqual(len(rules), 6)
 
         self.assertEqual(len(rules[1:4]), 3)
 
         self.assertEqual(type(rules.as_df()), pd.DataFrame)
```

