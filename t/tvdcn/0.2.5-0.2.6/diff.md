# Comparing `tmp/tvdcn-0.2.5.tar.gz` & `tmp/tvdcn-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.2.5.tar", last modified: Wed May 17 15:41:48 2023, max compression
+gzip compressed data, was "tvdcn-0.2.6.tar", last modified: Sun May 21 03:58:32 2023, max compression
```

## Comparing `tvdcn-0.2.5.tar` & `tvdcn-0.2.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:41:48.859250 tvdcn-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 15:39:47.000000 tvdcn-0.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-05-17 15:41:48.859250 tvdcn-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-17 15:39:47.000000 tvdcn-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-17 15:39:47.000000 tvdcn-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-17 15:41:48.859250 tvdcn-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-17 15:39:47.000000 tvdcn-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:41:48.847249 tvdcn-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tests/test_compatibility_with_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:41:48.847249 tvdcn-0.2.5/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:41:48.847249 tvdcn-0.2.5/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:41:48.851250 tvdcn-0.2.5/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:41:48.851250 tvdcn-0.2.5/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26828 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27086 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:41:48.855250 tvdcn-0.2.5/tvdcn/csrc/ops/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:41:48.855250 tvdcn-0.2.5/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:41:48.855250 tvdcn-0.2.5/tvdcn/ops/activations/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/ops/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/ops/activations/mask_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/ops/activations/mask_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    35826 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    38767 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-17 15:39:47.000000 tvdcn-0.2.5/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:41:48.847249 tvdcn-0.2.5/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-05-17 15:41:48.000000 tvdcn-0.2.5/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-17 15:41:48.000000 tvdcn-0.2.5/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:41:48.000000 tvdcn-0.2.5/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:41:48.000000 tvdcn-0.2.5/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-17 15:41:48.000000 tvdcn-0.2.5/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 15:41:48.000000 tvdcn-0.2.5/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.107993 tvdcn-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 03:56:17.000000 tvdcn-0.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-05-21 03:58:32.107993 tvdcn-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-05-21 03:56:17.000000 tvdcn-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-21 03:56:17.000000 tvdcn-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-21 03:58:32.107993 tvdcn-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-21 03:56:17.000000 tvdcn-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.087992 tvdcn-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.091992 tvdcn-0.2.6/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.091992 tvdcn-0.2.6/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.095992 tvdcn-0.2.6/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.099992 tvdcn-0.2.6/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26828 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27084 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.099992 tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.103993 tvdcn-0.2.6/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.103993 tvdcn-0.2.6/tvdcn/ops/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/activations/mask_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/activations/mask_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36102 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39157 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.091992 tvdcn-0.2.6/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.2.5/LICENSE.txt` & `tvdcn-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.5/PKG-INFO` & `tvdcn-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.5
+Version: 0.2.6
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
@@ -28,17 +28,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 Provides-Extra: tests
 License-File: LICENSE.txt
 
 Torchvision+ Deformable Convolution Networks
 ========
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/inspiros/tvdcn/build_wheels.yml)
-![PyPI](https://img.shields.io/pypi/v/tvdcn)
-![GitHub](https://img.shields.io/github/license/inspiros/tvdcn)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/inspiros/tvdcn/build_wheels.yml)](https://github.com/inspiros/tvdcn/actions)
+[![PyPI](https://img.shields.io/pypi/v/tvdcn)](https://pypi.org/project/tvdcn)
+[![GitHub](https://img.shields.io/github/license/inspiros/tvdcn)](LICENSE.txt)
 
 This package contains the PyTorch implementations of the **2D Deformable Convolution** operation
 (the commonly used  `torchvision.ops.deform_conv2d`) proposed in https://arxiv.org/abs/1811.11168,
 as well as its **1D** and **3D** equivalences, which are not available in `torchvision` (thus the name).
 
 And beyond that, the package also provides the **transposed** versions of them,
 which interestingly noone has ever proposed to use.
```

### Comparing `tvdcn-0.2.5/README.md` & `tvdcn-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Torchvision+ Deformable Convolution Networks
 ========
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/inspiros/tvdcn/build_wheels.yml)
-![PyPI](https://img.shields.io/pypi/v/tvdcn)
-![GitHub](https://img.shields.io/github/license/inspiros/tvdcn)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/inspiros/tvdcn/build_wheels.yml)](https://github.com/inspiros/tvdcn/actions)
+[![PyPI](https://img.shields.io/pypi/v/tvdcn)](https://pypi.org/project/tvdcn)
+[![GitHub](https://img.shields.io/github/license/inspiros/tvdcn)](LICENSE.txt)
 
 This package contains the PyTorch implementations of the **2D Deformable Convolution** operation
 (the commonly used  `torchvision.ops.deform_conv2d`) proposed in https://arxiv.org/abs/1811.11168,
 as well as its **1D** and **3D** equivalences, which are not available in `torchvision` (thus the name).
 
 And beyond that, the package also provides the **transposed** versions of them,
 which interestingly noone has ever proposed to use.
```

### Comparing `tvdcn-0.2.5/pyproject.toml` & `tvdcn-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.5/setup.cfg` & `tvdcn-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.5/setup.py` & `tvdcn-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.5/tests/test_compatibility_with_torchvision.py` & `tvdcn-0.2.6/tests/test_compatibility_with_torchvision.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.5/tests/test_grad.py` & `tvdcn-0.2.6/tests/test_grad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 from torch.autograd.gradcheck import gradcheck
 
 import tvdcn
 from utils.deform_conv_test_args import DeformConvTestArgs
 
 
-def test_deform_conv_grad(dim=1,
+def test_deform_conv_grad(dim=2,
                           transposed=False,
                           dtype=torch.float64,
                           device='cuda'):
     torch.manual_seed(12)
     conv_func = getattr(tvdcn, f'deform_conv{"_transpose" if transposed else ""}{dim}d')
     args = DeformConvTestArgs(dim=dim, transposed=transposed, dtype=dtype, device=device)
     print(args)
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -100,16 +100,16 @@
         static void arr2col_kernel(
                 const index_t n_kernels,
                 const at::TensorAccessor<scalar_t, 3> input,
                 const at::TensorAccessor<scalar_t, 5> offset,
                 const at::TensorAccessor<scalar_t, 4> mask,
                 const index_t width,
                 const index_t weight_w,
-                const index_t pad_w,
                 const index_t stride_w,
+                const index_t pad_w,
                 const index_t dilation_w,
                 const index_t out_w,
                 const index_t in_channels,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
                 at::TensorAccessor<scalar_t, 4> columns) {
             CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
@@ -141,16 +141,16 @@
         void arr2col_cpu(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int width,
                 const int weight_w,
-                const int pad_w,
                 const int stride_w,
+                const int pad_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
@@ -168,16 +168,16 @@
                         arr2col_kernel<deformable, modulated, scalar_t, index_t>(
                                 n_kernels,
                                 input.accessor<scalar_t, 3>(),
                                 offset.accessor<scalar_t, 5>(),
                                 mask.accessor<scalar_t, 4>(),
                                 width,
                                 weight_w,
-                                pad_w,
                                 stride_w,
+                                pad_w,
                                 dilation_w,
                                 out_w,
                                 in_channels,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 columns_accessor);
                     }));
@@ -190,16 +190,16 @@
                 const index_t n_kernels,
                 const at::TensorAccessor<scalar_t, 4> columns,
                 const at::TensorAccessor<scalar_t, 5> offset,
                 const at::TensorAccessor<scalar_t, 4> mask,
                 const index_t in_channels,
                 const index_t width,
                 const index_t weight_w,
-                const index_t pad_w,
                 const index_t stride_w,
+                const index_t pad_w,
                 const index_t dilation_w,
                 const index_t out_w,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
                 at::TensorAccessor<scalar_t, 3> grad_input) {
             CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
                 const index_t i = index % weight_w;
@@ -230,16 +230,16 @@
         void col2arr_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int width,
                 const int weight_w,
-                const int pad_w,
                 const int stride_w,
+                const int pad_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
@@ -258,16 +258,16 @@
                                 n_kernels,
                                 columns.accessor<scalar_t, 4>(),
                                 offset.accessor<scalar_t, 5>(),
                                 mask.accessor<scalar_t, 4>(),
                                 in_channels,
                                 width,
                                 weight_w,
-                                pad_w,
                                 stride_w,
+                                pad_w,
                                 dilation_w,
                                 out_w,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 grad_input_accessor);
                     }));
                 }));
@@ -279,16 +279,16 @@
                 const index_t n_kernels,
                 const at::TensorAccessor<scalar_t, 4> columns,
                 const at::TensorAccessor<scalar_t, 3> input,
                 const at::TensorAccessor<scalar_t, 5> offset,
                 const at::TensorAccessor<scalar_t, 4> mask,
                 const index_t width,
                 const index_t weight_w,
-                const index_t pad_w,
                 const index_t stride_w,
+                const index_t pad_w,
                 const index_t dilation_w,
                 const index_t out_w,
                 const index_t offset_groups,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
                 at::TensorAccessor<scalar_t, 5> grad_offset) {
             CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
@@ -324,16 +324,16 @@
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int width,
                 const int weight_w,
-                const int pad_w,
                 const int stride_w,
+                const int pad_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
@@ -353,16 +353,16 @@
                                 n_kernels,
                                 columns.accessor<scalar_t, 4>(),
                                 input.accessor<scalar_t, 3>(),
                                 offset.accessor<scalar_t, 5>(),
                                 mask.accessor<scalar_t, 4>(),
                                 width,
                                 weight_w,
-                                pad_w,
                                 stride_w,
+                                pad_w,
                                 dilation_w,
                                 out_w,
                                 offset_groups,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 grad_offset_accessor);
                     }));
