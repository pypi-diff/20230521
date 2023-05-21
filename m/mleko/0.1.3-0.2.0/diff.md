# Comparing `tmp/mleko-0.1.3.tar.gz` & `tmp/mleko-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-0.1.3.tar", max compression
+gzip compressed data, was "mleko-0.2.0.tar", max compression
```

## Comparing `mleko-0.1.3.tar` & `mleko-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0     1073 2023-05-13 20:42:48.653768 mleko-0.1.3/LICENSE
--rw-r--r--   0        0        0     2561 2023-05-13 20:42:48.653768 mleko-0.1.3/README.md
--rw-r--r--   0        0        0     2707 2023-05-13 20:43:22.029558 mleko-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1286 2023-05-13 20:43:21.981559 mleko-0.1.3/src/mleko/__init__.py
--rw-r--r--   0        0        0     1309 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/cache/__init__.py
--rw-r--r--   0        0        0    12625 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/cache/cache.py
--rw-r--r--   0        0        0     3098 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/cache/fingerprinters.py
--rw-r--r--   0        0        0      502 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/data/__init__.py
--rw-r--r--   0        0        0    12181 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/data/converters.py
--rw-r--r--   0        0        0      676 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/data/sources/__init__.py
--rw-r--r--   0        0        0     2778 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/data/sources/base_data_source.py
--rw-r--r--   0        0        0    17258 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/data/sources/kaggle_data_source.py
--rw-r--r--   0        0        0     8650 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/data/sources/s3_data_source.py
--rw-r--r--   0        0        0      608 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1061 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     3578 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     1577 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      473 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     1685 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/pipeline/steps/convert.py
--rw-r--r--   0        0        0     1548 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/pipeline/steps/ingest.py
--rw-r--r--   0        0        0        0 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/py.typed
--rw-r--r--   0        0        0      581 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/utils/__init__.py
--rw-r--r--   0        0        0     4523 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     2698 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/utils/decorators.py
--rw-r--r--   0        0        0      742 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1176 2023-05-13 20:42:48.657768 mleko-0.1.3/src/mleko/utils/tqdm.py
--rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 mleko-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-21 10:52:49.698292 mleko-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2561 2023-05-21 10:52:49.698292 mleko-0.2.0/README.md
+-rw-r--r--   0        0        0     2753 2023-05-21 10:53:17.698311 mleko-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1286 2023-05-21 10:53:17.646311 mleko-0.2.0/src/mleko/__init__.py
+-rw-r--r--   0        0        0     1372 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    15230 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/cache/cache.py
+-rw-r--r--   0        0        0     3573 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/cache/fingerprinters.py
+-rw-r--r--   0        0        0      502 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/__init__.py
+-rw-r--r--   0        0        0    11434 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/converters.py
+-rw-r--r--   0        0        0      676 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/sources/__init__.py
+-rw-r--r--   0        0        0     2760 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/sources/base_data_source.py
+-rw-r--r--   0        0        0    17181 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/sources/kaggle_data_source.py
+-rw-r--r--   0        0        0     8531 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/sources/s3_data_source.py
+-rw-r--r--   0        0        0     9986 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/data/splitters.py
+-rw-r--r--   0        0        0      608 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1095 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     3869 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3215 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      515 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/steps/convert.py
+-rw-r--r--   0        0        0     2080 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/steps/ingest.py
+-rw-r--r--   0        0        0     2110 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/pipeline/steps/split.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/py.typed
+-rw-r--r--   0        0        0      731 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     4497 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     2698 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      742 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1176 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/tqdm.py
+-rw-r--r--   0        0        0     1600 2023-05-21 10:52:49.702292 mleko-0.2.0/src/mleko/utils/vaex.py
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 mleko-0.2.0/PKG-INFO
```

### Comparing `mleko-0.1.3/LICENSE` & `mleko-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-0.1.3/README.md` & `mleko-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-0.1.3/pyproject.toml` & `mleko-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "0.1.3"
+version = "0.2.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErikBavenstrand/mleko"
 repository = "https://github.com/ErikBavenstrand/mleko"
 documentation = "https://mleko.readthedocs.io"
@@ -17,14 +17,15 @@
 
 [tool.poetry.dependencies]
 python = "3.10.* || 3.9.* || 3.8.*"
 boto3 = "^1.26.91"
 botocore = "^1.29.91"
 tqdm = "^4.65.0"
 vaex = "^4.16.0"
+scikit-learn = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 boto3-stubs = {extras = ["s3"], version = "^1.26.91"}
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
@@ -93,15 +94,16 @@
     "vaex",
     "tqdm",
     "boto3",
     "boto3.s3.transfer",
     "botocore.config",
     "pyarrow",
     "requests",
-    "requests.auth"
+    "requests.auth",
+    "sklearn.model_selection",
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
@@ -111,8 +113,8 @@
 version_toml = "pyproject.toml:tool.poetry.version"
 version_source = "tag"
 commit_version_number = true
 tag_commit = true
 upload_to_pypi = false
 upload_to_release = false
 hvcs = "github"
