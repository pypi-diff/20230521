# Comparing `tmp/classifier-free-guidance-pytorch-0.2.1.tar.gz` & `tmp/classifier-free-guidance-pytorch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classifier-free-guidance-pytorch-0.2.1.tar", last modified: Sun May 21 18:40:22 2023, max compression
+gzip compressed data, was "classifier-free-guidance-pytorch-0.2.2.tar", last modified: Sun May 21 18:47:21 2023, max compression
```

## Comparing `classifier-free-guidance-pytorch-0.2.1.tar` & `classifier-free-guidance-pytorch-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:40:22.270277 classifier-free-guidance-pytorch-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-21 18:40:22.270277 classifier-free-guidance-pytorch-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:40:22.266277 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18189 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:40:22.266277 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)  3194984 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:40:22.266277 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-21 18:40:22.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-21 18:40:22.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:40:22.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 18:40:22.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 18:40:22.000000 classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:40:22.270277 classifier-free-guidance-pytorch-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-21 18:40:11.000000 classifier-free-guidance-pytorch-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:47:21.276396 classifier-free-guidance-pytorch-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-21 18:47:21.276396 classifier-free-guidance-pytorch-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:47:21.268396 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:47:21.268396 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  3194984 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:47:21.268396 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-21 18:47:21.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-21 18:47:21.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:47:21.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 18:47:21.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 18:47:21.000000 classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:47:21.276396 classifier-free-guidance-pytorch-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-21 18:47:06.000000 classifier-free-guidance-pytorch-0.2.2/setup.py
```

### Comparing `classifier-free-guidance-pytorch-0.2.1/LICENSE` & `classifier-free-guidance-pytorch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.2.1/PKG-INFO` & `classifier-free-guidance-pytorch-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classifier-free-guidance-pytorch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Classifier Free Guidance - Pytorch
 Home-page: https://github.com/lucidrains/classifier-free-guidance-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,classifier free guidance,text conditioning and guidance
 Classifier: Development Status :: 4 - Beta
```

### Comparing `classifier-free-guidance-pytorch-0.2.1/README.md` & `classifier-free-guidance-pytorch-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/attend.py` & `classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py` & `classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,27 +128,24 @@
 
         if cond_scale == 1:
             return logits
 
         null_logits = fn_maybe_with_text(self, *args, **kwargs_with_cond_dropout)
         scaled_logits = null_logits + (logits - null_logits) * cond_scale
 
-        logits_out = scaled_logits
+        if rescale_phi <= 0:
+            return scaled_logits
 
-        if rescale_phi > 0:
-            # proposed in https://arxiv.org/abs/2305.08891
-            # as a way to prevent over-saturation with classifier free guidance
-            # works both in pixel as well as latent space as opposed to the solution from imagen
-
-            dims = tuple(range(1, logits.ndim - 1))
-            rescaled_logits = scaled_logits * (logits.std(dim = dims, keepdim = True) / scaled_logits.std(dim = dims, keepdim= True))
-
-            logits_out = rescaled_logits * rescale_phi + (1. - rescale_phi) * logits
-
-        return logits_out
+        # proposed in https://arxiv.org/abs/2305.08891
+        # as a way to prevent over-saturation with classifier free guidance
+        # works both in pixel as well as latent space as opposed to the solution from imagen
+
+        dims = tuple(range(1, logits.ndim - 1))
+        rescaled_logits = scaled_logits * (logits.std(dim = dims, keepdim = True) / scaled_logits.std(dim = dims, keepdim= True))
+        return rescaled_logits * rescale_phi + (1. - rescale_phi) * logits
 
     return inner
 
 # attention
 
 class Attention(nn.Module):
     def __init__(
```

### Comparing `classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt` & `classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/open_clip.py` & `classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/t5.py` & `classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch/tokenizer.py` & `classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch/tokenizer.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch.egg-info/PKG-INFO` & `classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classifier-free-guidance-pytorch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Classifier Free Guidance - Pytorch
 Home-page: https://github.com/lucidrains/classifier-free-guidance-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,classifier free guidance,text conditioning and guidance
 Classifier: Development Status :: 4 - Beta
```

### Comparing `classifier-free-guidance-pytorch-0.2.1/classifier_free_guidance_pytorch.egg-info/SOURCES.txt` & `classifier-free-guidance-pytorch-0.2.2/classifier_free_guidance_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.2.1/setup.py` & `classifier-free-guidance-pytorch-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'classifier-free-guidance-pytorch',
   packages = find_packages(exclude=[]),
   include_package_data = True,
-  version = '0.2.1',
+  version = '0.2.2',
   license='MIT',
   description = 'Classifier Free Guidance - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/classifier-free-guidance-pytorch',
   keywords = [
```

