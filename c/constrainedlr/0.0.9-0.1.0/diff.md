# Comparing `tmp/constrainedlr-0.0.9.tar.gz` & `tmp/constrainedlr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constrainedlr-0.0.9.tar", last modified: Sun May 21 15:17:49 2023, max compression
+gzip compressed data, was "constrainedlr-0.1.0.tar", last modified: Sun May 21 15:35:18 2023, max compression
```

## Comparing `constrainedlr-0.0.9.tar` & `constrainedlr-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:17:49.191474 constrainedlr-0.0.9/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrainedlr-0.0.9/LICENCE
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2161 2023-05-21 15:17:49.173475 constrainedlr-0.0.9/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1205 2023-05-21 15:16:34.000000 constrainedlr-0.0.9/README.md
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1304 2023-05-21 15:16:34.000000 constrainedlr-0.0.9/pyproject.toml
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-21 15:17:49.193462 constrainedlr-0.0.9/setup.cfg
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:17:48.373349 constrainedlr-0.0.9/src/
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:17:48.691398 constrainedlr-0.0.9/src/constrainedlr/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       61 2023-05-14 19:35:04.000000 constrainedlr-0.0.9/src/constrainedlr/__init__.py
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     4011 2023-05-21 15:16:34.000000 constrainedlr-0.0.9/src/constrainedlr/model.py
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:17:49.051463 constrainedlr-0.0.9/src/constrainedlr.egg-info/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2161 2023-05-21 15:17:47.000000 constrainedlr-0.0.9/src/constrainedlr.egg-info/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      311 2023-05-21 15:17:48.000000 constrainedlr-0.0.9/src/constrainedlr.egg-info/SOURCES.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-21 15:17:47.000000 constrainedlr-0.0.9/src/constrainedlr.egg-info/dependency_links.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-21 15:17:48.000000 constrainedlr-0.0.9/src/constrainedlr.egg-info/requires.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       14 2023-05-21 15:17:48.000000 constrainedlr-0.0.9/src/constrainedlr.egg-info/top_level.txt
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:17:49.094476 constrainedlr-0.0.9/tests/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3585 2023-05-21 15:16:34.000000 constrainedlr-0.0.9/tests/test_fit.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:35:18.743839 constrainedlr-0.1.0/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrainedlr-0.1.0/LICENCE
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2165 2023-05-21 15:35:18.738841 constrainedlr-0.1.0/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1209 2023-05-21 15:22:40.000000 constrainedlr-0.1.0/README.md
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1304 2023-05-21 15:34:06.000000 constrainedlr-0.1.0/pyproject.toml
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-21 15:35:18.745840 constrainedlr-0.1.0/setup.cfg
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:35:18.276847 constrainedlr-0.1.0/src/
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:35:18.467857 constrainedlr-0.1.0/src/constrainedlr/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       61 2023-05-21 15:30:34.000000 constrainedlr-0.1.0/src/constrainedlr/__init__.py
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     4246 2023-05-21 15:32:15.000000 constrainedlr-0.1.0/src/constrainedlr/model.py
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      774 2023-05-21 15:31:21.000000 constrainedlr-0.1.0/src/constrainedlr/validation.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:35:18.668841 constrainedlr-0.1.0/src/constrainedlr.egg-info/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2165 2023-05-21 15:35:18.000000 constrainedlr-0.1.0/src/constrainedlr.egg-info/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      343 2023-05-21 15:35:18.000000 constrainedlr-0.1.0/src/constrainedlr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-21 15:35:18.000000 constrainedlr-0.1.0/src/constrainedlr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-21 15:35:18.000000 constrainedlr-0.1.0/src/constrainedlr.egg-info/requires.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       14 2023-05-21 15:35:18.000000 constrainedlr-0.1.0/src/constrainedlr.egg-info/top_level.txt
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:35:18.701839 constrainedlr-0.1.0/tests/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3589 2023-05-21 15:22:05.000000 constrainedlr-0.1.0/tests/test_fit.py
```

### Comparing `constrainedlr-0.0.9/LICENCE` & `constrainedlr-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.0.9/PKG-INFO` & `constrainedlr-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.0.9
+Version: 0.1.0
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -38,15 +38,15 @@
 
 ### Example Usage
 ```python
 from constrainedlr import ConstrainedLinearRegression
 from sklearn.metrics import mean_squared_error
 
 model = ConstrainedLinearRegression()
-model.fit(X_train, y_train, features_sign_constraints={6: 1, 7: -1})  # 6th and 7th feature (s3 and s4)
+model.fit(X_train, y_train, coefficients_sign_constraints={6: 1, 7: -1})  # 6th and 7th feature (s3 and s4)
 
 y_pred = model.predict(X_test)
 print(mean_squared_error(y_test, y_pred))
 print(model.coef_)
 ```
 
 See full example in the [notebook](./notebooks/demo.ipynb)