-commit_message = "chore(release): release {version} [skip ci]"
+commit_message = "chore(release): release {version}"
```

### Comparing `mleko-0.1.3/src/mleko/__init__.py` & `mleko-0.2.0/src/mleko/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
    caching of method call results and tracking changes in data.
 
 * Utilities: A collection of utility functions for logging, decorating, file management, and TQDM wrappers.
 
 Each subpackage is designed to be modular and extensible, making it easy to customize and adapt the library to a wide
 range of model building processes and requirements.
 """
-__version__ = "0.1.3"
+__version__ = "0.2.0"
```

### Comparing `mleko-0.1.3/src/mleko/cache/__init__.py` & `mleko-0.2.0/src/mleko/cache/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,11 +12,17 @@
    and when used in combination with the caching mixins, can enhance the caching mechanisms by providing
    more unique and consistent cache keys.
 
 Together, these components allow efficient caching of method call results, reduce processing time and
 resource usage, and make it easier to identify and manage changes in data.
 """
 from .cache import CacheMixin, LRUCacheMixin
-from .fingerprinters import CSVFingerprinter, Fingerprinter
+from .fingerprinters import CSVFingerprinter, Fingerprinter, VaexFingerprinter
 
 
-__all__ = ["CacheMixin", "LRUCacheMixin", "CSVFingerprinter", "Fingerprinter"]
+__all__ = [
+    "CacheMixin",
+    "LRUCacheMixin",
+    "CSVFingerprinter",
+    "VaexFingerprinter",
+    "Fingerprinter",
+]
```

### Comparing `mleko-0.1.3/src/mleko/cache/cache.py` & `mleko-0.2.0/src/mleko/cache/cache.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,18 +17,22 @@
 
 import hashlib
 import inspect
 import pickle
 import re
 from collections import OrderedDict
 from pathlib import Path
-from typing import Any, Callable, Hashable
+from typing import Any, Callable, Hashable, Sequence
+
+import vaex
+from tqdm import tqdm
 
 from mleko.cache.fingerprinters import Fingerprinter
 from mleko.utils.custom_logger import CustomLogger
+from mleko.utils.tqdm import set_tqdm_percent_wrapper
 
 
 logger = CustomLogger()
 """A CustomLogger instance that's used throughout the module for logging."""
 
 
 def get_frame_qualname(frame: inspect.FrameInfo) -> str:
@@ -46,14 +50,51 @@
     module_name = caller_obj.__name__ if caller_obj is not None else "__main__"
     if "self" in frame.frame.f_locals:
         class_name = frame.frame.f_locals["self"].__class__.__name__
         return f"{module_name}.{class_name}.{caller_function}"
     return f"{module_name}.{caller_function}"
 
 
+class VaexArrowCacheFormatMixin:
+    """A mixin class for Vaex DataFrames to provide Arrow format caching capabilities.
+
+    This mixin class adds methods for reading and writing arrow cache files for Vaex DataFrames.
+    """
+
+    cache_file_suffix = "arrow"
+    """The file extension to use for cache files."""
+
+    def _read_cache_file(self, cache_file_path: Path) -> vaex.DataFrame:
+        """Reads a cache file containing a Vaex DataFrame.
+
+        Args:
+            cache_file_path: The path of the cache file to be read.
+
+        Returns:
+            The contents of the cache file as a DataFrame.
+        """
+        return vaex.open(cache_file_path)
+
+    def _write_cache_file(self, cache_file_path: Path, output: vaex.DataFrame) -> None:
+        """Writes the results of the DataFrame conversion to Arrow format in a cache file with arrow suffix.
+
+        Args:
+            cache_file_path: The path of the cache file to be written.
+            output: The Vaex DataFrame to be saved in the cache file.
+        """
+        with tqdm(total=100, desc="Writing DataFrame to Arrow file") as pbar:
+            output.export_arrow(
+                cache_file_path,
+                progress=set_tqdm_percent_wrapper(pbar),
+                parallel=True,
+                reduce_large=True,
+            )
+        output.close()
+
+
 class CacheMixin:
     """A mixin class for caching the results of method calls based on user-defined cache keys and fingerprints.
 
     Warning:
         This class maintains an ever-growing cache, which means that the cache size may increase indefinitely
         with new method calls, possibly consuming a large amount of disk space. It does not implement any
         cache eviction strategy. It is recommended to either clear the cache manually when needed or
@@ -84,15 +125,15 @@
         """Executes the given function, caching the results based on the provided cache keys and fingerprints.
 
         Args:
             lambda_func: A lambda function to execute.
             cache_keys: A list of cache keys that can be a mix of hashable values and tuples containing a value and a
                 Fingerprinter instance for generating fingerprints.
             force_recompute: A boolean indicating whether to force recompute the result and update the cache, even if a
-                cached result is available. Defaults to False.
+                cached result is available.
 
         Returns:
             The result of executing the given function. If a cached result is available and force_recompute is False,
             the cached result will be returned instead of recomputing the result.
         """
         frame_qualname = get_frame_qualname(inspect.stack()[1])
         class_method_name = ".".join(frame_qualname.split(".")[-2:])
@@ -136,15 +177,17 @@
             if isinstance(key, tuple) and len(key) == 2 and isinstance(key[1], Fingerprinter):
                 value, fingerprinter = key
                 values_to_hash.append(fingerprinter.fingerprint(value))
             else:
                 values_to_hash.append(key)
 
         data = pickle.dumps((frame_qualname, values_to_hash))
-        cache_key = hashlib.md5(data).hexdigest()
+
+        class_method_name = ".".join(frame_qualname.split(".")[-2:])
+        cache_key = f"{class_method_name}.{hashlib.md5(data).hexdigest()}"
 
         return cache_key
 
     def _read_cache_file(self, cache_file_path: Path) -> Any:
         """Reads the cache file from the specified path and returns the deserialized data.
 
         This method can be overridden in subclasses to customize the cache loading process.
