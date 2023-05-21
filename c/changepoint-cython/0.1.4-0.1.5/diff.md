# Comparing `tmp/changepoint_cython-0.1.4.tar.gz` & `tmp/changepoint_cython-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changepoint_cython-0.1.4.tar", max compression
+gzip compressed data, was "changepoint_cython-0.1.5.tar", max compression
```

## Comparing `changepoint_cython-0.1.4.tar` & `changepoint_cython-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-05-21 14:15:30.689733 changepoint_cython-0.1.4/LICENSE
--rw-r--r--   0        0        0     4474 2023-05-21 14:15:30.689733 changepoint_cython-0.1.4/README.md
--rw-r--r--   0        0        0     1577 2023-05-21 14:15:30.689733 changepoint_cython-0.1.4/build.py
--rw-r--r--   0        0        0       67 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/__init__.py
--rw-r--r--   0        0        0     5733 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/algo_changepoints.py
--rw-r--r--   0        0        0     3684 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/cost_function.pxd
--rw-r--r--   0        0        0     1289 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/cost_function_multiple.pxd
--rw-r--r--   0        0        0   220882 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/mutiple_algos.html
--rw-r--r--   0        0        0     7734 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/mutiple_algos.pyx
--rw-r--r--   0        0        0     3850 2023-05-21 14:15:30.701733 changepoint_cython-0.1.4/pychangepoints/nppelt.pyx
--rw-r--r--   0        0        0   236694 2023-05-21 14:15:30.705733 changepoint_cython-0.1.4/pychangepoints/pelt_cython.html
--rw-r--r--   0        0        0    11409 2023-05-21 14:15:30.705733 changepoint_cython-0.1.4/pychangepoints/pelt_cython.pyx
--rw-r--r--   0        0        0      499 2023-05-21 14:15:30.705733 changepoint_cython-0.1.4/pychangepoints/utils.pxd
--rw-r--r--   0        0        0      847 2023-05-21 14:15:30.705733 changepoint_cython-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 changepoint_cython-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-21 14:33:12.626611 changepoint_cython-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4474 2023-05-21 14:33:12.626611 changepoint_cython-0.1.5/README.md
+-rw-r--r--   0        0        0     1577 2023-05-21 14:33:12.626611 changepoint_cython-0.1.5/build.py
+-rw-r--r--   0        0        0       67 2023-05-21 14:33:12.638611 changepoint_cython-0.1.5/pychangepoints/__init__.py
+-rw-r--r--   0        0        0     5733 2023-05-21 14:33:12.638611 changepoint_cython-0.1.5/pychangepoints/algo_changepoints.py
+-rw-r--r--   0        0        0     3684 2023-05-21 14:33:12.638611 changepoint_cython-0.1.5/pychangepoints/cost_function.pxd
+-rw-r--r--   0        0        0     1289 2023-05-21 14:33:12.638611 changepoint_cython-0.1.5/pychangepoints/cost_function_multiple.pxd
+-rw-r--r--   0        0        0   220882 2023-05-21 14:33:12.642611 changepoint_cython-0.1.5/pychangepoints/mutiple_algos.html
+-rw-r--r--   0        0        0     7734 2023-05-21 14:33:12.642611 changepoint_cython-0.1.5/pychangepoints/mutiple_algos.pyx
+-rw-r--r--   0        0        0     3850 2023-05-21 14:33:12.642611 changepoint_cython-0.1.5/pychangepoints/nppelt.pyx
+-rw-r--r--   0        0        0   236694 2023-05-21 14:33:12.642611 changepoint_cython-0.1.5/pychangepoints/pelt_cython.html
+-rw-r--r--   0        0        0    11409 2023-05-21 14:33:12.642611 changepoint_cython-0.1.5/pychangepoints/pelt_cython.pyx
+-rw-r--r--   0        0        0      499 2023-05-21 14:33:12.642611 changepoint_cython-0.1.5/pychangepoints/utils.pxd
+-rw-r--r--   0        0        0      889 2023-05-21 14:33:12.642611 changepoint_cython-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 changepoint_cython-0.1.5/PKG-INFO
```

### Comparing `changepoint_cython-0.1.4/LICENSE` & `changepoint_cython-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/README.md` & `changepoint_cython-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/build.py` & `changepoint_cython-0.1.5/build.py`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/pychangepoints/algo_changepoints.py` & `changepoint_cython-0.1.5/pychangepoints/algo_changepoints.py`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/pychangepoints/cost_function.pxd` & `changepoint_cython-0.1.5/pychangepoints/cost_function.pxd`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/pychangepoints/cost_function_multiple.pxd` & `changepoint_cython-0.1.5/pychangepoints/cost_function_multiple.pxd`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/pychangepoints/mutiple_algos.html` & `changepoint_cython-0.1.5/pychangepoints/mutiple_algos.html`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/pychangepoints/mutiple_algos.pyx` & `changepoint_cython-0.1.5/pychangepoints/mutiple_algos.pyx`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/pychangepoints/nppelt.pyx` & `changepoint_cython-0.1.5/pychangepoints/nppelt.pyx`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/pychangepoints/pelt_cython.html` & `changepoint_cython-0.1.5/pychangepoints/pelt_cython.html`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/pychangepoints/pelt_cython.pyx` & `changepoint_cython-0.1.5/pychangepoints/pelt_cython.pyx`

 * *Files identical despite different names*

### Comparing `changepoint_cython-0.1.4/pyproject.toml` & `changepoint_cython-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "changepoint-cython"
-version = "0.1.4"
+version = "0.1.5"
 description = "A cython version of the changepoint R package"
 authors = ["Vianney Bruned"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 packages = [{include = "pychangepoints"}]
 include = [{ path = "pychangepoints/**/*.so", format = "wheel" }]
 
@@ -12,14 +12,15 @@
 python = "^3.8,<3.11"
 pandas = "^1.2.5"
 scikit-learn = "^1.2.0"
 
 
 [build-system]
 requires = ["poetry-core", "Cython~=0.29.34", "numpy>=1.22.1"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.build]
 generate-setup-file = false
 script = "build.py"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `changepoint_cython-0.1.4/PKG-INFO` & `changepoint_cython-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changepoint-cython
-Version: 0.1.4
+Version: 0.1.5
 Summary: A cython version of the changepoint R package
 License: GNU General Public License v3.0
 Author: Vianney Bruned
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

