# Comparing `tmp/pysparse-array-1.0.2.tar.gz` & `tmp/pysparse-array-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-1.0.2.tar", last modified: Sat May 20 21:19:15 2023, max compression
+gzip compressed data, was "pysparse-array-1.0.3.tar", last modified: Sun May 21 09:35:58 2023, max compression
```

## Comparing `pysparse-array-1.0.2.tar` & `pysparse-array-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 21:19:15.068871 pysparse-array-1.0.2/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2567 2023-05-20 21:18:00.000000 pysparse-array-1.0.2/HISTORY.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.2/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.2/MANIFEST.in
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-20 21:19:15.063377 pysparse-array-1.0.2/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     4694 2023-05-20 21:17:03.000000 pysparse-array-1.0.2/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-05-20 21:18:06.000000 pysparse-array-1.0.2/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 21:19:14.992187 pysparse-array-1.0.2/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-20 21:19:14.000000 pysparse-array-1.0.2/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-20 21:19:14.000000 pysparse-array-1.0.2/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-20 21:19:14.000000 pysparse-array-1.0.2/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-05-20 21:19:14.000000 pysparse-array-1.0.2/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-20 21:19:14.000000 pysparse-array-1.0.2/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-20 21:19:15.069342 pysparse-array-1.0.2/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-20 21:18:13.000000 pysparse-array-1.0.2/setup.py
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 21:19:15.041743 pysparse-array-1.0.2/sparse/
--rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.2/sparse/__init__.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)    10066 2023-05-20 21:07:15.000000 pysparse-array-1.0.2/sparse/array_api.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     7627 2023-05-20 06:59:53.000000 pysparse-array-1.0.2/sparse/core.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-21 09:35:58.849029 pysparse-array-1.0.3/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     2860 2023-05-21 09:35:11.000000 pysparse-array-1.0.3/HISTORY.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.3/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.3/MANIFEST.in
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-21 09:35:58.845931 pysparse-array-1.0.3/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     4694 2023-05-20 21:17:03.000000 pysparse-array-1.0.3/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-05-21 09:35:18.000000 pysparse-array-1.0.3/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-21 09:35:58.799236 pysparse-array-1.0.3/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-21 09:35:58.000000 pysparse-array-1.0.3/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-21 09:35:58.000000 pysparse-array-1.0.3/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-21 09:35:58.000000 pysparse-array-1.0.3/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-05-21 09:35:58.000000 pysparse-array-1.0.3/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-21 09:35:58.000000 pysparse-array-1.0.3/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-21 09:35:58.849331 pysparse-array-1.0.3/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-21 09:35:24.000000 pysparse-array-1.0.3/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-21 09:35:58.823658 pysparse-array-1.0.3/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.3/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     8750 2023-05-21 08:43:09.000000 pysparse-array-1.0.3/sparse/array_api.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     7483 2023-05-21 09:30:56.000000 pysparse-array-1.0.3/sparse/core.py
```

### Comparing `pysparse-array-1.0.2/HISTORY.md` & `pysparse-array-1.0.3/HISTORY.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 #Changelog
 
 All notable changes to the `PySparse` package will be documented in this file.
 
 ## [Unreleased]
 
+## [1.0.3]
+
+### Fixed
+- Fixed further bug around multi-index slicing, and in doing so, tidied up some unnecessary Class code
+- Fixed bug whereby the first value was being lost when converting to_sparse
+- Fixed bug whereby certain values were being lost in to_sparse due to a dictionary error
+
 ## [1.0.2]
 
 ### Added
 - Added .shape attribute alongside .dense_shape and .coords_shape
 
 ### Fixed
 - Fixed bug with indexing 1D data
```

### Comparing `pysparse-array-1.0.2/LICENSE.txt` & `pysparse-array-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.2/PKG-INFO` & `pysparse-array-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.2/README.md` & `pysparse-array-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.2/pyproject.toml` & `pysparse-array-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysparse-array"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
 	{ name="Thomas Frost", email="tdgfrost@gmail.com" },
 ]
 description = "A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries."
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
```

### Comparing `pysparse-array-1.0.2/pysparse_array.egg-info/PKG-INFO` & `pysparse-array-1.0.3/pysparse_array.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.2/setup.py` & `pysparse-array-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pysparse-array',
-    version='1.0.2',
+    version='1.0.3',
     description='Package to encode and decode large OOM numpy arrays as Sparse binaries',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     packages=find_packages(),
     author='Thomas Frost',
     author_email='tdgfrost@gmail.com',
     url='https://github.com/tdgfrost/PySparse',
