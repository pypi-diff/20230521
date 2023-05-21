# Comparing `tmp/pflacco-1.2.0.tar.gz` & `tmp/pflacco-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pflacco-1.2.0.tar", last modified: Thu Mar 23 10:59:45 2023, max compression
+gzip compressed data, was "pflacco-1.2.1.tar", last modified: Sun May 21 21:19:54 2023, max compression
```

## Comparing `pflacco-1.2.0.tar` & `pflacco-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 10:59:45.077443 pflacco-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-23 10:59:23.000000 pflacco-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-23 10:59:23.000000 pflacco-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-03-23 10:59:45.077443 pflacco-1.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 10:59:45.073443 pflacco-1.2.0/pflacco/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-23 10:59:23.000000 pflacco-1.2.0/pflacco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77838 2023-03-23 10:59:23.000000 pflacco-1.2.0/pflacco/classical_ela_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-03-23 10:59:23.000000 pflacco-1.2.0/pflacco/local_optima_network_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    22152 2023-03-23 10:59:23.000000 pflacco-1.2.0/pflacco/misc_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-03-23 10:59:23.000000 pflacco-1.2.0/pflacco/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-03-23 10:59:23.000000 pflacco-1.2.0/pflacco/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 10:59:45.073443 pflacco-1.2.0/pflacco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-03-23 10:59:45.000000 pflacco-1.2.0/pflacco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-23 10:59:45.000000 pflacco-1.2.0/pflacco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 10:59:45.000000 pflacco-1.2.0/pflacco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-23 10:59:45.000000 pflacco-1.2.0/pflacco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-23 10:59:45.000000 pflacco-1.2.0/pflacco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-23 10:59:23.000000 pflacco-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 10:59:45.077443 pflacco-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-23 10:59:23.000000 pflacco-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 10:59:45.077443 pflacco-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 10:59:23.000000 pflacco-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-03-23 10:59:23.000000 pflacco-1.2.0/tests/classical_ela_features_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-23 10:59:23.000000 pflacco-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-03-23 10:59:23.000000 pflacco-1.2.0/tests/generate_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-23 10:59:23.000000 pflacco-1.2.0/tests/local_optima_network_features_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-03-23 10:59:23.000000 pflacco-1.2.0/tests/misc_features_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-23 10:59:23.000000 pflacco-1.2.0/tests/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:19:54.802316 pflacco-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-21 21:19:39.000000 pflacco-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-21 21:19:39.000000 pflacco-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-05-21 21:19:54.802316 pflacco-1.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:19:54.802316 pflacco-1.2.1/pflacco/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-21 21:19:39.000000 pflacco-1.2.1/pflacco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79744 2023-05-21 21:19:39.000000 pflacco-1.2.1/pflacco/classical_ela_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-05-21 21:19:39.000000 pflacco-1.2.1/pflacco/local_optima_network_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22152 2023-05-21 21:19:39.000000 pflacco-1.2.1/pflacco/misc_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-21 21:19:39.000000 pflacco-1.2.1/pflacco/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-21 21:19:39.000000 pflacco-1.2.1/pflacco/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:19:54.802316 pflacco-1.2.1/pflacco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-05-21 21:19:54.000000 pflacco-1.2.1/pflacco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-21 21:19:54.000000 pflacco-1.2.1/pflacco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:19:54.000000 pflacco-1.2.1/pflacco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-21 21:19:54.000000 pflacco-1.2.1/pflacco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 21:19:54.000000 pflacco-1.2.1/pflacco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-21 21:19:39.000000 pflacco-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:19:54.802316 pflacco-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-21 21:19:39.000000 pflacco-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:19:54.802316 pflacco-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:19:39.000000 pflacco-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-05-21 21:19:39.000000 pflacco-1.2.1/tests/classical_ela_features_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-21 21:19:39.000000 pflacco-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-05-21 21:19:39.000000 pflacco-1.2.1/tests/generate_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-21 21:19:39.000000 pflacco-1.2.1/tests/local_optima_network_features_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-21 21:19:39.000000 pflacco-1.2.1/tests/misc_features_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-21 21:19:39.000000 pflacco-1.2.1/tests/sampling_test.py
```

### Comparing `pflacco-1.2.0/LICENSE` & `pflacco-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pflacco-1.2.0/PKG-INFO` & `pflacco-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pflacco
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python implementation and extension to the R package flacco for computing ELA features.
 Home-page: https://pypi.org/project/pflacco/
 Author: Raphael Patrick Prager
 Author-email: raphael.prager@gmx.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pflacco-1.2.0/pflacco/classical_ela_features.py` & `pflacco-1.2.1/pflacco/classical_ela_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from numdifftools.core import Gradient, Hessian
 
 from sklearn import linear_model
 from sklearn.decomposition import PCA
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis, QuadraticDiscriminantAnalysis
 from sklearn.neighbors import NearestNeighbors 
 from sklearn.model_selection import StratifiedKFold
