# Comparing `tmp/redcat-0.0.2.tar.gz` & `tmp/redcat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redcat-0.0.2.tar", max compression
+gzip compressed data, was "redcat-0.0.3.tar", max compression
```

## Comparing `redcat-0.0.2.tar` & `redcat-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1501 2023-05-19 18:45:14.291732 redcat-0.0.2/LICENSE
--rw-r--r--   0        0        0     2156 2023-05-19 18:45:14.291732 redcat-0.0.2/README.md
--rw-r--r--   0        0        0     4347 2023-05-19 18:45:14.291732 redcat-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      354 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/__init__.py
--rw-r--r--   0        0        0    17532 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/base.py
--rw-r--r--   0        0        0    16464 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/batchdict.py
--rw-r--r--   0        0        0     6626 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/batchlist.py
--rw-r--r--   0        0        0     2428 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/comparators.py
--rw-r--r--   0        0        0        0 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/datapipes/__init__.py
--rw-r--r--   0        0        0      315 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/datapipes/iter/__init__.py
--rw-r--r--   0        0        0     4071 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/datapipes/iter/batching.py
--rw-r--r--   0        0        0     3729 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/datapipes/iter/joining.py
--rw-r--r--   0        0        0     2111 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/datapipes/iter/shuffling.py
--rw-r--r--   0        0        0   140956 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/tensor.py
--rw-r--r--   0        0        0    51250 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/tensorseq.py
--rw-r--r--   0        0        0        0 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/utils/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-19 18:45:14.295733 redcat-0.0.2/src/redcat/utils/format.py
--rw-r--r--   0        0        0     1446 2023-05-19 18:45:14.295733 redcat-0.0.2/src/redcat/utils/imports.py
--rw-r--r--   0        0        0    10154 2023-05-19 18:45:14.295733 redcat-0.0.2/src/redcat/utils/tensor.py
--rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 redcat-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-05-21 04:17:02.338076 redcat-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2156 2023-05-21 04:17:02.338076 redcat-0.0.3/README.md
+-rw-r--r--   0        0        0     4368 2023-05-21 04:17:02.338076 redcat-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/__init__.py
+-rw-r--r--   0        0        0    17536 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/base.py
+-rw-r--r--   0        0        0    16464 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/batchdict.py
+-rw-r--r--   0        0        0     6626 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/batchlist.py
+-rw-r--r--   0        0        0     2428 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/comparators.py
+-rw-r--r--   0        0        0        0 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/datapipes/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/datapipes/iter/__init__.py
+-rw-r--r--   0        0        0     4087 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/datapipes/iter/batching.py
+-rw-r--r--   0        0        0     3729 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/datapipes/iter/joining.py
+-rw-r--r--   0        0        0     2123 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/datapipes/iter/shuffling.py
+-rw-r--r--   0        0        0   140956 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/tensor.py
+-rw-r--r--   0        0        0    52665 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/tensorseq.py
+-rw-r--r--   0        0        0        0 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/utils/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/utils/format.py
+-rw-r--r--   0        0        0     1446 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/utils/imports.py
+-rw-r--r--   0        0        0    10154 2023-05-21 04:17:02.338076 redcat-0.0.3/src/redcat/utils/tensor.py
+-rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 redcat-0.0.3/PKG-INFO
```

### Comparing `redcat-0.0.2/LICENSE` & `redcat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redcat-0.0.2/README.md` & `redcat-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `redcat-0.0.2/pyproject.toml` & `redcat-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redcat"
-version = "0.0.2"
+version = "0.0.3"
 description = "A library to manipulate batches of examples"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/redcat"
 repository = "https://github.com/durandtibo/redcat"
 keywords = ["batch"]
 license = "BSD-3-Clause"
@@ -26,34 +26,34 @@
 
 packages = [
     { include = "redcat", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
-coola = "^0.0, >=0.0.7"
+coola = "^0.0,>=0.0.7"
 numpy = "^1.24"
 python = "^3.9"
 torch = "^2.0"
 polars = { version = "^0.17", optional = true }
 
 [tool.poetry.extras]
 all = [
     "polars",
 ]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3"
-coverage = { extras = ["toml"], version = "^6.5" }
-pre-commit = "^2.21"
+coverage = { extras = ["toml"], version = ">=6.5,<8.0" }
+pre-commit = ">=2.21,<4.0"
 pylint = "^2.17"
 pytest = "^7.3"
 pytest-cov = "^4.0"
 pytest-timeout = "^2.1"
-ruff = "^0.0.262"
+ruff = ">=0.0.262,<0.0.270"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
```

### Comparing `redcat-0.0.2/src/redcat/base.py` & `redcat-0.0.3/src/redcat/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class BaseBatch(Generic[T], ABC):
     r"""Define the base class to implement a batch."""
 
     @property
     @abstractmethod
     def batch_size(self) -> int:
-        r"""int: The batch size."""
+        r"""``int``: The batch size."""
 
     @property
     @abstractmethod
     def data(self) -> T:
         r"""The data in the batch."""
 
     ###############################
