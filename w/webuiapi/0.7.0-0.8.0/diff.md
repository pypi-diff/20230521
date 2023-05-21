# Comparing `tmp/webuiapi-0.7.0-py3-none-any.whl.zip` & `tmp/webuiapi-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 11970 bytes, number of entries: 7
--rw-r--r--  2.0 unx      484 b- defN 23-May-09 15:10 webuiapi/__init__.py
--rw-r--r--  2.0 unx    32110 b- defN 23-May-09 15:09 webuiapi/webuiapi.py
--rw-r--r--  2.0 unx     1079 b- defN 23-May-09 15:17 webuiapi-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    12778 b- defN 23-May-09 15:17 webuiapi-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 15:17 webuiapi-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-09 15:17 webuiapi-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      545 b- defN 23-May-09 15:17 webuiapi-0.7.0.dist-info/RECORD
-7 files, 47097 bytes uncompressed, 11008 bytes compressed:  76.6%
+Zip file size: 12220 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      484 b- defN 23-May-21 01:52 webuiapi/__init__.py
+-rw-r--r--  2.0 unx    33443 b- defN 23-May-21 01:51 webuiapi/webuiapi.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-May-21 01:57 webuiapi-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12924 b- defN 23-May-21 01:57 webuiapi-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 01:57 webuiapi-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-21 01:57 webuiapi-0.8.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      545 b- defN 23-May-21 01:57 webuiapi-0.8.0.dist-info/RECORD
+7 files, 48576 bytes uncompressed, 11258 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webuiapi/__init__.py
 Comment: 
 
 Filename: webuiapi/webuiapi.py
 Comment: 
 
-Filename: webuiapi-0.7.0.dist-info/LICENSE
+Filename: webuiapi-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: webuiapi-0.7.0.dist-info/METADATA
+Filename: webuiapi-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: webuiapi-0.7.0.dist-info/WHEEL
+Filename: webuiapi-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: webuiapi-0.7.0.dist-info/top_level.txt
+Filename: webuiapi-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: webuiapi-0.7.0.dist-info/RECORD
+Filename: webuiapi-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webuiapi/__init__.py

```diff
@@ -1,10 +1,10 @@
 from .webuiapi import WebUIApi, WebUIApiResult, Upscaler, HiResUpscaler, b64_img, raw_b64_img, ModelKeywordResult, ModelKeywordInterface, InstructPix2PixInterface, ControlNetInterface, ControlNetUnit
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 __all__ = [
     "__version__",
     "WebUIApi",
     "WebUIApiResult",
     "Upscaler",
     "HiResUpscaler",
```

## webuiapi/webuiapi.py