@@ -163,40 +206,59 @@
 
         Args:
             cache_key: A string representing the cache key.
 
         Returns:
             The cached data if it exists, or None if there is no data for the given cache key.
         """
-        cache_file_path = self._cache_directory / f"{cache_key}.{self._cache_file_suffix}"
-        if cache_file_path.exists():
-            return self._read_cache_file(cache_file_path)
+
+        def extract_number(file_path: Path) -> int:
+            result = re.search(r"[a-fA-F\d]{32}_(\d+).", str(file_path))
+            return int(result.group(1)) if result else 0
+
+        cache_file_paths = sorted(
+            list(self._cache_directory.glob(f"{cache_key}*.{self._cache_file_suffix}")), key=extract_number
+        )
+        if cache_file_paths:
+            output_data = []
+            for cache_file_path in cache_file_paths:
+                output_data.append(self._read_cache_file(cache_file_path))
+            return tuple(output_data) if len(output_data) > 1 else output_data[0]
         return None
 
     def _write_cache_file(self, cache_file_path: Path, output: Any) -> None:
         """Writes the given data to a cache file at the specified path, serializing it using pickle.
 
         This method can be overridden in subclasses to customize the cache saving process.
 
         Args:
             cache_file_path: A Path object representing the location where the cache file should be saved.
             output: The data to be serialized and saved to the cache file.
         """
         with open(cache_file_path, "wb") as cache_file:
             pickle.dump(output, cache_file)
 
-    def _save_to_cache(self, cache_key: str, output: Any) -> None:
+    def _save_to_cache(self, cache_key: str, output: Any | Sequence[Any]) -> None:
         """Saves the given data to the cache using the provided cache key.
 
+        If the output is a sequence, each element will be saved to a separate cache file. Otherwise, the output will be
+        saved to a single cache file. The cache file will be saved in the cache directory with the cache key as the
+        filename and the cache file suffix as the file extension.
+
         Args:
             cache_key: A string representing the cache key.
             output: The data to be saved to the cache.
         """
-        cache_file_path = self._cache_directory / f"{cache_key}.{self._cache_file_suffix}"
-        self._write_cache_file(cache_file_path, output)
+        if isinstance(output, Sequence):
+            for i in range(len(output)):
+                cache_file_path = self._cache_directory / f"{cache_key}_{i}.{self._cache_file_suffix}"
+                self._write_cache_file(cache_file_path, output[i])
+        else:
+            cache_file_path = self._cache_directory / f"{cache_key}.{self._cache_file_suffix}"
+            self._write_cache_file(cache_file_path, output)
 
 
 class LRUCacheMixin(CacheMixin):
     """Least Recently Used Cache Mixin.
 
     This mixin class extends the CacheMixin to provide a Least Recently Used (LRU) cache mechanism.
     It evicts the least recently used cache entries when the maximum number of cache entries is exceeded.
@@ -218,56 +280,57 @@
         self._load_cache_from_disk()
 
     def _load_cache_from_disk(self) -> None:
         """Loads the cache entries from the cache directory and initializes the LRU cache.
 
         Cache entries are ordered by their modification time, and the cache is trimmed if needed.
         """
+        frame_qualname = get_frame_qualname(inspect.stack()[2])
+        class_name = frame_qualname.split(".")[-2]
         cache_files = [
             f
             for f in self._cache_directory.glob(f"*.{self._cache_file_suffix}")
-            if re.search(r"^[a-fA-F\d]{32}$", str(f.stem))
+            if re.search(rf"{class_name}\.[a-zA-Z]+\.[a-fA-F\d]{{32}}", str(f.stem))
         ]
         ordered_cache_files = sorted(cache_files, key=lambda x: x.stat().st_mtime)
-
-        for i, cache_file in enumerate(ordered_cache_files):
-            if i >= self._max_entries:
-                oldest_key = next(iter(self._cache))
-                del self._cache[oldest_key]
-                (self._cache_directory / f"{oldest_key}.{self._cache_file_suffix}").unlink()
-            cache_key = cache_file.stem
-            self._cache[cache_key] = True
+        for cache_file in ordered_cache_files:
+            cache_key = cache_file.stem.split("_")[0]
+            if cache_key not in self._cache:
+                if len(self._cache) >= self._max_entries:
+                    oldest_key = next(iter(self._cache))
+                    del self._cache[oldest_key]
+                    for file in self._cache_directory.glob(f"{oldest_key}*.{self._cache_file_suffix}"):
+                        file.unlink()
+                self._cache[cache_key] = True
 
     def _load_from_cache(self, cache_key: str) -> Any | None:
         """Loads data from the cache based on the provided cache key and updates the LRU cache.
 
         Args:
             cache_key: A string representing the cache key.
 
         Returns:
             The cached data if it exists, or None if there is no data for the given cache key.
         """
         if cache_key in self._cache:
             self._cache.move_to_end(cache_key)
