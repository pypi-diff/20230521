# Comparing `tmp/pykantorovich-0.1.0.tar.gz` & `tmp/pykantorovich-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykantorovich-0.1.0.tar", max compression
+gzip compressed data, was "pykantorovich-0.2.0.tar", max compression
```

## Comparing `pykantorovich-0.1.0.tar` & `pykantorovich-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-05-11 07:25:26.638678 pykantorovich-0.1.0/LICENSE
--rw-r--r--   0        0        0      254 2023-05-11 08:06:13.729835 pykantorovich-0.1.0/README.md
--rw-r--r--   0        0        0       25 2023-05-11 07:32:00.086057 pykantorovich-0.1.0/pykantorovich/__init__.py
--rw-r--r--   0        0        0    10709 2023-05-11 07:29:05.876103 pykantorovich-0.1.0/pykantorovich/kantorovich.py
--rw-r--r--   0        0        0     1114 2023-05-11 08:00:43.221696 pykantorovich-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 pykantorovich-0.1.0/setup.py
--rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 pykantorovich-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-11 07:25:26.638678 pykantorovich-0.2.0/LICENSE
+-rw-r--r--   0        0        0      254 2023-05-11 08:06:13.729835 pykantorovich-0.2.0/README.md
+-rw-r--r--   0        0        0       25 2023-05-21 12:01:28.846836 pykantorovich-0.2.0/pykantorovich/__init__.py
+-rw-r--r--   0        0        0    10733 2023-05-21 12:00:50.855252 pykantorovich-0.2.0/pykantorovich/kantorovich.py
+-rw-r--r--   0        0        0     1114 2023-05-21 12:01:43.774672 pykantorovich-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 pykantorovich-0.2.0/setup.py
+-rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 pykantorovich-0.2.0/PKG-INFO
```

### Comparing `pykantorovich-0.1.0/LICENSE` & `pykantorovich-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykantorovich-0.1.0/pykantorovich/kantorovich.py` & `pykantorovich-0.2.0/pykantorovich/kantorovich.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     
 def _kantorovich_cdd(
     mu, nu, number_type="fraction", distance_matrix="0-1", prettyprint=True
 ):
     mat, n = _makeH(mu, nu, number_type)
     mat.obj_type = cdd.LPObjType.MIN
-    if distance_matrix == "0-1":
+    if type(distance_matrix) == str:
         d = np.ones((n, n), dtype=int)
         np.fill_diagonal(d, 0)
         d = d.flatten()
     else:
         d = distance_matrix.flatten()
     d = np.concatenate(([0], d))
     mat.obj_func = d
@@ -61,19 +61,14 @@
         "\n}")
     return {
         "distance": lp.obj_value,
         "joining": np.reshape(sol, (n, n)),
         "optimal": "yes" if lp.status == cdd.LPStatusType.OPTIMAL else "no" 
     }
 
