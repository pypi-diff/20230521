# Comparing `tmp/mleko-0.3.0.tar.gz` & `tmp/mleko-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-0.3.0.tar", max compression
+gzip compressed data, was "mleko-0.3.1.tar", max compression
```

## Comparing `mleko-0.3.0.tar` & `mleko-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1073 2023-05-21 14:10:30.223787 mleko-0.3.0/LICENSE
--rw-r--r--   0        0        0     2561 2023-05-21 14:10:30.223787 mleko-0.3.0/README.md
--rw-r--r--   0        0        0     2753 2023-05-21 14:11:10.535467 mleko-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1286 2023-05-21 14:11:10.447468 mleko-0.3.0/src/mleko/__init__.py
--rw-r--r--   0        0        0     1372 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/cache/__init__.py
--rw-r--r--   0        0        0    15230 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/cache/cache.py
--rw-r--r--   0        0        0     3573 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/cache/fingerprinters.py
--rw-r--r--   0        0        0      502 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/__init__.py
--rw-r--r--   0        0        0    11680 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/converters.py
--rw-r--r--   0        0        0      676 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/sources/__init__.py
--rw-r--r--   0        0        0     2760 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/sources/base_data_source.py
--rw-r--r--   0        0        0    17181 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/sources/kaggle_data_source.py
--rw-r--r--   0        0        0     8531 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/sources/s3_data_source.py
--rw-r--r--   0        0        0    10930 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/data/splitters.py
--rw-r--r--   0        0        0      608 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1095 2023-05-21 14:10:30.227787 mleko-0.3.0/src/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     3869 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     3215 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      515 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/steps/convert.py
--rw-r--r--   0        0        0     2080 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/steps/ingest.py
--rw-r--r--   0        0        0     2110 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/pipeline/steps/split.py
--rw-r--r--   0        0        0        0 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/py.typed
--rw-r--r--   0        0        0      731 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/__init__.py
--rw-r--r--   0        0        0     4497 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     2698 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/decorators.py
--rw-r--r--   0        0        0      742 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1176 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/tqdm.py
--rw-r--r--   0        0        0     1600 2023-05-21 14:10:30.231787 mleko-0.3.0/src/mleko/utils/vaex.py
--rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 mleko-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-21 14:49:50.169455 mleko-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2561 2023-05-21 14:49:50.169455 mleko-0.3.1/README.md
+-rw-r--r--   0        0        0     2753 2023-05-21 14:50:31.169551 mleko-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1286 2023-05-21 14:50:31.101550 mleko-0.3.1/src/mleko/__init__.py
+-rw-r--r--   0        0        0     1372 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    15230 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/cache/cache.py
+-rw-r--r--   0        0        0     3573 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/cache/fingerprinters.py
+-rw-r--r--   0        0        0      502 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/data/__init__.py
+-rw-r--r--   0        0        0    11680 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/data/converters.py
+-rw-r--r--   0        0        0      676 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/data/sources/__init__.py
+-rw-r--r--   0        0        0     2760 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/data/sources/base_data_source.py
+-rw-r--r--   0        0        0    17518 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/data/sources/kaggle_data_source.py
+-rw-r--r--   0        0        0     8531 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/data/sources/s3_data_source.py
+-rw-r--r--   0        0        0    10930 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/data/splitters.py
+-rw-r--r--   0        0        0      608 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1095 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4205 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3425 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      515 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/steps/convert.py
+-rw-r--r--   0        0        0     2080 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/steps/ingest.py
+-rw-r--r--   0        0        0     2110 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/steps/split.py
+-rw-r--r--   0        0        0        0 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/py.typed
+-rw-r--r--   0        0        0      731 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     4497 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     2698 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      742 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1176 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/tqdm.py
+-rw-r--r--   0        0        0     1600 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/vaex.py
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 mleko-0.3.1/PKG-INFO
```

### Comparing `mleko-0.3.0/LICENSE` & `mleko-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/README.md` & `mleko-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/pyproject.toml` & `mleko-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "0.3.0"
+version = "0.3.1"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErikBavenstrand/mleko"
 repository = "https://github.com/ErikBavenstrand/mleko"
 documentation = "https://mleko.readthedocs.io"