+from sklearn.preprocessing import PolynomialFeatures
 
 from scipy.spatial.distance import pdist, squareform
 from scipy.stats import gaussian_kde, pearsonr
 from scipy.optimize import minimize as scipy_minimize
 from scipy.cluster.hierarchy import linkage, cut_tree, _order_cluster_tree
 
 from typing import Callable, Dict, List, Optional, Union
@@ -82,47 +83,41 @@
 
       lin_simple_intercept = model.intercept_
       lin_simple_coef_min = np.abs(model.coef_).min()
       lin_simple_coef_max = np.abs(model.coef_).max()
       lin_simple_coef_max_by_min = lin_simple_coef_max / lin_simple_coef_min
       lin_simple_adj_r2 = 1 - (1 - model.score(X, y)) * (len(y) - 1) / (len(y) - X.shape[1]-1)
       
-
       # Create linear model with interaction
       # Create pairwise interactions
-      X_interact = X.copy()
-      for idx in range(len(X.columns)):
-            tmp_idx = idx + 1
-            while tmp_idx < len(X.columns):         
-                  X_interact[X.columns[idx] + X.columns[tmp_idx]] = X[X.columns[idx]] * X[X.columns[tmp_idx]]
-                  tmp_idx += 1
-
+      poly = PolynomialFeatures(interaction_only=True, include_bias=False)
+      X_interact = poly.fit_transform(X)
+ 
       model = linear_model.LinearRegression()
       model.fit(X_interact, y)
       lin_w_interact_adj_r2 = 1 - (1 - model.score(X_interact, y)) * (len(y) - 1) / (len(y) - X_interact.shape[1] - 1)
 
-
       # Create quadratic model and calculate qm features
       model = linear_model.LinearRegression()
       X_squared = pd.concat([X, X.pow(2).add_suffix('^2')], axis = 1)
       model.fit(X_squared, y)
 
       quad_simple_adj_r2 = 1 - (1 - model.score(X_squared, y)) * (len(y) - 1) / (len(y) - X_squared.shape[1]-1)
 
       quad_model_con_min = np.abs(model.coef_[int(X_squared.shape[1]/2):]).min()
       quad_model_con_max = np.abs(model.coef_[int(X_squared.shape[1]/2):]).max()
       quad_simple_cond = quad_model_con_max/quad_model_con_min
 
-      # Create linear model with interaction
+      # Create quadratic model with interaction
       # Create pairwise interactions
-      X_interact = X_squared.copy()
+      X_interact = X_squared.to_numpy()
       for idx in range(len(X_squared.columns)):
             tmp_idx = idx + 1
