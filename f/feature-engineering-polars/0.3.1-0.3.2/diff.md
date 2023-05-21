# Comparing `tmp/feature_engineering_polars-0.3.1.tar.gz` & `tmp/feature_engineering_polars-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_engineering_polars-0.3.1.tar", max compression
+gzip compressed data, was "feature_engineering_polars-0.3.2.tar", max compression
```

## Comparing `feature_engineering_polars-0.3.1.tar` & `feature_engineering_polars-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/LICENSE
--rw-r--r--   0        0        0     1909 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/__init__.py
--rw-r--r--   0        0        0      133 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/encoding/__init__.py
--rw-r--r--   0        0        0     2066 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/encoding/one_hot_encoding.py
--rw-r--r--   0        0        0     4735 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/encoding/target_encoding.py
--rw-r--r--   0        0        0       58 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/imputing/__init__.py
--rw-r--r--   0        0        0     6948 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/imputing/base_imputing.py
--rw-r--r--   0        0        0     1270 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 feature_engineering_polars-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-21 12:33:52.548313 feature_engineering_polars-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1909 2023-05-21 12:33:52.548313 feature_engineering_polars-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 12:33:52.548313 feature_engineering_polars-0.3.2/fe_polars/__init__.py
+-rw-r--r--   0        0        0      133 2023-05-21 12:33:52.548313 feature_engineering_polars-0.3.2/fe_polars/encoding/__init__.py
+-rw-r--r--   0        0        0     2084 2023-05-21 12:33:52.548313 feature_engineering_polars-0.3.2/fe_polars/encoding/one_hot_encoding.py
+-rw-r--r--   0        0        0     5419 2023-05-21 12:33:52.548313 feature_engineering_polars-0.3.2/fe_polars/encoding/target_encoding.py
+-rw-r--r--   0        0        0       58 2023-05-21 12:33:52.548313 feature_engineering_polars-0.3.2/fe_polars/imputing/__init__.py
+-rw-r--r--   0        0        0     6953 2023-05-21 12:33:52.548313 feature_engineering_polars-0.3.2/fe_polars/imputing/base_imputing.py
+-rw-r--r--   0        0        0     1270 2023-05-21 12:33:52.548313 feature_engineering_polars-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 feature_engineering_polars-0.3.2/PKG-INFO
```

### Comparing `feature_engineering_polars-0.3.1/LICENSE` & `feature_engineering_polars-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feature_engineering_polars-0.3.1/README.md` & `feature_engineering_polars-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `feature_engineering_polars-0.3.1/fe_polars/encoding/one_hot_encoding.py` & `feature_engineering_polars-0.3.2/fe_polars/encoding/one_hot_encoding.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,20 +22,21 @@
         self.strategy = strategy
         self.features_to_encode = features_to_encode
 
     def fit(
         self,
         x: polars.DataFrame,
         y: Optional[Union[polars.Series, polars.DataFrame]] = None,
-    ) -> None:
+    ) -> "OneHotEncoder":
         """Fit One Hot Encoder.
 
-        Pass as not needed
+        Returns:
+            self
         """
-        return None
+        return self
 
     def transform(
         self,
         x: polars.DataFrame,
     ) -> polars.DataFrame:
         """Apply one hot encoding to the provided dataframe.
```

### Comparing `feature_engineering_polars-0.3.1/fe_polars/encoding/target_encoding.py` & `feature_engineering_polars-0.3.2/fe_polars/encoding/target_encoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,26 +23,44 @@
         if isinstance(features_to_encode, str):
             features_to_encode = [features_to_encode]
         self.smoothing = smoothing
         self.features_to_encode = features_to_encode
         self.global_mean: Union[int, float, None] = None
         self.mapping: Dict[str, Dict[str, Any]] = dict()
 
+    def _check_features_unique_values(self, x: polars.DataFrame) -> None:
+        """Check if the features to impute are numerical.
+
+        Args:
+            x (polars.DataFrame): feature dataset
+
+        Returns:
+            None
+        """
+        for feature in self.features_to_encode:
+            pct_unique = x[feature].n_unique() / x.height
+            if pct_unique >= 0.5 and x[feature].is_numeric():
+                logger = logging.getLogger(__name__)
+                logger.warning(f"Feature ['{feature}'] is possibly numerical")
+
     def fit(
         self, x: polars.DataFrame, y: Union[polars.Series, polars.DataFrame]
-    ) -> None:
+    ) -> "TargetEncoder":
         """Fit the target encoder.
 
         Args:
             x (polars.DataFrame): features table
             y (y: Union[polars.Series, polars.DataFrame]): target
 
         Returns:
-            None
+            self
         """
+        # Check if the features to impute are numerical and warn the user if not
+        self._check_features_unique_values(x)
+
         if isinstance(y, polars.DataFrame):
             on = y.columns[0]
         else:
             on = y.name
 
         x = x.with_columns(y)
 
@@ -66,15 +84,15 @@
                 )
                 / (polars.col("count") + self.smoothing)
             ).select([polars.col(feature), polars.col("encoding")])
             self.mapping[feature] = {
                 "table": smooth.to_dict(as_series=False),
                 "dtype": x.get_column(feature).dtype,
             }
-        return None
+        return self
 
     def transform(self, x: polars.DataFrame) -> polars.DataFrame:
         """Apply the mapping to the provided dataframe.
 
         Args:
             x (polars.DataFrame): features table to transform
```

### Comparing `feature_engineering_polars-0.3.1/fe_polars/imputing/base_imputing.py` & `feature_engineering_polars-0.3.2/fe_polars/imputing/base_imputing.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,23 +136,23 @@
         else:
             self.mapping[feature] = self.strategy_dict["fixed_value"][feature]
 
     def fit(
         self,
         x: polars.DataFrame,
         y: Optional[Union[polars.DataFrame, polars.Series]] = None,
-    ) -> None:
+    ) -> "Imputer":
         """Fit.
 
         Args:
             x (polars.DataFrame): feature dataset
             y (y: Union[polars.Series, polars.DataFrame]): target (not used)
 
         Returns:
-            None
+            self
         """
         # If no strategy dictionnary has been provided and neither was a list of feature
         # to impute, then we apply the strategy on all the columns that contain
         # null values
         if self._fit_strategy_dict:
             self.features_to_impute = [
                 col
@@ -163,15 +163,15 @@
 
         for strategy in self.strategy_dict.keys():
             for feature in self.strategy_dict[strategy]:
                 if not x[feature].is_numeric():
                     raise ValueError(f"{feature} is not a numerical feature")
                 self._process_strategy(strategy, feature, x)
 
-        return None
+        return self
 
     def transform(self, x: polars.DataFrame) -> polars.DataFrame:
         """Transform.
 
         Args:
             x (polars.DataFrame): feature dataset
```

### Comparing `feature_engineering_polars-0.3.1/pyproject.toml` & `feature_engineering_polars-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.poetry]
 name = "feature-engineering-polars"
-version = "0.3.1"
+version = "0.3.2"
 description = "Feature engineering done with Polars"
 authors = ["Jordan Delbar <jordandelbar@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{ include = "fe_polars" }]
 
 [tool.poetry.dependencies]
```

### Comparing `feature_engineering_polars-0.3.1/PKG-INFO` & `feature_engineering_polars-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-engineering-polars
-Version: 0.3.1
+Version: 0.3.2
 Summary: Feature engineering done with Polars
 License: MIT
 Author: Jordan Delbar
 Author-email: jordandelbar@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

