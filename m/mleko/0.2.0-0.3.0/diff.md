# Comparing `tmp/mleko-0.2.0.tar.gz` & `tmp/mleko-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-0.2.0.tar", max compression
+gzip compressed data, was "mleko-0.3.0.tar", max compression
```

## Comparing `mleko-0.2.0.tar` & `mleko-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1073 2023-05-21 10:52:49.698292 mleko-0.2.0/LICENSE
--rw-r--r--   0        0        0     2561 2023-05-21 10:52:49.698292 mleko-0.2.0/README.md
--rw-r--r--   0        0        0     2753 2023-05-21 10:53:17.698311 mleko-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1286 2023-05-21 10:53:17.646311 mleko-0.2.0/src/mleko/__init__.py
--rw-r--r--   0        0        0     1372 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/cache/__init__.py
--rw-r--r--   0        0        0    15230 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/cache/cache.py
--rw-r--r--   0        0        0     3573 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/cache/fingerprinters.py
--rw-r--r--   0        0        0      502 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/__init__.py
--rw-r--r--   0        0        0    11434 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/converters.py
--rw-r--r--   0        0        0      676 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/sources/__init__.py
--rw-r--r--   0        0        0     2760 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/sources/base_data_source.py
--rw-r--r--   0        0        0    17181 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/sources/kaggle_data_source.py
--rw-r--r--   0        0        0     8531 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/sources/s3_data_source.py
--rw-r--r--   0        0        0     9986 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/splitters.py
--rw-r--r--   0        0        0      608 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1095 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     3869 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     3215 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      515 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/steps/convert.py
--rw-r--r--   0        0        0     2080 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/steps/ingest.py
--rw-r--r--   0        0        0     2110 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/steps/split.py
--rw-r--r--   0        0        0        0 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/py.typed
--rw-r--r--   0        0        0      731 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/__init__.py
--rw-r--r--   0        0        0     4497 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     2698 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/decorators.py
--rw-r--r--   0        0        0      742 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1176 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/tqdm.py
--rw-r--r--   0        0        0     1600 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/vaex.py
--rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 mleko-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-21 14:10:30.223787 mleko-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2561 2023-05-21 14:10:30.223787 mleko-0.3.0/README.md
+-rw-r--r--   0        0        0     2753 2023-05-21 14:11:10.535467 mleko-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1286 2023-05-21 14:11:10.447468 mleko-0.3.0/src/mleko/__init__.py
+-rw-r--r--   0        0        0     1372 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    15230 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/cache/cache.py
+-rw-r--r--   0        0        0     3573 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/cache/fingerprinters.py
+-rw-r--r--   0        0        0      502 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/__init__.py
+-rw-r--r--   0        0        0    11680 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/converters.py
+-rw-r--r--   0        0        0      676 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/sources/__init__.py
+-rw-r--r--   0        0        0     2760 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/sources/base_data_source.py
+-rw-r--r--   0        0        0    17181 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/sources/kaggle_data_source.py
+-rw-r--r--   0        0        0     8531 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/sources/s3_data_source.py
+-rw-r--r--   0        0        0    10930 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/splitters.py
+-rw-r--r--   0        0        0      608 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1095 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     3869 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3215 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      515 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/steps/convert.py
+-rw-r--r--   0        0        0     2080 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/steps/ingest.py
+-rw-r--r--   0        0        0     2110 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/steps/split.py
+-rw-r--r--   0        0        0        0 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/py.typed
+-rw-r--r--   0        0        0      731 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     4497 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     2698 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      742 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1176 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/tqdm.py
+-rw-r--r--   0        0        0     1600 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/vaex.py
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 mleko-0.3.0/PKG-INFO
```

### Comparing `mleko-0.2.0/LICENSE` & `mleko-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/README.md` & `mleko-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/pyproject.toml` & `mleko-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "0.2.0"
+version = "0.3.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErikBavenstrand/mleko"
 repository = "https://github.com/ErikBavenstrand/mleko"
 documentation = "https://mleko.readthedocs.io"
```

### Comparing `mleko-0.2.0/src/mleko/__init__.py` & `mleko-0.3.0/src/mleko/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
    caching of method call results and tracking changes in data.
 
 * Utilities: A collection of utility functions for logging, decorating, file management, and TQDM wrappers.
 
 Each subpackage is designed to be modular and extensible, making it easy to customize and adapt the library to a wide
 range of model building processes and requirements.
 """
-__version__ = "0.2.0"
+__version__ = "0.3.0"
```

### Comparing `mleko-0.2.0/src/mleko/cache/__init__.py` & `mleko-0.3.0/src/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/cache/cache.py` & `mleko-0.3.0/src/mleko/cache/cache.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/cache/fingerprinters.py` & `mleko-0.3.0/src/mleko/cache/fingerprinters.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/data/converters.py` & `mleko-0.3.0/src/mleko/data/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,16 @@
         self._num_workers = num_workers
         self._random_state = random_state
 
     def convert(self, file_paths: list[Path] | list[str], force_recompute: bool = False) -> vaex.DataFrame:
         """Converts a list of CSV files to Arrow format and returns a vaex dataframe joined from the converted data.
 
         The method takes care of caching, and results will be reused accordingly unless force_recompute is set to True.
