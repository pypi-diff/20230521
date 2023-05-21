# Comparing `tmp/ElectronCounting-0.1.6.tar.gz` & `tmp/ElectronCounting-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElectronCounting-0.1.6.tar", last modified: Tue Jan 10 22:29:43 2023, max compression
+gzip compressed data, was "ElectronCounting-1.0.0.tar", last modified: Sun May 21 17:20:36 2023, max compression
```

## Comparing `ElectronCounting-0.1.6.tar` & `ElectronCounting-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-01-10 22:29:43.308468 ElectronCounting-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-01-10 22:29:43.308468 ElectronCounting-0.1.6/CountingNN/
--rw-rw-rw-   0        0        0      103 2022-12-02 18:22:40.000000 ElectronCounting-0.1.6/CountingNN/__init__.py
--rw-rw-rw-   0        0        0    12935 2022-11-20 21:15:39.000000 ElectronCounting-0.1.6/CountingNN/anchor_custom.py
--rw-rw-rw-   0        0        0    15909 2022-10-18 15:22:16.000000 ElectronCounting-0.1.6/CountingNN/blocks.py
--rw-rw-rw-   0        0        0     4140 2022-11-21 18:07:17.000000 ElectronCounting-0.1.6/CountingNN/dataset.py
--rw-rw-rw-   0        0        0    15903 2022-12-02 18:22:40.000000 ElectronCounting-0.1.6/CountingNN/faster_rcnn_custom.py
--rw-rw-rw-   0        0        0     4106 2022-12-02 18:22:40.000000 ElectronCounting-0.1.6/CountingNN/fcn.py
--rw-rw-rw-   0        0        0     4829 2022-11-21 15:50:24.000000 ElectronCounting-0.1.6/CountingNN/generalized_rcnn_custom.py
--rw-rw-rw-   0        0        0    13776 2022-12-23 21:42:27.000000 ElectronCounting-0.1.6/CountingNN/locator.py
--rw-rw-rw-   0        0        0    10443 2022-12-09 17:38:53.000000 ElectronCounting-0.1.6/CountingNN/locator_archive.py
--rw-rw-rw-   0        0        0    10775 2022-12-02 18:22:40.000000 ElectronCounting-0.1.6/CountingNN/model.py
-drwxrwxrwx   0        0        0        0 2023-01-10 22:29:43.308468 ElectronCounting-0.1.6/CountingNN/modelweights/
--rw-rw-rw-   0        0        0        0 2023-01-10 21:51:23.000000 ElectronCounting-0.1.6/CountingNN/modelweights/__init__.py
--rw-rw-rw-   0        0        0    37856 2022-10-18 17:41:53.000000 ElectronCounting-0.1.6/CountingNN/roi_heads_custom.py
--rw-rw-rw-   0        0        0    20409 2022-12-02 18:22:40.000000 ElectronCounting-0.1.6/CountingNN/rpn_custom.py
--rw-rw-rw-   0        0        0     8016 2022-12-02 18:22:40.000000 ElectronCounting-0.1.6/CountingNN/train.py
--rw-rw-rw-   0        0        0     3158 2022-11-21 19:09:25.000000 ElectronCounting-0.1.6/CountingNN/transform_custom.py
--rw-rw-rw-   0        0        0     5899 2022-10-13 20:14:29.000000 ElectronCounting-0.1.6/CountingNN/validator.py
-drwxrwxrwx   0        0        0        0 2023-01-10 22:29:43.308468 ElectronCounting-0.1.6/ElectronCounting.egg-info/
--rw-rw-rw-   0        0        0      354 2023-01-10 22:29:43.000000 ElectronCounting-0.1.6/ElectronCounting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      649 2023-01-10 22:29:43.000000 ElectronCounting-0.1.6/ElectronCounting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-10 22:29:43.000000 ElectronCounting-0.1.6/ElectronCounting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-01-10 22:29:43.000000 ElectronCounting-0.1.6/ElectronCounting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-10 22:29:43.000000 ElectronCounting-0.1.6/ElectronCounting.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      354 2023-01-10 22:29:43.308468 ElectronCounting-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      235 2022-12-09 00:01:48.000000 ElectronCounting-0.1.6/README.md
--rw-rw-rw-   0        0        0       86 2023-01-10 22:29:43.316714 ElectronCounting-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      775 2023-01-10 22:28:33.000000 ElectronCounting-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:20:36.589126 ElectronCounting-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-05-21 17:20:36.504157 ElectronCounting-1.0.0/CountingNN/
+-rw-rw-rw-   0        0        0      103 2022-12-02 18:22:40.000000 ElectronCounting-1.0.0/CountingNN/__init__.py
+-rw-rw-rw-   0        0        0    12935 2022-11-20 21:15:39.000000 ElectronCounting-1.0.0/CountingNN/anchor_custom.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:20:36.582842 ElectronCounting-1.0.0/CountingNN/archive/
+-rw-rw-rw-   0        0        0        0 2023-04-02 20:02:43.000000 ElectronCounting-1.0.0/CountingNN/archive/__init__.py
+-rw-rw-rw-   0        0        0     5115 2022-08-12 18:15:27.000000 ElectronCounting-1.0.0/CountingNN/archive/box_ops.py
+-rw-rw-rw-   0        0        0     2060 2022-08-05 18:55:47.000000 ElectronCounting-1.0.0/CountingNN/archive/gpu.py
+-rw-rw-rw-   0        0        0    11156 2022-12-02 18:27:40.000000 ElectronCounting-1.0.0/CountingNN/archive/mask_rcnn.py
+-rw-rw-rw-   0        0        0     2036 2022-12-02 18:27:40.000000 ElectronCounting-1.0.0/CountingNN/archive/pooler.py
+-rw-rw-rw-   0        0        0     7777 2022-12-02 18:27:40.000000 ElectronCounting-1.0.0/CountingNN/archive/roi_heads.py
+-rw-rw-rw-   0        0        0     4180 2022-12-02 18:27:40.000000 ElectronCounting-1.0.0/CountingNN/archive/rpn.py
+-rw-rw-rw-   0        0        0    13185 2022-12-02 18:22:40.000000 ElectronCounting-1.0.0/CountingNN/archive/train_archive.py
+-rw-rw-rw-   0        0        0     8682 2022-08-13 22:32:20.000000 ElectronCounting-1.0.0/CountingNN/archive/transform.py
+-rw-rw-rw-   0        0        0     4668 2022-08-12 15:35:51.000000 ElectronCounting-1.0.0/CountingNN/archive/utils.py
+-rw-rw-rw-   0        0        0    15909 2022-10-18 15:22:16.000000 ElectronCounting-1.0.0/CountingNN/blocks.py
+-rw-rw-rw-   0        0        0     4140 2022-11-21 18:07:17.000000 ElectronCounting-1.0.0/CountingNN/dataset.py
+-rw-rw-rw-   0        0        0    15903 2022-12-02 18:22:40.000000 ElectronCounting-1.0.0/CountingNN/faster_rcnn_custom.py
+-rw-rw-rw-   0        0        0     4106 2022-12-02 18:22:40.000000 ElectronCounting-1.0.0/CountingNN/fcn.py
+-rw-rw-rw-   0        0        0     4829 2022-11-21 15:50:24.000000 ElectronCounting-1.0.0/CountingNN/generalized_rcnn_custom.py
+-rw-rw-rw-   0        0        0    17975 2023-05-13 23:39:42.000000 ElectronCounting-1.0.0/CountingNN/locator.py
+-rw-rw-rw-   0        0        0    10443 2023-05-13 16:59:05.000000 ElectronCounting-1.0.0/CountingNN/locator_archive.py
+-rw-rw-rw-   0        0        0    10775 2022-12-02 18:22:40.000000 ElectronCounting-1.0.0/CountingNN/model.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:20:36.584938 ElectronCounting-1.0.0/CountingNN/modelweights/
+-rw-rw-rw-   0        0        0        0 2023-01-10 21:51:23.000000 ElectronCounting-1.0.0/CountingNN/modelweights/__init__.py
+-rw-rw-rw-   0        0        0    37856 2022-10-18 17:41:53.000000 ElectronCounting-1.0.0/CountingNN/roi_heads_custom.py
+-rw-rw-rw-   0        0        0    20409 2022-12-02 18:22:40.000000 ElectronCounting-1.0.0/CountingNN/rpn_custom.py
+-rw-rw-rw-   0        0        0     8016 2022-12-02 18:22:40.000000 ElectronCounting-1.0.0/CountingNN/train.py
+-rw-rw-rw-   0        0        0     3158 2022-11-21 19:09:25.000000 ElectronCounting-1.0.0/CountingNN/transform_custom.py
+-rw-rw-rw-   0        0        0     5899 2022-10-13 20:14:29.000000 ElectronCounting-1.0.0/CountingNN/validator.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:20:36.589126 ElectronCounting-1.0.0/ElectronCounting.egg-info/
+-rw-rw-rw-   0        0        0      354 2023-05-21 17:20:36.000000 ElectronCounting-1.0.0/ElectronCounting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-05-21 17:20:36.000000 ElectronCounting-1.0.0/ElectronCounting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 17:20:36.000000 ElectronCounting-1.0.0/ElectronCounting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-21 17:20:36.000000 ElectronCounting-1.0.0/ElectronCounting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-21 17:20:36.000000 ElectronCounting-1.0.0/ElectronCounting.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      354 2023-05-21 17:20:36.589126 ElectronCounting-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-05-13 23:39:51.000000 ElectronCounting-1.0.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-21 17:20:36.589126 ElectronCounting-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      781 2023-05-13 23:42:13.000000 ElectronCounting-1.0.0/setup.py
```

### Comparing `ElectronCounting-0.1.6/CountingNN/anchor_custom.py` & `ElectronCounting-1.0.0/CountingNN/anchor_custom.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/blocks.py` & `ElectronCounting-1.0.0/CountingNN/blocks.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/dataset.py` & `ElectronCounting-1.0.0/CountingNN/dataset.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/faster_rcnn_custom.py` & `ElectronCounting-1.0.0/CountingNN/faster_rcnn_custom.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/fcn.py` & `ElectronCounting-1.0.0/CountingNN/fcn.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/generalized_rcnn_custom.py` & `ElectronCounting-1.0.0/CountingNN/generalized_rcnn_custom.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/locator.py` & `ElectronCounting-1.0.0/CountingNN/locator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-import kornia
+# import kornia
 import torch
 import torch.nn.functional as F
 
 
 def map01(mat):
     return (mat - mat.min()) / (mat.max() - mat.min())
 