```

### Comparing `constrainedlr-0.0.9/README.md` & `constrainedlr-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 ### Example Usage
 ```python
 from constrainedlr import ConstrainedLinearRegression
 from sklearn.metrics import mean_squared_error
 
 model = ConstrainedLinearRegression()
-model.fit(X_train, y_train, features_sign_constraints={6: 1, 7: -1})  # 6th and 7th feature (s3 and s4)
+model.fit(X_train, y_train, coefficients_sign_constraints={6: 1, 7: -1})  # 6th and 7th feature (s3 and s4)
 
 y_pred = model.predict(X_test)
 print(mean_squared_error(y_test, y_pred))
 print(model.coef_)
 ```
 
 See full example in the [notebook](./notebooks/demo.ipynb)
```

### Comparing `constrainedlr-0.0.9/pyproject.toml` & `constrainedlr-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'constrainedlr'
-version = '0.0.9'
+version = '0.1.0'
 description = 'Constrained Linear Regression with sklearn-compatible API'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
```

### Comparing `constrainedlr-0.0.9/src/constrainedlr/model.py` & `constrainedlr-0.1.0/src/constrainedlr/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+from typing import Union
+
 import numpy as np
 import pandas as pd
 from cvxopt import matrix, solvers
 from sklearn.base import BaseEstimator, RegressorMixin
 from sklearn.utils.validation import check_array, check_is_fitted, check_X_y
 
+from .validation import validate_coefficients_sign_constraints
+
 
 class ConstrainedLinearRegression(BaseEstimator, RegressorMixin):
     def __init__(self, fit_intercept: bool = True, alpha: float = 0.0):
         self.fit_intercept = fit_intercept
         self.coef_ = None
         self.intercept_ = None
         self.alpha = alpha
 
     def fit(
         self,
-        X: pd.DataFrame,
+        X: Union[np.ndarray, pd.DataFrame],
         y: np.ndarray,
         sample_weight: np.ndarray = None,
-        features_sign_constraints: dict = {},
+        coefficients_sign_constraints: dict = {},
         intercept_sign_constraint: int = 0,
-        features_sum_constraint_equal: float = None,
+        coefficients_sum_constraint: float = None,
     ) -> "ConstrainedLinearRegression":
         """
         Fits a linear model with constraints
 
-        X : pandas.DataFrame of shape (n_samples, n_features)
+        X : {numpy.ndarray, pandas.DataFrame} of shape (n_samples, n_features)
             Training data.
 
         y : numpy.ndarray of shape (n_samples,)
             Target values.
 
         sample_weight : numpy.ndarray of shape (n_samples,), default=None
             Individual weights for each sample.
@@ -41,14 +45,16 @@
         intercept_sign_constraint : int
             Indicates the sign of intercept, if present, and must take the values: -1, 0, 1
 
         features_sum_constraint_equal : float
             Constraints the sum of all coefficients plus intercept (if present)
         """
         X, y = check_X_y(X, y)
+        validate_coefficients_sign_constraints(coefficients_sign_constraints, X)
+
         if np.ndim(y) == 1:
             y = y.reshape(-1, 1)
 
         n_samples, n_features = X.shape
 
         # Augment features to fit intercept
         if self.fit_intercept:
@@ -65,44 +71,44 @@
         # Quadratic program
         P = X.T.dot(W).dot(X) + self.alpha * np.eye(dim)
         P = matrix(P)
         q = (-y.T.dot(W).dot(X)).T
         q = matrix(q)
 
         features_sign_constraints_full = {feature: 0 for feature in range(n_features)}
-        features_sign_constraints_full.update(features_sign_constraints)
+        features_sign_constraints_full.update(coefficients_sign_constraints)
         diag_values = list(features_sign_constraints_full.values())
         if self.fit_intercept:
             diag_values.append(intercept_sign_constraint)
         G = -1.0 * np.diag(diag_values)  # Negate since cvxopt by convention accepts inequalities of the form Gx <= h
         G = matrix(G)
         h = np.zeros(dim)
         h = matrix(h)
 
         A, b = None, None
-        if features_sum_constraint_equal:
+        if coefficients_sum_constraint:
             A = np.ones(dim).astype("float")
             A = A.reshape(1, -1)
             A = matrix(A)