@@ -374,16 +374,16 @@
         static void deform_conv1d_compute_grad_mask_kernel(
                 const index_t n_kernels,
                 const at::TensorAccessor<scalar_t, 4> columns,
                 const at::TensorAccessor<scalar_t, 3> input,
                 const at::TensorAccessor<scalar_t, 5> offset,
                 const index_t width,
                 const index_t weight_w,
-                const index_t pad_w,
                 const index_t stride_w,
+                const index_t pad_w,
                 const index_t dilation_w,
                 const index_t out_w,
                 const index_t mask_groups,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
                 at::TensorAccessor<scalar_t, 4> grad_mask) {
             CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
@@ -418,16 +418,16 @@
         void deform_conv1d_compute_grad_mask_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const int in_channels,
                 const int width,
                 const int weight_w,
-                const int pad_w,
                 const int stride_w,
+                const int pad_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
@@ -446,16 +446,16 @@
                         deform_conv1d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
                                 n_kernels,
                                 columns.accessor<scalar_t, 4>(),
                                 input.accessor<scalar_t, 3>(),
                                 offset.accessor<scalar_t, 5>(),
                                 width,
                                 weight_w,
-                                pad_w,
                                 stride_w,
+                                pad_w,
                                 dilation_w,
                                 out_w,
                                 mask_groups,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 grad_mask_accessor);
                     }));
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -137,18 +137,18 @@
                 const at::TensorAccessor<scalar_t, 4> input,
                 const at::TensorAccessor<scalar_t, 7> offset,
                 const at::TensorAccessor<scalar_t, 6> mask,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
-                const index_t pad_h,
-                const index_t pad_w,
                 const index_t stride_h,
                 const index_t stride_w,
+                const index_t pad_h,
+                const index_t pad_w,
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t in_channels,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
@@ -189,18 +189,18 @@
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int height,
                 const int width,
                 const int weight_h,
                 const int weight_w,
-                const int pad_h,
-                const int pad_w,
                 const int stride_h,
                 const int stride_w,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
@@ -222,18 +222,18 @@
                                 input.accessor<scalar_t, 4>(),
                                 offset.accessor<scalar_t, 7>(),
                                 mask.accessor<scalar_t, 6>(),
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
-                                pad_h,
-                                pad_w,
                                 stride_h,
                                 stride_w,
+                                pad_h,
+                                pad_w,
                                 dilation_h,
                                 dilation_w,
                                 out_h,
                                 out_w,
                                 in_channels,
                                 c_per_offset_group,
                                 c_per_mask_group,
@@ -250,18 +250,18 @@
                 const at::TensorAccessor<scalar_t, 7> offset,
                 const at::TensorAccessor<scalar_t, 6> mask,
                 const index_t in_channels,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
-                const index_t pad_h,
-                const index_t pad_w,
                 const index_t stride_h,
                 const index_t stride_w,
+                const index_t pad_h,
+                const index_t pad_w,
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
                 at::TensorAccessor<scalar_t, 4> grad_input) {
@@ -300,18 +300,18 @@
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int height,
                 const int width,
                 const int weight_h,
                 const int weight_w,
-                const int pad_h,
-                const int pad_w,
                 const int stride_h,
                 const int stride_w,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
@@ -334,18 +334,18 @@
                                 offset.accessor<scalar_t, 7>(),
                                 mask.accessor<scalar_t, 6>(),
                                 in_channels,
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
-                                pad_h,
-                                pad_w,
                                 stride_h,
                                 stride_w,
+                                pad_h,
+                                pad_w,
                                 dilation_h,
                                 dilation_w,
                                 out_h,
                                 out_w,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 grad_input_accessor);
@@ -361,18 +361,18 @@
                 const at::TensorAccessor<scalar_t, 4> input,
                 const at::TensorAccessor<scalar_t, 7> offset,
                 const at::TensorAccessor<scalar_t, 6> mask,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
-                const index_t pad_h,
-                const index_t pad_w,
                 const index_t stride_h,
                 const index_t stride_w,
+                const index_t pad_h,
+                const index_t pad_w,
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t offset_groups,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
@@ -418,18 +418,18 @@
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int height,
                 const int width,
                 const int weight_h,
                 const int weight_w,
-                const int pad_h,
-                const int pad_w,
                 const int stride_h,
                 const int stride_w,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
@@ -453,18 +453,18 @@
                                 input.accessor<scalar_t, 4>(),
                                 offset.accessor<scalar_t, 7>(),
                                 mask.accessor<scalar_t, 6>(),
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
-                                pad_h,
-                                pad_w,
                                 stride_h,
                                 stride_w,
+                                pad_h,
+                                pad_w,
                                 dilation_h,
                                 dilation_w,
                                 out_h,
                                 out_w,
                                 offset_groups,
                                 c_per_offset_group,
                                 c_per_mask_group,
@@ -480,18 +480,18 @@
                 const at::TensorAccessor<scalar_t, 6> columns,
                 const at::TensorAccessor<scalar_t, 4> input,
                 const at::TensorAccessor<scalar_t, 7> offset,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
-                const index_t pad_h,
-                const index_t pad_w,
                 const index_t stride_h,
                 const index_t stride_w,
+                const index_t pad_h,
+                const index_t pad_w,
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t mask_groups,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
@@ -534,18 +534,18 @@
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const int in_channels,
                 const int height,
                 const int width,
                 const int weight_h,
                 const int weight_w,
-                const int pad_h,
-                const int pad_w,
                 const int stride_h,
                 const int stride_w,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
@@ -568,18 +568,18 @@
                                 columns.accessor<scalar_t, 6>(),
                                 input.accessor<scalar_t, 4>(),
                                 offset.accessor<scalar_t, 7>(),
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
-                                pad_h,
-                                pad_w,
                                 stride_h,
                                 stride_w,
+                                pad_h,
+                                pad_w,
                                 dilation_h,
                                 dilation_w,
                                 out_h,
                                 out_w,
                                 mask_groups,
                                 c_per_offset_group,
                                 c_per_mask_group,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -204,20 +204,20 @@
                 const at::TensorAccessor<scalar_t, 8> mask,
                 const index_t depth,
                 const index_t height,
                 const index_t width,
                 const index_t weight_d,
                 const index_t weight_h,
                 const index_t weight_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
                 const index_t stride_d,
                 const index_t stride_h,
                 const index_t stride_w,
+                const index_t pad_d,
+                const index_t pad_h,
+                const index_t pad_w,
                 const index_t dilation_d,
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_d,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t in_channels,
@@ -268,20 +268,20 @@
                 const int in_channels,
                 const int depth,
                 const int height,
                 const int width,
                 const int weight_d,
                 const int weight_h,
                 const int weight_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
                 const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int pad_d,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
@@ -307,20 +307,20 @@
                                 mask.accessor<scalar_t, 8>(),
                                 depth,
                                 height,
                                 width,
                                 weight_d,
                                 weight_h,
                                 weight_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
                                 stride_d,
                                 stride_h,
                                 stride_w,
+                                pad_d,
+                                pad_h,
+                                pad_w,
                                 dilation_d,
                                 dilation_h,
                                 dilation_w,
                                 out_d,
                                 out_h,
                                 out_w,
                                 in_channels,