```

### Comparing `mleko-0.3.0/src/mleko/__init__.py` & `mleko-0.3.1/src/mleko/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,8 +16,8 @@
    caching of method call results and tracking changes in data.
 
 * Utilities: A collection of utility functions for logging, decorating, file management, and TQDM wrappers.
 
 Each subpackage is designed to be modular and extensible, making it easy to customize and adapt the library to a wide
 range of model building processes and requirements.
 """
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `mleko-0.3.0/src/mleko/cache/__init__.py` & `mleko-0.3.1/src/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/cache/cache.py` & `mleko-0.3.1/src/mleko/cache/cache.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/cache/fingerprinters.py` & `mleko-0.3.1/src/mleko/cache/fingerprinters.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/data/converters.py` & `mleko-0.3.1/src/mleko/data/converters.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/data/sources/__init__.py` & `mleko-0.3.1/src/mleko/data/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/data/sources/base_data_source.py` & `mleko-0.3.1/src/mleko/data/sources/base_data_source.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/data/sources/kaggle_data_source.py` & `mleko-0.3.1/src/mleko/data/sources/kaggle_data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,19 @@
             file_names: A list of file names to download. If not provided or empty, all files in
                 the dataset will be downloaded.
             dataset_version: The specific dataset version number to download. If not provided,
                 the latest version will be fetched.
             kaggle_api_credentials_file: Path to a Kaggle API credentials JSON file. If not
                 provided, environment variables or the default file location will be used.
             num_workers: Number of concurrent threads to use when downloading files.
+
+        Note:
+            The Kaggle API is not perfect and sometimes returns incorrect metadata for files, where one or more of the
+            files are missing from the dataset. This can lead to the wrong files being downloaded or the download
+            failing altogether. If you encounter this issue, please report it to Kaggle.
         """
         super().__init__(destination_directory)
 
         self._owner_slug, self._dataset_slug, self._dataset_version = owner_slug, dataset_slug, dataset_version
         self._file_names: set[str] = set(file_names) if file_names is not None else set()
         self._kaggle_config = KaggleCredentialsManager.get_kaggle_credentials(kaggle_api_credentials_file)
         self._num_workers = num_workers
```

### Comparing `mleko-0.3.0/src/mleko/data/sources/s3_data_source.py` & `mleko-0.3.1/src/mleko/data/sources/s3_data_source.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/data/splitters.py` & `mleko-0.3.1/src/mleko/data/splitters.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/pipeline/__init__.py` & `mleko-0.3.1/src/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/pipeline/data_container.py` & `mleko-0.3.1/src/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/pipeline/pipeline.py` & `mleko-0.3.1/src/mleko/pipeline/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,19 @@
     def __init__(self, steps: list[PipelineStep] | None = None) -> None:
         """Creates a new Pipeline instance, initializing it with a list of steps or an empty list.
 
         Args:
             steps: An optional list of `PipelineStep` instances that define the data processing steps in the
                    pipeline. If not provided, the pipeline will be initialized with an empty list of steps,
                    allowing steps to be added later using the `add_step` method.
+
+        Note:
+            The steps list can be provided as an argument to the constructor, or the pipeline can be initialized
+            with an empty list of steps and have them added later using the `add_step` method. This allows for
+            more flexibility in the creation of the pipeline, as steps can be added dynamically.
         """
         self.steps = steps if steps is not None else []
 
     def __repr__(self) -> str:
         """Returns a string representation of the Pipeline, including the ordered list of steps.
 
         Returns:
```

### Comparing `mleko-0.3.0/src/mleko/pipeline/pipeline_step.py` & `mleko-0.3.1/src/mleko/pipeline/pipeline_step.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,19 @@
 
 
 class PipelineStep(ABC):
     """Base class for all pipeline steps, ensuring the standardized interface for performing data processing operations.
 
     Descendants of this class must implement the `execute` method, which carries out the data processing operation
     related to the step.
-    NOTE: the _num_inputs and _num_outputs attributes are used to validate the number of inputs and outputs and must be
-    set by the subclass.
+
+    Note:
+        The _num_inputs and _num_outputs attributes are used to validate the number of inputs and outputs, respectively,
+        for each step. These attributes are set by the subclasses, and should not be modified by the user.
+        When implementing a new step, you should set these attributes to the expected number of inputs and outputs.
     """
 
     _num_inputs: int
     """Number of inputs expected by the PipelineStep."""
 
     _num_outputs: int
     """Number of outputs expected by the PipelineStep."""
```

### Comparing `mleko-0.3.0/src/mleko/pipeline/steps/__init__.py` & `mleko-0.3.1/src/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/pipeline/steps/convert.py` & `mleko-0.3.1/src/mleko/pipeline/steps/convert.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/pipeline/steps/ingest.py` & `mleko-0.3.1/src/mleko/pipeline/steps/ingest.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/pipeline/steps/split.py` & `mleko-0.3.1/src/mleko/pipeline/steps/split.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/utils/__init__.py` & `mleko-0.3.1/src/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/utils/custom_logger.py` & `mleko-0.3.1/src/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/utils/decorators.py` & `mleko-0.3.1/src/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/utils/file_helpers.py` & `mleko-0.3.1/src/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/utils/tqdm.py` & `mleko-0.3.1/src/mleko/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/src/mleko/utils/vaex.py` & `mleko-0.3.1/src/mleko/utils/vaex.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.0/PKG-INFO` & `mleko-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 0.3.0
+Version: 0.3.1
 Summary: ML-Ekosystem
 Home-page: https://github.com/ErikBavenstrand/mleko
 License: MIT
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 3 - Alpha
```