-            b = np.array([features_sum_constraint_equal]).astype("float")
+            b = np.array([coefficients_sum_constraint]).astype("float")
             b = matrix(b)
 
         solvers.options["show_progress"] = False
         solver = solvers.qp(P=P, q=q, G=G, h=h, A=A, b=b)
         weights = np.array(solver["x"]).flatten()
 
         if self.fit_intercept:
             self.coef_ = weights[0:-1]
             self.intercept_ = weights[-1]
         else:
             self.coef_ = weights
 
         return self
 
-    def predict(self, X: pd.DataFrame) -> np.ndarray:
+    def predict(self, X: Union[np.ndarray, pd.DataFrame]) -> np.ndarray:
         check_is_fitted(self)
         X = check_array(X)
 
         n_samples = X.shape[0]
 
         # Augment features for intercept
         if self.fit_intercept:
```

### Comparing `constrainedlr-0.0.9/src/constrainedlr.egg-info/PKG-INFO` & `constrainedlr-0.1.0/src/constrainedlr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.0.9
+Version: 0.1.0
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -38,15 +38,15 @@
 
 ### Example Usage
 ```python
 from constrainedlr import ConstrainedLinearRegression
 from sklearn.metrics import mean_squared_error
 
 model = ConstrainedLinearRegression()
-model.fit(X_train, y_train, features_sign_constraints={6: 1, 7: -1})  # 6th and 7th feature (s3 and s4)
+model.fit(X_train, y_train, coefficients_sign_constraints={6: 1, 7: -1})  # 6th and 7th feature (s3 and s4)
 
 y_pred = model.predict(X_test)
 print(mean_squared_error(y_test, y_pred))
 print(model.coef_)
 ```
 
 See full example in the [notebook](./notebooks/demo.ipynb)
```

### Comparing `constrainedlr-0.0.9/tests/test_fit.py` & `constrainedlr-0.1.0/tests/test_fit.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     assert np.allclose(lr.intercept_, clr.intercept_, atol=atol)
     assert np.allclose(lr.coef_, clr.coef_, atol=atol)
 
 
 def test_all_positive():
     clr = ConstrainedLinearRegression(fit_intercept=True)
-    clr.fit(X, y, features_sign_constraints={col: 1 for col in range(X.shape[1])})
+    clr.fit(X, y, coefficients_sign_constraints={col: 1 for col in range(X.shape[1])})
 
     lr = LinearRegression(fit_intercept=True, positive=True)
     lr.fit(X, y)
 
     assert np.allclose(lr.intercept_, clr.intercept_, atol=atol)
     assert np.allclose(lr.coef_, clr.coef_, atol=atol)
 
@@ -54,15 +54,15 @@
     clr = ConstrainedLinearRegression(fit_intercept=True)
 
     # Perform multiple tests since signs are produced randomly
     np.random.seed(0)
     for _ in range(10):
         signs = np.random.choice([-1, 1], size=X.shape[1])
         features_sign_constraints = dict(zip(list(range(X.shape[1])), signs))
-        clr.fit(X, y, features_sign_constraints=features_sign_constraints)
+        clr.fit(X, y, coefficients_sign_constraints=features_sign_constraints)
 
         assert np.alltrue(np.sign(clr.coef_) == signs)
 
 
 def test_intercept_sign():
     clr = ConstrainedLinearRegression(fit_intercept=True)
     clr.fit(X, y, intercept_sign_constraint=1)
@@ -71,21 +71,21 @@
     clr.fit(X, y, intercept_sign_constraint=-1)
     assert clr.intercept_ < 0
 
 
 def test_features_sum():
     clr = ConstrainedLinearRegression(fit_intercept=True)
     features_sum_constraint_equal = 15
-    clr.fit(X, y, features_sum_constraint_equal=features_sum_constraint_equal)
+    clr.fit(X, y, coefficients_sum_constraint=features_sum_constraint_equal)
     sum_of_weights = clr.coef_.sum() + clr.intercept_
     assert np.allclose(sum_of_weights, features_sum_constraint_equal, atol=atol)
 
     clr = ConstrainedLinearRegression(fit_intercept=False)
     features_sum_constraint_equal = 15
-    clr.fit(X, y, features_sum_constraint_equal=features_sum_constraint_equal)
+    clr.fit(X, y, coefficients_sum_constraint=features_sum_constraint_equal)
     sum_of_weights = clr.coef_.sum()
     assert np.allclose(sum_of_weights, features_sum_constraint_equal, atol=atol)
 
 
 def test_alpha():
     clr = ConstrainedLinearRegression(fit_intercept=True, alpha=1.0)
     clr.fit(X, y)
```