```

### Comparing `pysparse-array-1.0.2/sparse/array_api.py` & `pysparse-array-1.0.3/sparse/array_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,40 +79,21 @@
         elif items is None:
             target_data = np.zeros((1,) + self.dense_shape[1:])
             target_data[tuple(self.coords.T)] = self.data
             shape = (1,) + self.dense_shape
             return target_data.reshape(shape)
 
         elif isinstance(items, tuple):
-            items = list(items)
             for idx, item in enumerate(items):
                 if not isinstance(item, (int, slice, np.ndarray, type(Ellipsis), type(None))):
                     raise TypeError(
                         'indices must be integers, slices, np.ndarray, Ellipsis, or NoneType - not {}'.format(
                             type(item)))
 
-            if isinstance(items[0], slice):
-                items[0] = np.arange(*items[0].indices(self.dense_shape[0]))
-                return self.__get_item(items)
-
-            elif isinstance(items[0], np.ndarray):
-                if items[0].dtype == bool:
-                    if len(items[0]) != self.dense_shape[0]:
-                        raise ValueError(
-                            'Boolean index shape mismatch: {} vs {}'.format(len(items[0]), self.dense_shape[0]))
-                    else:
-                        items[0] = np.where(items[0])[0]
-                        return self.__get_item(items)
-
-            elif (items[0] is Ellipsis) or (items[0] is None):
-                target_data = np.zeros((1,) + self.dense_shape[1:])
-                target_data[tuple(self.coords.T)] = self.data
-                return target_data[tuple(items)]
-
-            return self.__get_item(items)
+            return self.__getitem__(items[0])[items[1:]]
 
         else:
             raise TypeError(
                 'indices must be integers, slices, np.ndarray, Ellipsis, or NoneType - not {}'.format(type(items)))
 
     def __get_row(self, row_idx) -> np.ndarray:
         """
@@ -148,17 +129,21 @@
 
             # Re-create the dense array (of the shape requested) with all zeros
             target_data = np.zeros((1,) + self.dense_shape[1:], dtype=self.data_dtype) if isinstance(row_idx, int) else np.zeros(
                 (len(row_idx),) + self.dense_shape[1:], dtype=self.data_dtype)
 
             # Fill the dense array with the non-zero data at the target coordinates
             target_data[tuple(target_coords.T)] = self.data[find_coords]
+
+            # If only one row index was given, reduce the dimensionality
+            if isinstance(row_idx, int):
+                target_data = target_data[0]
         else:
             # If the row indices have no non-zero data, return an array of zeros
-            target_data = np.zeros((1,) + self.dense_shape[1:], dtype=self.data_dtype) if isinstance(row_idx, int) else np.zeros(
+            target_data = np.zeros(self.dense_shape[1:], dtype=self.data_dtype) if isinstance(row_idx, int) else np.zeros(
                 (len(row_idx),) + self.dense_shape[1:], dtype=self.data_dtype)
 
         return target_data
 
     @staticmethod
     @njit(types.Tuple((types.List(types.Array(types.int64, 1, 'C')),
                        types.boolean))(types.DictType(types.int64, types.UniTuple(types.int64, count=2)),
@@ -200,27 +185,10 @@
 
             coords_present += True if start >= 0 else False
 
         coords_present = bool(coords_present)
 
         return find_coords, coords_present
 
-    def __get_item(self, items) -> np.ndarray:
-        """
-        Get the values of the dense array at the given indices
-        :param items: tuple of indices
-        :return: dense numpy array values at the given indices
-        """
-
-        # Start by getting the values of the dense array at the given row indices,
-        # with the dense array fully in memory
-        target_data = self.__get_row(items[0])
-
-        # Then index the dense array with the remaining indices as usual
-        items[0] = Ellipsis
-        target_data = target_data[tuple(items)]
-
-        return target_data
-
     def __len__(self):
         return self.shape[0]
```

### Comparing `pysparse-array-1.0.2/sparse/core.py` & `pysparse-array-1.0.3/sparse/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,16 +60,16 @@
         for i in range(0, shape[0], chunksize):
             progress_bar(i, shape[0]) if verbose else None
             data_shape += np.count_nonzero(array[i:i + chunksize])
 
     return data_shape
 
 
-@njit
-def __convert_to_sparse_data(sparse_coords, sparse_values, iteration: int, chunksize, sparse_coords_idx_baseline) -> (np.ndarray, np.ndarray):
+#@njit
+def __convert_to_sparse_data(sparse_coords, sparse_values, iteration: int, chunksize, sparse_idx) -> (np.ndarray, np.ndarray):
     """
     Convert a chunk of a dense array to sparse data
     :param sparse_coords: sparse coordinates
     :param sparse_values: sparse values
     :param iteration: iteration number
     :param prev_sparse_coords_max: maximum idx of the previous sparse coordinates
     :return: tuple of sparse coordinates and sparse values
