# Comparing `tmp/politely-3.3.0.tar.gz` & `tmp/politely-3.3.1.tar.gz`

## Comparing `politely-3.3.0.tar` & `politely-3.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 politely-3.3.0/politely/__init__.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 politely-3.3.0/politely/errors.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 politely-3.3.0/politely/fetchers.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 politely-3.3.0/politely/modeling_gpt2_scorer.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 politely-3.3.0/politely/modeling_heuristic_scorer.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 politely-3.3.0/politely/modeling_scorer.py
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 politely-3.3.0/politely/rules.py
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 politely-3.3.0/politely/styler.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 politely-3.3.0/.gitignore
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 politely-3.3.0/README.md
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 politely-3.3.0/pyproject.toml
--rw-r--r--   0        0        0    11037 2020-02-02 00:00:00.000000 politely-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 politely-3.3.1/politely/__init__.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 politely-3.3.1/politely/errors.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 politely-3.3.1/politely/fetchers.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 politely-3.3.1/politely/modeling_gpt2_scorer.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 politely-3.3.1/politely/modeling_heuristic_scorer.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 politely-3.3.1/politely/modeling_scorer.py
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 politely-3.3.1/politely/rules.py
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 politely-3.3.1/politely/styler.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 politely-3.3.1/.gitignore
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 politely-3.3.1/README.md
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 politely-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 politely-3.3.1/PKG-INFO
```

### Comparing `politely-3.3.0/politely/errors.py` & `politely-3.3.1/politely/errors.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.0/politely/fetchers.py` & `politely-3.3.1/politely/fetchers.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.0/politely/modeling_gpt2_scorer.py` & `politely-3.3.1/politely/modeling_gpt2_scorer.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.0/politely/modeling_heuristic_scorer.py` & `politely-3.3.1/politely/modeling_heuristic_scorer.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.0/politely/rules.py` & `politely-3.3.1/politely/rules.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.0/politely/styler.py` & `politely-3.3.1/politely/styler.py`

 * *Files identical despite different names*

### Comparing `politely-3.3.0/.gitignore` & `politely-3.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `politely-3.3.0/README.md` & `politely-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `politely-3.3.0/pyproject.toml` & `politely-3.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,17 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = [
   "cmake>=3.25.2",
-  "kiwipiepy>=0.14.1"
+  "kiwipiepy>=0.14.1",
+  "transformers>=4.29.1",
+  "torch>=2.0.1"
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/unknown/politely#readme"
 Issues = "https://github.com/unknown/politely/issues"
```

### Comparing `politely-3.3.0/PKG-INFO` & `politely-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: politely
-Version: 3.3.0
+Version: 3.3.1
 Summary: A rule-based politeness styler for the Korean Language
 Project-URL: Documentation, https://github.com/unknown/politely#readme
 Project-URL: Issues, https://github.com/unknown/politely/issues
 Project-URL: Source, https://github.com/unknown/politely
 Author-email: Eu-Bin KIM <tlrndk123@gmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: cmake>=3.25.2
 Requires-Dist: kiwipiepy>=0.14.1
+Requires-Dist: torch>=2.0.1
+Requires-Dist: transformers>=4.29.1
 Description-Content-Type: text/markdown
 
 # Politely
 
 [![PyPI version](https://badge.fury.io/py/politely.svg)](https://badge.fury.io/py/politely)
 ![Workflow status](https://github.com/eubinecto/politely/actions/workflows/tests.yml/badge.svg)
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://eubinecto-politely-main-streamlit-4vmces.streamlitapp.com)
```