-mu = ['1/7','2/7','4/7']
-nu = ['1/4','1/4','1/2']
-
-# mu = ['1/2','1/4','1/4']
-# nu = ['1/4','1/4','1/2']
 
 def extreme_joinings(mu, nu, number_type="fraction", prettyprint=True):
     """
     Extreme joinings of two probabiity measures.
 
     Parameters
     ----------
@@ -163,15 +158,15 @@
     B = sparse.csr_matrix(np.ones(n, dtype = int))
     M1 = sparse.kron(A, B)
     M2 = sparse.hstack([eyen]*n, dtype=int)
     M = sparse.vstack([M1, M2])
     a1 = sparse.eye(n2, dtype = int)
     b1 = np.zeros(n2, dtype=int)
     b2 = np.concatenate((mu, nu))
-    if distance_matrix == "0-1":
+    if type(distance_matrix) == str:
         d = np.ones((n, n), dtype=int)
         np.fill_diagonal(d, 0)
         d = d.flatten()
     else:
         d = distance_matrix.flatten()
     res = linprog(
         d, A_ub = -a1, b_ub = b1, A_eq = M, b_eq = b2, 
@@ -179,31 +174,25 @@
     )
     return {
         "distance": res.fun,
         "joining": np.reshape(res.x, (n,n)),
         "message": res.message
     }
 
-# mu = [1/7,2/7,4/7]
-# nu = [1/4,1/4,1/2]
-
 
 def _kantorovich_cvx(mu, nu, distance_matrix = "0-1"):
     n = len(mu)
-    n2 = n*n
     eyen = np.eye(n, dtype = int)    
     A = eyen
     nones = np.ones(n, dtype = int)
     M1 = np.kron(A, nones)
     M2 = np.tile(np.diag(nones), n)
     M = np.vstack((M1, M2))
-    a1 = np.eye(n2, dtype = int)
-    b1 = np.zeros(n2, dtype=int)
     b2 = np.concatenate((mu, nu))
-    if distance_matrix == "0-1":
+    if type(distance_matrix) == str:
         d = np.ones((n, n), dtype=int)
         np.fill_diagonal(d, 0)
         d = d.flatten()
     else:
         d = distance_matrix.flatten()
     p = cp.Variable(n*n)
     constraints = [M @ p == b2, p >= 0]
@@ -267,19 +256,26 @@
     -------
     The Kantorovich distance between `mu` and `nu` and a joining of `mu` and 
     `nu` for which the Kantorovich distance is the probability that the two 
     margins differ.
     
     Examples
     --------
+    >>> from pykantorovich.kantorovich import kantorovich
+    >>> import numpy as np
     >>> mu = ['1/7','2/7','4/7']
     >>> nu = ['1/4','1/4','1/2']
-    >>> kantorovich(mu, nu)
+    >>> d = np.array([
+    ...   ['0', '1', '2'],    
+    ...   ['1', '0', '1'],    
+    ...   ['2', '1', '0']
+    ... ], dtype = "f")
+    >>> kantorovich(mu, nu, distance_matrix=d)
     {
-     distance: 3/28 
+     distance: 5/28 
      joining:
      [['1/7' '0' '0']
      ['1/28' '1/4' '0']
      ['1/14' '0' '1/2']] 
      optimal: yes 
     }
 
@@ -305,15 +301,15 @@
             raise ValueError("`mu` is not made of numbers.")
         if not np.all(np.frompyfunc(_is_number, 1, 1)(nu)):
             raise ValueError("`nu` is not made of numbers.")
         if not isclose(np.sum(mu), 1.0):
             raise ValueError("`mu` does not sum to one.")
         if not isclose(np.sum(nu), 1.0):
             raise ValueError("`nu` does not sum to one.")
-    if distance_matrix != "0-1":
+    if type(distance_matrix) != str:
         distance_matrix = np.asarray(distance_matrix)
         if distance_matrix.shape != (n, n):
             raise ValueError(f"The distance matrix must be square, with {n} rows and {n} columns.") 
         type_d = distance_matrix.dtype.kind
         if type_d != "f" and type_d != "i":
             raise ValueError("The distance matrix is not a matrix of numbers.")
     if method != "cdd" and method != "sparse" and method != "cvx":
```

### Comparing `pykantorovich-0.1.0/pyproject.toml` & `pykantorovich-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "PyKantorovich"
 packages = [
     { include = "pykantorovich" },
 ]
-version = "0.1.0"
+version = "0.2.0"
 description = "Kantorovich distance between probabilities on a finite space."
 homepage = "https://github.com/stla/PyKantorovich"
 authors = ["Stéphane Laurent <laurent_step@outlook.fr>"]
 documentation = "https://pykantorovich.readthedocs.io/en/latest/"
 keywords = ["Kantorovich distance", "linear programming"]
 license = "GPL-3.0-only"
 readme = "README.md"
```

### Comparing `pykantorovich-0.1.0/setup.py` & `pykantorovich-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'docs': ['sphinx>=5.3.0,<6.0.0',
           'sphinx-rtd-theme>=1.1.1,<2.0.0',
           'sphinxcontrib-napoleon>=0.7,<0.8',
           'sphinxcontrib-restbuilder>=0.3,<0.4']}
 
 setup_kwargs = {
     'name': 'pykantorovich',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'Kantorovich distance between probabilities on a finite space.',
     'long_description': '# PyKantorovich\n\n<!-- badges: start -->\n[![Documentation status](https://readthedocs.org/projects/pykantorovich/badge/)](http://pykantorovich.readthedocs.io)\n<!-- badges: end -->\n\nKantorovich distance with Python.\n\n___\n\n```\npip install pykantorovich\n```\n',
     'author': 'Stéphane Laurent',
     'author_email': 'laurent_step@outlook.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/stla/PyKantorovich',
```

### Comparing `pykantorovich-0.1.0/PKG-INFO` & `pykantorovich-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykantorovich
-Version: 0.1.0
+Version: 0.2.0
 Summary: Kantorovich distance between probabilities on a finite space.
 Home-page: https://github.com/stla/PyKantorovich
 License: GPL-3.0-only
 Keywords: Kantorovich distance,linear programming
 Author: Stéphane Laurent
 Author-email: laurent_step@outlook.fr
 Requires-Python: >=3.7.1,<3.10
```

