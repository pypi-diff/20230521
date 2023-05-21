# Comparing `tmp/sdgrate-0.2.3.tar.gz` & `tmp/sdgrate-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdgrate-0.2.3.tar", last modified: Wed Apr 19 18:52:30 2023, max compression
+gzip compressed data, was "sdgrate-0.2.4.tar", last modified: Sun May 21 10:34:39 2023, max compression
```

## Comparing `sdgrate-0.2.3.tar` & `sdgrate-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-19 18:52:30.712838 sdgrate-0.2.3/
--rw-r--r--   0 damian     (501) staff       (20)    34523 2017-09-30 07:16:25.000000 sdgrate-0.2.3/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)       26 2023-02-19 13:57:54.000000 sdgrate-0.2.3/MANIFEST.in
--rw-r--r--   0 damian     (501) staff       (20)    10570 2023-04-19 18:52:30.712684 sdgrate-0.2.3/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     9994 2023-04-19 18:51:14.000000 sdgrate-0.2.3/README.md
--rw-r--r--   0 damian     (501) staff       (20)      953 2023-04-19 18:31:40.000000 sdgrate-0.2.3/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-19 18:52:30.712877 sdgrate-0.2.3/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-19 18:52:30.706255 sdgrate-0.2.3/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-19 18:52:30.710906 sdgrate-0.2.3/src/sdgrate/
--rw-r--r--   0 damian     (501) staff       (20)   159676 2023-02-19 12:53:47.000000 sdgrate-0.2.3/src/sdgrate/LibreBaskerville-DpdE.ttf
--rw-r--r--   0 damian     (501) staff       (20)       21 2023-02-19 12:53:47.000000 sdgrate-0.2.3/src/sdgrate/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    16376 2023-02-28 22:12:45.000000 sdgrate-0.2.3/src/sdgrate/checkpoint_merger_mbw.py
--rw-r--r--   0 damian     (501) staff       (20)    28759 2023-04-19 18:30:59.000000 sdgrate-0.2.3/src/sdgrate/grate.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-19 18:52:30.712448 sdgrate-0.2.3/src/sdgrate.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)    10570 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      376 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       45 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/entry_points.txt
--rw-r--r--   0 damian     (501) staff       (20)       90 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        8 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-21 10:34:39.019837 sdgrate-0.2.4/
+-rw-r--r--   0 damian     (501) staff       (20)    34523 2017-09-30 07:16:25.000000 sdgrate-0.2.4/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)       26 2023-02-19 13:57:54.000000 sdgrate-0.2.4/MANIFEST.in
+-rw-r--r--   0 damian     (501) staff       (20)    11022 2023-05-21 10:34:39.019622 sdgrate-0.2.4/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)    10446 2023-05-21 10:34:14.000000 sdgrate-0.2.4/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      947 2023-05-21 10:32:58.000000 sdgrate-0.2.4/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-05-21 10:34:39.019886 sdgrate-0.2.4/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-21 10:34:39.016580 sdgrate-0.2.4/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-21 10:34:39.018622 sdgrate-0.2.4/src/sdgrate/
+-rw-r--r--   0 damian     (501) staff       (20)   159676 2023-02-19 12:53:47.000000 sdgrate-0.2.4/src/sdgrate/LibreBaskerville-DpdE.ttf
+-rw-r--r--   0 damian     (501) staff       (20)       21 2023-02-19 12:53:47.000000 sdgrate-0.2.4/src/sdgrate/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    16376 2023-02-28 22:12:45.000000 sdgrate-0.2.4/src/sdgrate/checkpoint_merger_mbw.py
+-rw-r--r--   0 damian     (501) staff       (20)    30821 2023-05-21 10:31:55.000000 sdgrate-0.2.4/src/sdgrate/grate.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-21 10:34:39.019435 sdgrate-0.2.4/src/sdgrate.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)    11022 2023-05-21 10:34:39.000000 sdgrate-0.2.4/src/sdgrate.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      376 2023-05-21 10:34:39.000000 sdgrate-0.2.4/src/sdgrate.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-05-21 10:34:39.000000 sdgrate-0.2.4/src/sdgrate.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       45 2023-05-21 10:34:39.000000 sdgrate-0.2.4/src/sdgrate.egg-info/entry_points.txt
+-rw-r--r--   0 damian     (501) staff       (20)       84 2023-05-21 10:34:39.000000 sdgrate-0.2.4/src/sdgrate.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        8 2023-05-21 10:34:39.000000 sdgrate-0.2.4/src/sdgrate.egg-info/top_level.txt
```

### Comparing `sdgrate-0.2.3/LICENSE` & `sdgrate-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sdgrate-0.2.3/PKG-INFO` & `sdgrate-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdgrate
-Version: 0.2.3
+Version: 0.2.4
 Summary: A grid image generator for Stable Diffusion models based on 🧨diffusers.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/grate
 Project-URL: Bug Tracker, https://github.com/damian0815/grate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -72,22 +72,24 @@
 Note that the number of values passed to `--merge_alphas` matches the number of strings passed to `--merge_unet_block_weights`.
 
 ## Full arguments list
 
 Run `python3 grate.py -h` for help:
 
 ```commandline
-$ grate -h
+$ grate -h 
 usage: grate [-h] --prompts PROMPTS [PROMPTS ...] --repo_ids_or_paths
              REPO_IDS_OR_PATHS [REPO_IDS_OR_PATHS ...] --output_path
              OUTPUT_PATH [--device DEVICE] [--batch_size BATCH_SIZE]
              [--width WIDTH] [--height HEIGHT]
              [--negative_prompts NEGATIVE_PROMPTS [NEGATIVE_PROMPTS ...]]
-             [--seeds SEEDS [SEEDS ...]] [--cfg CFG] [--steps STEPS]
-             [--disable_nsfw_checker] [--local_files_only]
+             [--seeds SEEDS [SEEDS ...]]
+             [--scheduler {ddim,lms,dpm++,k_dpm++,dpm++_sde,k_dpm++_sde,euler_a,k_euler_a,pndm,ddpm,k_dpm2_a}]
+             [--cfg CFG] [--steps STEPS] [--disable_nsfw_checker]
+             [--local_files_only]
              [--merge_alpha MERGE_ALPHA [MERGE_ALPHA ...]]
              [--merge_algorithm MERGE_ALGORITHM [MERGE_ALGORITHM ...]]
              [--merge_unet_block_weights MERGE_UNET_BLOCK_WEIGHTS [MERGE_UNET_BLOCK_WEIGHTS ...]]
              [--merge_unet_alpha MERGE_UNET_ALPHA [MERGE_UNET_ALPHA ...]]
              [--merge_text_encoder_alpha MERGE_TEXT_ENCODER_ALPHA [MERGE_TEXT_ENCODER_ALPHA ...]]
              [--save_merge_path_prefix SAVE_MERGE_PATH_PREFIX]
              [--save_merge_float32] [--use_penultimate_clip_layer]
@@ -131,14 +133,16 @@
                         (Optional) Negative prompts. Specify either one string
                         to share for all `--prompts`, or as many strings as
                         there are `--prompts`.
   --seeds SEEDS [SEEDS ...]
                         (Optional) Seeds. Specify either one seed to share for
                         all `--prompts`, or as many seeds as there are
                         `--prompts`.
+  --scheduler {ddim,lms,dpm++,k_dpm++,dpm++_sde,k_dpm++_sde,euler_a,k_euler_a,pndm,ddpm,k_dpm2_a}
+                        (Optional, default=dpm++) Scheduler to use.
   --cfg CFG             (Optional, default=7.5) CFG scale.
   --steps STEPS         (Optional, default=15) How many inference steps to run
   --disable_nsfw_checker
                         (Optional)
   --local_files_only    (Optional) Use only local data (do not attempt to
                         download or update models)
   --merge_alpha MERGE_ALPHA [MERGE_ALPHA ...]
@@ -163,24 +167,26 @@
   --save_merge_path_prefix SAVE_MERGE_PATH_PREFIX
                         (Optional) If doing a merge, save all merge
                         combinations using this path as a prefix.
   --save_merge_float32  (Optional) If saving merges, save with float32
                         precision (default is float16).
   --use_penultimate_clip_layer
                         (Optional) Use the outputs from penultimate (second to
-                        last) CLIP hidden layer.
-
+                        last) CLIP hidden layer. On detected SD2.x models this
+                        defaults on, otherwise it defaults off.
 ```
 
 Enjoy!
 
 ## Using as a library
 
 The main `sdgrate.grate` module includes the following functions, which may be useful: `merge_models`, `render_row`, `render_all`. 
 
 The model merger is implemented as a custom pipeline based on a modified version of the (checkpoint_merger pipeline)
 
 ## Changelog
 