```diff
@@ -114,14 +114,17 @@
     # XXX controlnet only accepts RAW base64 without headers
     buffered = io.BytesIO()
     image.save(buffered, format="PNG")
     img_base64 = str(base64.b64encode(buffered.getvalue()), 'utf-8')
     return img_base64
 
 class WebUIApi:
+
+    has_controlnet = False
+
     def __init__(self,
                  host='127.0.0.1',
                  port=7860,
                  baseurl=None,
                  sampler='Euler a',
                  steps=20,
                  use_https=False):
@@ -133,14 +136,23 @@
 
         self.baseurl = baseurl
         self.default_sampler = sampler
         self.default_steps = steps
 
         self.session = requests.Session()
 
+        self.check_controlnet()
+
+    def check_controlnet(self):
+        try:
+            scripts = self.get_scripts()
+            self.has_controlnet = 'controlnet m2m' in scripts['txt2img']
+        except:
+            pass
+
     def set_auth(self, username, password):
         self.session.auth = (username, password)
 
     def _to_api_result(self, response):
 
         if response.status_code != 200:
             raise RuntimeError(response.status_code, response.text)
@@ -270,14 +282,17 @@
             payload["controlnet_units"] = [x.to_dict() for x in controlnet_units]
             return self.custom_post('controlnet/txt2img', payload=payload)
 
         if controlnet_units and len(controlnet_units)>0:
             payload["alwayson_scripts"]["ControlNet"] = {
                 "args": [x.to_dict() for x in controlnet_units]
             }
+        elif self.has_controlnet:
+            # workaround : if not passed, webui will use previous args!
+            payload["alwayson_scripts"]["ControlNet"] = {"args": []}
 
         response = self.session.post(url=f'{self.baseurl}/txt2img', json=payload)
         return self._to_api_result(response)
 
     def img2img(self,
                 images=[],  # list of PIL Image
                 resize_mode=0,
@@ -387,14 +402,17 @@
             payload["controlnet_units"] = [x.to_dict() for x in controlnet_units]
             return self.custom_post('controlnet/img2img', payload=payload)
 
         if controlnet_units and len(controlnet_units)>0:
             payload["alwayson_scripts"]["ControlNet"] = {
                 "args": [x.to_dict() for x in controlnet_units]
             }
+        elif self.has_controlnet:
+            payload["alwayson_scripts"]["ControlNet"] = {"args": []}
+
         response = self.session.post(url=f'{self.baseurl}/img2img', json=payload)
         return self._to_api_result(response)
 
     def extra_single_image(self,
                            image,  # PIL Image
                            resize_mode=0,
                            show_extras_results=True,
@@ -494,22 +512,35 @@
     def interrogate(self, image):
         payload = {
             "image": b64_img(image),
         }
 
         response = self.session.post(url=f'{self.baseurl}/interrogate', json=payload)
         return self._to_api_result(response)
+    
+    def interrupt(self):
+        response = self.session.post(url=f'{self.baseurl}/interrupt')
+        return response.json()
+    
+    def skip(self):
+        response = self.session.post(url=f'{self.baseurl}/skip')
+        return response.json()
+
 
     def get_options(self):
         response = self.session.get(url=f'{self.baseurl}/options')
         return response.json()
     def set_options(self, options):
         response = self.session.post(url=f'{self.baseurl}/options', json=options)
         return response.json()
 
+    def get_cmd_flags(self):
+        response = self.session.get(url=f'{self.baseurl}/cmd-flags')
+        return response.json()
+
     def get_progress(self):
         response = self.session.get(url=f'{self.baseurl}/progress')
         return response.json()
 
     def get_cmd_flags(self):
         response = self.session.get(url=f'{self.baseurl}/cmd-flags')
         return response.json()
@@ -530,24 +561,33 @@
         return response.json()
     def get_realesrgan_models(self):        
         response = self.session.get(url=f'{self.baseurl}/realesrgan-models')
         return response.json()
     def get_prompt_styles(self):        
         response = self.session.get(url=f'{self.baseurl}/prompt-styles')
         return response.json()
-    def get_artist_categories(self):        
+    def get_artist_categories(self): # deprecated ?   
         response = self.session.get(url=f'{self.baseurl}/artist-categories')
         return response.json()
-    def get_artists(self):        
+    def get_artists(self): # deprecated ?
         response = self.session.get(url=f'{self.baseurl}/artists')
         return response.json()
     def refresh_checkpoints(self):
         response = self.session.post(url=f'{self.baseurl}/refresh-checkpoints')
         return response.json()
-
+    def get_scripts(self):
+        response = self.session.get(url=f'{self.baseurl}/scripts')
+        return response.json()
+    def get_embeddings(self):        
+        response = self.session.get(url=f'{self.baseurl}/embeddings')
+        return response.json()
+    def get_memory(self):        
+        response = self.session.get(url=f'{self.baseurl}/memory')
+        return response.json()
+    
     def get_endpoint(self, endpoint, baseurl):
         if baseurl:
             return f'{self.baseurl}/{endpoint}'
         else:
             from urllib.parse import urlparse, urlunparse
             parsed_url = urlparse(self.baseurl)
             basehost = parsed_url.netloc
```

## Comparing `webuiapi-0.7.0.dist-info/LICENSE` & `webuiapi-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webuiapi-0.7.0.dist-info/METADATA` & `webuiapi-0.8.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webuiapi
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python API client for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/mix1009/sdwebuiapi
 Author: ChunKoo Park
 Author-email: mix1009@gmail.com
 License: MIT
 Keywords: stable-diffuion-webui,AUTOMATIC1111,stable-diffusion,api
 Requires-Python: >=3.7, <4
@@ -283,17 +283,25 @@
 # misc get apis
 api.get_samplers()
 api.get_cmd_flags()      
 api.get_hypernetworks()
 api.get_face_restorers()
 api.get_realesrgan_models()
 api.get_prompt_styles()
-api.get_artist_categories()
-api.get_artists()
+api.get_artist_categories() # deprecated ?
+api.get_artists() # deprecated ?
 api.get_progress()
+api.get_embeddings()
+api.get_cmd_flags()
+api.get_scripts()
+api.get_memory()
+
+# misc apis
+api.interrupt()
+api.skip()
 ```
 
 ### Utility methods
 ```
 # save current model name
 old_model = api.util_get_current_model()
```

