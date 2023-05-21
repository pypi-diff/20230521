# Comparing `tmp/denoising-diffusion-pytorch-1.6.3.tar.gz` & `tmp/denoising-diffusion-pytorch-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.6.3.tar", last modified: Sat May 20 17:14:21 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.6.4.tar", last modified: Sun May 21 15:56:55 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.6.3.tar` & `denoising-diffusion-pytorch-1.6.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:14:21.366117 denoising-diffusion-pytorch-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 17:14:21.366117 denoising-diffusion-pytorch-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:14:21.366117 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28589 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36211 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:14:21.366117 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 17:14:21.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-20 17:14:21.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:14:21.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 17:14:21.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 17:14:21.000000 denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 17:14:21.366117 denoising-diffusion-pytorch-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-20 17:14:03.000000 denoising-diffusion-pytorch-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:56:55.148841 denoising-diffusion-pytorch-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-21 15:56:55.148841 denoising-diffusion-pytorch-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:56:55.148841 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28589 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36409 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:56:55.148841 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-21 15:56:55.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-21 15:56:55.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 15:56:55.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-21 15:56:55.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 15:56:55.000000 denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 15:56:55.148841 denoising-diffusion-pytorch-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-21 15:56:46.000000 denoising-diffusion-pytorch-1.6.4/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.6.3/LICENSE` & `denoising-diffusion-pytorch-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/PKG-INFO` & `denoising-diffusion-pytorch-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.6.3
+Version: 1.6.4
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.6.3/README.md` & `denoising-diffusion-pytorch-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -723,27 +723,32 @@
             img, x_start = self.p_sample(img, i, self_cond)
 
         return img
 
     def q_sample(self, x_start, t, noise = None):
         noise = default(noise, lambda: torch.randn_like(x_start))
 
-        if self.offset_noise_strength > 0.:
-            offset_noise = torch.randn(x_start.shape[:2], device = self.device)
-            noise += self.offset_noise_strength * rearrange(offset_noise, 'b c -> b c 1 1')
-
         return (
             extract(self.sqrt_alphas_cumprod, t, x_start.shape) * x_start +
             extract(self.sqrt_one_minus_alphas_cumprod, t, x_start.shape) * noise
         )
 
-    def p_losses(self, x_start, t, noise = None):
+    def p_losses(self, x_start, t, noise = None, offset_noise_strength = None):
         b, c, h, w = x_start.shape
+
         noise = default(noise, lambda: torch.randn_like(x_start))
 
+        # offset noise - https://www.crosslabs.org/blog/diffusion-with-offset-noise
+
+        offset_noise_strength = default(offset_noise_strength, self.offset_noise_strength)
+
+        if offset_noise_strength > 0.:
+            offset_noise = torch.randn(x_start.shape[:2], device = self.device)
+            noise += offset_noise_strength * rearrange(offset_noise, 'b c -> b c 1 1')
+
         # noise sample
 
         x = self.q_sample(x_start = x_start, t = t, noise = noise)
 
         # if doing self-conditioning, 50% of the time, predict x_start from current set of times
         # and condition with unet with that
         # this technique will slow down training by 25%, but seems to lower FID significantly
```

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.6.3
+Version: 1.6.4
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.6.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.6.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.6.3/setup.py` & `denoising-diffusion-pytorch-1.6.4/setup.py`

 * *Files identical despite different names*