-            cache_file_path = self._cache_directory / f"{cache_key}.{self._cache_file_suffix}"
-            return self._read_cache_file(cache_file_path)
-        return None
+        return super()._load_from_cache(cache_key)
 
     def _save_to_cache(self, cache_key: str, output: Any) -> None:
         """Saves the given data to the cache using the provided cache key, updating the LRU cache accordingly.
 
         If the cache reaches its maximum size, the least recently used entry will be evicted.
 
         Args:
             cache_key: A string representing the cache key.
             output: The data to be saved to the cache.
         """
         if cache_key not in self._cache:
             if len(self._cache) >= self._max_entries:
                 oldest_key = next(iter(self._cache))
                 del self._cache[oldest_key]
-                (self._cache_directory / f"{oldest_key}.{self._cache_file_suffix}").unlink()
+                for file in self._cache_directory.glob(f"{oldest_key}*.{self._cache_file_suffix}"):
+                    file.unlink()
             self._cache[cache_key] = True
         else:
             self._cache.move_to_end(cache_key)
-        cache_file_path = self._cache_directory / f"{cache_key}.{self._cache_file_suffix}"
-        self._write_cache_file(cache_file_path, output)
+        super()._save_to_cache(cache_key, output)
```

### Comparing `mleko-0.1.3/src/mleko/cache/fingerprinters.py` & `mleko-0.2.0/src/mleko/cache/fingerprinters.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import hashlib
 from abc import ABC, abstractmethod
 from concurrent import futures
 from itertools import islice
 from pathlib import Path
 from typing import Any
 
+import vaex
+
 
 class Fingerprinter(ABC):
     """Abstract base class for creating specialized fingerprinters."""
 
     @abstractmethod
     def fingerprint(self, data: Any) -> str:
         """Generate a fingerprint for the given data.
@@ -37,15 +39,15 @@
 class CSVFingerprinter(Fingerprinter):
     """A fingerprinter for CSV files supporting Gzipped and raw CSV files."""
 
     def __init__(self, n_rows: int = 1000):
         """Initialize the CSVFingerprinter.
 
         Args:
-            n_rows: The number of rows to sample from each CSV file for fingerprinting. Defaults to 1000.
+            n_rows: The number of rows to sample from each CSV file for fingerprinting.
         """
         self._n_rows = n_rows
 
     def fingerprint(self, file_paths: list[str] | list[Path]) -> str:
         """Generate a fingerprint for the given list of CSV files.
 
         The currently supported file types are `.csv`, `.gz`, and `.csv.gz`.
@@ -83,7 +85,23 @@
             with gzip.open(file_path, "rb") as f:
                 sample = b"".join(islice((f.readline() for _ in range(self._n_rows)), self._n_rows))
         else:
             with open(file_path, "rb") as f:
                 sample = b"".join(islice((f.readline() for _ in range(self._n_rows)), self._n_rows))
         fingerprint = hashlib.md5(str(sample).encode()).hexdigest()
         return fingerprint
+
+
+class VaexFingerprinter(Fingerprinter):
+    """A fingerprinter for Vaex DataFrames."""
+
+    def fingerprint(self, dataframe: vaex.DataFrame) -> str:
+        """Generate a fingerprint for a Vaex DataFrame.
+
+        Args:
+            dataframe: The Vaex DataFrame to be fingerprinted.
+
+        Returns:
+            The fingerprint as a hexadecimal string.
+        """
+        fingerprint = hashlib.md5(str(dataframe.fingerprint()).encode()).hexdigest()
+        return fingerprint
```

### Comparing `mleko-0.1.3/src/mleko/data/converters.py` & `mleko-0.2.0/src/mleko/data/converters.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 from itertools import repeat
 from pathlib import Path
 
 import vaex
 from pyarrow import csv as arrow_csv
 from tqdm import tqdm
 
-from mleko.cache.cache import LRUCacheMixin
+from mleko.cache.cache import LRUCacheMixin, VaexArrowCacheFormatMixin
 from mleko.cache.fingerprinters import CSVFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
-from mleko.utils.tqdm import set_tqdm_percent_wrapper
 
 
 logger = CustomLogger()
 """A CustomLogger instance that's used throughout the module for logging."""
 
 V_CPU_COUNT = multiprocessing.cpu_count()
 """A module-level constant representing the total number of CPUs available on the current system."""
@@ -36,36 +35,36 @@
     def __init__(self, output_directory: str | Path):
         """Initialize the BaseDataConverter with the output directory for the converted files.
 
         Args:
             output_directory: The directory where the converted files will be saved.
         """
         self._output_directory = Path(output_directory)
+        self._output_directory.mkdir(parents=True, exist_ok=True)
 
     @abstractmethod
     def convert(self, file_paths: list[Path] | list[str]) -> vaex.DataFrame:
         """Abstract method to convert the input file paths to the desired output format.
 
         Args:
             file_paths: A list of input file paths to be converted.
 
         Returns:
             vaex.DataFrame: The resulting DataFrame after conversion.
         """
         raise NotImplementedError
 
 