-            while tmp_idx < len(X_squared.columns):         
-                  X_interact[X_squared.columns[idx] + X_squared.columns[tmp_idx]] = X_squared[X_squared.columns[idx]] * X_squared[X_squared.columns[tmp_idx]]
+            while tmp_idx < len(X_squared.columns):
+                  X_interact = np.hstack((X_interact, (X_interact[:, idx] * X_interact[:, tmp_idx]).reshape(-1, 1)))
                   tmp_idx += 1
 
       model = linear_model.LinearRegression()
       model.fit(X_interact, y)
       quad_w_interact_adj_r2 = 1 - (1 - model.score(X_interact, y)) * (len(y) - 1) / (len(y) - X_interact.shape[1]-1)
 
       return {
@@ -323,14 +318,17 @@
                               elif dist_tie_breaker == 'first':
                                     i = i[0]
                               elif dist_tie_breaker == 'last':
                                     i = i[-1]
                               else:
                                     raise ValueError('Possible tie breaker methods are "sample", "first", and "last"')
 
+                        # Transform array of length 1 to a single scalar
+                        i = i[0]
+
                         results.append([idx, ind_alt[i], d[i]])
 
       nb_stats = np.array(results, dtype=np.float64)
       near_dist = np.array([x[1] for x in distances])
       near_better_dist = nb_stats[:, 2]
       nb_near_ratio = np.divide(near_better_dist, near_dist).reshape(-1, 1)
       nb_stats = np.hstack((nb_stats, near_dist.reshape(-1, 1), nb_near_ratio, y.reshape(-1, 1)))
@@ -736,15 +734,16 @@
       }
             
 def calculate_limo(
       X: Union[pd.DataFrame, np.ndarray, List[List[float]]],
       y: Union[pd.Series, np.ndarray, List[float]],
       lower_bound: Union[List[float], float],
       upper_bound: Union[List[float], float],
-      blocks: Optional[Union[List[int], np.ndarray, int]] = None) -> Dict[str, Optional[Union[int, float]]]:
+      blocks: Optional[Union[List[int], np.ndarray, int]] = None,
+      force: bool = False) -> Dict[str, Optional[Union[int, float]]]:
       """Linear Model features.
       Linear models are computed per cell, provided the decision space is divided into a grid of cells. Each one of the models has the form objective ~ features.
       
       - avg_length.{reg, norm}: length of the average coefficient vector (based on regular and normalized vectors)
       - length_{mean, sd}: arithmetic mean and standard deviation of the lengths of all coefficient vectors
       - cor.{reg, norm}: correlation of all coefficient vectors (based on regular and normalized vectors)
       - ratio_{mean, sd}: arithmetic mean and standard deviation of the ratios of (absolute) maximum and minimum (non-intercept) coefficients per cell
@@ -759,25 +758,33 @@
           A list-like object which contains the respective objective values of `X`.
       lower_bound : Union[List[float], float]
           Lower bound of variables of the decision space.
       upper_bound : Union[List[float], float]
           Upper bound of variables of the decision space.
       blocks : Optional[Union[List[int], np.ndarray, int]], optional
           Number of blocks per dimension, by default None.
+      force : bool, optional
+          The recommended number of blocks per dim is >2 and the minimum number of observation per cell is 3.
+          Meaning, that X has to have at least dim^blocks * 3 observations. This requirement can be circumenvented
+          by setting `force` to True. 
+          ATTENTION: The resulting feature values are not in line with any recommendation and may not have any predictive power, by default False.
 
       Returns
       -------
       Dict[str, Optional[Union[int, float]]]
           Dictionary consisting of the calculated features.
       """      
       start_time = time.monotonic()
       X, y = _validate_variable_types(X, y)
       dims = X.shape[1]
-      blocks = _check_blocks_variable(X, dims, blocks)
+      blocks = _check_blocks_variable(X, dims, blocks, force = force)
 
