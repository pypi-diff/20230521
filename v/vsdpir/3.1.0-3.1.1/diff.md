# Comparing `tmp/vsdpir-3.1.0-py3-none-any.whl.zip` & `tmp/vsdpir-3.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13151 bytes, number of entries: 12
+Zip file size: 13155 bytes, number of entries: 12
 -rw-r--r--  2.0 fat    12297 b- defN 20-Feb-02 00:00 vsdpir/__init__.py
--rw-r--r--  2.0 fat      912 b- defN 20-Feb-02 00:00 vsdpir/__main__.py
+-rw-r--r--  2.0 fat      922 b- defN 20-Feb-02 00:00 vsdpir/__main__.py
 -rw-r--r--  2.0 fat    21548 b- defN 20-Feb-02 00:00 vsdpir/basicblock.py
 -rw-r--r--  2.0 fat     2757 b- defN 20-Feb-02 00:00 vsdpir/network_unet.py
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_color.pth
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_deblocking_color.pth
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_deblocking_gray.pth
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_gray.pth
-?rw-r--r--  2.0 fat     3100 b- defN 20-Feb-02 00:00 vsdpir-3.1.0.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 vsdpir-3.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1089 b- defN 20-Feb-02 00:00 vsdpir-3.1.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat      962 b- defN 20-Feb-02 00:00 vsdpir-3.1.0.dist-info/RECORD
-12 files, 42752 bytes uncompressed, 11527 bytes compressed:  73.0%
+?rw-r--r--  2.0 fat     3100 b- defN 20-Feb-02 00:00 vsdpir-3.1.1.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 vsdpir-3.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1089 b- defN 20-Feb-02 00:00 vsdpir-3.1.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat      962 b- defN 20-Feb-02 00:00 vsdpir-3.1.1.dist-info/RECORD
+12 files, 42762 bytes uncompressed, 11531 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: vsdpir/models/drunet_deblocking_gray.pth
 Comment: 
 
 Filename: vsdpir/models/drunet_gray.pth
 Comment: 
 
-Filename: vsdpir-3.1.0.dist-info/METADATA
+Filename: vsdpir-3.1.1.dist-info/METADATA
 Comment: 
 
-Filename: vsdpir-3.1.0.dist-info/WHEEL
+Filename: vsdpir-3.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: vsdpir-3.1.0.dist-info/licenses/LICENSE
+Filename: vsdpir-3.1.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: vsdpir-3.1.0.dist-info/RECORD
+Filename: vsdpir-3.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vsdpir/__init__.py

```diff
@@ -12,15 +12,15 @@
 from torch_tensorrt.fx import LowerSetting
 from torch_tensorrt.fx.lower import Lowerer
 from torch_tensorrt.fx.utils import LowerPrecision
 from vstools import check_variable, fallback, vs
 
 from .network_unet import UNetRes
 
-__version__ = "3.1.0"
+__version__ = "3.1.1"
 
 os.environ["CUDA_MODULE_LOADING"] = "LAZY"
 
 model_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "models")
 
 
 class Backend:
```

## vsdpir/__main__.py

```diff
@@ -3,15 +3,15 @@
 import requests
 from tqdm import tqdm
 
 
 def download_model(url: str) -> None:
     filename = url.split("/")[-1]
     r = requests.get(url, stream=True)
-    with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), filename), "wb") as f:
+    with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), "models", filename), "wb") as f:
         with tqdm(
             unit="B",
             unit_scale=True,
             unit_divisor=1024,
             miniters=1,
             desc=filename,
             total=int(r.headers.get("content-length", 0)),
```

## Comparing `vsdpir-3.1.0.dist-info/METADATA` & `vsdpir-3.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdpir
-Version: 3.1.0
+Version: 3.1.1
 Summary: DPIR function for VapourSynth
 Project-URL: Homepage, https://github.com/HolyWu/vs-dpir
 Project-URL: Bug Tracker, https://github.com/HolyWu/vs-dpir/issues
 Author-email: HolyWu <holywu@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2023 HolyWu
```

## Comparing `vsdpir-3.1.0.dist-info/licenses/LICENSE` & `vsdpir-3.1.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `vsdpir-3.1.0.dist-info/RECORD` & `vsdpir-3.1.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-vsdpir/__init__.py,sha256=EmxC5LFDgCsdC3OTCrNQyGeckm0hdDXBzBtAXxIh25A,12297
-vsdpir/__main__.py,sha256=2t6FJP1a3X8Ut4czODKF0qV9bUIHV_tT2FGS88ZE83E,912
+vsdpir/__init__.py,sha256=ht4KP1FQK-uKWYLvrXHewRzhPZ7T1s2uepBaTOtQ5eA,12297
+vsdpir/__main__.py,sha256=YC0lk6_VwvF8PwUCOwEXF_c0zQ1Zh_x03EFjXr8vUOU,922
 vsdpir/basicblock.py,sha256=JgSHEeEWi4t2x1ZlDzjbQA2PH5gSECaN83ql0cN3Ptw,21548
 vsdpir/network_unet.py,sha256=4WzY7UAmfMlhYazd-tfeOOIz_mktNcU_OL4ZrgTJoY8,2757
 vsdpir/models/drunet_color.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsdpir/models/drunet_deblocking_color.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsdpir/models/drunet_deblocking_gray.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsdpir/models/drunet_gray.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vsdpir-3.1.0.dist-info/METADATA,sha256=-p6-1hg8Y-axgtN71B4RR16oiEHfRs569l3_8Ir9VZA,3100
-vsdpir-3.1.0.dist-info/WHEEL,sha256=y1bSCq4r5i4nMmpXeUJMqs3ipKvkZObrIXSvJHm1qCI,87
-vsdpir-3.1.0.dist-info/licenses/LICENSE,sha256=cgEoXz2kbESametJVH_uTy_eWfVY2ZCwfL6SOyI63bM,1089
-vsdpir-3.1.0.dist-info/RECORD,,
+vsdpir-3.1.1.dist-info/METADATA,sha256=zVFrxvOIdFXuHKSaXbORhFN80Vkq7KWmN6c_qQwr-8c,3100
+vsdpir-3.1.1.dist-info/WHEEL,sha256=y1bSCq4r5i4nMmpXeUJMqs3ipKvkZObrIXSvJHm1qCI,87
+vsdpir-3.1.1.dist-info/licenses/LICENSE,sha256=cgEoXz2kbESametJVH_uTy_eWfVY2ZCwfL6SOyI63bM,1089
+vsdpir-3.1.1.dist-info/RECORD,,
```