@@ -77,35 +77,35 @@
     sparse_coords = list(sparse_coords)
     sparse_coords[0] += iteration
     sparse_coords_arr = np.empty((len(sparse_coords), sparse_coords[0].shape[0]), dtype=np.int64)
     for row in range(len(sparse_coords)):
         sparse_coords_arr[row] = sparse_coords[row]
     sparse_coords = sparse_coords_arr.T
     sparse_coords_dict = __create_sparse_coords_dictionary(sparse_coords, iteration, chunksize,
-                                                           sparse_coords_idx_baseline)
+                                                           sparse_idx)
 
     return sparse_coords, sparse_values, sparse_coords_dict
 
 
-@njit(parallel=True)
-def __create_sparse_coords_dictionary(sparse_coords, iteration, chunksize, sparse_coords_idx_baseline):
+#@njit(parallel=True)
+def __create_sparse_coords_dictionary(sparse_coords, iteration, chunksize, sparse_idx):
     """
     Convert a chunk of a dense array to sparse data
     :param sparse_coords: sparse coordinates
     :return: dictionary mapping dense rows to sparse coordinates
     """
     min_value = sparse_coords[:, 0].min()
     max_value = sparse_coords[:, 0].max()
     sparse_coords_dict = {i: (-1, -1) for i in range(iteration, iteration + chunksize)}
 
     for dense_row in prange(min_value, max_value + 1):
         sparse_to_dense_coords = np.where(sparse_coords[:, 0] == dense_row)[0]
-        if np.any(sparse_to_dense_coords):
-            sparse_coords_dict[dense_row] = (sparse_to_dense_coords.min() + sparse_coords_idx_baseline,
-                                             sparse_to_dense_coords.max() + sparse_coords_idx_baseline)
+        if sparse_to_dense_coords.shape[0] > 0:
+            sparse_coords_dict[dense_row] = (sparse_to_dense_coords.min() + sparse_idx,
+                                             sparse_to_dense_coords.max() + sparse_idx)
 
     return sparse_coords_dict
 
 
 def __write_sparse_arrays(array: np.ndarray or np.memmap, path: 'str', chunksize: int, verbose: bool) -> None:
     """
     Simultaneously convert and write a dense array to sparse arrays
@@ -146,31 +146,33 @@
         sparse_coords, sparse_values, sparse_coords_dict = __convert_to_sparse_data(sparse_coords, sparse_values, 0, 0)
 
         memmap_sparse_coords[:] = sparse_coords
         memmap_sparse_data[:] = sparse_values
 
     else:
         sparse_coords_dict = {}
-        sparse_coords_idx_baseline = 0
         for chunk_idx in range(0, dense_shape[0], chunksize):
             progress_bar(chunk_idx, dense_shape[0]) if verbose else None
             array_chunk = array[chunk_idx:chunk_idx + chunksize]
             # Use of the bool dtype accelerates this step
             sparse_coords = array_chunk.astype(bool).nonzero()
             sparse_values = array_chunk[sparse_coords]
             sparse_coords, sparse_values, sparse_coords_dict_temp = __convert_to_sparse_data(sparse_coords, sparse_values,
                                                                                              chunk_idx, chunksize,
-                                                                                             sparse_coords_idx_baseline)
+                                                                                             sparse_index)
 
             memmap_sparse_coords[sparse_index:sparse_index + sparse_coords.shape[0]] = sparse_coords
             memmap_sparse_data[sparse_index:sparse_index + sparse_coords.shape[0]] = sparse_values
             sparse_coords_dict.update(sparse_coords_dict_temp)
 
             sparse_index += sparse_coords.shape[0]
-            sparse_coords_idx_baseline = sparse_coords_dict[min(chunk_idx + chunksize - 1, dense_shape[0]-1)][1] + 1
+
+            """
+            SOMEHOW things are getting reset with every chunk_idx
+            """
 
     with open(os.path.join(path, 'sparse_coords_dict.pkl'), 'wb') as f:
         pickle.dump(sparse_coords_dict, f)
 
     return
```