+      if blocks.min() <= 2 and force == False:
+            raise ValueError('The cell convexity features can only be computed when all dimensions have more than 2 cells.')
+      
       # Consolidate X, y, and cells into one data frame
       init = X.copy()
       init['y'] = y
       init['cells'], _ = _create_blocks(X, y, lower_bound, upper_bound, blocks)
 
       result = {
             'limo.avg_length': None,
@@ -838,14 +845,15 @@
 # TODO small todo inside function
 def calculate_cm_angle(
       X: Union[pd.DataFrame, np.ndarray, List[List[float]]],
       y: Union[pd.Series, np.ndarray, List[float]],
       lower_bound: Union[List[float], float],
       upper_bound: Union[List[float], float],
       blocks: Optional[Union[List[int], np.ndarray, int]] = None,
+      force: bool = False,
       minimize: bool = True) -> Dict[str, Union[int, float]]:
       """Cell Mapping Angle features.
       These features are based on the location of the worst and best element within each cell.
       To be precise, their distance to the cell center and the angle between these three elements (at the center) are the foundation:
 
       - dist_ctr2{best, worst}.{mean, sd}: arithmetic mean and standard deviation of distances from the cell center to the best / worst observation within the cell (over all cells)
       - angle.{mean, sd}: arithmetic mean and standard deviation of angles (in degree) between worst, center and best element of a cell (over all cells)
@@ -860,35 +868,36 @@
           A list-like object which contains the respective objective values of `X`.
       lower_bound : Union[List[float], float]
           Lower bound of variables of the decision space.
       upper_bound : Union[List[float], float]
           Upper bound of variables of the decision space.
       blocks : Optional[Union[List[int], np.ndarray, int]], optional
           Number of blocks per dimension, by default None.
+      force : bool, optional
+          The recommended number of blocks per dim is >2 and the minimum number of observation per cell is 3.
+          Meaning, that X has to have at least dim^blocks * 3 observations. This requirement can be circumenvented
+          by setting `force` to True. 
+          ATTENTION: The resulting feature values are not in line with any recommendation and may not have any predictive power, by default False.
       minimize : bool, optional
           Indicator whether the objective function should be minimized or maximized, by default True.
 
       Returns
       -------
       Dict[str, Union[int, float]]
           Dictionary consisting of the calculated features.
 
       """      
       start_time = time.monotonic()
       X, y = _validate_variable_types(X, y)
       dim = X.shape[1]
-      if blocks is None:
-            blocks = _determine_max_n_blocks(X)
-      if not isinstance(blocks, list) and type(blocks) is not np.ndarray:
-            blocks = np.array([blocks] * dim)
-      elif isinstance(blocks, list):
-            blocks = np.array(blocks)
-      if len(blocks) != dim:
-            raise ValueError('The provided value for "block" does not have the same length as the dimensionality of X.')
-
+      
+      blocks = _check_blocks_variable(X, dim, blocks, force = force)
+      if blocks.min() <= 2 and force == False:
+            raise ValueError('The cell convexity features can only be computed when all dimensions have more than 2 cells.')
+      
       init = X.copy()
       init['y'] = y if minimize == True else -1 * y
       init['cell'], cell_centers = _create_blocks(X, y, lower_bound, upper_bound, blocks)
 
       grid_best = init.loc[init.groupby('cell')['y'].idxmin()]
       grid_worst = init.loc[init.groupby('cell')['y'].idxmax()]
       y_global_best = grid_best['y'].min()
@@ -937,14 +946,15 @@
 
 def calculate_cm_conv(
       X: Union[pd.DataFrame, np.ndarray, List[List[float]]],
       y: Union[pd.Series, np.ndarray, List[float]],
       lower_bound: Union[List[float], float],
       upper_bound: Union[List[float], float],
       blocks: Optional[Union[List[int], np.ndarray, int]] = None,
+      force: bool = False,
       minimize: bool = True,
       cm_conv_diag: bool = False,
       cm_conv_fast_k: float = 0.05) -> Dict[str, Union[int, float]]:
       """Cell Mapping Convexity features.
       Each cell will be represented by an observation (of the initial design), which is located closest to the cell center. Then, the objectives of three neighbouring cells are compared:
       
       - {convex, concave}.hard: if the objective of the inner cell is above / below the two outer cells, there is strong evidence for convexity / concavity
@@ -959,14 +969,19 @@
           A list-like object which contains the respective objective values of `X`.
       lower_bound : Union[List[float], float]
           Lower bound of variables of the decision space.
       upper_bound : Union[List[float], float]
           Upper bound of variables of the decision space.
       blocks : Optional[Union[List[int], np.ndarray, int]], optional
           Number of blocks per dimension, by default None.
+      force : bool, optional
+          The recommended number of blocks per dim is >2 and the minimum number of observation per cell is 3.
+          Meaning, that X has to have at least dim^blocks * 3 observations. This requirement can be circumenvented
+          by setting `force` to True. 
+          ATTENTION: The resulting feature values are not in line with any recommendation and may not have any predictive power, by default False.
       minimize : bool, optional
           Indicator whether the objective function should be minimized or maximized, by default True.
       cm_conv_diag : bool, optional
           Indicator which, when true, consideres cells on the diagonal also as neighbours, by default False.
       cm_conv_fast_k : float, optional
           Percentage of elements that should be considered within the nearest neighbour computation, by default 0.05.
 
@@ -975,16 +990,16 @@
       Dict[str, Union[int, float]]
           Dictionary consisting of the calculated features.
 
       """      
       start_time = time.monotonic()
       X, y = _validate_variable_types(X, y)
       dim = X.shape[1]
-      blocks = _check_blocks_variable(X, dim, blocks)
-      if blocks.min() <= 2:
+      blocks = _check_blocks_variable(X, dim, blocks, force = force)
+      if blocks.min() <= 2 and force == False:
             raise ValueError('The cell convexity features can only be computed when all dimensions have more than 2 cells.')
       if cm_conv_fast_k < 0 or cm_conv_fast_k > X.shape[0]:
             raise ValueError('cm_conv_fast_k must be in the interval [0, n] where n is the number of observations in X.')
 
       init = X.copy()
       init['y'] = y if minimize == True else -1 * y
       init['cell'], cell_centers = _create_blocks(X, y, lower_bound, upper_bound, blocks)
@@ -1108,14 +1123,15 @@
 
 def calculate_cm_grad(
       X: Union[pd.DataFrame, np.ndarray, List[List[float]]],
       y: Union[pd.Series, np.ndarray, List[float]],
       lower_bound: Union[List[float], float],
       upper_bound: Union[List[float], float],
       blocks: Optional[Union[List[int], np.ndarray, int]] = None,
+      force: bool = False,
       minimize: bool = True) -> Dict[str, Union[int, float]]:
       """Cell Mapping Gradient Homogeneity features.
       Within a cell of the initial grid, the gradients between each observation and its nearest neighbour observation are computed.
       Those gradients are then directed towards the smaller of the two objective values and afterwards normalized.
       Then, the length of the sum of all the directed and normalized gradients within a cell is computed.
       Based on those measurements (one per cell) the following features are computed:
 
@@ -1130,29 +1146,34 @@
           A list-like object which contains the respective objective values of `X`.
       lower_bound : Union[List[float], float]
           Lower bound of variables of the decision space.
       upper_bound : Union[List[float], float]
           Upper bound of variables of the decision space.
       blocks : Optional[Union[List[int], np.ndarray, int]], optional
           Number of blocks per dimension, by default None.
+      force : bool, optional
+          The recommended number of blocks per dim is >2 and the minimum number of observation per cell is 3.
+          Meaning, that X has to have at least dim^blocks * 3 observations. This requirement can be circumenvented
+          by setting `force` to True. 
+          ATTENTION: The resulting feature values are not in line with any recommendation and may not have any predictive power, by default False.
       minimize : bool, optional
           Indicator whether the objective function should be minimized or maximized, by default True.
 
       Returns
       -------
       Dict[str, Union[int, float]]
           Dictionary consisting of the calculated features.
 
       """      
       start_time = time.monotonic()
       X, y = _validate_variable_types(X, y)
       dim = X.shape[1]
-      blocks = _check_blocks_variable(X, dim, blocks)
+      blocks = _check_blocks_variable(X, dim, blocks, force = force)
 
-      if blocks.min() <= 2:
+      if blocks.min() <= 2 and force == False:
             raise ValueError('The cell grad features can only be computed when all dimensions have more than 2 cells.')
 
       init = X.copy()
       init['y'] = y if minimize == True else -1 * y
       init['cell'], _ = _create_blocks(X, y, lower_bound, upper_bound, blocks)
 
       grad_homo = []
```

### Comparing `pflacco-1.2.0/pflacco/local_optima_network_features.py` & `pflacco-1.2.1/pflacco/local_optima_network_features.py`

 * *Files identical despite different names*

### Comparing `pflacco-1.2.0/pflacco/misc_features.py` & `pflacco-1.2.1/pflacco/misc_features.py`

 * *Files identical despite different names*

### Comparing `pflacco-1.2.0/pflacco/sampling.py` & `pflacco-1.2.1/pflacco/sampling.py`

 * *Files identical despite different names*

### Comparing `pflacco-1.2.0/pflacco/utils.py` & `pflacco-1.2.1/pflacco/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import itertools
 import numpy as np
 import pandas as pd
+import warnings
 
 #from rpy2.robjects.packages import importr, isinstalled
 
 #def _interface_mda():
 #    base = importr('base')
 #    utils = importr('utils')
 #    utils.chooseCRANmirror(ind=1)
@@ -60,30 +61,44 @@
 
 def _determine_max_n_blocks(X):
       blocks = 1
       while (X.shape[1] ** (blocks + 1)) * 3 < X.shape[0]:
             blocks += 1
       return blocks
 
-def _check_blocks_variable(X, dim, blocks):
+def _check_blocks_variable(X, dim, blocks, force = False):
       if blocks is None:
             blocks = max(_determine_max_n_blocks(X), 2)
+      else:
+            n_bl = _determine_max_n_blocks(X)
+            if isinstance(blocks, int):
+                  if blocks > n_bl:
+                        if force == False:
+                              raise ValueError('The provided value for "block" is too large, resulting in less than 3 observations per cell.')
+                        else:
+                              warnings.warn(f'For the given dataframe X, the recommended maximum number of blocks per dim is {n_bl}. The current value for blocks ({blocks}) exceeds that.')
+            else:
+                  if (np.array(blocks) > n_bl).any():
+                        if force == False:
+                              raise ValueError('The provided value for "block" is too large, resulting in less than 3 observations per cell.')
+                        else:
+                              warnings.warn(f'For the given dataframe X, the recommended maximum number of blocks per dim is {n_bl}. The current value for blocks ({blocks}) exceeds that.')
+                  
       if not isinstance(blocks, list) and type(blocks) is not np.ndarray:
             blocks = np.array([blocks] * dim)
       elif isinstance(blocks, list):
             blocks = np.array(blocks)
       if len(blocks) != dim:
             raise Exception('The provided value for "block" does not have the same length as the dimensionality of X.')
-
+      
       return blocks
 
 def _create_blocks(X, y, lower_bound, upper_bound, blocks = None):
       X, y, _validate_variable_types(X, y)
       dim = X.shape[1]
-      blocks = _check_blocks_variable(X, dim, blocks)
       lower_bound, upper_bound = _transform_bounds_to_canonical(dim, lower_bound, upper_bound)
 
       block_widths = (upper_bound - lower_bound)/blocks
       cp = np.cumprod(np.insert(blocks, 0, 1))
 
       cell_ids = []
       for idx, row in X.iterrows():
```

### Comparing `pflacco-1.2.0/pflacco.egg-info/PKG-INFO` & `pflacco-1.2.1/pflacco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pflacco
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python implementation and extension to the R package flacco for computing ELA features.
 Home-page: https://pypi.org/project/pflacco/
 Author: Raphael Patrick Prager
 Author-email: raphael.prager@gmx.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pflacco-1.2.0/pflacco.egg-info/SOURCES.txt` & `pflacco-1.2.1/pflacco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pflacco-1.2.0/setup.py` & `pflacco-1.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(
      name='pflacco',  
-     version='1.2.0',
+     version='1.2.1',
      author="Raphael Patrick Prager",
      author_email="raphael.prager@gmx.de",
      description="A Python implementation and extension to the R package flacco for computing ELA features.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      license='MIT',
      install_requires=required,
```

### Comparing `pflacco-1.2.0/tests/classical_ela_features_test.py` & `pflacco-1.2.1/tests/classical_ela_features_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,19 @@
     raise RuntimeError('Could not determine the system platform and therefore not load the appropriate test files.')
 
 @pytest.fixture
 def feature_values():
     X = pd.read_pickle(os.path.join(RSC, 'test_classical_ela_features.pkl'))
     return X
 
+@pytest.fixture
+def cm_feature_values():
+    X = pd.read_pickle(os.path.join(RSC, 'test_cm_ela_features.pkl'))
+    return X
+
 ########################################################
 # Deterministic Features
 def test_calculate_ela_meta(x_samples, feature_values):
     result = []
     for fid in range(1,25):
         for dim in DIMS:
             tmp = x_samples.iloc[:(dim*50), :dim]
@@ -187,23 +192,109 @@
             result.append(data)
     result = pd.concat(result).reset_index(drop = True)
     colnames = result.columns[~result.columns.str.contains('costs_runtime')]
     assert (assert_frame_equal(result[colnames], feature_values[colnames]) is None)
 
 ########################################################
 ## Cell Mapping Features
-@pytest.mark.skip(reason='To be implemented')
-def test_calculate_cell_mapping(feature_values):
+def test_calculate_cm_angle(x_samples, cm_feature_values):
     result = []
     for fid in range(1,25):
-        for dim in DIMS:
-            X = create_initial_sample(dim, n = 3 ** dim)
+        for dim in [2, 3, 5]:
+            force = False
+            if dim == 5:
+                force = True
+            tmp = x_samples.iloc[:(dim*50), :dim]
             f = get_problem(fid, 1, dim)
-            y = X.apply(lambda x: f(x), axis = 1)
-            features = calculate_information_content(X, y, seed = 100)
+            y = tmp.apply(lambda x: f(x), axis = 1)
+            features = calculate_cm_angle(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 3, force = force)
             data = pd.DataFrame(features, index = [0])
             data['fid'] = fid
             data['dim'] = dim
             result.append(data)
     result = pd.concat(result).reset_index(drop = True)
     colnames = result.columns[~result.columns.str.contains('costs_runtime')]
-    assert result[colnames].equals(feature_values[colnames])
+    assert (assert_frame_equal(result[colnames], cm_feature_values[colnames]) is None)
+
+def test_calculate_cm_conv(x_samples, cm_feature_values):
+    result = []
+    for fid in range(1,25):
+        for dim in [2, 3, 5]:
+            force = False
+            if dim == 5:
+                force = True
+            tmp = x_samples.iloc[:(dim*50), :dim]
+            f = get_problem(fid, 1, dim)
+            y = tmp.apply(lambda x: f(x), axis = 1)
+            features = calculate_cm_conv(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 3, force = force)
+            data = pd.DataFrame(features, index = [0])
+            data['fid'] = fid
+            data['dim'] = dim
+            result.append(data)
+    result = pd.concat(result).reset_index(drop = True)
+    colnames = result.columns[~result.columns.str.contains('costs_runtime')]
+    assert (assert_frame_equal(result[colnames], cm_feature_values[colnames]) is None)
+
+def test_calculate_cm_grad(x_samples, cm_feature_values):
+    result = []
+    for fid in range(1,25):
+        for dim in [2, 3, 5]:
+            force = False
+            if dim == 5:
+                force = True
+            tmp = x_samples.iloc[:(dim*50), :dim]
+            f = get_problem(fid, 1, dim)
+            y = tmp.apply(lambda x: f(x), axis = 1)
+            features = calculate_cm_grad(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 3, force = force)
+            data = pd.DataFrame(features, index = [0])
+            data['fid'] = fid
+            data['dim'] = dim
+            result.append(data)
+    result = pd.concat(result).reset_index(drop = True)
+    colnames = result.columns[~result.columns.str.contains('costs_runtime')]
+    assert (assert_frame_equal(result[colnames], cm_feature_values[colnames]) is None)
+
+def test_calculate_limo(x_samples, cm_feature_values):
+    result = []
+    for fid in range(1,25):
+        for dim in [2, 3, 5]:
+            force = False
+            if dim == 5:
+                force = True
+            tmp = x_samples.iloc[:(dim*50), :dim]
+            f = get_problem(fid, 1, dim)
+            y = tmp.apply(lambda x: f(x), axis = 1)
+            features = calculate_limo(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 3, force = force)
+            data = pd.DataFrame(features, index = [0])
+            data['fid'] = fid
+            data['dim'] = dim
+            result.append(data)
+    result = pd.concat(result).reset_index(drop = True)
+    colnames = result.columns[~result.columns.str.contains('costs_runtime')]
+    assert (assert_frame_equal(result[colnames], cm_feature_values[colnames]) is None)
+
+def test_block_value_prerequisite(x_samples):
+    with pytest.raises(ValueError, match='The provided value for "block" is too large, resulting in less than 3 observations per cell.'):
+        fid = 1
+        dim = 10
+        tmp = x_samples.iloc[:(dim*50), :dim]
+        f = get_problem(fid, 1, dim)
+        y = tmp.apply(lambda x: f(x), axis = 1)
+        calculate_limo(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 3)
+
+def test_block_value_too_low(x_samples):
+    with pytest.raises(ValueError, match='The cell convexity features can only be computed when all dimensions have more than 2 cells.'):
+        fid = 1
+        dim = 10
+        tmp = x_samples.iloc[:(dim*50), :dim]
+        f = get_problem(fid, 1, dim)
+        y = tmp.apply(lambda x: f(x), axis = 1)
+        calculate_cm_angle(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 2)
+
+def test_block_value_forced(x_samples):
+    with pytest.warns(UserWarning, match=r'For the given dataframe X, the recommended maximum number of blocks per dim is \d+. The current value for blocks \(\d+\) exceeds that.'):
+        fid = 1
+        dim = 3
+        tmp = x_samples.iloc[:(dim*50), :dim]
+        f = get_problem(fid, 1, dim)
+        y = tmp.apply(lambda x: f(x), axis = 1)
+        calculate_cm_conv(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 5, force = True)
```

### Comparing `pflacco-1.2.0/tests/generate_resources.py` & `pflacco-1.2.1/tests/generate_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import sys
+sys.path.append("../pflacco")
+
 from pflacco.classical_ela_features import *
 from pflacco.misc_features import *
 from pflacco.sampling import * 
 from pflacco.local_optima_network_features import *
 import os
 import pandas as pd
 from ioh import get_problem, ProblemType
@@ -104,59 +107,58 @@
         data['fid'] = fid
         data['dim'] = dim
         print(str(fid) + ' - ' + str(dim))
         result.append(data)
     result = pd.concat(result).reset_index(drop=True)
     result = result[result.columns[~result.columns.str.contains('costs_runtime')]]
     result = result.sort_values(by = ['fid', 'dim']).reset_index(drop = True)
-    print('test')
-
 
 def ls_investigation():
     result = []
     for rep in range(10):
         dim = 3
         fid = 1
         tmp = x_samples.iloc[:(dim*50), :dim]
         f = get_problem(fid, 1, dim, ProblemType.BBOB)
         y = tmp.apply(lambda x: f(x), axis = 1)
         ls = calculate_length_scales_features(f, dim, lower_bound=-5, upper_bound=5, seed = 200, budget_factor_per_dim = 10)
         data = pd.DataFrame({**ls}, index = [0])
         result.append(data)
 
     result = pd.concat(result).reset_index(drop=True)
-    print('test')
 
-    
 
 def gen_cell_features():
     result = []
     for fid in range(1,25):
-        for dim in DIMS:
-            #X = create_initial_sample(dim, n = (dim ** 3) * 3, seed = 100)
-            X = x_samples
+        for dim in [2, 3, 5]:
+            force = False
+            n = dim * 50
+            if dim == 5:
+                force = True
+            tmp = x_samples.iloc[:n, :dim]
             f = get_problem(fid, 1, dim, ProblemType.BBOB)
-            y = X.apply(lambda x: f(x), axis = 1)
-            cm_angle = calculate_cm_angle(X, y, lower_bound = -5, upper_bound = 5, blocks = 3)
-            cm_conv = calculate_cm_conv(X, y, lower_bound = -5, upper_bound = 5, blocks = 3)
-            cm_grad = calculate_cm_grad(X, y, lower_bound = -5, upper_bound = 5, blocks = 3)
-            limo = calculate_limo(X, y, lower_bound = -5, upper_bound = 5, blocks = 3)
+            y = tmp.apply(lambda x: f(x), axis = 1)
+            cm_angle = calculate_cm_angle(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 3, force = force)
+            cm_conv = calculate_cm_conv(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 3, force = force)
+            cm_grad = calculate_cm_grad(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 3, force = force)
+            limo = calculate_limo(tmp, y, lower_bound = -5, upper_bound = 5, blocks = 3, force = force)
 
             data = pd.DataFrame({**cm_angle, **cm_conv, **cm_grad, **limo, **{'fid':fid}, **{'dim':dim}}, index = [0])
             result.append(data)
             
     result = pd.concat(result).reset_index(drop=True)
     result = result[result.columns[~result.columns.str.contains('costs_runtime')]]
     result = result.sort_values(by = ['fid', 'dim']).reset_index(drop = True)
     result.to_pickle(os.path.join(RSC, 'test_cm_ela_features.pkl'))
 
 
 
 
 
-#gen_classical_features()
-#gen_sample()
-#gen_cell_features()
-#gen_misc_features()
+gen_classical_features()
+gen_sample()
+gen_cell_features()
+gen_misc_features()
 #ls_investigation()
 #gen_lon_features()
 #lon_investigation()
```

### Comparing `pflacco-1.2.0/tests/local_optima_network_features_test.py` & `pflacco-1.2.1/tests/local_optima_network_features_test.py`

 * *Files identical despite different names*

### Comparing `pflacco-1.2.0/tests/misc_features_test.py` & `pflacco-1.2.1/tests/misc_features_test.py`

 * *Files identical despite different names*

### Comparing `pflacco-1.2.0/tests/sampling_test.py` & `pflacco-1.2.1/tests/sampling_test.py`

 * *Files identical despite different names*