@@ -341,20 +341,20 @@
                 const index_t in_channels,
                 const index_t depth,
                 const index_t height,
                 const index_t width,
                 const index_t weight_d,
                 const index_t weight_h,
                 const index_t weight_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
                 const index_t stride_d,
                 const index_t stride_h,
                 const index_t stride_w,
+                const index_t pad_d,
+                const index_t pad_h,
+                const index_t pad_w,
                 const index_t dilation_d,
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_d,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t c_per_offset_group,
@@ -401,20 +401,20 @@
                 const int in_channels,
                 const int depth,
                 const int height,
                 const int width,
                 const int weight_d,
                 const int weight_h,
                 const int weight_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
                 const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int pad_d,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
@@ -442,20 +442,20 @@
                                 in_channels,
                                 depth,
                                 height,
                                 width,
                                 weight_d,
                                 weight_h,
                                 weight_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
                                 stride_d,
                                 stride_h,
                                 stride_w,
+                                pad_d,
+                                pad_h,
+                                pad_w,
                                 dilation_d,
                                 dilation_h,
                                 dilation_w,
                                 out_d,
                                 out_h,
                                 out_w,
                                 c_per_offset_group,
@@ -475,20 +475,20 @@
                 const at::TensorAccessor<scalar_t, 8> mask,
                 const index_t depth,
                 const index_t height,
                 const index_t width,
                 const index_t weight_d,
                 const index_t weight_h,
                 const index_t weight_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
                 const index_t stride_d,
                 const index_t stride_h,
                 const index_t stride_w,
+                const index_t pad_d,
+                const index_t pad_h,
+                const index_t pad_w,
                 const index_t dilation_d,
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_d,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t offset_groups,
@@ -544,20 +544,20 @@
                 const int in_channels,
                 const int depth,
                 const int height,
                 const int width,
                 const int weight_d,
                 const int weight_h,
                 const int weight_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
                 const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int pad_d,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
@@ -586,20 +586,20 @@
                                 mask.accessor<scalar_t, 8>(),
                                 depth,
                                 height,
                                 width,
                                 weight_d,
                                 weight_h,
                                 weight_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
                                 stride_d,
                                 stride_h,
                                 stride_w,
+                                pad_d,
+                                pad_h,
+                                pad_w,
                                 dilation_d,
                                 dilation_h,
                                 dilation_w,
                                 out_d,
                                 out_h,
                                 out_w,
                                 offset_groups,
@@ -619,20 +619,20 @@
                 const at::TensorAccessor<scalar_t, 9> offset,
                 const index_t depth,
                 const index_t height,
                 const index_t width,
                 const index_t weight_d,
                 const index_t weight_h,
                 const index_t weight_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
                 const index_t stride_d,
                 const index_t stride_h,
                 const index_t stride_w,
+                const index_t pad_d,
+                const index_t pad_h,
+                const index_t pad_w,
                 const index_t dilation_d,
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_d,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t mask_groups,
@@ -683,20 +683,20 @@
                 const int in_channels,
                 const int depth,
                 const int height,
                 const int width,
                 const int weight_d,
                 const int weight_h,
                 const int weight_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
                 const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int pad_d,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
@@ -724,20 +724,20 @@
                                 offset.accessor<scalar_t, 9>(),
                                 depth,
                                 height,
                                 width,
                                 weight_d,
                                 weight_h,
                                 weight_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
                                 stride_d,
                                 stride_h,
                                 stride_w,
+                                pad_d,
+                                pad_h,
+                                pad_w,
                                 dilation_d,
                                 dilation_h,
                                 dilation_w,
                                 out_d,
                                 out_h,
                                 out_w,
                                 mask_groups,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             TORCH_CHECK(weight_c.size(1) * groups == in_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * weight_w),
-                    "offset.shape[1] is not valid: got: ",
+                    "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
                     (!deformable || offset_c.size(2) == out_w),
