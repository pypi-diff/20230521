# Comparing `tmp/constrainedlr-0.0.8.tar.gz` & `tmp/constrainedlr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constrainedlr-0.0.8.tar", last modified: Sat May 20 18:13:49 2023, max compression
+gzip compressed data, was "constrainedlr-0.0.9.tar", last modified: Sun May 21 15:17:49 2023, max compression
```

## Comparing `constrainedlr-0.0.8.tar` & `constrainedlr-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 18:13:50.407065 constrainedlr-0.0.8/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrainedlr-0.0.8/LICENCE
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2156 2023-05-20 18:13:50.401059 constrainedlr-0.0.8/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1167 2023-05-14 20:43:16.000000 constrainedlr-0.0.8/README.md
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1304 2023-05-20 18:09:58.000000 constrainedlr-0.0.8/pyproject.toml
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-20 18:13:50.409064 constrainedlr-0.0.8/setup.cfg
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 18:13:49.745575 constrainedlr-0.0.8/src/
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 18:13:50.002060 constrainedlr-0.0.8/src/constrainedlr/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       61 2023-05-14 19:35:04.000000 constrainedlr-0.0.8/src/constrainedlr/__init__.py
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3924 2023-05-20 18:08:03.000000 constrainedlr-0.0.8/src/constrainedlr/model.py
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 18:13:50.284064 constrainedlr-0.0.8/src/constrainedlr.egg-info/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2156 2023-05-20 18:13:49.000000 constrainedlr-0.0.8/src/constrainedlr.egg-info/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      311 2023-05-20 18:13:49.000000 constrainedlr-0.0.8/src/constrainedlr.egg-info/SOURCES.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-20 18:13:49.000000 constrainedlr-0.0.8/src/constrainedlr.egg-info/dependency_links.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-20 18:13:49.000000 constrainedlr-0.0.8/src/constrainedlr.egg-info/requires.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       14 2023-05-20 18:13:49.000000 constrainedlr-0.0.8/src/constrainedlr.egg-info/top_level.txt
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-20 18:13:50.345069 constrainedlr-0.0.8/tests/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3611 2023-05-20 18:08:03.000000 constrainedlr-0.0.8/tests/test_fit.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:17:49.191474 constrainedlr-0.0.9/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrainedlr-0.0.9/LICENCE
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2161 2023-05-21 15:17:49.173475 constrainedlr-0.0.9/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1205 2023-05-21 15:16:34.000000 constrainedlr-0.0.9/README.md
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1304 2023-05-21 15:16:34.000000 constrainedlr-0.0.9/pyproject.toml
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-21 15:17:49.193462 constrainedlr-0.0.9/setup.cfg
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:17:48.373349 constrainedlr-0.0.9/src/
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:17:48.691398 constrainedlr-0.0.9/src/constrainedlr/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       61 2023-05-14 19:35:04.000000 constrainedlr-0.0.9/src/constrainedlr/__init__.py
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     4011 2023-05-21 15:16:34.000000 constrainedlr-0.0.9/src/constrainedlr/model.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:17:49.051463 constrainedlr-0.0.9/src/constrainedlr.egg-info/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2161 2023-05-21 15:17:47.000000 constrainedlr-0.0.9/src/constrainedlr.egg-info/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      311 2023-05-21 15:17:48.000000 constrainedlr-0.0.9/src/constrainedlr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-21 15:17:47.000000 constrainedlr-0.0.9/src/constrainedlr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-21 15:17:48.000000 constrainedlr-0.0.9/src/constrainedlr.egg-info/requires.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       14 2023-05-21 15:17:48.000000 constrainedlr-0.0.9/src/constrainedlr.egg-info/top_level.txt
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:17:49.094476 constrainedlr-0.0.9/tests/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3585 2023-05-21 15:16:34.000000 constrainedlr-0.0.9/tests/test_fit.py
```

### Comparing `constrainedlr-0.0.8/LICENCE` & `constrainedlr-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.0.8/PKG-INFO` & `constrainedlr-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.0.8
+Version: 0.0.9
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -29,28 +29,28 @@
 The Kernel SHAP algorithm includes the training of a constrainted linear regression model where the sum of its coefficients is equal to the model's prediction
 
 #### Marketing Mix Modeling
 In Marketing Mix Modeling (MMM), the attribution of sales to various marketing channels can be informed by business sense or prior knowledge, by enforcing the contribution of channel variables to be positive or negative.
 
 ### Installation
 ```bash
-pip install constrained-lr
+pip install constrainedlr
 ```
 
 ### Example Usage
 ```python
-from constrained_lr import ConstrainedLinearRegression
+from constrainedlr import ConstrainedLinearRegression
 from sklearn.metrics import mean_squared_error
 
 model = ConstrainedLinearRegression()
-model.fit(X_train, y_train, features_sign_constraints={"s3": 1, "s4": -1})
+model.fit(X_train, y_train, features_sign_constraints={6: 1, 7: -1})  # 6th and 7th feature (s3 and s4)
 
 y_pred = model.predict(X_test)
 print(mean_squared_error(y_test, y_pred))
-print(dict(zip(X.columns, model.coef_)))
+print(model.coef_)
 ```
 
 See full example in the [notebook](./notebooks/demo.ipynb)
 
 
 ### Licence
 MIT