-class CsvToArrowConverter(BaseDataConverter, LRUCacheMixin):
+class CsvToArrowConverter(BaseDataConverter, VaexArrowCacheFormatMixin, LRUCacheMixin):
     """A class that converts CSV files to Arrow format using the vaex library and caches the resulting dataframes."""
 
     @auto_repr
     def __init__(
         self,
         output_directory: str | Path,
-        forced_datetime_columns: list[str] | tuple[str, ...] | tuple[()] = (),
         forced_numerical_columns: list[str] | tuple[str, ...] | tuple[()] = (),
         forced_categorical_columns: list[str] | tuple[str, ...] | tuple[()] = (),
         forced_boolean_columns: list[str] | tuple[str, ...] | tuple[()] = (),
         drop_columns: list[str] | tuple[str, ...] | tuple[()] = (),
         na_values: list[str]
         | tuple[str, ...]
         | tuple[()] = (
@@ -86,48 +85,46 @@
             "N/a",
             "unknown",
             "missing",
         ),
         true_values: list[str] | tuple[str, ...] | tuple[()] = ("t", "True", "true", "1"),
         false_values: list[str] | tuple[str, ...] | tuple[()] = ("f", "False", "false", "0"),
         downcast_float: bool = False,
-        random_state: int = 1337,
-        workers: int = V_CPU_COUNT,
+        random_state: int | None = None,
+        num_workers: int = V_CPU_COUNT,
         max_cache_entries: int = 1,
     ) -> None:
         """Initializes the CsvToArrowConverter with the necessary configurations and parameters.
 
         Args:
             output_directory: The directory where the converted files will be saved.
-            forced_datetime_columns: A sequence of column names to force as datetime type.
             forced_numerical_columns: A sequence of column names to force as numerical type.
             forced_categorical_columns: A sequence of column names to force as categorical type.
             forced_boolean_columns: A sequence of column names to force as boolean type.
             drop_columns: A sequence of column names to drop during conversion.
             na_values: A sequence of strings to consider as NaN or missing values.
             true_values: A sequence of strings to consider as True values.
             false_values: A sequence of strings to consider as False values.
             downcast_float: If True, downcast float64 to float32 during conversion.
             random_state: A seed for the random number generator.
-            workers: Number of workers to use for parallel processing.
+            num_workers: Number of workers to use for parallel processing.
             max_cache_entries: Maximum number of cache entries for the LRUCacheMixin.
         """
-        self._dataframe_suffix = "arrow"
         BaseDataConverter.__init__(self, output_directory)
-        LRUCacheMixin.__init__(self, output_directory, self._dataframe_suffix, max_cache_entries)
-        self._forced_datetime_columns = tuple(forced_datetime_columns)
+        VaexArrowCacheFormatMixin.__init__(self)
+        LRUCacheMixin.__init__(self, output_directory, VaexArrowCacheFormatMixin.cache_file_suffix, max_cache_entries)
         self._forced_numerical_columns = tuple(forced_numerical_columns)
         self._forced_categorical_columns = tuple(forced_categorical_columns)
         self._forced_boolean_columns = tuple(forced_boolean_columns)
         self._drop_columns = tuple(drop_columns)
         self._na_values = tuple(na_values)
         self._true_values = tuple(true_values)
         self._false_values = tuple(false_values)
         self._downcast_float = downcast_float