@@ -158,15 +158,15 @@
                     ") - ",
                     "computed output dims: (",
                     out_w,
                     ")")
 
             TORCH_CHECK(
                     (!modulated || mask_c.size(1) == mask_groups * weight_w),
-                    "mask.shape[1] is not valid: got: ",
+                    "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
                     (!modulated || mask_c.size(2) == out_w),
@@ -246,16 +246,16 @@
                 arr2col(
                         input_c[b],
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_w,
                         weight_w,
-                        pad_w,
                         stride_w,
+                        pad_w,
                         dilation_w,
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
@@ -385,16 +385,16 @@
                         columns_view,
                         input_c[b],
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_w,
                         weight_w,
-                        pad_w,
                         stride_w,
+                        pad_w,
                         dilation_w,
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
@@ -404,16 +404,16 @@
                 deform_conv1d_compute_grad_mask(
                         columns_view,
                         input_c[b],
                         offset_c[b],
                         in_channels,
                         in_w,
                         weight_w,
-                        pad_w,
                         stride_w,
+                        pad_w,
                         dilation_w,
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
@@ -423,16 +423,16 @@
                 col2arr(
                         columns_view,
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_w,
                         weight_w,
-                        pad_w,
                         stride_w,
+                        pad_w,
                         dilation_w,
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
@@ -441,16 +441,16 @@
                 arr2col(
                         input_c[b],
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_w,
                         weight_w,
-                        pad_w,
                         stride_w,
+                        pad_w,
                         dilation_w,
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             TORCH_CHECK(weight_c.size(1) * groups == in_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w),
-                    "offset.shape[1] is not valid: got: ",
+                    "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 2 * weight_h * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
                     (!deformable || (offset_c.size(2) == out_h &&
@@ -173,15 +173,15 @@
                     out_h,
                     ", ",
                     out_w,
                     ")")
 
             TORCH_CHECK(
                     (!modulated || mask_c.size(1) == mask_groups * weight_h * weight_w),
-                    "mask.shape[1] is not valid: got: ",
+                    "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_h * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
                     (!modulated || (mask_c.size(2) == out_h &&
@@ -281,18 +281,18 @@
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_h,
                         in_w,
                         weight_h,
                         weight_w,
-                        pad_h,
-                        pad_w,
                         stride_h,
                         stride_w,
+                        pad_h,
+                        pad_w,
                         dilation_h,
                         dilation_w,
                         out_h,
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
@@ -442,18 +442,18 @@
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_h,
                         in_w,
                         weight_h,
                         weight_w,
-                        pad_h,
-                        pad_w,
                         stride_h,
                         stride_w,
+                        pad_h,
+                        pad_w,
                         dilation_h,
                         dilation_w,
                         out_h,
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
@@ -467,18 +467,18 @@
                         input_c[b],
                         offset_c[b],
                         in_channels,
                         in_h,
                         in_w,
                         weight_h,
                         weight_w,
-                        pad_h,
-                        pad_w,
                         stride_h,
                         stride_w,
+                        pad_h,
+                        pad_w,
                         dilation_h,
                         dilation_w,
                         out_h,
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
@@ -492,18 +492,18 @@
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_h,
                         in_w,
                         weight_h,
                         weight_w,
-                        pad_h,
-                        pad_w,
                         stride_h,
                         stride_w,
+                        pad_h,
+                        pad_w,
                         dilation_h,
                         dilation_w,
                         out_h,
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
@@ -516,18 +516,18 @@
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_h,
                         in_w,
                         weight_h,
                         weight_w,
-                        pad_h,
-                        pad_w,
                         stride_h,
                         stride_w,
+                        pad_h,
+                        pad_w,
                         dilation_h,
                         dilation_w,
                         out_h,
                         out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv3d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             TORCH_CHECK(weight_c.size(1) * groups == in_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w),
-                    "offset.shape[1] is not valid: got: ",
+                    "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
                     (!deformable || (offset_c.size(2) == out_d &&
@@ -189,15 +189,15 @@
                     out_h,
                     ", ",
                     out_w,
                     ")")
 
             TORCH_CHECK(
                     (!modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w),
-                    "mask.shape[1] is not valid: got: ",
+                    "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_d * weight_h * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
                     (!modulated || (mask_c.size(2) == out_d &&
@@ -317,20 +317,20 @@
                         in_channels,
                         in_d,
                         in_h,
                         in_w,
                         weight_d,
                         weight_h,
                         weight_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
                         stride_d,
                         stride_h,
                         stride_w,
+                        pad_d,
+                        pad_h,
+                        pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
                         out_d,
                         out_h,
                         out_w,
                         n_parallel_imgs,
@@ -500,20 +500,20 @@
                         in_channels,
                         in_d,
                         in_h,
                         in_w,
                         weight_d,
                         weight_h,
                         weight_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
                         stride_d,
                         stride_h,
                         stride_w,
+                        pad_d,
+                        pad_h,
+                        pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
                         out_d,
                         out_h,
                         out_w,
                         n_parallel_imgs,
@@ -531,20 +531,20 @@
                         in_channels,
                         in_d,
                         in_h,
                         in_w,
                         weight_d,
                         weight_h,
                         weight_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
                         stride_d,
                         stride_h,
                         stride_w,
+                        pad_d,
+                        pad_h,
+                        pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
                         out_d,
                         out_h,
                         out_w,
                         n_parallel_imgs,
@@ -562,20 +562,20 @@
                         in_channels,
                         in_d,
                         in_h,
                         in_w,
                         weight_d,
                         weight_h,
                         weight_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
                         stride_d,
                         stride_h,
                         stride_w,
+                        pad_d,
+                        pad_h,
+                        pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
                         out_d,
                         out_h,
                         out_w,
                         n_parallel_imgs,
@@ -592,20 +592,20 @@
                         in_channels,
                         in_d,
                         in_h,
                         in_w,
                         weight_d,
                         weight_h,
                         weight_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
                         stride_d,
                         stride_h,
                         stride_w,
+                        pad_d,
+                        pad_h,
+                        pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
                         out_d,
                         out_h,
                         out_w,
                         n_parallel_imgs,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * weight_w),
-                    "offset.shape[1] is not valid: got: ",
+                    "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
                     (!deformable || offset_c.size(2) == in_w),
@@ -161,15 +161,15 @@
                     ") - ",
                     "input dims: (",
                     in_w,
                     ")")
 
             TORCH_CHECK(
                     (!modulated || mask_c.size(1) == mask_groups * weight_w),
-                    "mask.shape[1] is not valid: got: ",
+                    "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
                     (!modulated || mask_c.size(2) == in_w),
@@ -244,16 +244,16 @@
                 col2arr(
                         columns_view,
                         offset_c[b],
                         mask_c[b],
                         out_channels,
                         out_w,
                         weight_w,
-                        pad_w,
                         stride_w,
+                        pad_w,
                         dilation_w,
                         in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
@@ -392,16 +392,16 @@
                         columns_view,
                         grad_out_c[b],
                         offset_c[b],
                         mask_c[b],
                         out_channels,
                         out_w,
                         weight_w,
-                        pad_w,
                         stride_w,
+                        pad_w,
                         dilation_w,
                         in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
@@ -411,16 +411,16 @@
                 deform_conv1d_compute_grad_mask(
                         columns_view,
                         grad_out_c[b],
                         offset_c[b],
                         out_channels,
                         out_w,
                         weight_w,
-                        pad_w,
                         stride_w,
+                        pad_w,
                         dilation_w,
                         in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
@@ -429,16 +429,16 @@
                 arr2col(
                         grad_out_c[b],
                         offset_c[b],
                         mask_c[b],
                         out_channels,
                         out_w,
                         weight_w,
-                        pad_w,
                         stride_w,
+                        pad_w,
                         dilation_w,
                         in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
             TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w),
-                    "offset.shape[1] is not valid: got: ",
+                    "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 2 * weight_h * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
                     (!deformable || (offset_c.size(2) == in_h &&
@@ -177,15 +177,15 @@
                     in_h,
                     ", ",
                     in_w,
                     ")")
 
             TORCH_CHECK(
                     (!modulated || mask_c.size(1) == mask_groups * weight_h * weight_w),
-                    "mask.shape[1] is not valid: got: ",
+                    "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_h * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
                     (!modulated || (mask_c.size(2) == in_h &&
@@ -278,18 +278,18 @@
                         offset_c[b],
                         mask_c[b],
                         out_channels,
                         out_h,
                         out_w,
                         weight_h,
                         weight_w,
-                        pad_h,
-                        pad_w,
                         stride_h,
                         stride_w,
+                        pad_h,
+                        pad_w,
                         dilation_h,
                         dilation_w,
                         in_h,
                         in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
@@ -451,18 +451,18 @@
                         offset_c[b],
                         mask_c[b],
                         out_channels,
                         out_h,
                         out_w,
                         weight_h,
                         weight_w,
-                        pad_h,
-                        pad_w,
                         stride_h,
                         stride_w,
+                        pad_h,
+                        pad_w,
                         dilation_h,
                         dilation_w,
                         in_h,
                         in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
@@ -476,18 +476,18 @@
                         grad_out_c[b],
                         offset_c[b],
                         out_channels,
                         out_h,
                         out_w,
                         weight_h,
                         weight_w,
-                        pad_h,
-                        pad_w,
                         stride_h,
                         stride_w,
+                        pad_h,
+                        pad_w,
                         dilation_h,
                         dilation_w,
                         in_h,
                         in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
@@ -500,18 +500,18 @@
                         offset_c[b],
                         mask_c[b],
                         out_channels,
                         out_h,
                         out_w,
                         weight_h,
                         weight_w,
-                        pad_h,
-                        pad_w,
                         stride_h,
                         stride_w,
+                        pad_h,
+                        pad_w,
                         dilation_h,
                         dilation_w,
                         in_h,
                         in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -167,25 +167,25 @@
             TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w),
-                    "offset.shape[1] is not valid: got: ",
+                    "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
                     (!deformable || (offset_c.size(2) == in_d &&
                                      offset_c.size(3) == in_h &&
                                      offset_c.size(4) == in_w)),
-                    "offset output dims: (",
+                    "offset input dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
                     ", ",
                     offset_c.size(4),
                     ") - ",
                     "input dims: (",
@@ -194,25 +194,25 @@
                     in_h,
                     ", ",
                     in_w,
                     ")")
 
             TORCH_CHECK(
                     (!modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w),
-                    "mask.shape[1] is not valid: got: ",
+                    "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_d * weight_h * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
                     (!modulated || (mask_c.size(2) == in_d &&
                                     mask_c.size(3) == in_h &&
                                     mask_c.size(4) == in_w)),
-                    "mask output dims: (",
+                    "mask input dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
                     ", ",
                     mask_c.size(4),
                     ") - ",
                     "input dims: (",
@@ -313,20 +313,20 @@
                         out_channels,
                         out_d,
                         out_h,
                         out_w,
                         weight_d,
                         weight_h,
                         weight_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
                         stride_d,
                         stride_h,
                         stride_w,
+                        pad_d,
+                        pad_h,
+                        pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
                         in_d,
                         in_h,
                         in_w,
                         n_parallel_imgs,
@@ -511,20 +511,20 @@
                         out_channels,
                         out_d,
                         out_h,
                         out_w,
                         weight_d,
                         weight_h,
                         weight_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
                         stride_d,
                         stride_h,
                         stride_w,
+                        pad_d,
+                        pad_h,
+                        pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
                         in_d,
                         in_h,
                         in_w,
                         n_parallel_imgs,
@@ -542,20 +542,20 @@
                         out_channels,
                         out_d,
                         out_h,
                         out_w,
                         weight_d,
                         weight_h,
                         weight_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
                         stride_d,
                         stride_h,
                         stride_w,
+                        pad_d,
+                        pad_h,
+                        pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
                         in_d,
                         in_h,
                         in_w,
                         n_parallel_imgs,
@@ -572,20 +572,20 @@
                         out_channels,
                         out_d,
                         out_h,
                         out_w,
                         weight_d,
                         weight_h,
                         weight_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
                         stride_d,
                         stride_h,
                         stride_w,
+                        pad_d,
+                        pad_h,
+                        pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
                         in_d,
                         in_h,
                         in_w,
                         n_parallel_imgs,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
         void arr2col(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int width,
                 const int weight_w,
-                const int pad_w,
                 const int stride_w,
+                const int pad_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
@@ -29,16 +29,16 @@
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 arr2col_cuda(input,
                              offset,
                              mask,
                              in_channels,
                              width,
                              weight_w,
-                             pad_w,
                              stride_w,
+                             pad_w,
                              dilation_w,
                              out_w,
                              batch_sz,
                              offset_groups,
                              mask_groups,
                              deformable,
                              modulated,
@@ -49,16 +49,16 @@
             } else {
                 arr2col_cpu(input,
                             offset,
                             mask,
                             in_channels,
                             width,
                             weight_w,
-                            pad_w,
                             stride_w,
+                            pad_w,
                             dilation_w,
                             out_w,
                             batch_sz,
                             offset_groups,
                             mask_groups,
                             deformable,
                             modulated,
@@ -69,16 +69,16 @@
         void col2arr(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int width,
                 const int weight_w,
-                const int pad_w,
                 const int stride_w,
+                const int pad_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
@@ -87,16 +87,16 @@
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 col2arr_cuda(columns,
                              offset,
                              mask,
                              in_channels,
                              width,
                              weight_w,
-                             pad_w,
                              stride_w,
+                             pad_w,
                              dilation_w,
                              out_w,
                              batch_sz,
                              offset_groups,
                              mask_groups,
                              deformable,
                              modulated,
@@ -107,16 +107,16 @@
             } else {
                 col2arr_cpu(columns,
                             offset,
                             mask,
                             in_channels,
                             width,
                             weight_w,
-                            pad_w,
                             stride_w,
+                            pad_w,
                             dilation_w,
                             out_w,
                             batch_sz,
                             offset_groups,
                             mask_groups,
                             deformable,
                             modulated,
@@ -128,16 +128,16 @@
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int width,
                 const int weight_w,
-                const int pad_w,
                 const int stride_w,
+                const int pad_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
@@ -147,16 +147,16 @@
                 deform_conv1d_compute_grad_offset_cuda(columns,
                                                        input,
                                                        offset,
                                                        mask,
                                                        in_channels,
                                                        width,
                                                        weight_w,
-                                                       pad_w,
                                                        stride_w,
+                                                       pad_w,
                                                        dilation_w,
                                                        out_w,
                                                        batch_sz,
                                                        offset_groups,
                                                        mask_groups,
                                                        deformable,
                                                        modulated,
@@ -168,16 +168,16 @@
                 deform_conv1d_compute_grad_offset_cpu(columns,
                                                       input,
                                                       offset,
                                                       mask,
                                                       in_channels,
                                                       width,
                                                       weight_w,
-                                                      pad_w,
                                                       stride_w,
+                                                      pad_w,
                                                       dilation_w,
                                                       out_w,
                                                       batch_sz,
                                                       offset_groups,
                                                       mask_groups,
                                                       deformable,
                                                       modulated,
@@ -188,16 +188,16 @@
         void deform_conv1d_compute_grad_mask(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const int in_channels,
                 const int width,
                 const int weight_w,
-                const int pad_w,
                 const int stride_w,
+                const int pad_w,
                 const int dilation_w,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
@@ -206,16 +206,16 @@
 #if defined(WITH_CUDA) || defined(WITH_HIP)
                 deform_conv1d_compute_grad_mask_cuda(columns,
                                                      input,
                                                      offset,
                                                      in_channels,
                                                      width,
                                                      weight_w,
-                                                     pad_w,
                                                      stride_w,
+                                                     pad_w,
                                                      dilation_w,
                                                      out_w,
                                                      batch_sz,
                                                      offset_groups,
                                                      mask_groups,
                                                      deformable,
                                                      modulated,
@@ -226,16 +226,16 @@
             } else {
                 deform_conv1d_compute_grad_mask_cpu(columns,
                                                     input,
                                                     offset,
                                                     in_channels,
                                                     width,
                                                     weight_w,
-                                                    pad_w,
                                                     stride_w,
+                                                    pad_w,
                                                     dilation_w,
                                                     out_w,
                                                     batch_sz,
                                                     offset_groups,
                                                     mask_groups,
                                                     deformable,
                                                     modulated,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int height,
                 const int width,
                 const int weight_h,
                 const int weight_w,
-                const int pad_h,
-                const int pad_w,
                 const int stride_h,
                 const int stride_w,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
@@ -37,18 +37,18 @@
                             offset,
                             mask,
                             in_channels,
                             height,
                             width,
                             weight_h,
                             weight_w,
-                            pad_h,
-                            pad_w,
                             stride_h,
                             stride_w,
+                            pad_h,
+                            pad_w,
                             dilation_h,
                             dilation_w,
                             out_h,
                             out_w,
                             batch_sz,
                             offset_groups,
                             mask_groups,
@@ -63,18 +63,18 @@
                            offset,
                            mask,
                            in_channels,
                            height,
                            width,
                            weight_h,
                            weight_w,
-                           pad_h,
-                           pad_w,
                            stride_h,
                            stride_w,
+                           pad_h,
+                           pad_w,
                            dilation_h,
                            dilation_w,
                            out_h,
                            out_w,
                            batch_sz,
                            offset_groups,
                            mask_groups,
@@ -89,18 +89,18 @@
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int height,
                 const int width,
                 const int weight_h,
                 const int weight_w,
-                const int pad_h,
-                const int pad_w,
                 const int stride_h,
                 const int stride_w,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
@@ -113,18 +113,18 @@
                             offset,
                             mask,
                             in_channels,
                             height,
                             width,
                             weight_h,
                             weight_w,
-                            pad_h,
-                            pad_w,
                             stride_h,
                             stride_w,
+                            pad_h,
+                            pad_w,
                             dilation_h,
                             dilation_w,
                             out_h,
                             out_w,
                             batch_sz,
                             offset_groups,
                             mask_groups,
@@ -139,18 +139,18 @@
                            offset,
                            mask,
                            in_channels,
                            height,
                            width,
                            weight_h,
                            weight_w,
-                           pad_h,
-                           pad_w,
                            stride_h,
                            stride_w,
+                           pad_h,
+                           pad_w,
                            dilation_h,
                            dilation_w,
                            out_h,
                            out_w,
                            batch_sz,
                            offset_groups,
                            mask_groups,
@@ -166,18 +166,18 @@
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const int in_channels,
                 const int height,
                 const int width,
                 const int weight_h,
                 const int weight_w,
-                const int pad_h,
-                const int pad_w,
                 const int stride_h,
                 const int stride_w,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
@@ -191,18 +191,18 @@
                                                        offset,
                                                        mask,
                                                        in_channels,
                                                        height,
                                                        width,
                                                        weight_h,
                                                        weight_w,
-                                                       pad_h,
-                                                       pad_w,
                                                        stride_h,
                                                        stride_w,
+                                                       pad_h,
+                                                       pad_w,
                                                        dilation_h,
                                                        dilation_w,
                                                        out_h,
                                                        out_w,
                                                        batch_sz,
                                                        offset_groups,
                                                        mask_groups,
@@ -218,18 +218,18 @@
                                                       offset,
                                                       mask,
                                                       in_channels,
                                                       height,
                                                       width,
                                                       weight_h,
                                                       weight_w,
-                                                      pad_h,
-                                                      pad_w,
                                                       stride_h,
                                                       stride_w,
+                                                      pad_h,
+                                                      pad_w,
                                                       dilation_h,
                                                       dilation_w,
                                                       out_h,
                                                       out_w,
                                                       batch_sz,
                                                       offset_groups,
                                                       mask_groups,
@@ -244,18 +244,18 @@
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const int in_channels,
                 const int height,
                 const int width,
                 const int weight_h,
                 const int weight_w,
-                const int pad_h,
-                const int pad_w,
                 const int stride_h,
                 const int stride_w,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
@@ -268,18 +268,18 @@
                                                      input,
                                                      offset,
                                                      in_channels,
                                                      height,
                                                      width,
                                                      weight_h,
                                                      weight_w,
-                                                     pad_h,
-                                                     pad_w,
                                                      stride_h,
                                                      stride_w,
+                                                     pad_h,
+                                                     pad_w,
                                                      dilation_h,
                                                      dilation_w,
                                                      out_h,
                                                      out_w,
                                                      batch_sz,
                                                      offset_groups,
                                                      mask_groups,
@@ -294,18 +294,18 @@
                                                     input,
                                                     offset,
                                                     in_channels,
                                                     height,
                                                     width,
                                                     weight_h,
                                                     weight_w,
-                                                    pad_h,
-                                                    pad_w,
                                                     stride_h,
                                                     stride_w,
+                                                    pad_h,
+                                                    pad_w,
                                                     dilation_h,
                                                     dilation_w,
                                                     out_h,
                                                     out_w,
                                                     batch_sz,
                                                     offset_groups,
                                                     mask_groups,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp` & `tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,20 @@
                 const int in_channels,
                 const int depth,
                 const int height,
                 const int width,
                 const int weight_d,
                 const int weight_h,
                 const int weight_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
                 const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int pad_d,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
@@ -45,20 +45,20 @@
                              in_channels,
                              depth,
                              height,
                              width,
                              weight_d,
                              weight_h,
                              weight_w,
-                             pad_d,
-                             pad_h,
-                             pad_w,
                              stride_d,
                              stride_h,
                              stride_w,
+                             pad_d,
+                             pad_h,
+                             pad_w,
                              dilation_d,
                              dilation_h,
                              dilation_w,
                              out_d,
                              out_h,
                              out_w,
                              batch_sz,
@@ -77,20 +77,20 @@
                             in_channels,
                             depth,
                             height,
                             width,
                             weight_d,
                             weight_h,
                             weight_w,
-                            pad_d,
-                            pad_h,
-                            pad_w,
                             stride_d,
                             stride_h,
                             stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
                             dilation_d,
                             dilation_h,
                             dilation_w,
                             out_d,
                             out_h,
                             out_w,
                             batch_sz,
@@ -109,20 +109,20 @@
                 const int in_channels,
                 const int depth,
                 const int height,
                 const int width,
                 const int weight_d,
                 const int weight_h,
                 const int weight_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
                 const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int pad_d,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
@@ -139,20 +139,20 @@
                              in_channels,
                              depth,
                              height,
                              width,
                              weight_d,
                              weight_h,
                              weight_w,
-                             pad_d,
-                             pad_h,
-                             pad_w,
                              stride_d,
                              stride_h,
                              stride_w,
+                             pad_d,
+                             pad_h,
+                             pad_w,
                              dilation_d,
                              dilation_h,
                              dilation_w,
                              out_d,
                              out_h,
                              out_w,
                              batch_sz,
@@ -171,20 +171,20 @@
                             in_channels,
                             depth,
                             height,
                             width,
                             weight_d,
                             weight_h,
                             weight_w,
-                            pad_d,
-                            pad_h,
-                            pad_w,
                             stride_d,
                             stride_h,
                             stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
                             dilation_d,
                             dilation_h,
                             dilation_w,
                             out_d,
                             out_h,
                             out_w,
                             batch_sz,
@@ -204,20 +204,20 @@
                 const int in_channels,
                 const int depth,
                 const int height,
                 const int width,
                 const int weight_d,
                 const int weight_h,
                 const int weight_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
                 const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int pad_d,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
@@ -235,20 +235,20 @@
                                                        in_channels,
                                                        depth,
                                                        height,
                                                        width,
                                                        weight_d,
                                                        weight_h,
                                                        weight_w,
-                                                       pad_d,
-                                                       pad_h,
-                                                       pad_w,
                                                        stride_d,
                                                        stride_h,
                                                        stride_w,
+                                                       pad_d,
+                                                       pad_h,
+                                                       pad_w,
                                                        dilation_d,
                                                        dilation_h,
                                                        dilation_w,
                                                        out_d,
                                                        out_h,
                                                        out_w,
                                                        batch_sz,
@@ -268,20 +268,20 @@
                                                       in_channels,
                                                       depth,
                                                       height,
                                                       width,
                                                       weight_d,
                                                       weight_h,
                                                       weight_w,
-                                                      pad_d,
-                                                      pad_h,
-                                                      pad_w,
                                                       stride_d,
                                                       stride_h,
                                                       stride_w,
+                                                      pad_d,
+                                                      pad_h,
+                                                      pad_w,
                                                       dilation_d,
                                                       dilation_h,
                                                       dilation_w,
                                                       out_d,
                                                       out_h,
                                                       out_w,
                                                       batch_sz,
@@ -300,20 +300,20 @@
                 const int in_channels,
                 const int depth,
                 const int height,
                 const int width,
                 const int weight_d,
                 const int weight_h,
                 const int weight_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
                 const int stride_d,
                 const int stride_h,
                 const int stride_w,
+                const int pad_d,
+                const int pad_h,
+                const int pad_w,
                 const int dilation_d,
                 const int dilation_h,
                 const int dilation_w,
                 const int out_d,
                 const int out_h,
                 const int out_w,
                 const int batch_sz,
@@ -330,20 +330,20 @@
                                                      in_channels,
                                                      depth,
                                                      height,
                                                      width,
                                                      weight_d,
                                                      weight_h,
                                                      weight_w,
-                                                     pad_d,
-                                                     pad_h,
-                                                     pad_w,
                                                      stride_d,
                                                      stride_h,
                                                      stride_w,
+                                                     pad_d,
+                                                     pad_h,
+                                                     pad_w,
                                                      dilation_d,
                                                      dilation_h,
                                                      dilation_w,
                                                      out_d,
                                                      out_h,
                                                      out_w,
                                                      batch_sz,
@@ -362,20 +362,20 @@
                                                     in_channels,
                                                     depth,
                                                     height,
                                                     width,
                                                     weight_d,
                                                     weight_h,
                                                     weight_w,
-                                                    pad_d,
-                                                    pad_h,
-                                                    pad_w,
                                                     stride_d,
                                                     stride_h,
                                                     stride_w,
+                                                    pad_d,
+                                                    pad_h,
+                                                    pad_w,
                                                     dilation_d,
                                                     dilation_h,
                                                     dilation_w,
                                                     out_d,
                                                     out_h,
                                                     out_w,
                                                     batch_sz,
```

### Comparing `tvdcn-0.2.5/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.2.6/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.5/tvdcn/extension.py` & `tvdcn-0.2.6/tvdcn/extension.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.5/tvdcn/ops/activations/mask_sigmoid.py` & `tvdcn-0.2.6/tvdcn/ops/activations/mask_sigmoid.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.5/tvdcn/ops/activations/mask_softmax.py` & `tvdcn-0.2.6/tvdcn/ops/activations/mask_softmax.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.5/tvdcn/ops/deform_conv.py` & `tvdcn-0.2.6/tvdcn/ops/deform_conv.py`

 * *Files 14% similar despite different names*

```diff
@@ -538,15 +538,15 @@
                  stride: _size_1_t = 1,
                  padding: Union[str, _size_1_t] = 0,
                  dilation: _size_1_t = 1,
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
-                 auxiliary_bias: bool = False,
+                 generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
                  mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
@@ -577,71 +577,71 @@
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
 
         self.deformable = deformable
         self.modulated = modulated
 
         if self.deformable:
-            self.conv_offset = nn.Conv1d(
+            self.offset_generator = nn.Conv1d(
                 self.in_channels,
                 self.kernel_size[0] * self.offset_groups,
                 kernel_size=self.kernel_size,
                 stride=self.stride,
                 padding=self.padding,
                 dilation=self.dilation,
-                groups=self.groups,
-                bias=auxiliary_bias,
+                groups=self.offset_groups,
+                bias=generator_bias,
                 device=device,
                 dtype=dtype)
         else:
-            self.register_module('conv_offset', None)
+            self.register_module('offset_generator', None)
 
         if self.modulated:
-            self.conv_mask = nn.Conv1d(
+            self.mask_generator = nn.Conv1d(
                 self.in_channels,
                 self.kernel_size[0] * self.mask_groups,
                 kernel_size=self.kernel_size,
                 stride=self.stride,
                 padding=self.padding,
                 dilation=self.dilation,
-                groups=self.groups,
-                bias=auxiliary_bias,
+                groups=self.mask_groups,
+                bias=generator_bias,
                 device=device,
                 dtype=dtype)
         else:
-            self.register_module('conv_mask', None)
+            self.register_module('mask_generator', None)
 
         self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
-        if self.conv_offset is not None:
-            init.zeros_(self.conv_offset.weight)
-            if self.conv_offset.bias is not None:
-                init.zeros_(self.conv_offset.bias)
-        if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
-            if self.conv_mask.bias is not None:
-                init.zeros_(self.conv_mask.bias)
+        if self.offset_generator is not None:
+            init.zeros_(self.offset_generator.weight)
+            if self.offset_generator.bias is not None:
+                init.zeros_(self.offset_generator.bias)
+        if self.mask_generator is not None:
+            init.zeros_(self.mask_generator.weight)
+            if self.mask_generator.bias is not None:
+                init.zeros_(self.mask_generator.bias)
 
     def forward(self, input: Tensor) -> Tensor:
-        if self.deformable and self.conv_offset is not None:
-            offset = self.conv_offset(input)
+        if self.deformable and self.offset_generator is not None:
+            offset = self.offset_generator(input)
             if self.offset_activation is not None:
                 offset = self.offset_activation(offset)
         else:
             offset = None
 
-        if self.modulated and self.conv_mask is not None:
-            mask = self.conv_mask(input)
+        if self.modulated and self.mask_generator is not None:
+            mask = self.mask_generator(input)
             if self.mask_activation is not None:
                 mask = self.mask_activation(mask)
         else:
             mask = None
 
         return self._conv_forward(input, self.weight, offset, mask, self.bias)
 
@@ -659,15 +659,15 @@
                  stride: _size_2_t = 1,
                  padding: Union[str, _size_2_t] = 0,
                  dilation: _size_2_t = 1,
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
-                 auxiliary_bias: bool = False,
+                 generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
                  mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
@@ -698,71 +698,71 @@
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
 
         self.deformable = deformable
         self.modulated = modulated
 
         if self.deformable:
-            self.conv_offset = nn.Conv2d(
+            self.offset_generator = nn.Conv2d(
                 self.in_channels,
                 2 * self.kernel_size[0] * self.kernel_size[1] * self.offset_groups,
                 kernel_size=self.kernel_size,  # type: ignore[arg-type]
                 stride=self.stride,  # type: ignore[arg-type]
                 padding=self.padding,
                 dilation=self.dilation,  # type: ignore[arg-type]
-                groups=self.groups,
-                bias=auxiliary_bias,
+                groups=self.offset_groups,
+                bias=generator_bias,
                 device=device,
                 dtype=dtype)
         else:
-            self.register_module('conv_offset', None)
+            self.register_module('offset_generator', None)
 
         if self.modulated:
-            self.conv_mask = nn.Conv2d(
+            self.mask_generator = nn.Conv2d(
                 self.in_channels,
                 self.kernel_size[0] * self.kernel_size[1] * self.mask_groups,
                 kernel_size=self.kernel_size,  # type: ignore[arg-type]
                 stride=self.stride,  # type: ignore[arg-type]
                 padding=self.padding,
                 dilation=self.dilation,  # type: ignore[arg-type]
-                groups=self.groups,
-                bias=auxiliary_bias,
+                groups=self.mask_groups,
+                bias=generator_bias,
                 device=device,
                 dtype=dtype)
         else:
-            self.register_module('conv_mask', None)
+            self.register_module('mask_generator', None)
 
         self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
-        if self.conv_offset is not None:
-            init.zeros_(self.conv_offset.weight)
-            if self.conv_offset.bias is not None:
-                init.zeros_(self.conv_offset.bias)
-        if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
-            if self.conv_mask.bias is not None:
-                init.zeros_(self.conv_mask.bias)
+        if self.offset_generator is not None:
+            init.zeros_(self.offset_generator.weight)
+            if self.offset_generator.bias is not None:
+                init.zeros_(self.offset_generator.bias)
+        if self.mask_generator is not None:
+            init.zeros_(self.mask_generator.weight)
+            if self.mask_generator.bias is not None:
+                init.zeros_(self.mask_generator.bias)
 
     def forward(self, input: Tensor) -> Tensor:
-        if self.deformable and self.conv_offset is not None:
-            offset = self.conv_offset(input)
+        if self.deformable and self.offset_generator is not None:
+            offset = self.offset_generator(input)
             if self.offset_activation is not None:
                 offset = self.offset_activation(offset)
         else:
             offset = None
 
-        if self.modulated and self.conv_mask is not None:
-            mask = self.conv_mask(input)
+        if self.modulated and self.mask_generator is not None:
+            mask = self.mask_generator(input)
             if self.mask_activation is not None:
                 mask = self.mask_activation(mask)
         else:
             mask = None
 
         return self._conv_forward(input, self.weight, offset, mask, self.bias)
 
@@ -780,15 +780,15 @@
                  stride: _size_3_t = 1,
                  padding: Union[str, _size_3_t] = 0,
                  dilation: _size_3_t = 1,
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
-                 auxiliary_bias: bool = False,
+                 generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
                  mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
@@ -819,70 +819,70 @@
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
 
         self.deformable = deformable
         self.modulated = modulated
 
         if self.deformable:
-            self.conv_offset = nn.Conv3d(
+            self.offset_generator = nn.Conv3d(
                 self.in_channels,
                 3 * self.kernel_size[0] * self.kernel_size[1] * self.kernel_size[2] * self.offset_groups,
                 kernel_size=self.kernel_size,  # type: ignore[arg-type]
                 stride=self.stride,  # type: ignore[arg-type]
                 padding=self.padding,
                 dilation=self.dilation,  # type: ignore[arg-type]
-                groups=self.groups,
-                bias=auxiliary_bias,
+                groups=self.offset_groups,
+                bias=generator_bias,
                 device=dtype,
                 dtype=device)
         else:
-            self.register_module('conv_offset', None)
+            self.register_module('offset_generator', None)
 
         if self.modulated:
-            self.conv_mask = nn.Conv3d(
+            self.mask_generator = nn.Conv3d(
                 self.in_channels,
                 self.kernel_size[0] * self.kernel_size[1] * self.kernel_size[2] * self.mask_groups,
                 kernel_size=self.kernel_size,  # type: ignore[arg-type]
                 stride=self.stride,  # type: ignore[arg-type]
                 padding=self.padding,
                 dilation=self.dilation,  # type: ignore[arg-type]
-                groups=self.groups,
-                bias=auxiliary_bias,
+                groups=self.mask_groups,
+                bias=generator_bias,
                 device=dtype,
                 dtype=device)
         else:
-            self.register_module('conv_mask', None)
+            self.register_module('mask_generator', None)
 
         self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
-        if self.conv_offset is not None:
-            init.zeros_(self.conv_offset.weight)
-            if self.conv_offset.bias is not None:
-                init.zeros_(self.conv_offset.bias)
-        if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
-            if self.conv_mask.bias is not None:
-                init.zeros_(self.conv_mask.bias)
+        if self.offset_generator is not None:
+            init.zeros_(self.offset_generator.weight)
+            if self.offset_generator.bias is not None:
+                init.zeros_(self.offset_generator.bias)
+        if self.mask_generator is not None:
+            init.zeros_(self.mask_generator.weight)
+            if self.mask_generator.bias is not None:
+                init.zeros_(self.mask_generator.bias)
 
     def forward(self, input: Tensor) -> Tensor:
-        if self.deformable and self.conv_offset is not None:
-            offset = self.conv_offset(input)
+        if self.deformable and self.offset_generator is not None:
+            offset = self.offset_generator(input)
             if self.offset_activation is not None:
                 offset = self.offset_activation(offset)
         else:
             offset = None
 
-        if self.modulated and self.conv_mask is not None:
-            mask = self.conv_mask(input)
+        if self.modulated and self.mask_generator is not None:
+            mask = self.mask_generator(input)
             if self.mask_activation is not None:
                 mask = self.mask_activation(mask)
         else:
             mask = None
 
         return self._conv_forward(input, self.weight, offset, mask, self.bias)
```

### Comparing `tvdcn-0.2.5/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.2.6/tvdcn/ops/deform_conv_transpose.py`

 * *Files 12% similar despite different names*

```diff
@@ -597,15 +597,15 @@
                  padding: Union[str, _size_1_t] = 0,
                  dilation: _size_1_t = 1,
                  output_padding: Union[str, _size_1_t] = 0,
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
-                 auxiliary_bias: bool = False,
+                 generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
                  mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
@@ -636,63 +636,65 @@
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
 
         self.deformable = deformable
         self.modulated = modulated
 
         if self.deformable:
-            self.conv_offset = nn.Conv1d(
+            self.offset_generator = nn.Conv1d(
                 self.in_channels,
                 self.kernel_size[0] * self.offset_groups,
                 kernel_size=1,
-                bias=auxiliary_bias,
+                groups=self.offset_groups,
+                bias=generator_bias,
                 device=dtype,
                 dtype=device)
         else:
-            self.register_module('conv_offset', None)
+            self.register_module('offset_generator', None)
 
         if self.modulated:
-            self.conv_mask = nn.Conv1d(
+            self.mask_generator = nn.Conv1d(
                 self.in_channels,
                 self.kernel_size[0] * self.mask_groups,
                 kernel_size=1,
-                bias=auxiliary_bias,
+                groups=self.mask_groups,
+                bias=generator_bias,
                 device=dtype,
                 dtype=device)
         else:
-            self.register_module('conv_mask', None)
+            self.register_module('mask_generator', None)
 
         self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
-        if self.conv_offset is not None:
-            init.zeros_(self.conv_offset.weight)
-            if self.conv_offset.bias is not None:
-                init.zeros_(self.conv_offset.bias)
-        if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
-            if self.conv_mask.bias is not None:
-                init.zeros_(self.conv_mask.bias)
+        if self.offset_generator is not None:
+            init.zeros_(self.offset_generator.weight)
+            if self.offset_generator.bias is not None:
+                init.zeros_(self.offset_generator.bias)
+        if self.mask_generator is not None:
+            init.zeros_(self.mask_generator.weight)
+            if self.mask_generator.bias is not None:
+                init.zeros_(self.mask_generator.bias)
 
     def forward(self, input: Tensor, output_size: Optional[List[int]] = None) -> Tensor:
-        if self.deformable and self.conv_offset is not None:
-            offset = self.conv_offset(input)
+        if self.deformable and self.offset_generator is not None:
+            offset = self.offset_generator(input)
             if self.offset_activation is not None:
                 offset = self.offset_activation(offset)
         else:
             offset = None
 
-        if self.modulated and self.conv_mask is not None:
-            mask = self.conv_mask(input)
+        if self.modulated and self.mask_generator is not None:
+            mask = self.mask_generator(input)
             if self.mask_activation is not None:
                 mask = self.mask_activation(mask)
         else:
             mask = None
 
         return self._conv_transpose_forward(input, self.weight, offset, mask, self.bias, output_size)
 
@@ -711,15 +713,15 @@
                  padding: Union[str, _size_2_t] = 0,
                  dilation: _size_2_t = 1,
                  output_padding: Union[str, _size_2_t] = 0,
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
-                 auxiliary_bias: bool = False,
+                 generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
                  mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
@@ -750,64 +752,65 @@
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
 
         self.deformable = deformable
         self.modulated = modulated
 
         if self.deformable:
-            self.conv_offset = nn.Conv2d(
+            self.offset_generator = nn.Conv2d(
                 self.in_channels,
                 2 * self.kernel_size[0] * self.kernel_size[1] * self.offset_groups,
                 kernel_size=1,
-                bias=auxiliary_bias,
+                groups=self.offset_groups,
+                bias=generator_bias,
                 device=dtype,
                 dtype=device)
         else:
-            self.register_module('conv_offset', None)
-        self.offset_activation = offset_activation
+            self.register_module('offset_generator', None)
 
         if self.modulated:
-            self.conv_mask = nn.Conv2d(
+            self.mask_generator = nn.Conv2d(
                 self.in_channels,
                 self.kernel_size[0] * self.kernel_size[1] * self.mask_groups,
                 kernel_size=1,
-                bias=auxiliary_bias,
+                groups=self.mask_groups,
+                bias=generator_bias,
                 device=dtype,
                 dtype=device)
         else:
-            self.register_module('conv_mask', None)
+            self.register_module('mask_generator', None)
 
         self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
-        if self.conv_offset is not None:
-            init.zeros_(self.conv_offset.weight)
-            if self.conv_offset.bias is not None:
-                init.zeros_(self.conv_offset.bias)
-        if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
-            if self.conv_mask.bias is not None:
-                init.zeros_(self.conv_mask.bias)
+        if self.offset_generator is not None:
+            init.zeros_(self.offset_generator.weight)
+            if self.offset_generator.bias is not None:
+                init.zeros_(self.offset_generator.bias)
+        if self.mask_generator is not None:
+            init.zeros_(self.mask_generator.weight)
+            if self.mask_generator.bias is not None:
+                init.zeros_(self.mask_generator.bias)
 
     def forward(self, input: Tensor, output_size: Optional[List[int]] = None) -> Tensor:
-        if self.deformable and self.conv_offset is not None:
-            offset = self.conv_offset(input)
+        if self.deformable and self.offset_generator is not None:
+            offset = self.offset_generator(input)
             if self.offset_activation is not None:
                 offset = self.offset_activation(offset)
         else:
             offset = None
 
-        if self.modulated and self.conv_mask is not None:
-            mask = self.conv_mask(input)
+        if self.modulated and self.mask_generator is not None:
+            mask = self.mask_generator(input)
             if self.mask_activation is not None:
                 mask = self.mask_activation(mask)
         else:
             mask = None
 
         return self._conv_transpose_forward(input, self.weight, offset, mask, self.bias, output_size)
 
@@ -826,15 +829,15 @@
                  padding: Union[str, _size_3_t] = 0,
                  dilation: _size_3_t = 1,
                  output_padding: Union[str, _size_3_t] = 0,
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
-                 auxiliary_bias: bool = False,
+                 generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
                  offset_activation: Union[str, _Activation] = None,
                  mask_activation: Union[str, _Activation] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
@@ -865,63 +868,64 @@
         self.offset_groups = offset_groups
         self.mask_groups = mask_groups
 
         self.deformable = deformable
         self.modulated = modulated
 
         if self.deformable:
-            self.conv_offset = nn.Conv3d(
+            self.offset_generator = nn.Conv3d(
                 self.in_channels,
                 3 * self.kernel_size[0] * self.kernel_size[1] * self.kernel_size[2] * self.offset_groups,
                 kernel_size=1,
-                bias=auxiliary_bias,
+                groups=self.offset_groups,
+                bias=generator_bias,
                 device=dtype,
                 dtype=device)
         else:
-            self.register_module('conv_offset', None)
-        self.offset_activation = offset_activation
+            self.register_module('offset_generator', None)
 
         if self.modulated:
-            self.conv_mask = nn.Conv3d(
+            self.mask_generator = nn.Conv3d(
                 self.in_channels,
                 self.kernel_size[0] * self.kernel_size[1] * self.kernel_size[2] * self.mask_groups,
                 kernel_size=1,
-                bias=auxiliary_bias,
+                groups=self.mask_groups,
+                bias=generator_bias,
                 device=dtype,
                 dtype=device)
         else:
-            self.register_module('conv_mask', None)
+            self.register_module('mask_generator', None)
 
         self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         if not hasattr(self, 'modulated'):
             return
         super().reset_parameters()
-        if self.conv_offset is not None:
-            init.zeros_(self.conv_offset.weight)
-            if self.conv_offset.bias is not None:
-                init.zeros_(self.conv_offset.bias)
-        if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
-            if self.conv_mask.bias is not None:
-                init.zeros_(self.conv_mask.bias)
+        if self.offset_generator is not None:
+            init.zeros_(self.offset_generator.weight)
+            if self.offset_generator.bias is not None:
+                init.zeros_(self.offset_generator.bias)
+        if self.mask_generator is not None:
+            init.zeros_(self.mask_generator.weight)
+            if self.mask_generator.bias is not None:
+                init.zeros_(self.mask_generator.bias)
 
     def forward(self, input: Tensor, output_size: Optional[List[int]] = None) -> Tensor:
-        if self.deformable and self.conv_offset is not None:
-            offset = self.conv_offset(input)
+        if self.deformable and self.offset_generator is not None:
+            offset = self.offset_generator(input)
             if self.offset_activation is not None:
                 offset = self.offset_activation(offset)
         else:
             offset = None
 
-        if self.modulated and self.conv_mask is not None:
-            mask = self.conv_mask(input)
+        if self.modulated and self.mask_generator is not None:
+            mask = self.mask_generator(input)
             if self.mask_activation is not None:
                 mask = self.mask_activation(mask)
         else:
             mask = None
 
         return self._conv_transpose_forward(input, self.weight, offset, mask, self.bias, output_size)
```

### Comparing `tvdcn-0.2.5/tvdcn/utils.py` & `tvdcn-0.2.6/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.5/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.2.6/tvdcn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.5
+Version: 0.2.6
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
@@ -28,17 +28,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 Provides-Extra: tests
 License-File: LICENSE.txt
 
 Torchvision+ Deformable Convolution Networks
 ========
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/inspiros/tvdcn/build_wheels.yml)
-![PyPI](https://img.shields.io/pypi/v/tvdcn)
-![GitHub](https://img.shields.io/github/license/inspiros/tvdcn)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/inspiros/tvdcn/build_wheels.yml)](https://github.com/inspiros/tvdcn/actions)
+[![PyPI](https://img.shields.io/pypi/v/tvdcn)](https://pypi.org/project/tvdcn)
+[![GitHub](https://img.shields.io/github/license/inspiros/tvdcn)](LICENSE.txt)
 
 This package contains the PyTorch implementations of the **2D Deformable Convolution** operation
 (the commonly used  `torchvision.ops.deform_conv2d`) proposed in https://arxiv.org/abs/1811.11168,
 as well as its **1D** and **3D** equivalences, which are not available in `torchvision` (thus the name).
 
 And beyond that, the package also provides the **transposed** versions of them,
 which interestingly noone has ever proposed to use.
```

### Comparing `tvdcn-0.2.5/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.2.6/tvdcn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