+#### 0.2.4 - add `--scheduler` arg and fix diffusers 0.16 support 
+
 #### 0.2.3 - fix crash when running compel, fix diffusers 0.15 support actually
 
 #### 0.2.2 - added `--use_penultimate_clip_layer` arg ~~for improved SD2 generation quality~~ (aka "clip skip")
```

### Comparing `sdgrate-0.2.3/README.md` & `sdgrate-0.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -58,22 +58,24 @@
 Note that the number of values passed to `--merge_alphas` matches the number of strings passed to `--merge_unet_block_weights`.
 
 ## Full arguments list
 
 Run `python3 grate.py -h` for help:
 
 ```commandline
-$ grate -h
+$ grate -h 
 usage: grate [-h] --prompts PROMPTS [PROMPTS ...] --repo_ids_or_paths
              REPO_IDS_OR_PATHS [REPO_IDS_OR_PATHS ...] --output_path
              OUTPUT_PATH [--device DEVICE] [--batch_size BATCH_SIZE]
              [--width WIDTH] [--height HEIGHT]
              [--negative_prompts NEGATIVE_PROMPTS [NEGATIVE_PROMPTS ...]]
-             [--seeds SEEDS [SEEDS ...]] [--cfg CFG] [--steps STEPS]
-             [--disable_nsfw_checker] [--local_files_only]
+             [--seeds SEEDS [SEEDS ...]]
+             [--scheduler {ddim,lms,dpm++,k_dpm++,dpm++_sde,k_dpm++_sde,euler_a,k_euler_a,pndm,ddpm,k_dpm2_a}]
+             [--cfg CFG] [--steps STEPS] [--disable_nsfw_checker]
+             [--local_files_only]
              [--merge_alpha MERGE_ALPHA [MERGE_ALPHA ...]]
              [--merge_algorithm MERGE_ALGORITHM [MERGE_ALGORITHM ...]]
              [--merge_unet_block_weights MERGE_UNET_BLOCK_WEIGHTS [MERGE_UNET_BLOCK_WEIGHTS ...]]
              [--merge_unet_alpha MERGE_UNET_ALPHA [MERGE_UNET_ALPHA ...]]
              [--merge_text_encoder_alpha MERGE_TEXT_ENCODER_ALPHA [MERGE_TEXT_ENCODER_ALPHA ...]]
              [--save_merge_path_prefix SAVE_MERGE_PATH_PREFIX]
              [--save_merge_float32] [--use_penultimate_clip_layer]
@@ -117,14 +119,16 @@
                         (Optional) Negative prompts. Specify either one string
                         to share for all `--prompts`, or as many strings as
                         there are `--prompts`.
   --seeds SEEDS [SEEDS ...]
                         (Optional) Seeds. Specify either one seed to share for
                         all `--prompts`, or as many seeds as there are
                         `--prompts`.
+  --scheduler {ddim,lms,dpm++,k_dpm++,dpm++_sde,k_dpm++_sde,euler_a,k_euler_a,pndm,ddpm,k_dpm2_a}
+                        (Optional, default=dpm++) Scheduler to use.
   --cfg CFG             (Optional, default=7.5) CFG scale.
   --steps STEPS         (Optional, default=15) How many inference steps to run
   --disable_nsfw_checker
                         (Optional)
   --local_files_only    (Optional) Use only local data (do not attempt to
                         download or update models)
   --merge_alpha MERGE_ALPHA [MERGE_ALPHA ...]
@@ -149,24 +153,26 @@
   --save_merge_path_prefix SAVE_MERGE_PATH_PREFIX
                         (Optional) If doing a merge, save all merge
                         combinations using this path as a prefix.
   --save_merge_float32  (Optional) If saving merges, save with float32
                         precision (default is float16).
   --use_penultimate_clip_layer
                         (Optional) Use the outputs from penultimate (second to
-                        last) CLIP hidden layer.
-
+                        last) CLIP hidden layer. On detected SD2.x models this
+                        defaults on, otherwise it defaults off.
 ```
 
 Enjoy!
 
 ## Using as a library
 
 The main `sdgrate.grate` module includes the following functions, which may be useful: `merge_models`, `render_row`, `render_all`. 
 
 The model merger is implemented as a custom pipeline based on a modified version of the (checkpoint_merger pipeline)
 
 ## Changelog
 