-        self._workers = workers
+        self._num_workers = num_workers
         self._random_state = random_state
 
     def convert(self, file_paths: list[Path] | list[str], force_recompute: bool = False) -> vaex.DataFrame:
         """Converts a list of CSV files to Arrow format and returns a vaex dataframe joined from the converted data.
 
         The method takes care of caching, and results will be reused accordingly unless force_recompute is set to True.
 
@@ -137,15 +134,14 @@
 
         Returns:
             vaex.DataFrame: The resulting dataframe with the combined converted data.
         """
         return self._cached_execute(
             lambda_func=lambda: self._convert(file_paths),
             cache_keys=[
-                self._forced_datetime_columns,
                 self._forced_numerical_columns,
                 self._forced_categorical_columns,
                 self._forced_boolean_columns,
                 self._drop_columns,
                 self._na_values,
                 self._true_values,
                 self._false_values,
@@ -156,15 +152,14 @@
         )
 
     @staticmethod
     def _convert_csv_file_to_arrow(
         file_path: Path | str,
         output_directory: Path,
         dataframe_suffix: str,
-        forced_datetime_columns: tuple[str, ...],
         forced_numerical_columns: tuple[str, ...],
         forced_categorical_columns: tuple[str, ...],
         forced_boolean_columns: tuple[str, ...],
         drop_columns: tuple[str, ...],
         na_values: tuple[str, ...],
         true_values: tuple[str, ...],
         false_values: tuple[str, ...],
@@ -174,15 +169,14 @@
 
         This operation is done in chunks to optimize parallel processing.
 
         Args:
             file_path: The path of the CSV file to be converted.
             output_directory: The directory where the converted file should be saved.
             dataframe_suffix: The suffix for the converted dataframe files.
-            forced_datetime_columns: A sequence of column names to be forced to datetime type.
             forced_numerical_columns: A sequence of column names to be forced to numerical type.
             forced_categorical_columns: A sequence of column names to be forced to categorical type.
             forced_boolean_columns: A sequence of column names to be forced to boolean type.
             drop_columns: A sequence of column names to be dropped from the dataframe.
             na_values: A sequence of values to be considered as NaN.
             true_values: A sequence of values to be considered as True.
             false_values: A sequence of values to be considered as False.
@@ -191,16 +185,14 @@
         file_path = Path(file_path)
 
         float_type = "float64"
         if downcast_float:
             float_type = "float32"
 
         dtypes = {}
-        for col in forced_datetime_columns:
-            dtypes[col] = "date32"
         for col in forced_numerical_columns:
             dtypes[col] = float_type
         for col in forced_categorical_columns:
             dtypes[col] = "string"
         for col in forced_boolean_columns:
             dtypes[col] = "boolean"
 
@@ -210,14 +202,21 @@
             convert_options=arrow_csv.ConvertOptions(
                 column_types=dtypes,
                 null_values=na_values,
                 true_values=true_values,
                 false_values=false_values,
                 strings_can_be_null=True,
                 quoted_strings_can_be_null=True,
+                timestamp_parsers=[
+                    arrow_csv.ISO8601,
+                    "%Y-%m-%d %H:%M:%S",
+                    "%Y-%m-%d %H:%M:%S.%f",
+                    "%Y-%m-%dT%H:%M:%S",
+                    "%Y-%m-%dT%H:%M:%S.%f",
+                ],
             ),
         ).drop(drop_columns)
 
         output_path = output_directory / f"df_chunk_{file_path.stem}.{dataframe_suffix}"
         df_chunk.export_arrow(output_path)
         df_chunk.close()
 
@@ -229,57 +228,37 @@
         Args:
             file_paths: A list of file paths to be converted.
 
         Returns:
             A DataFrame containing the merged chunks.
         """
         with tqdm(total=len(file_paths), desc="Converting CSV files") as pbar:
-            with futures.ProcessPoolExecutor(max_workers=min(self._workers, len(file_paths))) as executor:
+            with futures.ProcessPoolExecutor(max_workers=min(self._num_workers, len(file_paths))) as executor:
                 for _ in executor.map(
                     CsvToArrowConverter._convert_csv_file_to_arrow,
                     file_paths,
                     repeat(self._output_directory),
-                    repeat(self._dataframe_suffix),
-                    repeat(self._forced_datetime_columns),
+                    repeat(VaexArrowCacheFormatMixin.cache_file_suffix),
                     repeat(self._forced_numerical_columns),
                     repeat(self._forced_categorical_columns),
                     repeat(self._forced_boolean_columns),
                     repeat(self._drop_columns),
                     repeat(self._na_values),
                     repeat(self._true_values),
                     repeat(self._false_values),
                     repeat(self._downcast_float),
                 ):
                     pbar.update(1)
 
-        return vaex.open(self._output_directory / f"df_chunk_*.{self._dataframe_suffix}")
-
-    def _read_cache_file(self, cache_file_path: Path) -> vaex.DataFrame:
-        """Reads a cache file containing a vaex dataframe.
-
-        Args:
-            cache_file_path: The path of the cache file to be read.
-
-        Returns:
-            vaex.DataFrame: The contents of the cache file as a dataframe.
-        """
-        return vaex.open(cache_file_path)
+        return vaex.open(self._output_directory / f"df_chunk_*.{VaexArrowCacheFormatMixin.cache_file_suffix}")
 
     def _write_cache_file(self, cache_file_path: Path, output: vaex.DataFrame) -> None:
-        """Writes the results of the dataframe conversion to Arrow format in a cache file with arrow suffix.
+        """Writes the results of the DataFrame conversion to Arrow format in a cache file with arrow suffix.
 
         Args:
             cache_file_path: The path of the cache file to be written.
-            output: The vaex dataframe to be saved in the cache file.
+            output: The Vaex DataFrame to be saved in the cache file.
         """
-        with tqdm(total=100, desc=f"Merging chunked {self._dataframe_suffix} files") as pbar:
-            output.export_arrow(
-                cache_file_path,
-                progress=set_tqdm_percent_wrapper(pbar),
-                parallel=True,
-                reduce_large=True,
-            )
-
-        output.close()
-        df_chunks = cache_file_path.parent.glob(f"df_chunk_*.{self._dataframe_suffix}")
+        super()._write_cache_file(cache_file_path, output)
+        df_chunks = cache_file_path.parent.glob(f"df_chunk_*.{VaexArrowCacheFormatMixin.cache_file_suffix}")
         for df_chunk in df_chunks:
             df_chunk.unlink()
```

### Comparing `mleko-0.1.3/src/mleko/data/sources/__init__.py` & `mleko-0.2.0/src/mleko/data/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.1.3/src/mleko/data/sources/base_data_source.py` & `mleko-0.2.0/src/mleko/data/sources/base_data_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     @abstractmethod
     def fetch_data(self, use_cache: bool = True) -> list[Path]:
         """Downloads and stores data in the 'destination_directory' using the specific data source implementation.
 
         Args:
             use_cache: If supported by the child class, skips data fetching when up-to-date data is already present
-                in 'destination_directory'. Defaults to True.
+                in 'destination_directory'.
 
         Raises:
             NotImplementedError: Must be implemented in the child class that inherits from `BaseDataSource`.
 
         Returns:
             A list of Path objects pointing to the downloaded data files.
         """
```

### Comparing `mleko-0.1.3/src/mleko/data/sources/kaggle_data_source.py` & `mleko-0.2.0/src/mleko/data/sources/kaggle_data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """Name of the key in the Kaggle API credentials file containing the Kaggle API key."""
 
     @staticmethod
     def get_kaggle_credentials(credentials_file_path: str | Path | None = None) -> KaggleCredentials:
         """Retrieves Kaggle API credentials from the specified file, environment variables, or the default location.
 
         Args:
-            credentials_file_path: Path to the Kaggle API credentials file. Defaults to None.
+            credentials_file_path: Path to the Kaggle API credentials file.
 
         Returns:
             A KaggleCredentials instance with the retrieved username and API key.
         """
         if credentials_file_path is not None:
             logger.info(f"Attempting to fetch Kaggle API credentials from config at {credentials_file_path}.")
             credentials = KaggleCredentialsManager._read_config_file(Path(credentials_file_path))
@@ -219,20 +219,20 @@
         """Initializes a KaggleDataSource instance to fetch data from a specific Kaggle dataset.
 
         Args:
             destination_directory: The directory where the downloaded files will be stored.
             owner_slug: The owner's Kaggle username or organization name.
             dataset_slug: The dataset's unique Kaggle identifier (slug).
             file_names: A list of file names to download. If not provided or empty, all files in
-                the dataset will be downloaded. Defaults to None.
+                the dataset will be downloaded.
             dataset_version: The specific dataset version number to download. If not provided,
-                the latest version will be fetched. Defaults to None.
+                the latest version will be fetched.
             kaggle_api_credentials_file: Path to a Kaggle API credentials JSON file. If not
-                provided, environment variables or the default file location will be used. Defaults to None.
-            num_workers: Number of concurrent threads to use when downloading files. Defaults to 64.
+                provided, environment variables or the default file location will be used.
+            num_workers: Number of concurrent threads to use when downloading files.
         """
         super().__init__(destination_directory)
 
         self._owner_slug, self._dataset_slug, self._dataset_version = owner_slug, dataset_slug, dataset_version
         self._file_names: set[str] = set(file_names) if file_names is not None else set()
         self._kaggle_config = KaggleCredentialsManager.get_kaggle_credentials(kaggle_api_credentials_file)
         self._num_workers = num_workers
@@ -242,15 +242,15 @@
 
         This method downloads files from the Kaggle dataset and returns the local file paths of the downloaded files.
         The method checks if local files are up-to-date and skips downloading if everything is already in place and
         `use_cache` is set to True.
 
         Args:
             use_cache: If set to True, the method will check if the local files are up-to-date and
-                skip downloading if everything is already in place. Defaults to True.
+                skip downloading if everything is already in place.
 
         Returns:
             A list of local file paths pointing to the downloaded files.
 
         Raises:
             ValueError: If Kaggle returns 0 files for the given dataset. This could occur if the API is broken.
         """
@@ -363,15 +363,15 @@
         """Downloads multiple Kaggle dataset files concurrently.
 
         Args:
             kaggle_file_paths: A list of Kaggle file paths to download.
             params: The request parameters containing the dataset version number, if applicable.
         """
         with tqdm(total=len(kaggle_file_paths), desc="Downloading files from Kaggle") as pbar:
-            with futures.ThreadPoolExecutor(max_workers=self._num_workers) as executor:
+            with futures.ThreadPoolExecutor(max_workers=min(self._num_workers, len(kaggle_file_paths))) as executor:
                 for _ in executor.map(
                     self._kaggle_fetch_file,
                     kaggle_file_paths,
                     repeat(params),
                 ):
                     pbar.update(1)
```

### Comparing `mleko-0.1.3/src/mleko/data/sources/s3_data_source.py` & `mleko-0.2.0/src/mleko/data/sources/s3_data_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,19 @@
     ) -> None:
         """Initializes the S3 bucket client, configures the destination directory, and sets client-related parameters.
 
         Args:
             destination_directory: Directory to store the fetched data locally.
             s3_bucket_name: Name of the S3 bucket containing the data.
             s3_key_prefix: Prefix of the S3 keys for the files to download.
-            aws_profile_name: AWS profile name to use. Defaults to None.
-            aws_region_name: AWS region name where the S3 bucket is located. Defaults to "eu-west-1".
-            num_workers: Number of workers to use for concurrent downloads. Defaults to 64.
-            manifest_file_name: Name of the manifest file. Defaults to "manifest".
-            check_s3_timestamps: Whether to check if all S3 files have the same timestamp. Defaults to True.
+            aws_profile_name: AWS profile name to use.
+            aws_region_name: AWS region name where the S3 bucket is located.
+            num_workers: Number of workers to use for concurrent downloads.
+            manifest_file_name: Name of the manifest file.
+            check_s3_timestamps: Whether to check if all S3 files have the same timestamp.
         """
         super().__init__(destination_directory)
 
         self._s3_bucket_name = s3_bucket_name
         self._s3_key_prefix = s3_key_prefix
         self._s3_client = self._get_s3_client(aws_profile_name, aws_region_name)
 
@@ -74,15 +74,15 @@
     def fetch_data(self, use_cache: bool = True) -> list[Path]:
         """Downloads the data from the S3 bucket and stores it in the 'destination_directory'.
 
         If 'use_cache' is True, verifies whether the data in the local 'destination_directory' is current with the
         S3 bucket contents based on the manifest file, and skips downloading if it is up to date.
 
         Args:
-            use_cache: Whether to skip downloading if the local data is up to date. Defaults to True.
+            use_cache: Whether to skip downloading if the local data is up to date.
 
         Raises:
             Exception: If files in the S3 bucket have different last modified dates, indicating potential corruption
                        or duplication.
 
         Returns:
             A list of Path objects pointing to the downloaded data files.
```

### Comparing `mleko-0.1.3/src/mleko/pipeline/__init__.py` & `mleko-0.2.0/src/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.1.3/src/mleko/pipeline/data_container.py` & `mleko-0.2.0/src/mleko/pipeline/data_container.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Data management module for handling data used in the pipeline.
 
 This module provides the DataContainer class, which serves as a common interface for various types of data,
 enforcing shared structure and behavior. The goal is to facilitate data handling throughout the pipeline.
 """
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from pathlib import Path
 
 import vaex
 
 
 @dataclass
 class DataContainer:
     """Class for holding data used in the pipeline.
 
     This class serves as a common interface and can be extended to enforce
     a shared structure or behavior across different types of data.
     """
 
-    data: list[Path] | vaex.DataFrame | None = None
+    data: dict[str, list[Path] | vaex.DataFrame] = field(default_factory=dict)
     """The data stored in the DataContainer."""
 
     def __repr__(self) -> str:
         """Get string representation of DataContainer.
 
         Returns:
             String representation of the DataContainer, including data type and stored data.
```

### Comparing `mleko-0.1.3/src/mleko/pipeline/pipeline.py` & `mleko-0.2.0/src/mleko/pipeline/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 and visualize these steps. Each step's output is passed as input to the next step, effectively managing the flow
 of data through the processing pipeline.
 """
 from __future__ import annotations
 
 from mleko.pipeline.data_container import DataContainer
 from mleko.pipeline.pipeline_step import PipelineStep
+from mleko.utils.custom_logger import CustomLogger
+
+
+logger = CustomLogger()
+"""A CustomLogger instance that's used throughout the module for logging."""
 
 
 class Pipeline:
     """Encapsulates a pipeline that manages and executes a series of data processing steps in a defined order."""
 
     def __init__(self, steps: list[PipelineStep] | None = None) -> None:
         """Creates a new Pipeline instance, initializing it with a list of steps or an empty list.
@@ -61,11 +66,12 @@
 
         Returns:
             The output as a DataContainer instance from the last step in the pipeline after processing the data.
         """
         if data_container is None:
             data_container = DataContainer()
 
-        for step in self.steps:
+        for i, step in enumerate(self.steps):
+            logger.info(f"Executing step {i+1}: {step.__class__.__name__}")
             data_container = step.execute(data_container)
-
+            logger.info(f"Finished step {i+1}")
         return data_container
```

### Comparing `mleko-0.1.3/src/mleko/pipeline/steps/ingest.py` & `mleko-0.2.0/src/mleko/pipeline/steps/ingest.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,27 +11,42 @@
 from mleko.pipeline.pipeline_step import PipelineStep
 from mleko.utils import auto_repr
 
 
 class IngestStep(PipelineStep):
     """Pipeline step that manages data ingestion from a configured data source."""
 
+    _num_inputs = 0
+    """Number of inputs expected by the IngestStep."""
+
+    _num_outputs = 1
+    """Number of outputs expected by the IngestStep."""
+
     @auto_repr
-    def __init__(self, data_source: BaseDataSource) -> None:
+    def __init__(
+        self,
+        data_source: BaseDataSource,
+        inputs: list[str] | tuple[str, ...] | tuple[()] = (),
+        outputs: list[str] | tuple[str, ...] | tuple[()] = (),
+    ) -> None:
         """Initialize the IngestStep with the specified data source.
 
         Args:
             data_source: The data source from which to fetch the data, a BaseDataSource instance.
+            inputs: List or tuple of input keys expected by this step.
+            outputs: List or tuple of output keys produced by this step.
         """
+        super().__init__(inputs, outputs)
         self._data_source = data_source
 
     def execute(self, _data_container: DataContainer) -> DataContainer:
         """Fetch data from the configured data source and return a DataContainer with fetched files.
 
         The `_data_container` parameter is unused in this step as this operation only deals with data ingestion
         and no input data is required.
 
         Returns:
             DataContainer: A DataContainer containing a list of fetched files.
         """
         files = self._data_source.fetch_data()
-        return DataContainer(data=files)
+        _data_container.data[self.outputs[0]] = files
+        return _data_container
```

### Comparing `mleko-0.1.3/src/mleko/utils/custom_logger.py` & `mleko-0.2.0/src/mleko/utils/custom_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             self.addHandler(handler)
 
     @staticmethod
     def set_global_log_level(log_level: int) -> None:
         """Set the global log level for all instances of CustomLogger.
 
         Args:
-            log_level: The minimum log level to output. Defaults to logging.INFO.
+            log_level: The minimum log level to output.
         """
         CustomLogger._global_log_level = log_level
         for instance in CustomLogger._instances:
             instance.set_level(log_level)
 
     def debug(self, msg: object, *args: object) -> None:  # type: ignore
         """Log a debug message.
```

### Comparing `mleko-0.1.3/src/mleko/utils/decorators.py` & `mleko-0.2.0/src/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-0.1.3/src/mleko/utils/file_helpers.py` & `mleko-0.2.0/src/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.1.3/src/mleko/utils/tqdm.py` & `mleko-0.2.0/src/mleko/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `mleko-0.1.3/PKG-INFO` & `mleko-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 0.1.3
+Version: 0.2.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/ErikBavenstrand/mleko
 License: MIT
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: boto3 (>=1.26.91,<2.0.0)
 Requires-Dist: botocore (>=1.29.91,<2.0.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: vaex (>=4.16.0,<5.0.0)
 Project-URL: Changelog, https://github.com/ErikBavenstrand/mleko/releases
 Project-URL: Documentation, https://mleko.readthedocs.io
 Project-URL: Repository, https://github.com/ErikBavenstrand/mleko
 Description-Content-Type: text/markdown
```