@@ -38,14 +38,68 @@
                          [windows[-1, -1][k:, k:]], dim=1)
 
     final = torch.cat([row0] + rows + [row_last], dim=0)
     final = final[:cropx, :cropy]
     return final
 
 
+def connected_components(image: torch.Tensor, num_iterations: int = 100) -> torch.Tensor:
+    r"""Computes the Connected-component labelling (CCL) algorithm.
+
+    .. image:: https://github.com/kornia/data/raw/main/cells_segmented.png
+
+    The implementation is an adaptation of the following repository:
+
+    https://gist.github.com/efirdc/5d8bd66859e574c683a504a4690ae8bc
+
+    .. warning::
+        This is an experimental API subject to changes and optimization improvements.
+
+    .. note::
+       See a working example `here <https://kornia-tutorials.readthedocs.io/en/latest/
+       connected_components.html>`__.
+
+    Args:
+        image: the binarized input image with shape :math:`(*, 1, H, W)`.
+          The image must be in floating point with range [0, 1].
+        num_iterations: the number of iterations to make the algorithm to converge.
+
+    Return:
+        The labels image with the same shape of the input image.
+
+    Example:
+        >>> img = torch.rand(2, 1, 4, 5)
+        >>> img_labels = connected_components(img, num_iterations=100)
+    """
+    if not isinstance(image, torch.Tensor):
+        raise TypeError(f"Input imagetype is not a torch.Tensor. Got: {type(image)}")
+
+    if not isinstance(num_iterations, int) or num_iterations < 1:
+        raise TypeError("Input num_iterations must be a positive integer.")
+
+    if len(image.shape) < 3 or image.shape[-3] != 1:
+        raise ValueError(f"Input image shape must be (*,1,H,W). Got: {image.shape}")
+
+    H, W = image.shape[-2:]
+    image_view = image.view(-1, 1, H, W)
+
+    # precompute a mask with the valid values
+    mask = image_view == 1
+
+    # allocate the output tensors for labels
+    B, _, _, _ = image_view.shape
+    out = torch.arange(B * H * W, device=image.device, dtype=image.dtype).view((-1, 1, H, W))
+    out[~mask] = 0
+
+    for _ in range(num_iterations):
+        out[mask] = F.max_pool2d(out, kernel_size=3, stride=1, padding=1)[mask]
+
+    return out.view_as(image)
+
+
 class Locator:
     """
     Implements Faster R-CNN on a single image to detect boxes for electron events,
     then use finding maximum or pre-trained FCN to assign the entry positions
     The grid_predict and predict function works for image stack, but the locate is set to work for single image.
     Returns boxes as xmin, ymin, xmax,  ymax, x means horizontal and y means vertical.
 
@@ -59,14 +113,16 @@
         locating_model: the loaded fcn model for assigning entry position
         mode: dynamic mode, whether apply model tune for images with different electron density.
         'static': static parameters, same threshold, no model tune
         'dynamic_window': apply model tune separately for each window
         'dynamic_frame': apply model tune equally the whole frame based on whole frame intensity.
         p_list: optional list of five multiplier for model tune, if none, will use default numbers: [6, 6, 1.3, 1.5, 23]
         meanADU: optional float for mean intensity per electron (ADU), if none, will use default 241 for 200kV.
+        dynamic_thres: optional bool for wheather lift the threshold above some density within modeltune.
+        pretune_thresholding: optional threshold for reset noise pixels before model tune.
     Example::
 
         >>>from CountingNN.locator import Locator
         >>>counting = Locator(model_object, device, process_stride, method,
         >>>dark_threshold, locating_model, dynamic_param, p_list = p_list, meanADU=meanADU)
         >>>filtered = counting.predict_sequence(inputs)  # inputs as the image tensor in shape [N,h,w]
 
@@ -84,39 +140,53 @@
         self.dark_threshold = dark_threshold
         self.p_list = kwargs.get('p_list')
         if self.p_list is None:
             self.p_list = [8, 6, 1.5, 1, 50]
         self.meanADU = kwargs.get('meanADU')
         if self.meanADU is None:
             self.meanADU = 241.0
-
+        self.dynamic_thres = kwargs.get('dynamic_thres')
+        self.pretune_thresholding = kwargs.get('pretune_thresholding')
+        if self.dynamic_thres is None:
+            self.dynamic_thres = True
         self.fastrcnn_model = self.fastrcnn_model.to(self.device)
 
     def model_tune(self, arr):
         """
         Change the detection limits and thresholds of Fast R-CNN model by estimating the image sparsity
         """
         meanADU = self.meanADU * 4  # mean ADU * upsample_factor^2
         offset = 0
         # fit from 200kV Validation data, between a 64x64
         # up-sampled-by-2 image cell ans its original ground truth.
         limit = int(arr.sum() / meanADU + offset)
         arr_t = torch.as_tensor(arr[None, None, ...] > 30, dtype=torch.float32)
-        limit_cca = kornia.contrib.connected_components(arr_t, num_iterations=10)
+        limit_cca = connected_components(arr_t, num_iterations=10)
         limit = max(torch.unique(limit_cca).shape[0], limit)
-        if limit < 1:  # make the minimum limit as 1.
-            limit = 1
+        limit = max(limit, 1)
+
+        # if limit > (0.035 * 2 * arr.shape[0] * arr.shape[1]):  # no pre-tune thresholding if density beyond 3%
+        #     self.pretune_thresholding = None
+        #
+        # if self.pretune_thresholding is not None:  # recalculate the limit after thresholding
+        #     arr[arr < self.pretune_thresholding] = 0
+        #     limit = int(arr.sum() / meanADU + offset)
+        #     limit = max(torch.unique(limit_cca).shape[0], limit)
+        #     limit = max(limit, 1)
+
         self.fastrcnn_model.rpn._pre_nms_top_n = {'training': limit * self.p_list[0], 'testing': limit * self.p_list[0]}
         self.fastrcnn_model.rpn._post_nms_top_n = {'training': limit * self.p_list[1],
                                                    'testing': limit * self.p_list[1]}
         self.fastrcnn_model.roi_heads.detections_per_img = int(limit * self.p_list[2])
-        self.fastrcnn_model.roi_heads.score_thresh = self.p_list[3] / limit if limit < self.p_list[4] else 0
+        # self.fastrcnn_model.roi_heads.score_thresh = self.p_list[3] / limit if limit < self.p_list[4] else 0
+        self.fastrcnn_model.roi_heads.score_thresh = self.p_list[3] / limit
+
         self.fastrcnn_model.roi_heads.nms_thresh = 0.02  # smaller, delete more detections
 
-        if limit > (0.005 * arr.shape[0] * arr.shape[1]):  # 0.002 is minimum for model13
+        if limit > (0.005 * arr.shape[0] * arr.shape[1]) and self.dynamic_thres:  # 0.002 is minimum for model13
             self.dark_threshold = 0  # for image that not quite sparse, lift the pre-thresholding.
 
     def images_to_window_lists(self, inputs: torch.tensor) -> List[torch.tensor]:
         """
         transform a batch of images(3D tensor) into windows of the images, with up-sampling by 2.
         if stride = None, not spliting and return whole images.
         """
@@ -163,44 +233,43 @@
 
     @torch.no_grad()
     def predict_sequence(self, inputs: torch.tensor):
         """
         apply model on image one patch after another. The patches size equals the image size in training data, so that
         no need to tune the model detection limits for different limit sizes.
         """
-        self.fastrcnn_model.transform.crop_max = max(inputs.shape[1], inputs.shape[2])*2
+        self.fastrcnn_model.transform.crop_max = max(inputs.shape[1], inputs.shape[2]) * 2
         # make size_divisible equals process_stride here to avoid inconsistent padding issue.
         # self.fastrcnn_model.transform.size_divisible = self.process_stride * 2
         self.fastrcnn_model.eval()
 
         counted_list = []
         eventsize_all = []
         inputs = torch.as_tensor(inputs, dtype=torch.float32)
         counted_images = torch.zeros_like(inputs)
 
         image_cell_list, windowshape, maxs, mins = self.images_to_window_lists(inputs)
         for i, image_cell in enumerate(image_cell_list):
 
-
-            if self.mode =='dynamic_window':
+            if self.mode == 'dynamic_window':
                 self.model_tune(image_cell)
-            elif self.mode =='dynamic_frame':
-                image_i = torch.div(i,  windowshape[0] * windowshape[1], rounding_mode='floor')
+            elif self.mode == 'dynamic_frame':  # incorrect
+                image_i = torch.div(i, windowshape[0] * windowshape[1], rounding_mode='floor')
                 self.model_tune(torch.nn.Upsample(scale_factor=2, mode='nearest')(inputs[image_i][None, None, ...]))
             elif self.mode == 'static':
-                torch._assert(self.process_stride==64,
+                torch._assert(self.process_stride == 64,
                               f"please use process_stride=64 for static mode."
                               )
                 pass
             else:
                 raise ValueError("Use mode = 'dynamic_window', dynamic_frame or 'static'. ")
-                
+
             # thresholding to remove dark noise before applying the model
             image_cell[image_cell < self.dark_threshold] = 0
-            
+
             image_cell_ori = image_cell
 
             image_cell = (image_cell - mins[i]) / (maxs[i] - mins[i])  # norm the image cells equally
             # boxes = self.fastrcnn_model([image_cell[None, ...]])[0]['boxes']
             boxes = self.fastrcnn_model(image_cell[None, None, ...])[0]['boxes']  # model direct input [N, C, H, W]
 
             select = []
@@ -251,23 +320,43 @@
                 patch = patch[:(width + 2), :(width + 2)]
             else:
                 patch = F.pad(xarea, (1, (width - xarea.shape[1] + 1), 1, (width - xarea.shape[0] + 1)))
 
             if self.method == 'max':
 
                 (model_x, model_y) = unravel_index(torch.argmax(patch), shape=(width + 2, width + 2))
-
+            elif self.method == 'binary_com':
+                patch[patch < 30] = 0
+                patch[patch >= 30] = 1
+                x = torch.linspace(0, patch.shape[0] - 1, patch.shape[0])
+                y = torch.linspace(0, patch.shape[1] - 1, patch.shape[1])
+                weights_x, weights_y = torch.meshgrid(x, y)
+                model_x = (patch * weights_x).sum() / patch.sum()
+                model_y = (patch * weights_y).sum() / patch.sum()
+                model_x = int(torch.round(model_x))
+                model_y = int(torch.round(model_y))
+            elif self.method == 'com':
+                x = torch.linspace(0, patch.shape[0] - 1, patch.shape[0])
+                y = torch.linspace(0, patch.shape[1] - 1, patch.shape[1])
+                weights_x, weights_y = torch.meshgrid(x, y)
+                model_x = (patch * weights_x).sum() / patch.sum()
+                model_y = (patch * weights_y).sum() / patch.sum()
+                model_x = int(torch.round(model_x))
+                model_y = int(torch.round(model_y))
             else:
-                raise ValueError("Use 'max' to locate the entry position. ")
+                raise ValueError("Use 'max','com,'binary_com' to locate the entry position. ")
 
             cx = model_x + box[1] - 1
             cy = model_y + box[0] - 1
             if cx > (image_array.shape[0] - 1) or cy > (image_array.shape[1] - 1) or cx < 0 or cy < 0:
                 continue
             coor.append((cx, cy))
             eventsize.append((torch.sum(patch > 20)).item())
 
         coords = torch.as_tensor(coor, dtype=torch.long).to(self.device)
         # eventsize = torch.as_tensor(eventsize, dtype=torch.long).to(self.device)
         if coords.shape[0]:
-            filtered[coords[:, 0], coords[:, 1]] = 1
+            # filtered[coords[:, 0], coords[:, 1]] = 1 # this does not account for >1 e on single pixel.
+            for point in coords:
+                filtered[point[0], point[1]] = filtered[point[0], point[1]] + 1
+
         return filtered, coords, eventsize
```

### Comparing `ElectronCounting-0.1.6/CountingNN/locator_archive.py` & `ElectronCounting-1.0.0/CountingNN/locator_archive.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/model.py` & `ElectronCounting-1.0.0/CountingNN/model.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/roi_heads_custom.py` & `ElectronCounting-1.0.0/CountingNN/roi_heads_custom.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/rpn_custom.py` & `ElectronCounting-1.0.0/CountingNN/rpn_custom.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/train.py` & `ElectronCounting-1.0.0/CountingNN/train.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/transform_custom.py` & `ElectronCounting-1.0.0/CountingNN/transform_custom.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/CountingNN/validator.py` & `ElectronCounting-1.0.0/CountingNN/validator.py`

 * *Files identical despite different names*

### Comparing `ElectronCounting-0.1.6/setup.py` & `ElectronCounting-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 # from distutils.core import setup
 
 setup(
     name='ElectronCounting',
-    version='0.1.6',
+    version='1.0.0',
     packages=find_packages(),
     url='https://github.com/wdwzyyg/ElectronCounting.git',
     license='MIT',
     author='Jingrui Wei',
     author_email='jwei74@wisc.edu',
     description='Count single electron in direct electron detector data',
     keywords=[
@@ -17,13 +17,13 @@
         "object detection",
         "Faster R-CNN",
     ],
     install_requires=[
         "torch==1.12.0",
         "torchvision==0.13.0",
         "numpy>=1.20.1",
-        "scikit-learn>=1.0.2",
-        "matplotlib>=3.2.2",
-        "kornia>=0.6.9",
+        # "scikit-learn>=1.0.2",
+        # "matplotlib>=3.2.2",
+        # "kornia>=0.6.9",
     ],
 
 )
```