+#### 0.2.4 - add `--scheduler` arg and fix diffusers 0.16 support 
+
 #### 0.2.3 - fix crash when running compel, fix diffusers 0.15 support actually
 
 #### 0.2.2 - added `--use_penultimate_clip_layer` arg ~~for improved SD2 generation quality~~ (aka "clip skip")
```

### Comparing `sdgrate-0.2.3/pyproject.toml` & `sdgrate-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdgrate"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A grid image generator for Stable Diffusion models based on 🧨diffusers."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -15,15 +15,15 @@
 dependencies = [
     "diffusers[torch]>=0.13",
     "compel~=1.1.3",
     "huggingface-hub",
     "Pillow",
     "tqdm",
     "transformers",
-    "safetensors"
+    "scipy"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/damian0815/grate"
 "Bug Tracker" = "https://github.com/damian0815/grate/issues"
 
 [project.scripts]
```

### Comparing `sdgrate-0.2.3/src/sdgrate/LibreBaskerville-DpdE.ttf` & `sdgrate-0.2.4/src/sdgrate/LibreBaskerville-DpdE.ttf`

 * *Files identical despite different names*

### Comparing `sdgrate-0.2.3/src/sdgrate/checkpoint_merger_mbw.py` & `sdgrate-0.2.4/src/sdgrate/checkpoint_merger_mbw.py`

 * *Files identical despite different names*

### Comparing `sdgrate-0.2.3/src/sdgrate/grate.py` & `sdgrate-0.2.4/src/sdgrate/grate.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import os
 import argparse
 import pathlib
 from typing import Optional
 
 import torch
 from compel import Compel
-from diffusers import StableDiffusionPipeline, DPMSolverMultistepScheduler
+from diffusers import StableDiffusionPipeline, LMSDiscreteScheduler, DPMSolverMultistepScheduler, \
+    EulerAncestralDiscreteScheduler, PNDMScheduler, DDPMScheduler, KDPM2AncestralDiscreteScheduler, DDIMScheduler
 from PIL import Image, ImageDraw, ImageFont
 from diffusers.pipelines.stable_diffusion import StableDiffusionPipelineOutput
 from diffusers.utils import is_xformers_available
 from tqdm import tqdm
 
 from huggingface_hub import list_repo_refs
 
@@ -168,39 +169,65 @@
             refs = list_repo_refs(repo_id_or_path)
             fp16_ref = next((r for r in refs.branches if r.name == 'fp16'), None)
             if fp16_ref is not None:
                 revision = 'fp16'
         return StableDiffusionPipeline.from_pretrained(repo_id_or_path, revision=revision,
                                                        local_files_only=local_files_only)
 
+def make_scheduler(which: str, config):
+
+    if which == 'ddim':
+        return DDIMScheduler.from_config(config)
+    elif which == "lms":
+        return LMSDiscreteScheduler.from_config(config)
+    elif which == "dpm++":
+        return DPMSolverMultistepScheduler.from_config(config, algorithm_type="dpmsolver++", use_karras_sigmas=False)
+    elif which == "k_dpm++":
+        return DPMSolverMultistepScheduler.from_config(config, algorithm_type="dpmsolver++", use_karras_sigmas=True)
+    elif which == "dpm++_sde":
+        return DPMSolverMultistepScheduler.from_config(config, algorithm_type="sde-dpmsolver++",
+                                                       use_karras_sigmas=False)
+    elif which == "k_dpm++_sde":
+        return DPMSolverMultistepScheduler.from_config(config, algorithm_type="sde-dpmsolver++",
+                                                       use_karras_sigmas=True)
+    elif which == "euler_a":
+        return EulerAncestralDiscreteScheduler.from_config(config, use_karras_sigmas=False)
+    elif which == "k_euler_a":
+        return EulerAncestralDiscreteScheduler.from_config(config, use_karras_sigmas=True)
+    elif which == 'pndm':
+        return PNDMScheduler.from_config(config)
+    elif which == 'ddpm':
+        return DDPMScheduler.from_config(config)
+    elif which == 'k_dpm2_a':
+        return KDPM2AncestralDiscreteScheduler.from_config(config)
+    else:
+        raise ValueError(f"Unrecognized scheduler {which}")
+
 
 def render_row(prompts: list[str],
                negative_prompts: Optional[list[str]],
                seeds: list[int],
                pipeline: StableDiffusionPipeline,
+               scheduler_name: str="dpm++",
                device: str = None,
                batch_size=1,
                sample_w=512,
                sample_h=512,
                cfg=7.5,
-               num_inference_steps=15,  # ddpm++ solver: 15 is typically enough
+               num_inference_steps=15, # for dpm++ solver, 15 is typically enough
                disable_nsfw_checker: bool = False,
                use_penultimate_clip_layer: bool = False
                ) -> list[Image]:
-    # ddpm++
-    pipeline.scheduler = DPMSolverMultistepScheduler.from_config(pipeline.scheduler.config,
-                                                                 algorithm_type="dpmsolver++")
+    pipeline.scheduler = make_scheduler(which=scheduler_name, config=pipeline.scheduler.config)
     if device is None:
         device = 'cuda' if torch.cuda.is_available() else 'mps' if torch.backends.mps.is_available() else 'cpu'
-    if device == 'cuda':
-        # noinspection PyTypeChecker
-        pipeline = pipeline.to(torch.float16)
-        if is_xformers_available():
-            pipeline.enable_xformers_memory_efficient_attention()
-    pipeline = pipeline.to(device)
+    # noinspection PyTypeChecker
+    pipeline = pipeline.to(device, torch.float16)
+    if is_xformers_available():
+        pipeline.enable_xformers_memory_efficient_attention()
     if disable_nsfw_checker:
         pipeline.safety_checker = disable_nsfw_safety_checker
     images = []
     negative_prompts = negative_prompts or [""] * len(prompts)
     batches = chunk_list(list(zip(prompts, negative_prompts, seeds)), batch_size)
     progress_bar = tqdm(list(batches))
     compel = Compel(tokenizer=pipeline.tokenizer,
@@ -298,14 +325,15 @@
     return merge_configs
 
 
 
 
 def render_all(prompts: list[str], negative_prompts: Optional[list[str]], seeds: list[int], cfg: float,
                repo_ids_or_paths: list[str],
+               scheduler: str,
                device: str,
                size: tuple[int, int],
                batch_size: int,
                inference_steps: int = 15,
                save_partial_filename: Optional[str] = None,
                local_files_only: bool = False,
                merge_config: Optional[dict] = None,
@@ -353,29 +381,30 @@
                                     algorithm=merge_algorithm, unet_block_weights=unet_block_weights,
                                     per_module_alphas=per_module_alphas,
                                     local_files_only=local_files_only)
             row_images = render_row(prompts,
                                     negative_prompts=negative_prompts,
                                     seeds=seeds,
                                     pipeline=pipeline,
+                                    scheduler_name=scheduler,
                                     device=device,
                                     batch_size=batch_size,
                                     cfg=cfg,
                                     num_inference_steps=inference_steps,
                                     sample_w=size[0], sample_h=size[1],
                                     disable_nsfw_checker=disable_nsfw_checker,
                                     use_penultimate_clip_layer=use_penultimate_clip_layer)
             all_images += row_images
             save_partial_if_requested()
 
             save_merge_path_prefix = merge_config.get('save_merge_path_prefix', None)
             if save_merge_path_prefix is not None:
                 save_half = merge_config.get('save_merge_half', True)
                 if save_half:
-                    pipeline.to(torch.float16)
+                    pipeline.to(pipeline.device, torch.float16)
                 save_merge_path = f"{save_merge_path_prefix}_{merge_index:02d}"
                 pipeline.save_pretrained(save_merge_path)
 
             del pipeline
 
         grid_image = make_image_grid(all_images, len(merge_configs), len(prompts), row_labels, prompts)
     else:
@@ -383,14 +412,15 @@
         for repo_id_or_path in tqdm(repo_ids_or_paths):
             print(f"model {repo_id_or_path}:")
             pipeline = load_model(repo_id_or_path, local_files_only=local_files_only)
             row_images = render_row(prompts,
                                     negative_prompts=negative_prompts,
                                     seeds=seeds,
                                     pipeline=pipeline,
+                                    scheduler_name=scheduler,
                                     device=device,
                                     batch_size=batch_size,
                                     cfg=cfg,
                                     num_inference_steps=inference_steps,
                                     sample_w=size[0], sample_h=size[1],
                                     disable_nsfw_checker=disable_nsfw_checker,
                                     use_penultimate_clip_layer=use_penultimate_clip_layer)
@@ -459,14 +489,20 @@
                         nargs="+",
                         help="(Optional) Negative prompts. Specify either one string to share for all `--prompts`, or as many strings as there are `--prompts`.")
     parser.add_argument("--seeds",
                         required=False,
                         type=int,
                         nargs="+",
                         help="(Optional) Seeds. Specify either one seed to share for all `--prompts`, or as many seeds as there are `--prompts`.")
+    parser.add_argument("--scheduler",
+                        choices=['ddim', "lms", "dpm++", "k_dpm++", "dpm++_sde", "k_dpm++_sde",
+                                 "euler_a", "k_euler_a", 'pndm', 'ddpm', 'k_dpm2_a'],
+                        default="dpm++",
+                        type=str,
+                        help="(Optional, default=dpm++) Scheduler to use.")
     parser.add_argument("--cfg",
                         required=False,
                         type=float,
                         default=7.5,
                         help="(Optional, default=7.5) CFG scale.")
     parser.add_argument("--steps",
                         required=False,
@@ -557,14 +593,15 @@
     else:
         merge_config['save_merge_path_prefix'] = args.save_merge_path_prefix
         merge_config['save_merge_half'] = not args.save_merge_float32
 
 
     render_all(prompts=prompts,
                negative_prompts=negative_prompts,
+               scheduler=args.scheduler,
                seeds=seeds,
                repo_ids_or_paths=args.repo_ids_or_paths,
                merge_config=merge_config,
                device=args.device,
                size=(args.width, args.height),
                batch_size=args.batch_size,
                cfg=args.cfg,
```

### Comparing `sdgrate-0.2.3/src/sdgrate.egg-info/PKG-INFO` & `sdgrate-0.2.4/src/sdgrate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdgrate
-Version: 0.2.3
+Version: 0.2.4
 Summary: A grid image generator for Stable Diffusion models based on 🧨diffusers.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/grate
 Project-URL: Bug Tracker, https://github.com/damian0815/grate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -72,22 +72,24 @@
 Note that the number of values passed to `--merge_alphas` matches the number of strings passed to `--merge_unet_block_weights`.
 
 ## Full arguments list
 
 Run `python3 grate.py -h` for help:
 
 ```commandline
-$ grate -h
+$ grate -h 
 usage: grate [-h] --prompts PROMPTS [PROMPTS ...] --repo_ids_or_paths
              REPO_IDS_OR_PATHS [REPO_IDS_OR_PATHS ...] --output_path
              OUTPUT_PATH [--device DEVICE] [--batch_size BATCH_SIZE]
              [--width WIDTH] [--height HEIGHT]
              [--negative_prompts NEGATIVE_PROMPTS [NEGATIVE_PROMPTS ...]]
-             [--seeds SEEDS [SEEDS ...]] [--cfg CFG] [--steps STEPS]
-             [--disable_nsfw_checker] [--local_files_only]
+             [--seeds SEEDS [SEEDS ...]]
+             [--scheduler {ddim,lms,dpm++,k_dpm++,dpm++_sde,k_dpm++_sde,euler_a,k_euler_a,pndm,ddpm,k_dpm2_a}]
+             [--cfg CFG] [--steps STEPS] [--disable_nsfw_checker]
+             [--local_files_only]
              [--merge_alpha MERGE_ALPHA [MERGE_ALPHA ...]]
              [--merge_algorithm MERGE_ALGORITHM [MERGE_ALGORITHM ...]]
              [--merge_unet_block_weights MERGE_UNET_BLOCK_WEIGHTS [MERGE_UNET_BLOCK_WEIGHTS ...]]
              [--merge_unet_alpha MERGE_UNET_ALPHA [MERGE_UNET_ALPHA ...]]
              [--merge_text_encoder_alpha MERGE_TEXT_ENCODER_ALPHA [MERGE_TEXT_ENCODER_ALPHA ...]]
              [--save_merge_path_prefix SAVE_MERGE_PATH_PREFIX]
              [--save_merge_float32] [--use_penultimate_clip_layer]
@@ -131,14 +133,16 @@
                         (Optional) Negative prompts. Specify either one string
                         to share for all `--prompts`, or as many strings as
                         there are `--prompts`.
   --seeds SEEDS [SEEDS ...]
                         (Optional) Seeds. Specify either one seed to share for
                         all `--prompts`, or as many seeds as there are
                         `--prompts`.
+  --scheduler {ddim,lms,dpm++,k_dpm++,dpm++_sde,k_dpm++_sde,euler_a,k_euler_a,pndm,ddpm,k_dpm2_a}
+                        (Optional, default=dpm++) Scheduler to use.
   --cfg CFG             (Optional, default=7.5) CFG scale.
   --steps STEPS         (Optional, default=15) How many inference steps to run
   --disable_nsfw_checker
                         (Optional)
   --local_files_only    (Optional) Use only local data (do not attempt to
                         download or update models)
   --merge_alpha MERGE_ALPHA [MERGE_ALPHA ...]
@@ -163,24 +167,26 @@
   --save_merge_path_prefix SAVE_MERGE_PATH_PREFIX
                         (Optional) If doing a merge, save all merge
                         combinations using this path as a prefix.
   --save_merge_float32  (Optional) If saving merges, save with float32
                         precision (default is float16).
   --use_penultimate_clip_layer
                         (Optional) Use the outputs from penultimate (second to
-                        last) CLIP hidden layer.
-
+                        last) CLIP hidden layer. On detected SD2.x models this
+                        defaults on, otherwise it defaults off.
 ```
 
 Enjoy!
 
 ## Using as a library
 
 The main `sdgrate.grate` module includes the following functions, which may be useful: `merge_models`, `render_row`, `render_all`. 
 
 The model merger is implemented as a custom pipeline based on a modified version of the (checkpoint_merger pipeline)
 
 ## Changelog
 
+#### 0.2.4 - add `--scheduler` arg and fix diffusers 0.16 support 
+
 #### 0.2.3 - fix crash when running compel, fix diffusers 0.15 support actually
 
 #### 0.2.2 - added `--use_penultimate_clip_layer` arg ~~for improved SD2 generation quality~~ (aka "clip skip")
```