```

### Comparing `redcat-0.0.2/src/redcat/batchdict.py` & `redcat-0.0.3/src/redcat/batchdict.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.2/src/redcat/batchlist.py` & `redcat-0.0.3/src/redcat/batchlist.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.2/src/redcat/comparators.py` & `redcat-0.0.3/src/redcat/comparators.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.2/src/redcat/datapipes/iter/batching.py` & `redcat-0.0.3/src/redcat/datapipes/iter/batching.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
             f"  shuffle={self._shuffle},\n"
             f"  random_seed={self.random_seed},\n"
             f"  datapipe_or_batch={str_indent(self._datapipe_or_batch)},\n)"
         )
 
     @property
     def batch_size(self) -> int:
-        r"""int: The batch size."""
+        r"""``int``: The batch size."""
         return self._batch_size
 
     @property
     def random_seed(self) -> int:
-        r"""int: The random seed used to initialize the pseudo random generator."""
+        r"""``int``: The random seed used to initialize the pseudo random
+        generator."""
         return self._generator.initial_seed()
```

### Comparing `redcat-0.0.2/src/redcat/datapipes/iter/joining.py` & `redcat-0.0.3/src/redcat/datapipes/iter/joining.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.2/src/redcat/datapipes/iter/shuffling.py` & `redcat-0.0.3/src/redcat/datapipes/iter/shuffling.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,9 +59,10 @@
             f"{self.__class__.__qualname__}(\n"
             f"  random_seed={self.random_seed},\n"
             f"  datapipe={str_indent(self._datapipe)},\n)"
         )
 
     @property
     def random_seed(self) -> int:
-        r"""int: The random seed used to initialize the pseudo random generator."""
+        r"""``int``: The random seed used to initialize the pseudo random
+        generator."""
         return self._generator.initial_seed()
```

### Comparing `redcat-0.0.2/src/redcat/tensor.py` & `redcat-0.0.3/src/redcat/tensor.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.2/src/redcat/tensorseq.py` & `redcat-0.0.3/src/redcat/tensorseq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from __future__ import annotations
 
-__all__ = ["BatchedTensorSeq", "check_data_and_dims", "check_seq_dims", "get_seq_dims"]
+__all__ = [
+    "BatchedTensorSeq",
+    "check_data_and_dims",
+    "check_seq_dims",
+    "get_seq_dims",
+    "from_sequences",
+]
 
 import functools
 from collections.abc import Callable, Iterable, Mapping, Sequence
 from typing import Any, overload
 
 import torch
 from torch import Tensor
+from torch.nn.utils.rnn import pad_sequence
 
 from redcat import BaseBatch, tensor
 from redcat.tensor import BatchedTensor, check_batch_dims, get_batch_dims
 from redcat.utils.tensor import (
     align_to_batch_seq,
     align_to_seq_batch,
     compute_batch_seq_permutation,
@@ -76,15 +83,15 @@
     @property
     def seq_dim(self) -> int:
         r"""int: The sequence dimension in the ``torch.Tensor`` object."""
         return self._seq_dim
 
     @property
     def seq_len(self) -> int:
-        r"""int: The sequence length."""
+        r"""``int``: The sequence length."""
         return self._data.shape[self._seq_dim]
 
     ###############################
     #     Creation operations     #
     ###############################
 
     def new_full(
@@ -1403,7 +1410,45 @@
     if dim is None:
         return torch.take_along_dim(input, indices)
     return BatchedTensorSeq(
         torch.take_along_dim(input, indices, dim=dim),
         batch_dim=batch_dims.pop(),
         seq_dim=seq_dims.pop(),
     )
+
+
+def from_sequences(
+    sequences: Iterable[torch.Tensor], padding_value: bool | int | float = 0
+) -> BatchedTensorSeq:
+    r"""Converts variable length sequences to a single padded tensor.
+
+    Args:
+        sequences (iterable): Specifies an iterable over the variable
+            length sequences. Each sequence is a ``torch.Tensor`` of
+            shape ``(sequence_length, *)``. This function assumes
+            trailing dimensions and type of all the tensors in
+            sequences are same.
+        padding_value (bool or int or float, optional): Specifies the
+        padding value. Default: ``0``
+
+    Returns:
+        ``BatchedTensorSeq``: A padded tensor. The underlying data is
+            a ``torch.Tensor`` of shape
+            ``(batch_size, sequence_length, *)``.
+
+    Example usage:
+
+    .. code-block:: python
+
+        >>> import torch
+        >>> import redcat
+        >>> redcat.tensorseq.from_sequences(
+        ...     [torch.ones(3), torch.ones(5), torch.ones(1), torch.ones(0)]
+        ... )
+        tensor([[1., 1., 1., 0., 0.],
+                [1., 1., 1., 1., 1.],
+                [1., 0., 0., 0., 0.],
+                [0., 0., 0., 0., 0.]], batch_dim=0, seq_dim=1)
+    """
+    return BatchedTensorSeq(
+        pad_sequence(list(sequences), padding_value=padding_value, batch_first=True)
+    )
```

### Comparing `redcat-0.0.2/src/redcat/utils/format.py` & `redcat-0.0.3/src/redcat/utils/format.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.2/src/redcat/utils/imports.py` & `redcat-0.0.3/src/redcat/utils/imports.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.2/src/redcat/utils/tensor.py` & `redcat-0.0.3/src/redcat/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.2/PKG-INFO` & `redcat-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redcat
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library to manipulate batches of examples
 Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause
 Keywords: batch
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: redcat Version: 0.0.2 Summary: A library to
+Metadata-Version: 2.1 Name: redcat Version: 0.0.3 Summary: A library to
 manipulate batches of examples Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause Keywords: batch Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

