# Comparing `tmp/webuiapi-0.8.0-py3-none-any.whl.zip` & `tmp/webuiapi-0.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12220 bytes, number of entries: 7
--rw-r--r--  2.0 unx      484 b- defN 23-May-21 01:52 webuiapi/__init__.py
--rw-r--r--  2.0 unx    33443 b- defN 23-May-21 01:51 webuiapi/webuiapi.py
--rw-r--r--  2.0 unx     1079 b- defN 23-May-21 01:57 webuiapi-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    12924 b- defN 23-May-21 01:57 webuiapi-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-21 01:57 webuiapi-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-21 01:57 webuiapi-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      545 b- defN 23-May-21 01:57 webuiapi-0.8.0.dist-info/RECORD
-7 files, 48576 bytes uncompressed, 11258 bytes compressed:  76.8%
+Zip file size: 12329 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      484 b- defN 23-May-21 06:47 webuiapi/__init__.py
+-rw-r--r--  2.0 unx    33972 b- defN 23-May-21 06:46 webuiapi/webuiapi.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-May-21 06:49 webuiapi-0.8.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12995 b- defN 23-May-21 06:49 webuiapi-0.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 06:49 webuiapi-0.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-21 06:49 webuiapi-0.8.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      545 b- defN 23-May-21 06:49 webuiapi-0.8.1.dist-info/RECORD
+7 files, 49176 bytes uncompressed, 11367 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webuiapi/__init__.py
 Comment: 
 
 Filename: webuiapi/webuiapi.py
 Comment: 
 
-Filename: webuiapi-0.8.0.dist-info/LICENSE
+Filename: webuiapi-0.8.1.dist-info/LICENSE
 Comment: 
 
-Filename: webuiapi-0.8.0.dist-info/METADATA
+Filename: webuiapi-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: webuiapi-0.8.0.dist-info/WHEEL
+Filename: webuiapi-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: webuiapi-0.8.0.dist-info/top_level.txt
+Filename: webuiapi-0.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: webuiapi-0.8.0.dist-info/RECORD
+Filename: webuiapi-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webuiapi/__init__.py

```diff
@@ -1,10 +1,10 @@
 from .webuiapi import WebUIApi, WebUIApiResult, Upscaler, HiResUpscaler, b64_img, raw_b64_img, ModelKeywordResult, ModelKeywordInterface, InstructPix2PixInterface, ControlNetInterface, ControlNetUnit
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 __all__ = [
     "__version__",
     "WebUIApi",
     "WebUIApiResult",
     "Upscaler",
     "HiResUpscaler",
```

## webuiapi/webuiapi.py

```diff
@@ -609,15 +609,27 @@
     def controlnet_model_list(self):
         r = self.custom_get('controlnet/model_list')
         return r['model_list']
     
     def controlnet_module_list(self):
         r = self.custom_get('controlnet/module_list')
         return r['module_list']
-    
+
+    def controlnet_detect(self, images, module="none", processor_res=512, threshold_a=64, threshold_b=64):
+        input_images = [b64_img(x) for x in images]
+        payload = {
+            "controlnet_module": module,
+            "controlnet_input_images": input_images,
+            "controlnet_processor_res": processor_res,
+            "controlnet_threshold_a": threshold_a,
+            "controlnet_threshold_b": threshold_b,
+        }
+        r = self.custom_post('controlnet/detect', payload=payload)
+        return r
+        
     def util_get_model_names(self):
         return sorted([x['title'] for x in self.get_sd_models()])
     def util_set_model(self, name, find_closest=True):
         if find_closest:
             name = name.lower()
         models = self.util_get_model_names()
         found_model = None
```

## Comparing `webuiapi-0.8.0.dist-info/LICENSE` & `webuiapi-0.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webuiapi-0.8.0.dist-info/METADATA` & `webuiapi-0.8.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webuiapi
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python API client for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/mix1009/sdwebuiapi
 Author: ChunKoo Park
 Author-email: mix1009@gmail.com
 License: MIT
 Keywords: stable-diffuion-webui,AUTOMATIC1111,stable-diffusion,api
 Requires-Python: >=3.7, <4
@@ -418,8 +418,11 @@
 
 ```
 r2.images[2]
 ```
 ![cn5](https://user-images.githubusercontent.com/1288793/222315859-e6b6286e-854d-40c1-a516-5a08c827c49a.png)
 
 
-
+```
+r = api.controlnet_detect(images=[img], module='canny')
+r.image
+```
```