+        The resulting dataframe is a vaex DataFrame joined from the converted data. The conversion is done in chunks
+        to optimize parallel processing.
 
         Args:
             file_paths: A list of file paths to be converted.
             force_recompute: If set to True, forces recomputation and ignores the cache.
 
         Returns:
             vaex.DataFrame: The resulting dataframe with the combined converted data.
@@ -163,15 +165,16 @@
         na_values: tuple[str, ...],
         true_values: tuple[str, ...],
         false_values: tuple[str, ...],
         downcast_float: bool,
     ) -> None:
         """Converts a single CSV file to Arrow format using the provided options and saves it to the output directory.
 
-        This operation is done in chunks to optimize parallel processing.
+        This operation is done in chunks to optimize parallel processing. The resulting dataframe is saved in the
+        output directory with the given suffix.
 
         Args:
             file_path: The path of the CSV file to be converted.
             output_directory: The directory where the converted file should be saved.
             dataframe_suffix: The suffix for the converted dataframe files.
             forced_numerical_columns: A sequence of column names to be forced to numerical type.
             forced_categorical_columns: A sequence of column names to be forced to categorical type.
```

### Comparing `mleko-0.2.0/src/mleko/data/sources/__init__.py` & `mleko-0.3.0/src/mleko/data/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/data/sources/base_data_source.py` & `mleko-0.3.0/src/mleko/data/sources/base_data_source.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/data/sources/kaggle_data_source.py` & `mleko-0.3.0/src/mleko/data/sources/kaggle_data_source.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/data/sources/s3_data_source.py` & `mleko-0.3.0/src/mleko/data/sources/s3_data_source.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/data/splitters.py` & `mleko-0.3.0/src/mleko/data/splitters.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,35 @@
 
 
 class RandomDataSplitter(BaseDataSplitter, VaexArrowCacheFormatMixin, LRUCacheMixin):
     """A class that handles random splitting of Vaex DataFrames.
 
     This class provides a method for splitting a Vaex DataFrame into two parts, with the split being performed
     randomly. The split can be stratified by specifying a column name to use for stratification.
+
+    Note:
+        The stratification is performed before the split, meaning that the split will be performed on the stratified
+        data. For example, if the data is split into 80% train and 20% test, and the stratification column contains
+        80% of the rows with value 0 and 20% of the rows with value 1, the resulting split will contain 80% of the
+        rows with value 0 and 20% of the rows with value 1.
+
+    Example:
+        >>> import vaex
+        >>> from mleko.data.splitters import RandomDataSplitter
+        >>> df = vaex.from_arrays(x=[1, 2, 3, 4], y=[0, 1, 1, 0])
+        >>> splitter = RandomDataSplitter(output_directory="cache", data_split=(0.50, 0.50), shuffle=True, stratify="y")
+        >>> df_train, df_test = splitter.split(df)
+        >>> df_train
+            #    x    y
+            0    1    0
+            1    3    1
+        >>> df_test
+            #    x    y
+            0    2    1
+            1    4    0
     """
 
     @auto_repr
     def __init__(
         self,
         output_directory: str | Path,
         data_split: tuple[float, float] = (0.80, 0.20),
```

### Comparing `mleko-0.2.0/src/mleko/pipeline/__init__.py` & `mleko-0.3.0/src/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/pipeline/data_container.py` & `mleko-0.3.0/src/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/pipeline/pipeline.py` & `mleko-0.3.0/src/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/pipeline/pipeline_step.py` & `mleko-0.3.0/src/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/pipeline/steps/__init__.py` & `mleko-0.3.0/src/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/pipeline/steps/convert.py` & `mleko-0.3.0/src/mleko/pipeline/steps/convert.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/pipeline/steps/ingest.py` & `mleko-0.3.0/src/mleko/pipeline/steps/ingest.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/pipeline/steps/split.py` & `mleko-0.3.0/src/mleko/pipeline/steps/split.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/utils/__init__.py` & `mleko-0.3.0/src/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/utils/custom_logger.py` & `mleko-0.3.0/src/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/utils/decorators.py` & `mleko-0.3.0/src/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/utils/file_helpers.py` & `mleko-0.3.0/src/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/utils/tqdm.py` & `mleko-0.3.0/src/mleko/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/src/mleko/utils/vaex.py` & `mleko-0.3.0/src/mleko/utils/vaex.py`

 * *Files identical despite different names*

### Comparing `mleko-0.2.0/PKG-INFO` & `mleko-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 0.2.0
+Version: 0.3.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/ErikBavenstrand/mleko
 License: MIT
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 3 - Alpha
```

