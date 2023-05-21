# Comparing `tmp/onnx2kerastl-0.0.92.tar.gz` & `tmp/onnx2kerastl-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.92.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.93.tar", max compression
```

## Comparing `onnx2kerastl-0.0.92.tar` & `onnx2kerastl-0.0.93.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1067 2022-05-24 13:45:54.506384 onnx2kerastl-0.0.92/LICENSE
--rw-r--r--   0        0        0       66 2022-05-26 14:37:02.229998 onnx2kerastl-0.0.92/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-30 14:23:13.629683 onnx2kerastl-0.0.92/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-07-21 11:24:20.166257 onnx2kerastl-0.0.92/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2022-10-13 14:52:08.546058 onnx2kerastl-0.0.92/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13572 2023-05-14 16:26:09.893812 onnx2kerastl-0.0.92/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11968 2023-05-14 16:26:09.894508 onnx2kerastl-0.0.92/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      697 2023-05-16 16:00:58.651041 onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2022-10-19 12:00:07.113921 onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-05-30 10:49:29.064709 onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0     4942 2023-05-17 13:23:53.712854 onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxgridsampler.py
--rw-r--r--   0        0        0      606 2022-05-24 13:45:54.510879 onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1730 2023-05-14 16:26:09.897336 onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2022-08-04 16:14:29.703956 onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-05-30 11:45:55.347781 onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9372 2023-04-30 14:23:13.630051 onnx2kerastl-0.0.92/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-07-21 11:24:20.167508 onnx2kerastl-0.0.92/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3867 2023-04-30 14:23:13.630361 onnx2kerastl-0.0.92/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-04-02 11:17:38.561077 onnx2kerastl-0.0.92/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3791 2023-05-14 16:26:09.898000 onnx2kerastl-0.0.92/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-05-24 13:45:54.512524 onnx2kerastl-0.0.92/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-14 16:26:09.898639 onnx2kerastl-0.0.92/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15619 2023-04-30 14:23:13.630719 onnx2kerastl-0.0.92/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-04-30 14:23:13.631034 onnx2kerastl-0.0.92/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-04-02 11:17:38.563036 onnx2kerastl-0.0.92/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    17943 2023-05-14 16:26:09.900619 onnx2kerastl-0.0.92/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     4965 2023-05-16 15:44:21.797652 onnx2kerastl-0.0.92/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-04-02 11:17:38.563943 onnx2kerastl-0.0.92/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-04-02 11:17:38.564336 onnx2kerastl-0.0.92/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1030 2023-05-17 13:25:09.107932 onnx2kerastl-0.0.92/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.92/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-05-24 13:45:54.506384 onnx2kerastl-0.0.93/LICENSE
+-rw-r--r--   0        0        0       66 2022-05-26 14:37:02.229998 onnx2kerastl-0.0.93/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-30 14:23:13.629683 onnx2kerastl-0.0.93/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-07-21 11:24:20.166257 onnx2kerastl-0.0.93/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2022-10-13 14:52:08.546058 onnx2kerastl-0.0.93/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13572 2023-05-14 16:26:09.893812 onnx2kerastl-0.0.93/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-14 16:26:09.894508 onnx2kerastl-0.0.93/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      697 2023-05-16 16:00:58.651041 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2022-10-19 12:00:07.113921 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-05-30 10:49:29.064709 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0     4950 2023-05-17 13:31:53.385365 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxgridsampler.py
+-rw-r--r--   0        0        0      606 2022-05-24 13:45:54.510879 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1730 2023-05-14 16:26:09.897336 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2022-08-04 16:14:29.703956 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-05-30 11:45:55.347781 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9372 2023-04-30 14:23:13.630051 onnx2kerastl-0.0.93/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-07-21 11:24:20.167508 onnx2kerastl-0.0.93/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-04-30 14:23:13.630361 onnx2kerastl-0.0.93/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-04-02 11:17:38.561077 onnx2kerastl-0.0.93/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3791 2023-05-14 16:26:09.898000 onnx2kerastl-0.0.93/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-05-24 13:45:54.512524 onnx2kerastl-0.0.93/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-14 16:26:09.898639 onnx2kerastl-0.0.93/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15619 2023-04-30 14:23:13.630719 onnx2kerastl-0.0.93/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-30 14:23:13.631034 onnx2kerastl-0.0.93/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-04-02 11:17:38.563036 onnx2kerastl-0.0.93/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    17943 2023-05-14 16:26:09.900619 onnx2kerastl-0.0.93/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     4965 2023-05-16 15:44:21.797652 onnx2kerastl-0.0.93/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-04-02 11:17:38.563943 onnx2kerastl-0.0.93/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-04-02 11:17:38.564336 onnx2kerastl-0.0.93/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1030 2023-05-17 13:32:39.118919 onnx2kerastl-0.0.93/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.93/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.92/LICENSE` & `onnx2kerastl-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.93/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxgridsampler.py` & `onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxgridsampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from keras.layers import Layer
 import tensorflow as tf
 
 
 class OnnxGridSampler(Layer):
     """
 Args:
-sample_grid: tuple
-**kwargs:
+    sample_grid: tuple
+    **kwargs:
 """
     def __init__(self, sample_grid: List[int], **kwargs):
         super().__init__(**kwargs)
         self.sample_grid = sample_grid
 
     def get_config(self):
         config = super().get_config()
```

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/reshape_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/sampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.93/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.93/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.92/pyproject.toml` & `onnx2kerastl-0.0.93/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.92"
+version = "0.0.93"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.92/PKG-INFO` & `onnx2kerastl-0.0.93/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.92
+Version: 0.0.93
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