```

### Comparing `constrainedlr-0.0.8/README.md` & `constrainedlr-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Constrained Linear Regression
-constrained-lr is a drop-in replacement for `scikit-learn`'s `linear_model.LinearRegression` with the additional flexibility to define more complex (but linear) constraints on the model's coefficients.
-
-### Use-cases
-#### SHAP
-The Kernel SHAP algorithm includes the training of a constrainted linear regression model where the sum of its coefficients is equal to the model's prediction
-
-#### Marketing Mix Modeling
-In Marketing Mix Modeling (MMM), the attribution of sales to various marketing channels can be informed by business sense or prior knowledge, by enforcing the contribution of channel variables to be positive or negative.
-
-### Installation
-```bash
-pip install constrained-lr
-```
-
-### Example Usage
-```python
-from constrained_lr import ConstrainedLinearRegression
-from sklearn.metrics import mean_squared_error
-
-model = ConstrainedLinearRegression()
-model.fit(X_train, y_train, features_sign_constraints={"s3": 1, "s4": -1})
-
-y_pred = model.predict(X_test)
-print(mean_squared_error(y_test, y_pred))
-print(dict(zip(X.columns, model.coef_)))
-```
-
-See full example in the [notebook](./notebooks/demo.ipynb)
-
-
-### Licence
-MIT
+# Constrained Linear Regression
+constrained-lr is a drop-in replacement for `scikit-learn`'s `linear_model.LinearRegression` with the additional flexibility to define more complex (but linear) constraints on the model's coefficients.
+
+### Use-cases
+#### SHAP
+The Kernel SHAP algorithm includes the training of a constrainted linear regression model where the sum of its coefficients is equal to the model's prediction
+
+#### Marketing Mix Modeling
+In Marketing Mix Modeling (MMM), the attribution of sales to various marketing channels can be informed by business sense or prior knowledge, by enforcing the contribution of channel variables to be positive or negative.
+
+### Installation
+```bash
+pip install constrainedlr
+```
+
+### Example Usage
+```python
+from constrainedlr import ConstrainedLinearRegression
+from sklearn.metrics import mean_squared_error
+
+model = ConstrainedLinearRegression()
+model.fit(X_train, y_train, features_sign_constraints={6: 1, 7: -1})  # 6th and 7th feature (s3 and s4)
+
+y_pred = model.predict(X_test)
+print(mean_squared_error(y_test, y_pred))
+print(model.coef_)
+```
+
+See full example in the [notebook](./notebooks/demo.ipynb)
+
+
+### Licence
+MIT
```

### Comparing `constrainedlr-0.0.8/pyproject.toml` & `constrainedlr-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'constrainedlr'
-version = '0.0.8'
+version = '0.0.9'
 description = 'Constrained Linear Regression with sklearn-compatible API'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
 dependencies = [
-  "pandas>=2.0.0",
+  "numpy>=1.18.0",
   "scikit-learn>=1.2.2",
   "cvxopt>=1.3.1",
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
```

### Comparing `constrainedlr-0.0.8/src/constrainedlr/model.py` & `constrainedlr-0.0.9/src/constrainedlr/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pandas as pd
 from cvxopt import matrix, solvers
 from sklearn.base import BaseEstimator, RegressorMixin
+from sklearn.utils.validation import check_array, check_is_fitted, check_X_y
 
 
 class ConstrainedLinearRegression(BaseEstimator, RegressorMixin):
     def __init__(self, fit_intercept: bool = True, alpha: float = 0.0):
         self.fit_intercept = fit_intercept
         self.coef_ = None
         self.intercept_ = None
@@ -39,41 +40,39 @@
 
         intercept_sign_constraint : int
             Indicates the sign of intercept, if present, and must take the values: -1, 0, 1
 
         features_sum_constraint_equal : float
             Constraints the sum of all coefficients plus intercept (if present)
         """
-        X_ = X.values.copy()
-        y_ = y.copy()
+        X, y = check_X_y(X, y)
+        if np.ndim(y) == 1:
+            y = y.reshape(-1, 1)
 
-        if np.ndim(y_) == 1:
-            y_ = y_.reshape(-1, 1)
-
-        n_samples = X.shape[0]
+        n_samples, n_features = X.shape
 
         # Augment features to fit intercept
         if self.fit_intercept:
-            X_ = np.hstack([X_, np.ones(n_samples).reshape(-1, 1)])
+            X = np.hstack([X, np.ones(n_samples).reshape(-1, 1)])
 
-        dim = X_.shape[1]
+        dim = X.shape[1]
 
         # Weight matrix
         if sample_weight is None:
             W = np.eye(n_samples)
         else:
             W = np.diag(sample_weight)
 
         # Quadratic program
-        P = X_.T.dot(W).dot(X_) + self.alpha * np.eye(dim)
+        P = X.T.dot(W).dot(X) + self.alpha * np.eye(dim)
         P = matrix(P)
-        q = (-y_.T.dot(W).dot(X_)).T
+        q = (-y.T.dot(W).dot(X)).T
         q = matrix(q)
 
-        features_sign_constraints_full = {feature: 0 for feature in X.columns}
+        features_sign_constraints_full = {feature: 0 for feature in range(n_features)}
         features_sign_constraints_full.update(features_sign_constraints)
         diag_values = list(features_sign_constraints_full.values())
         if self.fit_intercept:
             diag_values.append(intercept_sign_constraint)
         G = -1.0 * np.diag(diag_values)  # Negate since cvxopt by convention accepts inequalities of the form Gx <= h
         G = matrix(G)
         h = np.zeros(dim)
@@ -96,20 +95,21 @@
             self.intercept_ = weights[-1]
         else:
             self.coef_ = weights
 
         return self
 
     def predict(self, X: pd.DataFrame) -> np.ndarray:
-        X_ = X.values.copy()
+        check_is_fitted(self)
+        X = check_array(X)
 
-        n_samples = X_.shape[0]
+        n_samples = X.shape[0]
 
         # Augment features for intercept
         if self.fit_intercept:
-            X_ = np.hstack([X_, np.ones(n_samples).reshape(-1, 1)])
+            X = np.hstack([X, np.ones(n_samples).reshape(-1, 1)])
             weights = np.concatenate([self.coef_, [self.intercept_]])
         else:
             weights = self.coef_
 
-        y_pred = X_.dot(weights)
+        y_pred = X.dot(weights)
         return y_pred
```

### Comparing `constrainedlr-0.0.8/src/constrainedlr.egg-info/PKG-INFO` & `constrainedlr-0.0.9/src/constrainedlr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.0.8
+Version: 0.0.9
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -29,28 +29,28 @@
 The Kernel SHAP algorithm includes the training of a constrainted linear regression model where the sum of its coefficients is equal to the model's prediction
 
 #### Marketing Mix Modeling
 In Marketing Mix Modeling (MMM), the attribution of sales to various marketing channels can be informed by business sense or prior knowledge, by enforcing the contribution of channel variables to be positive or negative.
 
 ### Installation
 ```bash
-pip install constrained-lr
+pip install constrainedlr
 ```
 
 ### Example Usage
 ```python
-from constrained_lr import ConstrainedLinearRegression
+from constrainedlr import ConstrainedLinearRegression
 from sklearn.metrics import mean_squared_error
 
 model = ConstrainedLinearRegression()
-model.fit(X_train, y_train, features_sign_constraints={"s3": 1, "s4": -1})
+model.fit(X_train, y_train, features_sign_constraints={6: 1, 7: -1})  # 6th and 7th feature (s3 and s4)
 
 y_pred = model.predict(X_test)
 print(mean_squared_error(y_test, y_pred))
-print(dict(zip(X.columns, model.coef_)))
+print(model.coef_)
 ```
 
 See full example in the [notebook](./notebooks/demo.ipynb)
 
 
 ### Licence
 MIT
```

### Comparing `constrainedlr-0.0.8/tests/test_fit.py` & `constrainedlr-0.0.9/tests/test_fit.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sklearn.linear_model import LinearRegression, Ridge
 
 from constrainedlr.model import ConstrainedLinearRegression
 
 atol = 1e-5
 
 dataset = load_diabetes()
-X = pd.DataFrame(dataset["data"], columns=dataset["feature_names"])
+X = dataset["data"]
 y = dataset["target"]
 
 
 def test_no_intercept():
     clr = ConstrainedLinearRegression(fit_intercept=False)
     clr.fit(X, y)
     assert clr.intercept_ is None
@@ -37,15 +37,15 @@
 
     assert np.allclose(lr.intercept_, clr.intercept_, atol=atol)
     assert np.allclose(lr.coef_, clr.coef_, atol=atol)
 
 
 def test_all_positive():
     clr = ConstrainedLinearRegression(fit_intercept=True)
-    clr.fit(X, y, features_sign_constraints={col: 1 for col in X.columns})
+    clr.fit(X, y, features_sign_constraints={col: 1 for col in range(X.shape[1])})
 
     lr = LinearRegression(fit_intercept=True, positive=True)
     lr.fit(X, y)
 
     assert np.allclose(lr.intercept_, clr.intercept_, atol=atol)
     assert np.allclose(lr.coef_, clr.coef_, atol=atol)
 
@@ -53,15 +53,15 @@
 def test_feature_signs():
     clr = ConstrainedLinearRegression(fit_intercept=True)
 
     # Perform multiple tests since signs are produced randomly
     np.random.seed(0)
     for _ in range(10):
         signs = np.random.choice([-1, 1], size=X.shape[1])
-        features_sign_constraints = dict(zip(X.columns, signs))
+        features_sign_constraints = dict(zip(list(range(X.shape[1])), signs))
         clr.fit(X, y, features_sign_constraints=features_sign_constraints)
 
         assert np.alltrue(np.sign(clr.coef_) == signs)
 
 
 def test_intercept_sign():
     clr = ConstrainedLinearRegression(fit_intercept=True)
```

