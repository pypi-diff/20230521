# Comparing `tmp/hordelib-1.1.2.tar.gz` & `tmp/hordelib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-1.1.2.tar", last modified: Fri May 19 22:09:18 2023, max compression
+gzip compressed data, was "hordelib-1.2.0.tar", last modified: Sun May 21 07:48:05 2023, max compression
```

## Comparing `hordelib-1.1.2.tar` & `hordelib-1.2.0.tar`

### file list

```diff
@@ -1,923 +1,929 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.326949 hordelib-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 22:09:01.000000 hordelib-1.1.2/.changelog
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-19 22:09:01.000000 hordelib-1.1.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.210950 hordelib-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.222950 hordelib-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-19 22:09:01.000000 hordelib-1.1.2/.github/workflows/maintests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-19 22:09:01.000000 hordelib-1.1.2/.github/workflows/prtests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-19 22:09:01.000000 hordelib-1.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-19 22:09:01.000000 hordelib-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    42761 2023-05-19 22:09:08.000000 hordelib-1.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-19 22:09:01.000000 hordelib-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-19 22:09:01.000000 hordelib-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50821 2023-05-19 22:09:18.326949 hordelib-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-19 22:09:01.000000 hordelib-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-19 22:09:01.000000 hordelib-1.1.2/build_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.226950 hordelib-1.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/kudos.py
--rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/lora_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/make_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/make_index_all_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_all_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_all_stress_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_facefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_img2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_img2img_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_img2img_inpaint_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_img2img_outpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_kudos_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_long_prompt_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_stress_test_cnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_stress_test_cnet_preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_stress_test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_stress_test_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_stress_test_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_stress_test_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_stress_test_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_stress_test_txt2img_hiresfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_txt2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_txt2img_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 22:09:01.000000 hordelib-1.1.2/examples/run_upscale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.230949 hordelib-1.1.2/hordelib/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.230949 hordelib-1.1.2/hordelib/_comfyui/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/cldm/
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/cldm/cldm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/clip_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/clip_vision_config_h.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/diffusers_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/extra_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)    38661 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/gligen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/gns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/models/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    27584 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
--rw-r--r--   0 runner    (1001) docker     (123)    89264 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.234950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.238950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37803 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.238950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/ema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.238950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.238950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.238950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
--rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.238950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.238950 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    29815 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    46096 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/sd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.242950 hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/sd2_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/sd2_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.242950 hordelib-1.1.2/hordelib/_comfyui/comfy/t2i_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.242950 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.242950 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.246950 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
--rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
--rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.246950 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.246950 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.246950 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/nodes_hypernetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/nodes_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/nodes_rebatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/comfyui_screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/custom_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/custom_nodes/example_node.py.example
--rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/extra_model_paths.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/extra_model_paths.yaml.example
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/folder_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/input/
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/input/example.png
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.214950 hordelib-1.1.2/hordelib/_comfyui/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/checkpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/clip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/clip_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/anything_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/v1-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/v2-inference-v.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/v2-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/gligen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/gligen/put_gligen_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/hypernetworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/hypernetworks/put_hypernetworks_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/loras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/loras/put_loras_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/style_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/upscale_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/models/vae/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/models/vae/put_vae_here
--rw-r--r--   0 runner    (1001) docker     (123)    51038 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/output/_output_images_will_be_put_here
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/script_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/script_examples/basic_api_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.250949 hordelib-1.1.2/hordelib/_comfyui/web/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.254950 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/clipspace.js
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/colorPalette.js
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/editAttention.js
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/keybinds.js
--rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/maskeditor.js
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/noteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/rerouteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/slotDefaults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/snapToGrid.js
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/uploadImage.js
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/widgetInputs.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/extensions/logging.js.example
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/jsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.254950 hordelib-1.1.2/hordelib/_comfyui/web/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   486763 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/lib/litegraph.core.js
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/lib/litegraph.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.254950 hordelib-1.1.2/hordelib/_comfyui/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/scripts/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    36531 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/scripts/defaultGraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/scripts/pnginfo.js
--rw-r--r--   0 runner    (1001) docker     (123)    15749 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/scripts/ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/scripts/widgets.js
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.254950 hordelib-1.1.2/hordelib/_comfyui/web/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/types/comfy.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-05-19 22:09:10.000000 hordelib-1.1.2/hordelib/_comfyui/web/types/litegraph.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-19 22:09:17.000000 hordelib-1.1.2/hordelib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.254950 hordelib-1.1.2/hordelib/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/blip/caption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.258950 hordelib-1.1.2/hordelib/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/cache/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.258950 hordelib-1.1.2/hordelib/clip/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/interrogate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.258950 hordelib-1.1.2/hordelib/clip/ranking_lists/
--rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/ranking_lists/artists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/ranking_lists/flavors.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/ranking_lists/mediums.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/ranking_lists/movements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/ranking_lists/sites.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/ranking_lists/tags.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/ranking_lists/techniques.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/clip/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    26071 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/comfy_horde.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/config_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    22227 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/horde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35773 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/install_comfy.patch
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/install_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.258950 hordelib-1.1.2/hordelib/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_database/db_dep.json
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_database/db_embeds.json
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_database/diffusers.json
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_database/med_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.258950 hordelib-1.1.2/hordelib/model_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36751 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/model_manager/safety_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.262950 hordelib-1.1.2/hordelib/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.262950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.262950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.262950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/canny/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.262950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/color/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.262950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/hed/
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.262950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.262950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.262950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.262950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.266950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.266950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.266950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.266950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.266950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.266950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.266950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.266950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.266950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.266950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.270949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.218950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.270949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.270949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.274949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.274949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.218950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.274949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.274949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.274949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.274949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.278950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.278950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25256 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.278950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.278950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.282950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.282950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.282950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.286949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.290949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.290949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.290949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.294949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.294949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.294949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.294949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.294949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.298950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.222950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.298950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.298950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.298950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.298950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.298950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.298950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.298950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14268 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.302950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.302950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.302950 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.306949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.306949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.306949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.306949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/facerestore/
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.310949 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.314949 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/facerestore/facelib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/node_clip_similarities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/node_controlnet_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/node_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/node_image_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/node_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/nodes/node_upscale_model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.314949 hordelib-1.1.2/hordelib/pipeline_designs/
--rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipeline_designs/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipeline_designs/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipeline_designs/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.314949 hordelib-1.1.2/hordelib/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipelines/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipelines/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipelines/pipeline_controlnet_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipelines/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipelines/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/pipelines/pipeline_stable_diffusion_paint.json
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/preload.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.314949 hordelib-1.1.2/hordelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.314949 hordelib-1.1.2/hordelib/utils/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/blip/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    41378 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/blip/med.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/blip/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/dynamicprompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/gpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/ioredirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-19 22:09:01.000000 hordelib-1.1.2/hordelib/utils/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.230949 hordelib-1.1.2/hordelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50821 2023-05-19 22:09:18.000000 hordelib-1.1.2/hordelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    50481 2023-05-19 22:09:18.000000 hordelib-1.1.2/hordelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:09:18.000000 hordelib-1.1.2/hordelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-19 22:09:18.000000 hordelib-1.1.2/hordelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-19 22:09:18.000000 hordelib-1.1.2/hordelib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.318949 hordelib-1.1.2/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-05-19 22:09:01.000000 hordelib-1.1.2/images/test_annotator.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-05-19 22:09:01.000000 hordelib-1.1.2/images/test_db0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-05-19 22:09:01.000000 hordelib-1.1.2/images/test_facefix.png
--rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-05-19 22:09:01.000000 hordelib-1.1.2/images/test_inpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-05-19 22:09:01.000000 hordelib-1.1.2/images/test_inpaint_alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-05-19 22:09:01.000000 hordelib-1.1.2/images/test_inpaint_mask.png
--rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-05-19 22:09:01.000000 hordelib-1.1.2/images/test_inpaint_original.png
--rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-05-19 22:09:01.000000 hordelib-1.1.2/images/test_outpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-19 22:09:10.000000 hordelib-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 22:09:01.000000 hordelib-1.1.2/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-19 22:09:10.000000 hordelib-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:09:18.326949 hordelib-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.322950 hordelib-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.322950 hordelib-1.1.2/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/meta/test_build_helper_import_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:18.326949 hordelib-1.1.2/tests/model_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/model_managers/test_annotators.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/model_managers/test_comvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/model_managers/test_hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/model_managers/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_comfy.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_dynamic_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_horde_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_horde_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_horde_inference_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_horde_inference_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_horde_inference_painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_horde_lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_horde_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_horde_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_image_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-19 22:09:01.000000 hordelib-1.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-19 22:09:01.000000 hordelib-1.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.410052 hordelib-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-21 07:47:44.000000 hordelib-1.2.0/.changelog
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-21 07:47:44.000000 hordelib-1.2.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.226051 hordelib-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.246051 hordelib-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-21 07:47:44.000000 hordelib-1.2.0/.github/workflows/maintests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-21 07:47:44.000000 hordelib-1.2.0/.github/workflows/prtests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-21 07:47:44.000000 hordelib-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-21 07:47:44.000000 hordelib-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    43221 2023-05-21 07:47:54.000000 hordelib-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-21 07:47:44.000000 hordelib-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-21 07:47:44.000000 hordelib-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50821 2023-05-21 07:48:05.410052 hordelib-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-21 07:47:44.000000 hordelib-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-21 07:47:44.000000 hordelib-1.2.0/build_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.250051 hordelib-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/kudos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/lora_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/make_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/make_index_all_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_all_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_all_stress_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_facefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_img2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_img2img_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_img2img_inpaint_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_img2img_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_img2img_outpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_kudos_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_long_prompt_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_stress_test_cnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_stress_test_cnet_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_stress_test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_stress_test_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_stress_test_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_stress_test_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_stress_test_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_stress_test_txt2img_hiresfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_txt2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_txt2img_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-21 07:47:44.000000 hordelib-1.2.0/examples/run_upscale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.254051 hordelib-1.2.0/hordelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.258051 hordelib-1.2.0/hordelib/_comfyui/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.258051 hordelib-1.2.0/hordelib/_comfyui/comfy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.258051 hordelib-1.2.0/hordelib/_comfyui/comfy/cldm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/cldm/cldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/clip_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/clip_vision_config_h.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/diffusers_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.262051 hordelib-1.2.0/hordelib/_comfyui/comfy/extra_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)    38661 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/gligen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.262051 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/gns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.262051 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27584 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.262051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.262051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.262051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.262051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89264 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.262051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.266051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.266051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37803 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.266051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/ema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.266051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.266051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.266051 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.270052 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.270052 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29815 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46096 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.270052 hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/sd2_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/sd2_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.274052 hordelib-1.2.0/hordelib/_comfyui/comfy/t2i_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.274052 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.274052 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.278051 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.282051 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.282051 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.282051 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/nodes_hypernetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/nodes_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/nodes_rebatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/comfyui_screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.282051 hordelib-1.2.0/hordelib/_comfyui/custom_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/custom_nodes/example_node.py.example
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/extra_model_paths.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/extra_model_paths.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/folder_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.282051 hordelib-1.2.0/hordelib/_comfyui/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/input/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.230051 hordelib-1.2.0/hordelib/_comfyui/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.282051 hordelib-1.2.0/hordelib/_comfyui/models/checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.282051 hordelib-1.2.0/hordelib/_comfyui/models/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.282051 hordelib-1.2.0/hordelib/_comfyui/models/clip_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/models/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/anything_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/v1-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/v2-inference-v.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/v2-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/models/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/models/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/models/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/models/gligen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/gligen/put_gligen_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/models/hypernetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/hypernetworks/put_hypernetworks_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/models/loras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/loras/put_loras_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/models/style_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/models/upscale_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/models/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/models/vae/put_vae_here
+-rw-r--r--   0 runner    (1001) docker     (123)    51038 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/output/_output_images_will_be_put_here
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/script_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/script_examples/basic_api_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.286052 hordelib-1.2.0/hordelib/_comfyui/web/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.290052 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/clipspace.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/colorPalette.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/editAttention.js
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/keybinds.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/maskeditor.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/noteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/rerouteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/slotDefaults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/snapToGrid.js
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/uploadImage.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/widgetInputs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/extensions/logging.js.example
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/jsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.290052 hordelib-1.2.0/hordelib/_comfyui/web/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   486763 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/lib/litegraph.core.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/lib/litegraph.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.294052 hordelib-1.2.0/hordelib/_comfyui/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/scripts/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36531 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/scripts/defaultGraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/scripts/pnginfo.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15749 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/scripts/ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/scripts/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.294052 hordelib-1.2.0/hordelib/_comfyui/web/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/types/comfy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-05-21 07:47:56.000000 hordelib-1.2.0/hordelib/_comfyui/web/types/litegraph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-21 07:48:04.000000 hordelib-1.2.0/hordelib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.294052 hordelib-1.2.0/hordelib/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/blip/caption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.294052 hordelib-1.2.0/hordelib/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.294052 hordelib-1.2.0/hordelib/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/interrogate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.298051 hordelib-1.2.0/hordelib/clip/ranking_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/ranking_lists/artists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/ranking_lists/flavors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/ranking_lists/mediums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/ranking_lists/movements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/ranking_lists/sites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/ranking_lists/tags.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/ranking_lists/techniques.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/clip/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21322 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/comfy_horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/config_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23708 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35773 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/install_comfy.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/install_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.298051 hordelib-1.2.0/hordelib/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_database/db_dep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_database/db_embeds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_database/diffusers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_database/med_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.298051 hordelib-1.2.0/hordelib/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36751 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/model_manager/safety_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.302052 hordelib-1.2.0/hordelib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.302052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.302052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.302052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/canny/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.302052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.302052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.302052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.306052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.306052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.306052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.306052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.306052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.310052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.310052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.310052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.310052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.310052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.310052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.310052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.310052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.314051 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.234051 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.314051 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.314051 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.322052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.322052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.238051 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.322052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.322052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.322052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.322052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.326052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.330052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25256 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.330052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.330052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.330052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.334052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.334052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.342052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.346052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.350052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.354052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.354052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.354052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.358052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.358052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.358052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.362052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.242051 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.362052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.362052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.362052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.362052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.362052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.362052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.366052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14268 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.370052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.370052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.370052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.378052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.378052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.378052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.378052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.382052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.382052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.382052 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.382052 hordelib-1.2.0/hordelib/nodes/facerestore/
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.382052 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.382052 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.382052 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.386052 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.386052 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.386052 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.390052 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.390052 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/facerestore/facelib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/node_clip_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/node_controlnet_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/node_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/node_image_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/node_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/nodes/node_upscale_model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.390052 hordelib-1.2.0/hordelib/pipeline_designs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipeline_designs/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipeline_designs/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion_img2img_mask.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.394052 hordelib-1.2.0/hordelib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipelines/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipelines/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipelines/pipeline_controlnet_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipelines/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipelines/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipelines/pipeline_stable_diffusion_img2img_mask.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/preload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.394052 hordelib-1.2.0/hordelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.394052 hordelib-1.2.0/hordelib/utils/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/blip/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41378 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/blip/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/blip/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/dynamicprompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/gpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/ioredirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-21 07:47:44.000000 hordelib-1.2.0/hordelib/utils/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.254051 hordelib-1.2.0/hordelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50821 2023-05-21 07:48:05.000000 hordelib-1.2.0/hordelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    50733 2023-05-21 07:48:05.000000 hordelib-1.2.0/hordelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 07:48:05.000000 hordelib-1.2.0/hordelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-21 07:48:05.000000 hordelib-1.2.0/hordelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-21 07:48:05.000000 hordelib-1.2.0/hordelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.402052 hordelib-1.2.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    47993 2023-05-21 07:47:44.000000 hordelib-1.2.0/images/test_annotator.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-05-21 07:47:44.000000 hordelib-1.2.0/images/test_db0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-05-21 07:47:44.000000 hordelib-1.2.0/images/test_facefix.png
+-rw-r--r--   0 runner    (1001) docker     (123)   461877 2023-05-21 07:47:44.000000 hordelib-1.2.0/images/test_img2img_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-05-21 07:47:44.000000 hordelib-1.2.0/images/test_inpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)   461877 2023-05-21 07:47:44.000000 hordelib-1.2.0/images/test_inpaint_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-05-21 07:47:44.000000 hordelib-1.2.0/images/test_inpaint_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-05-21 07:47:44.000000 hordelib-1.2.0/images/test_inpaint_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-05-21 07:47:44.000000 hordelib-1.2.0/images/test_outpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-21 07:47:56.000000 hordelib-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 07:47:44.000000 hordelib-1.2.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-21 07:47:56.000000 hordelib-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 07:48:05.410052 hordelib-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.410052 hordelib-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.410052 hordelib-1.2.0/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/meta/test_build_helper_import_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:48:05.410052 hordelib-1.2.0/tests/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/model_managers/test_annotators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/model_managers/test_comvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/model_managers/test_hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/model_managers/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_dynamic_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_horde_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_horde_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_horde_inference_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_horde_inference_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_horde_inference_painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_horde_lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_horde_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_horde_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_image_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_payload_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-21 07:47:44.000000 hordelib-1.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-21 07:47:44.000000 hordelib-1.2.0/tox.ini
```

### Comparing `hordelib-1.1.2/.changelog` & `hordelib-1.2.0/.changelog`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/.github/workflows/maintests.yml` & `hordelib-1.2.0/.github/workflows/maintests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/.github/workflows/prtests.yml` & `hordelib-1.2.0/.github/workflows/prtests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/.github/workflows/release.yml` & `hordelib-1.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/.gitignore` & `hordelib-1.2.0/.gitignore`

 * *Files 25% similar despite different names*

```diff
@@ -146,29 +146,19 @@
 hordelib/model_database/esrgan.json
 hordelib/model_database/gfpgan.json
 hordelib/model_database/safety_checker.json
 hordelib/model_database/stable_diffusion.json
 ComfyUI
 model.ckpt
 coverage.lcov
-images/pip*.png
-images/test.png
-images/hor*.png
-images/hor*.webp
-images/pip*.webp
-images/test.webp
-images/run_*
-images/all_models
 profiles/
-images/perftest
-images/stresstest
-images/longprompts
 longprompts.zip
 comfy-prompt*.json
-images/index.html
+images/*
+!images/test_*
 hordelib/_comfyui
 _version.py
 _comfyui
 tmp/
 
 .vscode
 *.ckpt
```

### Comparing `hordelib-1.1.2/CHANGELOG.md` & `hordelib-1.2.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 ## hordelib Changelog
 
+## [v1.2.0](https://github.com/Haidra-Org/hordelib/compare/v1.1.2...v1.2.0)
+
+21 May 2023
+
+- fix: unit tests use about 6GB VRAM max now. [`#293`](https://github.com/Haidra-Org/hordelib/pull/293) (Jug)
+- feat: refactor for clarity, tweak img2img and inpainting, tidy tests [`#290`](https://github.com/Haidra-Org/hordelib/pull/290) (Jug)
+- Add alt pipeline design for img2img with mask [`#279`](https://github.com/Haidra-Org/hordelib/pull/279) (Wolfgang Meyers)
+
 ## [v1.1.2](https://github.com/Haidra-Org/hordelib/compare/v1.1.1...v1.1.2)
 
 19 May 2023
 
 ## [v1.1.1](https://github.com/Haidra-Org/hordelib/compare/v1.1.0...v1.1.1)
 
 19 May 2023
```

### Comparing `hordelib-1.1.2/LICENSE` & `hordelib-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/PKG-INFO` & `hordelib-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 1.1.2
+Version: 1.2.0
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hordelib-1.1.2/README.md` & `hordelib-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/build_helper.py` & `hordelib-1.2.0/build_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/kudos.py` & `hordelib-1.2.0/examples/kudos.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/lora_downloader.py` & `hordelib-1.2.0/examples/lora_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                 lora["triggers"] = triggers
                 break
         # If we don't have everything required, fail
         if not lora.get("sha256") or not lora.get("filename") or not lora.get("url") or not lora.get("triggers"):
             return
         # Fixup A1111 centric triggers
         for i, trigger in enumerate(lora["triggers"]):
-            if matched := re.match("<lora:(.*):.*>", trigger):
+            if re.match("<lora:(.*):.*>", trigger):
                 lora["triggers"][i] = re.sub("<lora:(.*):.*>", "\\1", trigger)
         return lora
 
     def _download_thread(self):
         # We try to download the LORA. There are tens of thousands of these things, we aren't
         # picky if downloads fail, as they often will if civitai is the host, we just move on to
         # the next one
```

### Comparing `hordelib-1.1.2/examples/make_index.py` & `hordelib-1.2.0/examples/make_index.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/make_index_all_models.py` & `hordelib-1.2.0/examples/make_index_all_models.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_all_models.py` & `hordelib-1.2.0/examples/run_all_models.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_all_stress_tests.py` & `hordelib-1.2.0/examples/run_all_stress_tests.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_clip.py` & `hordelib-1.2.0/examples/run_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_controlnet.py` & `hordelib-1.2.0/examples/run_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_controlnet_annotator.py` & `hordelib-1.2.0/examples/run_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_facefix.py` & `hordelib-1.2.0/examples/run_facefix.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_img2img.py` & `hordelib-1.2.0/examples/run_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_img2img_hires.py` & `hordelib-1.2.0/examples/run_img2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_img2img_inpaint.py` & `hordelib-1.2.0/examples/run_img2img_inpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_img2img_inpaint_mask.py` & `hordelib-1.2.0/examples/run_img2img_inpaint_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_img2img_outpaint.py` & `hordelib-1.2.0/examples/run_img2img_outpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_inpainting.py` & `hordelib-1.2.0/examples/run_inpainting.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_kudos_test.py` & `hordelib-1.2.0/examples/run_kudos_test.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_long_prompt_check.py` & `hordelib-1.2.0/examples/run_long_prompt_check.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_lora.py` & `hordelib-1.2.0/examples/run_lora.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_memory_test.py` & `hordelib-1.2.0/examples/run_memory_test.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_stress_test_cnet.py` & `hordelib-1.2.0/examples/run_stress_test_cnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_stress_test_cnet_preproc.py` & `hordelib-1.2.0/examples/run_stress_test_cnet_preproc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_stress_test_dynamic.py` & `hordelib-1.2.0/examples/run_stress_test_dynamic.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_stress_test_img2img.py` & `hordelib-1.2.0/examples/run_stress_test_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_stress_test_mixed.py` & `hordelib-1.2.0/examples/run_stress_test_mixed.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_stress_test_pp.py` & `hordelib-1.2.0/examples/run_stress_test_pp.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_stress_test_txt2img.py` & `hordelib-1.2.0/examples/run_stress_test_txt2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_stress_test_txt2img_hiresfix.py` & `hordelib-1.2.0/examples/run_stress_test_txt2img_hiresfix.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_txt2img.py` & `hordelib-1.2.0/examples/run_txt2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_txt2img_hires.py` & `hordelib-1.2.0/examples/run_txt2img_hires.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     SharedModelManager.manager.load("Deliberate")
 
     data = {
         "sampler_name": "k_dpmpp_2m",
         "cfg_scale": 7.5,
         "denoising_strength": 1.0,
         "seed": 123456789,
-        "height": 512,
-        "width": 512,
+        "height": 768,
+        "width": 768,
         "karras": True,
         "tiling": False,
         "hires_fix": True,
         "clip_skip": 1,
         "control_type": None,
         "image_is_control": False,
         "return_control_map": False,
```

### Comparing `hordelib-1.1.2/examples/run_txt2img_local_model.py` & `hordelib-1.2.0/examples/run_txt2img_local_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/examples/run_upscale.py` & `hordelib-1.2.0/examples/run_upscale.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/LICENSE` & `hordelib-1.2.0/hordelib/_comfyui/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/README.md` & `hordelib-1.2.0/hordelib/_comfyui/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/cldm/cldm.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/cldm/cldm.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/cli_args.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/cli_args.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/clip_vision.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/clip_vision.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/diffusers_convert.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/diffusers_convert.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/gligen.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/gligen.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/augmentation.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/augmentation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/config.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/evaluation.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/external.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/external.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/gns.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/gns.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/layers.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/layers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/sampling.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/sampling.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/k_diffusion/utils.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/k_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/data/util.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/data/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/autoencoder.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/attention.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/ema.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/api.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/modules/tomesd.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/modules/tomesd.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/ldm/util.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/ldm/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/model_management.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/model_management.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/sample.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/samplers.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/samplers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/sd.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/sd.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_clip.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_clip_config.json` & `hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt` & `hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json` & `hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json` & `hordelib-1.2.0/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/sd2_clip.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/sd2_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/sd2_clip_config.json` & `hordelib-1.2.0/hordelib/_comfyui/comfy/sd2_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/t2i_adapter/adapter.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/t2i_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy/utils.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/chainner_models/types.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/chainner_models/types.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/nodes_hypernetwork.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/nodes_hypernetwork.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/nodes_mask.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/nodes_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/nodes_post_processing.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/nodes_post_processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/nodes_rebatch.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/nodes_rebatch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py` & `hordelib-1.2.0/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/comfyui_screenshot.png` & `hordelib-1.2.0/hordelib/_comfyui/comfyui_screenshot.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/custom_nodes/example_node.py.example` & `hordelib-1.2.0/hordelib/_comfyui/custom_nodes/example_node.py.example`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/execution.py` & `hordelib-1.2.0/hordelib/_comfyui/execution.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/extra_model_paths.yaml.example` & `hordelib-1.2.0/hordelib/_comfyui/extra_model_paths.yaml.example`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/folder_paths.py` & `hordelib-1.2.0/hordelib/_comfyui/folder_paths.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/input/example.png` & `hordelib-1.2.0/hordelib/_comfyui/input/example.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/main.py` & `hordelib-1.2.0/hordelib/_comfyui/main.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/anything_v3.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/anything_v3.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/v1-inference.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/v2-inference-v.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/v2-inference.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml` & `hordelib-1.2.0/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/nodes.py` & `hordelib-1.2.0/hordelib/_comfyui/nodes.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/notebooks/comfyui_colab.ipynb` & `hordelib-1.2.0/hordelib/_comfyui/notebooks/comfyui_colab.ipynb`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/script_examples/basic_api_example.py` & `hordelib-1.2.0/hordelib/_comfyui/script_examples/basic_api_example.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/server.py` & `hordelib-1.2.0/hordelib/_comfyui/server.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/clipspace.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/clipspace.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/colorPalette.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/colorPalette.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/editAttention.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/editAttention.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/keybinds.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/keybinds.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/maskeditor.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/maskeditor.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/nodeTemplates.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/nodeTemplates.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/noteNode.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/noteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/rerouteNode.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/rerouteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/slotDefaults.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/slotDefaults.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/snapToGrid.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/snapToGrid.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/core/widgetInputs.js` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/core/widgetInputs.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/extensions/logging.js.example` & `hordelib-1.2.0/hordelib/_comfyui/web/extensions/logging.js.example`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/index.html` & `hordelib-1.2.0/hordelib/_comfyui/web/index.html`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/lib/litegraph.core.js` & `hordelib-1.2.0/hordelib/_comfyui/web/lib/litegraph.core.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/lib/litegraph.css` & `hordelib-1.2.0/hordelib/_comfyui/web/lib/litegraph.css`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/scripts/api.js` & `hordelib-1.2.0/hordelib/_comfyui/web/scripts/api.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/scripts/app.js` & `hordelib-1.2.0/hordelib/_comfyui/web/scripts/app.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/scripts/defaultGraph.js` & `hordelib-1.2.0/hordelib/_comfyui/web/scripts/defaultGraph.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/scripts/pnginfo.js` & `hordelib-1.2.0/hordelib/_comfyui/web/scripts/pnginfo.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/scripts/ui.js` & `hordelib-1.2.0/hordelib/_comfyui/web/scripts/ui.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/scripts/widgets.js` & `hordelib-1.2.0/hordelib/_comfyui/web/scripts/widgets.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/style.css` & `hordelib-1.2.0/hordelib/_comfyui/web/style.css`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/types/comfy.d.ts` & `hordelib-1.2.0/hordelib/_comfyui/web/types/comfy.d.ts`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/_comfyui/web/types/litegraph.d.ts` & `hordelib-1.2.0/hordelib/_comfyui/web/types/litegraph.d.ts`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/benchmark.py` & `hordelib-1.2.0/hordelib/benchmark.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/blip/caption.py` & `hordelib-1.2.0/hordelib/blip/caption.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/cache/cache.py` & `hordelib-1.2.0/hordelib/cache/cache.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/bulk.py` & `hordelib-1.2.0/hordelib/clip/bulk.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/coca.py` & `hordelib-1.2.0/hordelib/clip/coca.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/image.py` & `hordelib-1.2.0/hordelib/clip/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/interrogate.py` & `hordelib-1.2.0/hordelib/clip/interrogate.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/ranking_lists/artists.txt` & `hordelib-1.2.0/hordelib/clip/ranking_lists/artists.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/ranking_lists/flavors.txt` & `hordelib-1.2.0/hordelib/clip/ranking_lists/flavors.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/ranking_lists/mediums.txt` & `hordelib-1.2.0/hordelib/clip/ranking_lists/mediums.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/ranking_lists/movements.txt` & `hordelib-1.2.0/hordelib/clip/ranking_lists/movements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/ranking_lists/tags.txt` & `hordelib-1.2.0/hordelib/clip/ranking_lists/tags.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/ranking_lists/techniques.txt` & `hordelib-1.2.0/hordelib/clip/ranking_lists/techniques.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/clip/text.py` & `hordelib-1.2.0/hordelib/clip/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/comfy_horde.py` & `hordelib-1.2.0/hordelib/comfy_horde.py`

 * *Files 16% similar despite different names*

```diff
@@ -197,27 +197,14 @@
     NODE_PARAMETER_REPLACEMENTS = {
         "HordeCheckpointLoader": {
             # We name this "model_name" as then we can use the same generic code in our model loaders
             "ckpt_name": "model_name",
         },
     }
 
-    # Enforce min/max bounds on some parameters
-    PARAMETER_BOUNDS = {
-        "sampler.cfg": (1, 100),
-        "sampler.denoise": (0.1, 1.0),
-        "empty_latent_image.height": (64, 8192),
-        "empty_latent_image.width": (64, 8192),
-        "sampler.steps": (1, 500),
-        "empty_latent_image.batch_size": (1, 500),
-        "clip_skip.stop_at_clip_layer": (-10, -1),
-        "latent_upscale.width": (64, 8192),
-        "latent_upscale.height": (64, 8192),
-    }
-
     # Approximate number of seconds to force garbage collection
     GC_TIME = 30
 
     _property_mutex = threading.Lock()
 
     # We maintain one "client_id" per thread
     @property
@@ -256,15 +243,14 @@
         self._gc_timer = time.time()
         self._counter_mutex = threading.Lock()
         # FIXME Temporary hack to set the model dir for LORAs
         _comfy_folder_paths["loras"] = (
             [os.path.join(get_cache_directory(), "loras")],
             [".safetensors"],
         )
-        logger.warning(_comfy_folder_paths["loras"])
         # Set custom node path
         _comfy_folder_paths["custom_nodes"] = ([os.path.join(get_hordelib_path(), "nodes")], [])
         # Load our pipelines
         self._load_pipelines()
 
         stdio = OutputCollector()
         with contextlib.redirect_stdout(stdio):
@@ -308,14 +294,20 @@
     def _load_custom_nodes(self) -> None:
         _comfy_nodes.init_custom_nodes()
 
     def _get_executor(self, pipeline):
         executor = _comfy_PromptExecutor(self)
         return executor
 
+    def get_pipeline_data(self, pipeline_name):
+        pipeline_data = copy.deepcopy(self.pipelines.get(pipeline_name, {}))
+        if pipeline_data:
+            logger.info(f"Running pipeline {pipeline_name}")
+        return pipeline_data
+
     def _fix_pipeline_types(self, data: dict) -> dict:
         # We have a list of nodes and each node has a class type, which we may want to change
         for nodename, node in data.items():
             if ("class_type" in node) and (node["class_type"] in Comfy_Horde.NODE_REPLACEMENTS):
                 logger.debug(
                     (
                         f"Changed type {data[nodename]['class_type']} to "
@@ -352,24 +344,14 @@
         for node in newnodes.values():
             if "inputs" in node:
                 for _, input in node["inputs"].items():
                     if type(input) is list and input and input[0] in renames:
                         input[0] = renames[input[0]]
         return newnodes
 
-    def _assert_parameter_bounds(self, params):
-        for key, value in params.items():
-            if key in self.PARAMETER_BOUNDS:
-                pmin, pmax = self.PARAMETER_BOUNDS[key]
-                if value < pmin:
-                    value = pmin
-                elif value > pmax:
-                    value = pmax
-                params[key] = value
-
     # We are passed a valid comfy pipeline and a design file from the comfyui web app.
     # Why?
     #
     # 1. We replace some nodes with our own hordelib nodes, for example "CheckpointLoaderSimple"
     #    with "HordeCheckpointLoader".
     # 2. We replace unfriendly node names like "3" and "7" with friendly names taken from the
     #    "title" attribute in the webui so we can have nicer parameter names when we call the
@@ -488,121 +470,25 @@
             self.images = data["output"]["images"]
             logger.debug("Received output image(s) from comfyui")
         else:
             logger.debug(f"{label}, {data}, {_id}")
 
     # Execute the named pipeline and pass the pipeline the parameter provided.
     # For the horde we assume the pipeline returns an array of images.
-    def run_pipeline(self, pipeline_name: str, params: dict) -> dict | None:
-        # Sanity
-        if pipeline_name not in self.pipelines:
-            logger.error(f"Unknown inference pipeline: {pipeline_name}")
-            return None
+    def _run_pipeline(self, pipeline: dict, params: dict) -> dict | None:
 
         # Update user settings
         _comfy_model_manager.set_user_reserved_vram(UserSettings.get_vram_to_leave_free_mb())
         _comfy_model_manager.set_batch_optimisations(UserSettings.enable_batch_optimisations.active)
 
-        logger.info(f"Running pipeline {pipeline_name}")
-
-        # Grab a copy of the pipeline
-        pipeline = copy.deepcopy(self.pipelines[pipeline_name])
-
-        # Inject our model manager if required
-        from hordelib.shared_model_manager import SharedModelManager
-
-        if "model_loader.model_manager" not in params:
-            logger.debug("Injecting model manager")
-            params["model_loader.model_manager"] = SharedModelManager
-
-        # If we have a source image, use that rather than noise (i.e. img2img)
-        # XXX This probably shouldn't be here. But for the moment, it works.
-        if params.get("image_loader.image"):
-            self.reconnect_input(pipeline, "sampler.latent_image", "vae_encode")
-
-        # XXX This shouldn't be here either, but it's not clear to me yet where the
-        # XXX correct place for dynamic connection of nodes is. Need to do a few more
-        # XXX pipelines to see.
-        if params.get("control_type"):
-            # Inject control net model manager
-            if "controlnet_model_loader.model_manager" not in params:
-                logger.debug("Injecting controlnet model manager")
-                params["controlnet_model_loader.model_manager"] = SharedModelManager
-            # Connect to the correct pre-processor node
-            if params.get("return_control_map", False):
-                # Connect annotator to output image directly
-                self.reconnect_input(
-                    pipeline,
-                    "output_image.images",
-                    params["control_type"],
-                )
-            else:
-                # Connect annotator to controlnet apply node
-                self.reconnect_input(
-                    pipeline,
-                    "controlnet_apply.image",
-                    params["control_type"],
-                )
-
-        # XXX Also shouldn't be here, but I'm noticing the pattern of dynamic pipeline
-        # XXX modification now. Here we dynamically build a lora pipeline
-
-        if params.get("loras"):
-
-            for lora_index, lora in enumerate(params.get("loras")):
-
-                # Inject a lora node (first lora)
-                if lora_index == 0:
-                    pipeline[f"lora_{lora_index}"] = {
-                        "inputs": {
-                            "model": ["model_loader", 0],
-                            "clip": ["model_loader", 1],
-                            "lora_name": f"{lora['name']}.safetensors",
-                            "strength_model": lora["model"],
-                            "strength_clip": lora["clip"],
-                        },
-                        "class_type": "LoraLoader",
-                    }
-                else:
-                    # Subsequent chained loras
-                    pipeline[f"lora_{lora_index}"] = {
-                        "inputs": {
-                            "model": [f"lora_{lora_index-1}", 0],
-                            "clip": [f"lora_{lora_index-1}", 1],
-                            "lora_name": f"{lora['name']}.safetensors",
-                            "strength_model": lora["model"],
-                            "strength_clip": lora["clip"],
-                        },
-                        "class_type": "LoraLoader",
-                    }
-
-            for lora_index, lora in enumerate(params.get("loras")):
-
-                # The first LORA always connects to the model loader
-                if lora_index == 0:
-                    self.reconnect_input(pipeline, "lora_0.model", "model_loader")
-                    self.reconnect_input(pipeline, "lora_0.clip", "model_loader")
-                else:
-                    # Other loras connect to the previous lora
-                    self.reconnect_input(pipeline, f"lora_{lora_index}.model", f"lora_{lora_index-1}.model")
-                    self.reconnect_input(pipeline, f"lora_{lora_index}.clip", f"lora_{lora_index-1}.clip")
-
-                # The last LORA always connects to the sampler and clip text encoders
-                if lora_index == len(params.get("loras")) - 1:
-                    self.reconnect_input(pipeline, "sampler.model", f"lora_{lora_index}")
-                    self.reconnect_input(pipeline, "clip_skip.clip", f"lora_{lora_index}")
-
-        # Enforce our parameter bounds
-        self._assert_parameter_bounds(params)
-
         # Set the pipeline parameters
         self._set(pipeline, **params)
 
         # Create (or retrieve) our prompt executive
-        inference = self._get_executor(pipeline_name)
+        inference = self._get_executor(pipeline)
 
         # This is useful for dumping the entire pipeline to the terminal when
         # developing and debugging new pipelines. A badly structured pipeline
         # file just results in a cryptic error from comfy
         pretty_pipeline = pformat(pipeline)
         if False:  # This isn't here Tazlin :)
             logger.error(pretty_pipeline)
@@ -624,36 +510,47 @@
         if time.time() - self._gc_timer > Comfy_Horde.GC_TIME:
             self._gc_timer = time.time()
             garbage_collect()
 
         return self.images
 
     # Run a pipeline that returns an image in pixel space
-    def run_image_pipeline(self, pipeline_name: str, params: dict) -> list[dict] | None:
+    def run_image_pipeline(self, pipeline, params: dict) -> list[dict] | None:
         # From the horde point of view, let us assume the output we are interested in
         # is always in a HordeImageOutput node named "output_image". This is an array of
         # dicts of the form:
         # [ {
         #     "imagedata": <BytesIO>,
         #     "type": "PNG"
         #   },
         # ]
         # See node_image_output.py
 
+        # We may be passed a pipeline name or a pipeline data structure
+        if isinstance(pipeline, str):
+            # Grab pipeline data structure
+            pipeline_data = self.get_pipeline_data(pipeline)
+            # Sanity
+            if not pipeline_data:
+                logger.error(f"Unknown inference pipeline: {pipeline}")
+                return None
+        else:
+            pipeline_data = pipeline
+
         # If no callers for a while, announce it
         if self._callers == 0 and self._exit_time:
             idle_time = time.time() - self._exit_time
             if idle_time > 1:
                 logger.warning(f"No job ran for {round(idle_time, 3)} seconds")
 
         # We have just been entered
         with self._counter_mutex:
             self._callers += 1
 
-        result = self.run_pipeline(pipeline_name, params)
+        result = self._run_pipeline(pipeline_data, params)
 
         # We are being exited
         with self._counter_mutex:
             self._exit_time = time.time()
             self._callers -= 1
 
         if result:
```

### Comparing `hordelib-1.1.2/hordelib/config_path.py` & `hordelib-1.2.0/hordelib/config_path.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/consts.py` & `hordelib-1.2.0/hordelib/consts.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/horde.py` & `hordelib-1.2.0/hordelib/horde.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # horde.py
 # Main interface for the horde to this library.
+import json
 import random
 import sys
 import time
+from copy import deepcopy
 
 from loguru import logger
-from PIL import Image, ImageOps, PngImagePlugin, UnidentifiedImageError
+from PIL import Image
 
 from hordelib.comfy_horde import Comfy_Horde
 from hordelib.shared_model_manager import SharedModelManager
 from hordelib.utils.dynamicprompt import DynamicPromptParser
+from hordelib.utils.image_utils import ImageUtils
 
 
 class HordeLib:
     _instance = None
     _initialised = False
 
     # Horde to comfy sampler mapping
@@ -31,429 +34,408 @@
         "k_dpmpp_2m": "dpmpp_2m",
         "ddim": "ddim",
         "uni_pc": "uni_pc",
         "uni_pc_bh2": "uni_pc_bh2",
         "plms": "euler",
     }
 
-    # Horde to tex2img parameter mapping
-    # XXX Items mapped to None are ignored for now
-    BASIC_INFERENCE_PARAMS = {
-        "sampler_name": "sampler.sampler_name",
-        "cfg_scale": "sampler.cfg",
-        "denoising_strength": "sampler.denoise",
-        "seed": "sampler.seed",
-        "height": "empty_latent_image.height",
-        "width": "empty_latent_image.width",
-        # "karras": Handled below
-        "tiling": None,
-        # "hires_fix": Handled below
-        "clip_skip": "clip_skip.stop_at_clip_layer",
-        # "control_type": Handled below
-        "image_is_control": None,
-        "return_control_map": "return_control_map",
-        # "prompt": Handled below
-        # "loras": Handled below
-        "ddim_steps": "sampler.steps",
-        "n_iter": "empty_latent_image.batch_size",
-        "model": "model_loader.model_name",
-        "source_image": "image_loader.image",
-        "source_mask": None,
-        "source_processing": "source_processing",
-        "control_strength": "controlnet_apply.strength",
-        "hires_fix_denoising_strength": "upscale_sampler.denoise",
-    }
-
     # Horde names on the left, our node names on the right
     # We use this to dynamically route the image through the
     # right node by reconnect inputs.
     CONTROLNET_IMAGE_PREPROCESSOR_MAP = {
         "canny": "canny",
         "hed": "hed",
         "depth": "depth",
         "normal": "normal",
         "openpose": "openpose",
         "seg": "seg",
         "scribble": "scribble",
         "fakescribbles": "fakescribble",
-        "hough": "mlsd",
+        "hough": "mlsd",  # horde backward compatibility
+        "mlsd": "mlsd",
         # "<unused>": "MiDaS-DepthMapPreprocessor",
         # "<unused>": "MediaPipe-HandPosePreprocessor",
         # "<unused>": "MediaPipe-FaceMeshPreprocessor",
         # "<unused>": "BinaryPreprocessor",
         # "<unused>": "ColorPreprocessor",
         # "<unused>": "PiDiNetPreprocessor",
     }
 
     SOURCE_IMAGE_PROCESSING_OPTIONS = ["img2img", "inpainting", "outpainting"]
 
+    SCHEDULERS = ["normal", "karras", "simple", "ddim_uniform"]
+
+    # Describe a valid payload, it's types and bounds. All incoming payload data is validated against,
+    # and normalised to, this schema.
+    PAYLOAD_SCHEMA = {
+        "sampler_name": {"datatype": str, "values": list(SAMPLERS_MAP.keys()), "default": "k_euler"},
+        "cfg_scale": {"datatype": float, "min": 1, "max": 100, "default": 8.0},
+        "denoising_strength": {"datatype": float, "min": 0.0, "max": 1.0, "default": 1.0},
+        "control_strength": {"datatype": float, "min": 0.0, "max": 1.0, "default": 1.0},
+        "seed": {"datatype": int, "default": random.randint(0, sys.maxsize)},
+        "width": {"datatype": int, "min": 64, "max": 8192, "default": 512, "divisible": 64},
+        "height": {"datatype": int, "min": 64, "max": 8192, "default": 512, "divisible": 64},
+        "hires_fix": {"datatype": bool, "default": False},
+        "clip_skip": {"datatype": int, "min": 1, "max": 20, "default": 1},
+        "control_type": {"datatype": str, "values": list(CONTROLNET_IMAGE_PREPROCESSOR_MAP.keys()), "default": None},
+        "image_is_control": {"datatype": bool, "default": False},
+        "return_control_map": {"datatype": bool, "default": False},
+        "prompt": {"datatype": str, "default": ""},
+        "negative_prompt": {"datatype": str, "default": ""},
+        "loras": {"datatype": list, "default": []},
+        "ddim_steps": {"datatype": int, "min": 1, "max": 500, "default": 30},
+        "n_iter": {"datatype": int, "min": 1, "max": 100, "default": 1},
+        "model": {"datatype": str, "default": "stable_diffusion"},
+        "source_mask": {"datatype": Image.Image, "default": None},
+        "source_image": {"datatype": Image.Image, "default": None},
+        "source_processing": {"datatype": str, "values": SOURCE_IMAGE_PROCESSING_OPTIONS, "default": None},
+        "hires_fix_denoising_strength": {"datatype": float, "min": 0.0, "max": 1.0, "default": 0.65},
+        "scheduler": {"datatype": str, "values": SCHEDULERS, "default": "normal"},
+    }
+
+    LORA_SCHEMA = {
+        "name": {"datatype": str, "default": ""},
+        "model": {"datatype": float, "min": 0.0, "max": 1.0, "default": 1.0},
+        "clip": {"datatype": float, "min": 0.0, "max": 1.0, "default": 1.0},
+    }
+
+    # pipeline parameter <- hordelib payload parameter mapping
+    PAYLOAD_TO_PIPELINE_PARAMETER_MAPPING = {
+        "sampler.sampler_name": "sampler_name",
+        "sampler.cfg": "cfg_scale",
+        "sampler.denoise": "denoising_strength",
+        "sampler.seed": "seed",
+        "empty_latent_image.height": "height",
+        "empty_latent_image.width": "width",
+        "sampler.scheduler": "scheduler",
+        "clip_skip.stop_at_clip_layer": "clip_skip",
+        "prompt.text": "prompt",
+        "negative_prompt.text": "negative_prompt",
+        "sampler.steps": "ddim_steps",
+        "empty_latent_image.batch_size": "n_iter",
+        "model_loader.model_name": "model",
+        "image_loader.image": "source_image",
+        "loras": "loras",
+        "upscale_sampler.denoise": "hires_fix_denoising_strength",
+        "upscale_sampler.seed": "seed",
+        "upscale_sampler.cfg": "cfg_scale",
+        "upscale_sampler.steps": "ddim_steps",
+        "upscale_sampler.sampler_name": "sampler_name",
+        "controlnet_apply.strength": "control_strength",
+        "controlnet_model_loader.control_net_name": "control_type",
+    }
+
     # We are a singleton
     def __new__(cls):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
         return cls._instance
 
     # We initialise only ever once (in the lifetime of the singleton)
     def __init__(self):
         if not self._initialised:
             self.generator = Comfy_Horde()
             self.__class__._initialised = True
 
-    def _check_payload(self, payload):
-        # Valid CFG, if it exists
-        if payload.get("cfg_scale"):
-            if payload.get("cfg_scale") < 0:
-                payload["cfg_scale"] = 0
-            elif payload.get("cfg_scale", 8.0) > 100:
-                payload["cfg_scale"] = 100
-        # valid width
-        if payload.get("width"):
-            try:
-                payload["width"] = int(payload.get("width"))
-                if payload["width"] < 64:
-                    payload["width"] = 64
-            except ValueError:
-                payload["width"] = 512
-        # valid height
-        if payload.get("height"):
+    def _json_hack(self, obj):
+        # Helper to serialise json which contains non-serialisable types
+        if hasattr(obj, "__class__"):
+            return f"{obj.__class__.__name__} instance"
+        return f"Object of type {type(obj).__name__}"
+
+    def dump_json(self, adict):
+        logger.warning(json.dumps(adict, indent=4, default=self._json_hack))
+
+    def _validate(self, value, datatype, min=None, max=None, default=None, values=None, divisible=None):
+        """Check the given value against the given constraints. Return the fixed value."""
+
+        # First, if we are passed no value at all, use the default
+        if value is None:
+            return default
+
+        # We have a value, check the type
+        if not isinstance(value, datatype):
+            # try to coerce the type
             try:
-                payload["height"] = int(payload.get("height"))
-                if payload["height"] < 64:
-                    payload["height"] = 64
-            except ValueError:
-                payload["height"] = 512
-        # Validate denoising
-        if payload.get("denoising_strength"):
-            try:
-                payload["denoising_strength"] = float(payload.get("denoising_strength"))
-                if payload["denoising_strength"] < 0.0:
-                    payload["denoising_strength"] = 0.0
-                elif payload["denoising_strength"] > 1.0:
-                    payload["denoising_strength"] = 1.0
-            except ValueError:
-                payload["denoising_strength"] = 1.0
-        if payload.get("hires_fix_denoising_strength"):
-            try:
-                payload["hires_fix_denoising_strength"] = float(payload.get("hires_fix_denoising_strength"))
-                if payload["hires_fix_denoising_strength"] < 0.0:
-                    payload["hires_fix_denoising_strength"] = 0.0
-                elif payload["hires_fix_denoising_strength"] > 1.0:
-                    payload["hires_fix_denoising_strength"] = 1.0
-            except ValueError:
-                payload["hires_fix_denoising_strength"] = 1.0
-        # Validate loras
-        fixed_loras = []
-        if payload.get("loras"):
-            try:
-                for lora in payload["loras"]:
-                    new_lora = {
-                        "name": lora.get("name", ""),
-                        "model": lora.get("model", 1.0),
-                        "clip": lora.get("clip", 1.0),
-                    }
-                    if new_lora["name"]:
-                        fixed_loras.append(new_lora)
-            except Exception:
-                fixed_loras = []
-        payload["loras"] = fixed_loras
-
-    def _parameter_remap(self, payload: dict[str, str | None]) -> dict[str, str | None]:
-        params = {}
-        # Extract from the payload things we understand
-        for key, value in payload.items():
-            newkey = HordeLib.BASIC_INFERENCE_PARAMS.get(key, None)
-            if newkey:
-                params[newkey] = value
-
-        # Inject model manager if needed
-        if "model_loader.model_manager" not in params:
-            params["model_loader.model_manager"] = SharedModelManager
-
-        return params
-
-    def _calculate_source_image_size(self, width, height):
-        if width > 512 and height > 512:
-            final_width = width
-            final_height = height
-            first_pass_ratio = min(final_height / 512, final_width / 512)
-            width = (int(final_width / first_pass_ratio) // 64) * 64
-            height = (int(final_height / first_pass_ratio) // 64) * 64
-            return (width, height)
-        return (width, height)
-
-    def _parameter_remap_basic_inference(
-        self,
-        payload: dict[str, str | None],
-    ) -> dict[str, str | None]:
-        params = self._parameter_remap(payload)
-
-        # XXX I think we need seed as an integer
-        try:
-            params["sampler.seed"] = int(params["sampler.seed"])
-        except ValueError:
-            # Now what? Pick a random one I guess?
-            params["sampler.seed"] = random.randint(0, sys.maxsize)
-
-        # Process dynamic prompts
-        if new_prompt := DynamicPromptParser(params["sampler.seed"]).parse(payload.get("prompt", "")):
-            payload["prompt"] = new_prompt
+                value = datatype(value)
+            except (ValueError, TypeError):
+                # epic fail, use the default
+                return default
+
+        # If the value must be divisible by some amount, assert that
+        if divisible:
+            if value % divisible != 0:
+                value = ((value + (divisible - 1)) // divisible) * divisible
+
+        # If we have a minimum, assert it
+        if min and value < min:
+            value = min
+
+        # If we have a maximum, assert it
+        if max and value > max:
+            value = max
+
+        # If we have a list of allowed values, make sure the value is permitted
+        if values:
+            if isinstance(value, str):
+                if value.lower() not in values:
+                    # not an allowed value, use the default
+                    return default
+                else:
+                    value = value.lower()
+            else:
+                if value not in values:
+                    # not an allowed value, use the default
+                    return default
+
+        return value
+
+    def _validate_data_structure(self, data, schema_definition=PAYLOAD_SCHEMA):
+        """Validate a data structure, assert parameters fall within the allowed bounds."""
+        data = deepcopy(data)
+
+        # Remove anything from the payload that isn't in our schema
+        for key in data.copy().keys():
+            if key.lower() not in schema_definition.keys():
+                del data[key]
+
+        # Build a valid schema payload, create attributes that don't exist using default values
+        for key, schema in schema_definition.items():
+            data[key.lower()] = self._validate(data.get(key.lower()), **schema)
+
+        # Do the same for loras, if we have loras in this data structure
+        if data.get("loras"):
+            for i, lora in enumerate(data.get("loras")):
+                data["loras"][i] = self._validate_data_structure(lora, HordeLib.LORA_SCHEMA)
+            # Remove invalid loras
+            data["loras"] = [x for x in data["loras"] if x.get("name")]
+
+        return data
+
+    def _apply_aihorde_compatibility_hacks(self, payload):
+        """For use by the AI Horde worker we require various counterintuitive hacks to the payload data.
+
+        We encapsulate all of this implicit witchcraft in one function, here.
+        """
+        payload = deepcopy(payload)
 
-        # karras flag determines which scheduler we use
+        # Rather than specify a scheduler, only karras or not karras is specified
         if payload.get("karras", False):
-            params["sampler.scheduler"] = "karras"
+            payload["scheduler"] = "karras"
         else:
-            params["sampler.scheduler"] = "normal"
-
-        # We break prompt up on horde's "###"
-        promptsCombined = payload.get("prompt", "")
-
-        if promptsCombined is None:  # XXX
-            raise TypeError("`None` value encountered!")
-
-        promptsSplit = [x.strip() for x in promptsCombined.split("###")][:2]
-        if len(promptsSplit) == 1:
-            params["prompt.text"] = promptsSplit[0]
-            params["negative_prompt.text"] = ""
-        elif len(promptsSplit) == 2:
-            params["prompt.text"] = promptsSplit[0]
-            params["negative_prompt.text"] = promptsSplit[1]
-
-        # Sampler remap
-        sampler = HordeLib.SAMPLERS_MAP.get(params["sampler.sampler_name"], "unknown")
-        if sampler == "unknown":
-            logger.warning(f"Unknown sampler {params['sampler.sampler_name']} defaulting to euler")
-            sampler = "euler"
-        params["sampler.sampler_name"] = sampler
-
-        # Clip skip inversion, comfy uses -1, -2, etc
-        clip_skip_key = "clip_skip.stop_at_clip_layer"
-        if params.get(clip_skip_key, 0) > 0:
-            params[clip_skip_key] = -params[clip_skip_key]
-
-        # If hires fix is enabled, use the same parameters as the main
-        # sampler in our upscale sampler.
-        if payload.get("hires_fix"):
-            params["upscale_sampler.seed"] = params["sampler.seed"]
-            params["upscale_sampler.scheduler"] = params["sampler.scheduler"]
-            params["upscale_sampler.cfg"] = params["sampler.cfg"]
-            params["upscale_sampler.steps"] = params["sampler.steps"]
-            params["upscale_sampler.sampler_name"] = params["sampler.sampler_name"]
-            if not params.get("upscale_sampler.denoise"):
-                params["upscale_sampler.denoise"] = 0.65  # XXX 0.65 default upscaler denoising strength
-            # Adjust image sizes
-            width = params.get("empty_latent_image.width", 0)
-            height = params.get("empty_latent_image.height", 0)
-            if width > 512 and height > 512:
-                newwidth, newheight = self._calculate_source_image_size(width, height)
-                params["latent_upscale.width"] = width
-                params["latent_upscale.height"] = height
-                params["empty_latent_image.width"] = newwidth
-                params["empty_latent_image.height"] = newheight
-                # Finally mark that we are using hires fix
-                params["hires_fix"] = True
-
-        # ControlNet?
-        if cnet := payload.get("control_type"):
-            # Determine the pre-processor that was requested
-            pre_processor = HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.get(cnet)
-            if not pre_processor:
-                logger.warning("Unknown controlnet pre-processor type {cnet} defaulting to canny")
-                pre_processor = "canny"
-
-            # The controlnet type becomes a direct parameter to the pipeline
-            # It is translated to its model as required my ComfyUI from the CN ModelManager
-            params["controlnet_model_loader.control_net_name"] = cnet
-
-            # For the pre-processor we dynamically reroute nodes in the pipeline later
-            params["control_type"] = pre_processor
-
-            # Remove the source_processing settings in case they conflict later
-            if "source_processing" in params:
-                del params["source_processing"]
-
-        # LORAs?
-        params["loras"] = payload.get("loras", [])
-
-        return params
-
-    # Fix any nonsensical requests
-    def _validate_inference_params(self, payload):
-
-        # Fix width/height not divisable by 64
-        if payload["width"] % 64 != 0:
-            payload["width"] = ((payload["width"] + 63) // 64) * 64
+            payload["scheduler"] = "normal"
 
-        if payload["height"] % 64 != 0:
-            payload["height"] = ((payload["height"] + 63) // 64) * 64
+        # Negative and positive prompts are merged together
+        if payload.get("prompt"):
+            split_prompts = [x.strip() for x in payload.get("prompt").split("###")][:2]
+            if len(split_prompts) == 2:
+                payload["prompt"] = split_prompts[0]
+                payload["negative_prompt"] = split_prompts[1]
 
-        # Turn off hires fix if we're not generating a hires image
-        if "hires_fix" in payload and (payload["width"] <= 512 or payload["height"] <= 512):
+        # Turn off hires fix if we're not generating a hires image, or if the params are just confused
+        try:
+            if "hires_fix" in payload and (payload["width"] <= 512 or payload["height"] <= 512):
+                payload["hires_fix"] = False
+        except (TypeError, KeyError):
             payload["hires_fix"] = False
 
-        # Remove source_processing if it's not valid
-        img_proc = payload.get("source_processing")
-        if img_proc and img_proc not in HordeLib.SOURCE_IMAGE_PROCESSING_OPTIONS:
-            del payload["source_processing"]
-        # Remove source image if we don't need it
-        if payload.get("source_image"):
-            if not img_proc or img_proc not in HordeLib.SOURCE_IMAGE_PROCESSING_OPTIONS:
-                del payload["source_image"]
-
-        # Turn off hires fix if we're painting as the dimensions are from the image
-        if "hires_fix" in payload and (img_proc == "inpainting" or img_proc == "outpainting"):
+        # Turn off hires fix if we're inpainting as the dimensions are from the source image
+        if "hires_fix" in payload and (
+            payload.get("source_processing") == "inpainting" or payload.get("source_processing") == "outpainting"
+        ):
             payload["hires_fix"] = False
 
-        # Use denoising strength for both samplers if no second denoiser specified in hires fix
+        # Use denoising strength for both samplers if no second denoiser specified
         # but not for txt2img where denoising will always generally be 1.0
         if payload.get("hires_fix"):
             if payload.get("source_processing") and payload.get("source_processing") != "txt2img":
                 if not payload.get("hires_fix_denoising_strength"):
                     payload["hires_fix_denoising_strength"] = payload.get("denoising_strength")
 
-        # Remap "denoising" to "controlnet strength" if that's what we actually wanted
+        # Remap "denoising" to "controlnet strength", historical hack
         if payload.get("control_type"):
             if payload.get("denoising_strength"):
                 if not payload.get("control_strength"):
                     payload["control_strength"] = payload["denoising_strength"]
                     del payload["denoising_strength"]
                 else:
                     del payload["denoising_strength"]
 
-    def _get_appropriate_pipeline(self, params):
-        # Determine the correct pipeline based on the parameters we have
-        pipeline = None
+        return payload
 
-        # ControlNet
-        if params.get("control_type"):
-            if params.get("return_control_map", False):
-                pipeline = "controlnet_annotator"
+    def _final_pipeline_adjustments(self, payload, pipeline_data):
+
+        payload = deepcopy(payload)
+
+        # Process dynamic prompts
+        if new_prompt := DynamicPromptParser(payload["seed"]).parse(payload.get("prompt", "")):
+            payload["prompt"] = new_prompt
+
+        # Clip skip inversion, comfy uses -1, -2, etc
+        if payload.get("clip_skip", 0) > 0:
+            payload["clip_skip"] = -payload["clip_skip"]
+
+        # Remap sampler name, horde to comfy
+        payload["sampler_name"] = HordeLib.SAMPLERS_MAP.get(payload["sampler_name"])
+
+        # Remap controlnet models, horde to comfy
+        if payload.get("control_type"):
+            payload["control_type"] = HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.get(payload.get("control_type"))
+
+        # Translate the payload parameters into pipeline parameters
+        pipeline_params = {}
+        for newkey, key in HordeLib.PAYLOAD_TO_PIPELINE_PARAMETER_MAPPING.items():
+            if key in payload:
+                pipeline_params[newkey] = payload.get(key)
             else:
-                if "hires_fix" in params:
-                    del params["hires_fix"]
-                    pipeline = "controlnet_hires_fix"
-                else:
-                    pipeline = "controlnet"
+                logger.error(f"Parameter {key} not found")
 
-            return pipeline
+        # Inject our model manager
+        pipeline_params["model_loader.model_manager"] = SharedModelManager
 
-        # Hires fix
-        if "hires_fix" in params:
-            del params["hires_fix"]
-            pipeline = "stable_diffusion_hires_fix"
-        else:
-            pipeline = "stable_diffusion"
+        # For hires fix, change the image sizes as we create an intermediate image first
+        if payload.get("hires_fix", False):
+            width = pipeline_params.get("empty_latent_image.width", 0)
+            height = pipeline_params.get("empty_latent_image.height", 0)
+            if width > 512 and height > 512:
+                newwidth, newheight = ImageUtils.calculate_source_image_size(width, height)
+                pipeline_params["latent_upscale.width"] = width
+                pipeline_params["latent_upscale.height"] = height
+                pipeline_params["empty_latent_image.width"] = newwidth
+                pipeline_params["empty_latent_image.height"] = newheight
+
+        # If we have a source image, use that rather than latent noise (i.e. img2img)
+        # We do this by reconnecting the nodes in the pipeline to make the input to the vae encoder
+        # the source image instead of the latent noise generator
+        if pipeline_params.get("image_loader.image"):
+            self.generator.reconnect_input(pipeline_data, "sampler.latent_image", "vae_encode")
 
-        # Source processing modes
-        source_proc = params.get("source_processing")
-        if source_proc:
-            del params["source_processing"]
-        if source_proc == "img2img":
-            # FIXME: Probably will have a different name from BASIC_INFERENCE_PARAMS
-            if params.get("source_mask"):
-                pipeline = "stable_diffusion_paint"
-            elif len(params.get("image_loader.image").split()) == 4:
-                pipeline = "stable_diffusion_paint"
-        elif source_proc == "inpainting":
-            pipeline = "stable_diffusion_paint"
-        elif source_proc == "outpainting":
-            pipeline = "stable_diffusion_paint"
-
-        return pipeline
-
-    def _add_image_alpha_channel(self, source_image, alpha_image):
-        # Convert images to RGBA mode
-        source_image = source_image.convert("RGBA")
-        # Convert alpha image to greyscale
-        alpha_image = alpha_image.convert("L")
-        # Resize alpha_image if its size is different from source_image
-        if alpha_image.size != source_image.size:
-            alpha_image = alpha_image.resize(source_image.size)
-        # Create a new alpha channel from the second image
-        alpha_image = ImageOps.invert(alpha_image)
-        alpha_data = alpha_image.split()[0]
-        source_image.putalpha(alpha_data)
-
-        # Return the resulting image
-        return source_image
-
-    def _resize_sources_to_request(self, payload):
-        """Ensures the source_image and source_mask are at the size requested by the client"""
-        source_image = payload.get("source_image")
-        if not source_image:
-            return
-        try:
-            newwidth = payload["width"]
-            newheight = payload["height"]
-            if payload.get("hires_fix") or payload.get("control_type"):
-                newwidth, newheight = self._calculate_source_image_size(payload["width"], payload["height"])
-            if source_image.size != (newwidth, newheight):
-                payload["source_image"] = source_image.resize(
-                    (newwidth, newheight),
-                    Image.Resampling.LANCZOS,
+        # Setup controlnet if required
+        if payload.get("control_type"):
+            # Inject control net model manager
+            pipeline_params["controlnet_model_loader.model_manager"] = SharedModelManager
+
+            # Dynamically reconnect nodes in the pipeline to connect the correct pre-processor node
+            if payload.get("return_control_map"):
+                # Connect annotator to output image directly if we need to return the control map
+                self.generator.reconnect_input(
+                    pipeline_data,
+                    "output_image.images",
+                    payload["control_type"],
                 )
-        except (UnidentifiedImageError, AttributeError):
-            logger.warning("Source image could not be parsed. Falling back to text2img")
-            del payload["source_image"]
-            del payload["source_processing"]
-            return
-
-        source_mask = payload.get("source_mask")
-        if not source_mask:
-            return
-        try:
-            if source_mask.size != (payload["width"], payload["height"]):
-                payload["source_mask"] = source_mask.resize(
-                    (payload["width"], payload["height"]),
+            else:
+                # Connect annotator to controlnet apply node
+                self.generator.reconnect_input(
+                    pipeline_data,
+                    "controlnet_apply.image",
+                    payload["control_type"],
                 )
-        except (UnidentifiedImageError, AttributeError):
-            logger.warning(
-                "Source mask could not be parsed. Falling back to img2img without mask",
-            )
-            del payload["source_mask"]
 
-        if payload.get("source_mask"):
-            payload["source_image"] = self._add_image_alpha_channel(payload["source_image"], payload["source_mask"])
+        # For LORAs we completely build the LORA section of the pipeline dynamically, as we have
+        # to handle n LORA models which form chained nodes in the pipeline.
+        # Note that we build this between several nodes, the model_loader, clip_skip and the sampler,
+        # plus the upscale sampler (used in hires fix) if there is one
+        if payload.get("loras"):
 
-    def _shrink_image(self, image, width, height, preserve_aspect=False):
-        # Check if the provided image is an instance of the PIL.Image.Image class
-        if not isinstance(image, Image.Image):
-            logger.warning("Bad image passed to shrink_image")
-            return
-
-        # If both width and height are not specified, return
-        if width is None and height is None:
-            logger.warning("Bad image size passed to shrink_image")
-            return
-
-        # Only shrink
-        if width >= image.width or height >= image.height:
-            return image
-
-        # Calculate new dimensions
-        if preserve_aspect:
-            aspect_ratio = float(image.width) / float(image.height)
+            for lora_index, lora in enumerate(payload.get("loras")):
 
-            if width is not None:
-                height = int(width / aspect_ratio)
-            else:
-                width = int(height * aspect_ratio)
+                # Inject a lora node (first lora)
+                if lora_index == 0:
+                    pipeline_data[f"lora_{lora_index}"] = {
+                        "inputs": {
+                            "model": ["model_loader", 0],
+                            "clip": ["model_loader", 1],
+                            "lora_name": f"{lora['name']}.safetensors",
+                            "strength_model": lora["model"],
+                            "strength_clip": lora["clip"],
+                        },
+                        "class_type": "LoraLoader",
+                    }
+                else:
+                    # Subsequent chained loras
+                    pipeline_data[f"lora_{lora_index}"] = {
+                        "inputs": {
+                            "model": [f"lora_{lora_index-1}", 0],
+                            "clip": [f"lora_{lora_index-1}", 1],
+                            "lora_name": f"{lora['name']}.safetensors",
+                            "strength_model": lora["model"],
+                            "strength_clip": lora["clip"],
+                        },
+                        "class_type": "LoraLoader",
+                    }
+
+            for lora_index, lora in enumerate(payload.get("loras")):
 
-        # Resize the image
-        resized_image = image.resize((width, height), Image.LANCZOS)
+                # The first LORA always connects to the model loader
+                if lora_index == 0:
+                    self.generator.reconnect_input(pipeline_data, "lora_0.model", "model_loader")
+                    self.generator.reconnect_input(pipeline_data, "lora_0.clip", "model_loader")
+                else:
+                    # Other loras connect to the previous lora
+                    self.generator.reconnect_input(
+                        pipeline_data,
+                        f"lora_{lora_index}.model",
+                        f"lora_{lora_index-1}.model",
+                    )
+                    self.generator.reconnect_input(
+                        pipeline_data,
+                        f"lora_{lora_index}.clip",
+                        f"lora_{lora_index-1}.clip",
+                    )
+
+                # The last LORA always connects to the sampler and clip text encoders (via the clip_skip)
+                if lora_index == len(payload.get("loras")) - 1:
+                    self.generator.reconnect_input(pipeline_data, "sampler.model", f"lora_{lora_index}")
+                    self.generator.reconnect_input(pipeline_data, "upscale_sampler.model", f"lora_{lora_index}")
+                    self.generator.reconnect_input(pipeline_data, "clip_skip.clip", f"lora_{lora_index}")
+
+        return pipeline_params
+
+    def _get_appropriate_pipeline(self, params):
+        # Determine the correct pipeline based on the parameters we have
+        #
+        # The pipelines are:
+        #
+        #     stable_diffusion
+        #       stable_diffusion_hires_fix
+        #     stable_diffusion_img2img_mask
+        #     stable_diffusion_paint
+        #     controlnet
+        #       controlnet_hires_fix
+        #       controlnet_annotator
+        #     image_facefix
+        #     image_upscale
 
-        return resized_image
+        # controlnet, controlnet_hires_fix controlnet_annotator
+        if params.get("control_type"):
+            if params.get("return_control_map", False):
+                return "controlnet_annotator"
+            else:
+                if params.get("hires_fix"):
+                    return "controlnet_hires_fix"
+                else:
+                    return "controlnet"
 
-    def _copy_image_metadata(self, src_image, dest_image):
-        metadata = src_image.info
-        pnginfo = PngImagePlugin.PngInfo()
-        for k, v in metadata.items():
-            if k not in ("dpi", "gamma", "transparency", "aspect"):
-                pnginfo.add_text(k, v)
-        dest_image.info["pnginfo"] = pnginfo
-        return dest_image
+        # stable_diffusion_paint, stable_diffusion_img2img_mask
+        if params.get("source_processing") == "img2img":
+            has_mask = params.get("source_mask") or (
+                params.get("source_image") and len(params.get("source_image", "").getbands()) == 4
+            )
+            if has_mask:
+                return "stable_diffusion_img2img_mask"
+        elif params.get("source_processing") == "inpainting":
+            return "stable_diffusion_paint"
+        elif params.get("source_processing") == "outpainting":
+            return "stable_diffusion_paint"
+
+        # stable_diffusion and stable_diffusion_hires_fix
+        if params.get("hires_fix", False):
+            return "stable_diffusion_hires_fix"
+        else:
+            return "stable_diffusion"  # also includes img2img mode
 
     def _process_results(self, images, rawpng):
         if images is None:
             return None  # XXX Log error and/or raise Exception here
         # Return image(s) or raw PNG bytestream
         if not rawpng:
             results = [Image.open(x["imagedata"]) for x in images]
@@ -473,71 +455,79 @@
         logger.debug(f"Locked models {','.join(models)}")
 
     def unlock_models(self, models):
         models = [x.strip() for x in models if x]
         self.generator.unlock_models(models)
         logger.debug(f"Unlocked models {','.join(models)}")
 
-    def basic_inference(self, payload: dict[str, str | None], rawpng=False) -> Image.Image | None:
-        # Check payload types
-        self._check_payload(payload)
-        # Validate our payload parameters
-        self._validate_inference_params(payload)
+    def basic_inference(self, payload, rawpng=False):
+        # AIHorde hacks to payload
+        payload = self._apply_aihorde_compatibility_hacks(payload)
+        # Check payload types/values and normalise it's format
+        payload = self._validate_data_structure(payload)
         # Resize the source image and mask to actual final width/height requested
-        self._resize_sources_to_request(payload)
-        # Determine our parameters
-        params = self._parameter_remap_basic_inference(payload)
-        # Determine the correct pipeline
-        pipeline = self._get_appropriate_pipeline(params)
+        ImageUtils.resize_sources_to_request(payload)
+        # Determine the correct pipeline to use
+        pipeline = self._get_appropriate_pipeline(payload)
+        # Final adjustments to the pipeline
+        pipeline_data = self.generator.get_pipeline_data(pipeline)
+        payload = self._final_pipeline_adjustments(payload, pipeline_data)
         # Run the pipeline
         try:
             # Add prefix to loras to avoid name collisions with other models
-            models = [f"lora-{x['name']}" for x in payload.get("loras", [])]
+            models = [f"lora-{x['name']}" for x in payload.get("loras", []) if x]
             # main model
             models.append(payload.get("model"))
             # controlnet model
             models.append(payload.get("control_type"))
             # Acquire a lock on all these models
             self.lock_models(models)
             # Call the inference pipeline
-            images = self.generator.run_image_pipeline(pipeline, params)
+            images = self.generator.run_image_pipeline(pipeline_data, payload)
         finally:
             self.unlock_models(models)
 
         return self._process_results(images, rawpng)
 
-    def image_upscale(self, payload: dict[str, str | None], rawpng=False) -> Image.Image | None:
-        # Check payload types
-        self._check_payload(payload)
-        # Determine our parameters
-        params = self._parameter_remap(payload)
-        # Determine the correct pipeline
-        pipeline = "image_upscale"
+    def image_upscale(self, payload, rawpng=False) -> Image.Image | None:
+        # AIHorde hacks to payload
+        payload = self._apply_aihorde_compatibility_hacks(payload)
+        # Remember if we were passed width and height, we wouldn't normally be passed width and height
+        # because the upscale models upscale to a fixed multiple of image size. However, if we *are*
+        # passed a width and height we rescale the upscale output image to this size.
+        width = payload.get("width")
+        height = payload.get("width")
+        # Check payload types/values and normalise it's format
+        payload = self._validate_data_structure(payload)
+        # Final adjustments to the pipeline
+        pipeline_name = "image_upscale"
+        pipeline_data = self.generator.get_pipeline_data(pipeline_name)
+        payload = self._final_pipeline_adjustments(payload, pipeline_data)
         # Run the pipeline
         try:
             self.lock_models([payload.get("model")])
-            images = self.generator.run_image_pipeline(pipeline, params)
+            images = self.generator.run_image_pipeline(pipeline_data, payload)
         finally:
             self.unlock_models([payload.get("model")])
         if images is None:
             return None  # XXX Log error and/or raise Exception here
-        # Allow arbitrary resizing
-        width = payload.get("width")
-        height = payload.get("height")
+        # Allow arbitrary resizing by shrinking the image back down
         if width or height:
-            return self._shrink_image(Image.open(images[0]["imagedata"]), width, height)
+            return ImageUtils.shrink_image(Image.open(images[0]["imagedata"]), width, height)
         return self._process_results(images, rawpng)
 
-    def image_facefix(self, payload: dict[str, str | None], rawpng=False) -> Image.Image | None:
-        # Check payload types
-        self._check_payload(payload)
-        # Determine our parameters
-        params = self._parameter_remap(payload)
-        # Determine the correct pipeline
-        pipeline = "image_facefix"
+    def image_facefix(self, payload, rawpng=False) -> Image.Image | None:
+        # AIHorde hacks to payload
+        payload = self._apply_aihorde_compatibility_hacks(payload)
+        # Check payload types/values and normalise it's format
+        payload = self._validate_data_structure(payload)
+        # Final adjustments to the pipeline
+        pipeline_name = "image_facefix"
+        pipeline_data = self.generator.get_pipeline_data(pipeline_name)
+        payload = self._final_pipeline_adjustments(payload, pipeline_data)
         # Run the pipeline
         try:
             self.lock_models([payload.get("model")])
-            images = self.generator.run_image_pipeline(pipeline, params)
+            images = self.generator.run_image_pipeline(pipeline_data, payload)
         finally:
             self.unlock_models([payload.get("model")])
         return self._process_results(images, rawpng)
```

### Comparing `hordelib-1.1.2/hordelib/initialisation.py` & `hordelib-1.2.0/hordelib/initialisation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/install_comfy.patch` & `hordelib-1.2.0/hordelib/install_comfy.patch`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/install_comfy.py` & `hordelib-1.2.0/hordelib/install_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_database/db_dep.json` & `hordelib-1.2.0/hordelib/model_database/db_dep.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_database/db_embeds.json` & `hordelib-1.2.0/hordelib/model_database/db_embeds.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_database/diffusers.json` & `hordelib-1.2.0/hordelib/model_database/diffusers.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/base.py` & `hordelib-1.2.0/hordelib/model_manager/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/blip.py` & `hordelib-1.2.0/hordelib/model_manager/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/clip.py` & `hordelib-1.2.0/hordelib/model_manager/clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/codeformer.py` & `hordelib-1.2.0/hordelib/model_manager/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/compvis.py` & `hordelib-1.2.0/hordelib/model_manager/compvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/controlnet.py` & `hordelib-1.2.0/hordelib/model_manager/controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/diffusers.py` & `hordelib-1.2.0/hordelib/model_manager/diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/esrgan.py` & `hordelib-1.2.0/hordelib/model_manager/esrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/gfpgan.py` & `hordelib-1.2.0/hordelib/model_manager/gfpgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/hyper.py` & `hordelib-1.2.0/hordelib/model_manager/hyper.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/model_manager/safety_checker.py` & `hordelib-1.2.0/hordelib/model_manager/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/README.md` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/comfy_controlnet_preprocessors/util.py` & `hordelib-1.2.0/hordelib/nodes/comfy_controlnet_preprocessors/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/__init__.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/__init__.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/align_trans.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/parsing/__init__.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/parsing/bisenet.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/parsing/parsenet.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/parsing/resnet.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/utils/face_utils.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/facerestore/facelib/utils/misc.py` & `hordelib-1.2.0/hordelib/nodes/facerestore/facelib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/node_clip_similarities.py` & `hordelib-1.2.0/hordelib/nodes/node_clip_similarities.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/node_controlnet_model_loader.py` & `hordelib-1.2.0/hordelib/nodes/node_controlnet_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/node_image_loader.py` & `hordelib-1.2.0/hordelib/nodes/node_image_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/node_image_output.py` & `hordelib-1.2.0/hordelib/nodes/node_image_output.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/node_model_loader.py` & `hordelib-1.2.0/hordelib/nodes/node_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/nodes/node_upscale_model_loader.py` & `hordelib-1.2.0/hordelib/nodes/node_upscale_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipeline_designs/pipeline_controlnet.json` & `hordelib-1.2.0/hordelib/pipeline_designs/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipeline_designs/pipeline_controlnet_annotator.json` & `hordelib-1.2.0/hordelib/pipeline_designs/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json` & `hordelib-1.2.0/hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipeline_designs/pipeline_image_facefix.json` & `hordelib-1.2.0/hordelib/pipeline_designs/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipeline_designs/pipeline_image_upscale.json` & `hordelib-1.2.0/hordelib/pipeline_designs/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipeline_designs/pipeline_stable_diffusion.json` & `hordelib-1.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json` & `hordelib-1.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json` & `hordelib-1.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipelines/pipeline_controlnet.json` & `hordelib-1.2.0/hordelib/pipelines/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipelines/pipeline_controlnet_annotator.json` & `hordelib-1.2.0/hordelib/pipelines/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipelines/pipeline_controlnet_hires_fix.json` & `hordelib-1.2.0/hordelib/pipelines/pipeline_controlnet_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipelines/pipeline_image_facefix.json` & `hordelib-1.2.0/hordelib/pipelines/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipelines/pipeline_image_upscale.json` & `hordelib-1.2.0/hordelib/pipelines/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-1.2.0/hordelib/pipelines/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-1.2.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/pipelines/pipeline_stable_diffusion_paint.json` & `hordelib-1.2.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/preload.py` & `hordelib-1.2.0/hordelib/preload.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/safety_checker.py` & `hordelib-1.2.0/hordelib/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/settings.py` & `hordelib-1.2.0/hordelib/settings.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/shared_model_manager.py` & `hordelib-1.2.0/hordelib/shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/train.py` & `hordelib-1.2.0/hordelib/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/utils/blip/blip.py` & `hordelib-1.2.0/hordelib/utils/blip/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/utils/blip/med.py` & `hordelib-1.2.0/hordelib/utils/blip/med.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/utils/blip/vit.py` & `hordelib-1.2.0/hordelib/utils/blip/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/utils/cast.py` & `hordelib-1.2.0/hordelib/utils/cast.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/utils/dynamicprompt.py` & `hordelib-1.2.0/hordelib/utils/dynamicprompt.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/utils/gpuinfo.py` & `hordelib-1.2.0/hordelib/utils/gpuinfo.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/utils/ioredirect.py` & `hordelib-1.2.0/hordelib/utils/ioredirect.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib/utils/logger.py` & `hordelib-1.2.0/hordelib/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/hordelib.egg-info/PKG-INFO` & `hordelib-1.2.0/hordelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 1.1.2
+Version: 1.2.0
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hordelib-1.1.2/hordelib.egg-info/SOURCES.txt` & `hordelib-1.2.0/hordelib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 examples/run_controlnet.py
 examples/run_controlnet_annotator.py
 examples/run_facefix.py
 examples/run_img2img.py
 examples/run_img2img_hires.py
 examples/run_img2img_inpaint.py
 examples/run_img2img_inpaint_mask.py
+examples/run_img2img_mask.py
 examples/run_img2img_outpaint.py
 examples/run_inpainting.py
 examples/run_kudos_test.py
 examples/run_long_prompt_check.py
 examples/run_lora.py
 examples/run_memory_test.py
 examples/run_stress_test_cnet.py
@@ -715,37 +716,41 @@
 hordelib/pipeline_designs/pipeline_controlnet.json
 hordelib/pipeline_designs/pipeline_controlnet_annotator.json
 hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json
 hordelib/pipeline_designs/pipeline_image_facefix.json
 hordelib/pipeline_designs/pipeline_image_upscale.json
 hordelib/pipeline_designs/pipeline_stable_diffusion.json
 hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+hordelib/pipeline_designs/pipeline_stable_diffusion_img2img_mask.json
 hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
 hordelib/pipelines/pipeline_controlnet.json
 hordelib/pipelines/pipeline_controlnet_annotator.json
 hordelib/pipelines/pipeline_controlnet_hires_fix.json
 hordelib/pipelines/pipeline_image_facefix.json
 hordelib/pipelines/pipeline_image_upscale.json
 hordelib/pipelines/pipeline_stable_diffusion.json
 hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+hordelib/pipelines/pipeline_stable_diffusion_img2img_mask.json
 hordelib/pipelines/pipeline_stable_diffusion_paint.json
 hordelib/utils/__init__.py
 hordelib/utils/cast.py
 hordelib/utils/dynamicprompt.py
 hordelib/utils/gpuinfo.py
+hordelib/utils/image_utils.py
 hordelib/utils/ioredirect.py
 hordelib/utils/logger.py
 hordelib/utils/switch.py
 hordelib/utils/blip/__init__.py
 hordelib/utils/blip/blip.py
 hordelib/utils/blip/med.py
 hordelib/utils/blip/vit.py
 images/test_annotator.jpg
 images/test_db0.jpg
 images/test_facefix.png
+images/test_img2img_alpha.png
 images/test_inpaint.png
 images/test_inpaint_alpha.png
 images/test_inpaint_mask.png
 images/test_inpaint_original.png
 images/test_outpaint.png
 tests/__init__.py
 tests/test_blip.py
@@ -760,14 +765,15 @@
 tests/test_horde_inference_painting.py
 tests/test_horde_lora.py
 tests/test_horde_pp.py
 tests/test_horde_samplers.py
 tests/test_image_metadata.py
 tests/test_inference.py
 tests/test_initialisation.py
+tests/test_payload_mapping.py
 tests/test_safety_checker.py
 tests/test_shared_model_manager.py
 tests/test_utils.py
 tests/meta/test_build_helper_import_check.py
 tests/model_managers/test_annotators.py
 tests/model_managers/test_comvis.py
 tests/model_managers/test_hyper.py
```

### Comparing `hordelib-1.1.2/images/test_db0.jpg` & `hordelib-1.2.0/images/test_db0.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/images/test_facefix.png` & `hordelib-1.2.0/images/test_facefix.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/images/test_inpaint.png` & `hordelib-1.2.0/images/test_inpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/images/test_inpaint_mask.png` & `hordelib-1.2.0/images/test_inpaint_mask.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/images/test_inpaint_original.png` & `hordelib-1.2.0/images/test_inpaint_original.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/images/test_outpaint.png` & `hordelib-1.2.0/images/test_outpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/pyproject.toml` & `hordelib-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/requirements.txt` & `hordelib-1.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/model_managers/test_annotators.py` & `hordelib-1.2.0/tests/model_managers/test_annotators.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/model_managers/test_comvis.py` & `hordelib-1.2.0/tests/model_managers/test_comvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/model_managers/test_hyper.py` & `hordelib-1.2.0/tests/model_managers/test_hyper.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/model_managers/test_safety_checker.py` & `hordelib-1.2.0/tests/model_managers/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/test_blip.py` & `hordelib-1.2.0/tests/test_blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/test_clip.py` & `hordelib-1.2.0/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/test_comfy.py` & `hordelib-1.2.0/tests/test_comfy.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,34 +56,14 @@
         }
         self.comfy._set(test_dict, **params)
         assert test_dict["a"]["inputs"]["b"]
         assert test_dict["c"]["inputs"]["d"]["e"]
         assert test_dict["c"]["inputs"]["d"]["f"]
         assert "unknown.parameter" not in test_dict
 
-    def test_parameter_bounds(self):
-        test_dict = {
-            "sampler.cfg": 0,
-            "sampler.denoise": 0,
-            "empty_latent_image.height": 10000,
-            "sampler.steps": 0.9,
-            "clip_skip.stop_at_clip_layer": 0,
-            "unknown.parameter": 9999,
-        }
-        expected = {
-            "sampler.cfg": 1,
-            "sampler.denoise": 0.1,
-            "empty_latent_image.height": 8192,
-            "sampler.steps": 1,
-            "clip_skip.stop_at_clip_layer": -1,
-            "unknown.parameter": 9999,
-        }
-        self.comfy._assert_parameter_bounds(test_dict)
-        assert test_dict == expected
-
     def test_fix_pipeline_types(self):
         data = {
             "node1": {"class_type": "ShouldNotBeReplaced"},
             "node2": {"no_class": "NoClassType"},
             "node3-should-be-replaced": {"class_type": "CheckpointLoaderSimple"},
         }
         data = self.comfy._fix_pipeline_types(data)
```

### Comparing `hordelib-1.1.2/tests/test_dynamic_prompt.py` & `hordelib-1.2.0/tests/test_dynamic_prompt.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/test_horde_controlnet_annotator.py` & `hordelib-1.2.0/tests/test_horde_controlnet_annotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,8 +69,8 @@
                     "stable diffusion 1",
                 )
                 is True
             )
             data["control_type"] = preproc
             pil_image = self.horde.basic_inference(data)
             assert pil_image is not None
-            pil_image.save(f"images/horde_annotator_{preproc}.webp", quality=90)
+            pil_image.save(f"images/annotator_{preproc}.webp", quality=90)
```

### Comparing `hordelib-1.1.2/tests/test_horde_inference.py` & `hordelib-1.2.0/tests/test_horde_inference_img2img.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,206 +13,223 @@
 
         TestHordeInference.default_model_manager_args = {
             # aitemplate
             # "blip": True,
             # "clip": True,
             # "codeformer": True,
             "compvis": True,
-            "controlnet": True,
+            # "controlnet": True,
             # "diffusers": True,
             # "esrgan": True,
             # "gfpgan": True,
             # "safety_checker": True,
         }
         SharedModelManager.loadModelManagers(**self.default_model_manager_args)
         assert SharedModelManager.manager is not None
         SharedModelManager.manager.load("Deliberate")
         yield
         del TestHordeInference.horde
         SharedModelManager._instance = None
         SharedModelManager.manager = None
 
-    def test_parameter_remap_basic_inference_simple(self):
+    def test_image_to_image(self):
         data = {
-            "sampler_name": "k_lms",
-            "cfg_scale": 5,
-            "denoising_strength": 0.75,
-            "seed": "23113",
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 0.4,
+            "seed": 666,
             "height": 512,
             "width": 512,
-            "karras": True,
+            "karras": False,
             "tiling": False,
             "hires_fix": False,
             "clip_skip": 1,
             "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
-            "prompt": "a dog ### cat, mouse, lion",
-            "ddim_steps": 30,
+            "prompt": "a dinosaur",
+            "ddim_steps": 25,
             "n_iter": 1,
             "model": "Deliberate",
-        }
-
-        expected = {
-            "sampler.sampler_name": "lms",
-            "sampler.cfg": 5,
-            "sampler.denoise": 0.75,
-            "sampler.seed": 23113,
-            "empty_latent_image.height": 512,
-            "empty_latent_image.width": 512,
-            "sampler.steps": 30,
-            "empty_latent_image.batch_size": 1,
-            "model_loader.model_name": "Deliberate",
-            "sampler.scheduler": "karras",
-            "prompt.text": "a dog",
-            "negative_prompt.text": "cat, mouse, lion",
-            "clip_skip.stop_at_clip_layer": -1,
-            "model_loader.model_manager": SharedModelManager,
-            "return_control_map": False,
-            "loras": [],
+            "source_image": Image.open("images/test_db0.jpg"),
+            "source_processing": "img2img",
         }
         assert self.horde is not None
-        result = self.horde._parameter_remap_basic_inference(data)
-        assert result == expected, f"Dictionaries don't match: {result} != {expected}"
+        pil_image = self.horde.basic_inference(data)
+        assert pil_image is not None
+        assert pil_image.size == (512, 512)
+        pil_image.save("images/image_to_image.webp", quality=90)
 
-    def test_parameter_remap_variation(self):
+    def test_image_to_image_hires_fix_small(self):
         data = {
-            "sampler_name": "k_lms",
-            "cfg_scale": 5,
-            "denoising_strength": 0.75,
-            "seed": "23113",
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 0.4,
+            "seed": 666,
             "height": 512,
             "width": 512,
             "karras": False,
             "tiling": False,
-            "hires_fix": False,
+            "hires_fix": True,
             "clip_skip": 1,
             "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
-            "prompt": "a dog",
-            "ddim_steps": 30,
+            "prompt": "a dinosaur",
+            "ddim_steps": 25,
             "n_iter": 1,
             "model": "Deliberate",
-        }
-
-        expected = {
-            "sampler.sampler_name": "lms",
-            "sampler.cfg": 5,
-            "sampler.denoise": 0.75,
-            "sampler.seed": 23113,
-            "empty_latent_image.height": 512,
-            "empty_latent_image.width": 512,
-            "sampler.steps": 30,
-            "empty_latent_image.batch_size": 1,
-            "model_loader.model_name": "Deliberate",
-            "sampler.scheduler": "normal",
-            "prompt.text": "a dog",
-            "negative_prompt.text": "",
-            "clip_skip.stop_at_clip_layer": -1,
-            "model_loader.model_manager": SharedModelManager,
-            "return_control_map": False,
-            "loras": [],
+            "source_image": Image.open("images/test_db0.jpg"),
+            "source_processing": "img2img",
         }
         assert self.horde is not None
-        result = self.horde._parameter_remap_basic_inference(data)
-        assert result == expected, f"Dictionaries don't match: {result} != {expected}"
+        pil_image = self.horde.basic_inference(data)
+        assert pil_image is not None
+        assert pil_image.size == (512, 512)
+        pil_image.save("images/image_to_image_hires_fix_small.webp", quality=90)
 
-    def test_text_to_image(self):
+    def test_image_to_image_hires_fix_large(self):
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
-            "denoising_strength": 1.0,
-            "seed": 123456789,
-            "height": 512.1,  # test param fix
-            "width": 512.1,  # test param fix
-            "karras": True,
+            "denoising_strength": 0.4,
+            "seed": 1312,
+            "height": 768,
+            "width": 768,
+            "karras": False,
             "tiling": False,
-            "hires_fix": False,
+            "hires_fix": True,
             "clip_skip": 1,
             "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
-            "prompt": "an ancient llamia monster",
+            "prompt": "a dinosaur",
             "ddim_steps": 25,
             "n_iter": 1,
             "model": "Deliberate",
+            "source_image": Image.open("images/test_db0.jpg"),
+            "source_processing": "img2img",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
-        pil_image.save("images/horde_text_to_image.webp", quality=90)
+        assert pil_image.size == (768, 768)
+        pil_image.save("images/image_to_image_hires_fix_large.webp", quality=90)
 
-    def test_text_to_image_small(self):
+    def test_img2img_masked_denoise_1(self):
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
-            "denoising_strength": 1.0,
-            "seed": 32323,
-            "height": 320,
-            "width": 320,
+            "denoising_strength": 1,
+            "seed": 24636666,
+            "height": 512,
+            "width": 512,
             "karras": True,
-            "tiling": False,
-            "hires_fix": False,
             "clip_skip": 1,
-            "control_type": None,
-            "image_is_control": False,
-            "return_control_map": False,
-            "prompt": "a photo of cute dinosaur ### painting, drawing, artwork, red border",
+            "prompt": "a mecha robot sitting on a bench",
             "ddim_steps": 20,
             "n_iter": 1,
             "model": "Deliberate",
+            "source_image": Image.open("images/test_img2img_alpha.png"),
+            "source_processing": "img2img",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
-        pil_image.save("images/horde_text_to_image_small.webp", quality=90)
+        assert pil_image.size == (512, 512)
+        pil_image.save("images/img2img_to_masked_denoise_1.webp", quality=90)
 
-    def test_text_to_image_clip_skip_2(self):
+    def test_img2img_masked_denoise_high(self):
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
-            "denoising_strength": 1.0,
-            "seed": 123456789,
+            "denoising_strength": 0.6,
+            "seed": 3,
             "height": 512,
             "width": 512,
             "karras": True,
-            "tiling": False,
-            "hires_fix": False,
-            "clip_skip": 2,
-            "control_type": None,
-            "image_is_control": False,
-            "return_control_map": False,
-            "prompt": "an ancient llamia monster",
-            "ddim_steps": 25,
+            "clip_skip": 1,
+            "prompt": "a mecha robot sitting on a bench",
+            "ddim_steps": 20,
+            "n_iter": 1,
+            "model": "Deliberate",
+            "source_image": Image.open("images/test_img2img_alpha.png"),
+            "source_processing": "img2img",
+        }
+        assert self.horde is not None
+        pil_image = self.horde.basic_inference(data)
+        assert pil_image is not None
+        assert pil_image.size == (512, 512)
+        pil_image.save("images/img2img_to_masked_denoise_0.6.webp", quality=90)
+
+    def test_img2img_masked_denoise_mid(self):
+        data = {
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 0.4,
+            "seed": 3,
+            "height": 512,
+            "width": 512,
+            "karras": True,
+            "clip_skip": 1,
+            "prompt": "a mecha robot sitting on a bench",
+            "ddim_steps": 20,
             "n_iter": 1,
             "model": "Deliberate",
+            "source_image": Image.open("images/test_img2img_alpha.png"),
+            "source_processing": "img2img",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
-        pil_image.save("images/horde_text_to_image_clip_skip_2.webp", quality=90)
+        assert pil_image.size == (512, 512)
+        pil_image.save("images/img2img_to_masked_denoise_0.4.webp", quality=90)
 
-    def test_text_to_image_hires_fix(self):
+    def test_img2img_masked_denoise_low(self):
+        data = {
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 0.2,
+            "seed": 3,
+            "height": 512,
+            "width": 512,
+            "karras": True,
+            "clip_skip": 1,
+            "prompt": "a mecha robot sitting on a bench",
+            "ddim_steps": 20,
+            "n_iter": 1,
+            "model": "Deliberate",
+            "source_image": Image.open("images/test_img2img_alpha.png"),
+            "source_processing": "img2img",
+        }
+        assert self.horde is not None
+        pil_image = self.horde.basic_inference(data)
+        assert pil_image is not None
+        assert pil_image.size == (512, 512)
+        pil_image.save("images/img2img_to_masked_denoise_0.2.webp", quality=90)
+
+    def test_image_to_faulty_source_image(self):
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
             "denoising_strength": 1.0,
             "seed": 123456789,
-            "height": 768,
-            "width": 768,
+            "height": 512.1,  # test param fix
+            "width": 512.1,  # test param fix
             "karras": True,
             "tiling": False,
-            "hires_fix": True,
+            "hires_fix": False,
             "clip_skip": 1,
             "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "an ancient llamia monster",
             "ddim_steps": 25,
             "n_iter": 1,
             "model": "Deliberate",
+            "source_image": "THIS SHOULD FAILOVER TO TEXT2IMG",
+            "source_processing": "img2img",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
-        pil_image.save("images/horde_text_to_image_hires_fix.webp", quality=90)
+        pil_image.save("images/img2img_fallback_to_txt2img.webp", quality=90)
```

### Comparing `hordelib-1.1.2/tests/test_horde_inference_controlnet.py` & `hordelib-1.2.0/tests/test_horde_inference_controlnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,28 +54,28 @@
             "model": "Deliberate",
             "source_image": Image.open("images/test_db0.jpg"),
             "source_processing": "img2img",
         }
         assert self.horde is not None
 
         for preproc in HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.keys():
-            if preproc == "scribble":
-                # Not valid for normal image input test
+            if preproc == "scribble" or preproc == "mlsd":
+                # Skip
                 continue
             assert (
                 SharedModelManager.manager.controlnet.check_control_type_available(
                     preproc,
                     "stable diffusion 1",
                 )
                 is True
             )
             data["control_type"] = preproc
             pil_image = self.horde.basic_inference(data)
             assert pil_image is not None
-            pil_image.save(f"images/horde_controlnet_{preproc}.webp", quality=90)
+            pil_image.save(f"images/controlnet_{preproc}.webp", quality=90)
 
     def test_controlnet_strength(self):
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
             "denoising_strength": 1.0,
             "seed": 123456789,
@@ -95,15 +95,15 @@
             "source_image": Image.open("images/test_db0.jpg"),
             "source_processing": "img2img",
         }
         for strength in [1.0, 0.5, 0.2]:
             data["control_strength"] = strength
             pil_image = self.horde.basic_inference(data)
             assert pil_image is not None
-            pil_image.save(f"images/horde_controlnet_strength_{strength}.webp", quality=90)
+            pil_image.save(f"images/controlnet_strength_{strength}.webp", quality=90)
 
     def test_controlnet_hires_fix(self):
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
             "denoising_strength": 1.0,
             "seed": 1234345378856789,
@@ -124,8 +124,8 @@
             "source_image": Image.open("images/test_db0.jpg"),
             "source_processing": "img2img",
         }
         for denoise in [0.4, 0.5, 0.6]:
             data["hires_fix_denoising_strength"] = denoise
             pil_image = self.horde.basic_inference(data)
             assert pil_image is not None
-            pil_image.save(f"images/horde_controlnet_hires_fix_denoise_{denoise}.webp", quality=90)
+            pil_image.save(f"images/controlnet_hires_fix_denoise_{denoise}.webp", quality=90)
```

### Comparing `hordelib-1.1.2/tests/test_horde_inference_painting.py` & `hordelib-1.2.0/tests/test_horde_inference.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,93 +3,130 @@
 from PIL import Image
 
 from hordelib.horde import HordeLib
 from hordelib.shared_model_manager import SharedModelManager
 
 
 class TestHordeInference:
-    @pytest.fixture(autouse=True)
+    @pytest.fixture(autouse=True, scope="class")
     def setup_and_teardown(self):
-        self.horde = HordeLib()
+        TestHordeInference.horde = HordeLib()
 
-        self.default_model_manager_args = {
+        TestHordeInference.default_model_manager_args = {
             # aitemplate
             # "blip": True,
             # "clip": True,
             # "codeformer": True,
             "compvis": True,
-            # "controlnet": True,
+            "controlnet": True,
             # "diffusers": True,
             # "esrgan": True,
             # "gfpgan": True,
             # "safety_checker": True,
         }
         SharedModelManager.loadModelManagers(**self.default_model_manager_args)
         assert SharedModelManager.manager is not None
+        SharedModelManager.manager.load("Deliberate")
         yield
-        del self.horde
+        del TestHordeInference.horde
         SharedModelManager._instance = None
         SharedModelManager.manager = None
 
-    def test_inpainting_alpha_mask(self):
-        SharedModelManager.manager.load("stable_diffusion_inpainting")
-        assert (
-            SharedModelManager.manager.compvis.is_model_loaded(
-                "stable_diffusion_inpainting",
-            )
-            is True
-        )
+    def test_text_to_image(self):
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
-            "denoising_strength": 0.6,
-            "seed": 3,
-            "height": 512,
-            "width": 512,
+            "denoising_strength": 1.0,
+            "seed": 123456789,
+            "height": 512.1,  # test param fix
+            "width": 512.1,  # test param fix
             "karras": True,
+            "tiling": False,
+            "hires_fix": False,
             "clip_skip": 1,
-            "prompt": "a mecha robot sitting on a bench",
+            "control_type": None,
+            "image_is_control": False,
+            "return_control_map": False,
+            "prompt": "an ancient llamia monster",
+            "ddim_steps": 25,
+            "n_iter": 1,
+            "model": "Deliberate",
+        }
+        assert self.horde is not None
+        pil_image = self.horde.basic_inference(data)
+        assert pil_image is not None
+        pil_image.save("images/text_to_image.webp", quality=90)
+
+    def test_text_to_image_small(self):
+        data = {
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 1.0,
+            "seed": 32323,
+            "height": 320,
+            "width": 320,
+            "karras": True,
+            "tiling": False,
+            "hires_fix": False,
+            "clip_skip": 1,
+            "control_type": None,
+            "image_is_control": False,
+            "return_control_map": False,
+            "prompt": "a photo of cute dinosaur ### painting, drawing, artwork, red border",
             "ddim_steps": 20,
             "n_iter": 1,
-            "model": "stable_diffusion_inpainting",
-            "source_image": Image.open("images/test_inpaint_alpha.png"),
-            "source_processing": "img2img",
+            "model": "Deliberate",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
-        pil_image.save("images/horde_inpainting_alpha_mask.webp", quality=90)
+        pil_image.save("images/text_to_image_small.webp", quality=90)
 
-    def test_inpainting_separate_mask(self):
-        SharedModelManager.manager.load("stable_diffusion_inpainting")
-        assert (
-            SharedModelManager.manager.compvis.is_model_loaded(
-                "stable_diffusion_inpainting",
-            )
-            is True
-        )
+    def test_text_to_image_clip_skip_2(self):
         data = {
-            "sampler_name": "euler",
-            "cfg_scale": 8,
-            "denoising_strength": 1,
-            "seed": 836138046008,
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 1.0,
+            "seed": 123456789,
             "height": 512,
             "width": 512,
-            "karras": False,
+            "karras": True,
             "tiling": False,
             "hires_fix": False,
+            "clip_skip": 2,
+            "control_type": None,
+            "image_is_control": False,
+            "return_control_map": False,
+            "prompt": "an ancient llamia monster",
+            "ddim_steps": 25,
+            "n_iter": 1,
+            "model": "Deliberate",
+        }
+        assert self.horde is not None
+        pil_image = self.horde.basic_inference(data)
+        assert pil_image is not None
+        pil_image.save("images/text_to_image_clip_skip_2.webp", quality=90)
+
+    def test_text_to_image_hires_fix(self):
+        data = {
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 1.0,
+            "seed": 123456789,
+            "height": 768,
+            "width": 768,
+            "karras": True,
+            "tiling": False,
+            "hires_fix": True,
             "clip_skip": 1,
             "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
-            "prompt": "a dinosaur",
-            "ddim_steps": 20,
+            "prompt": "an ancient llamia monster",
+            "ddim_steps": 25,
             "n_iter": 1,
-            "model": "stable_diffusion_inpainting",
-            "source_image": Image.open("images/test_inpaint_original.png"),
-            "source_mask": Image.open("images/test_inpaint_mask.png"),
-            "source_processing": "inpainting",
+            "model": "Deliberate",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
-        pil_image.save("images/horde_inpainting_separate_mask.webp", quality=90)
+        pil_image.save("images/text_to_image_hires_fix.webp", quality=90)
```

### Comparing `hordelib-1.1.2/tests/test_horde_lora.py` & `hordelib-1.2.0/tests/test_horde_lora.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,59 +18,14 @@
         assert SharedModelManager.manager is not None
         SharedModelManager.manager.load("Deliberate")
         yield
         del TestHordeLora.horde
         SharedModelManager._instance = None
         SharedModelManager.manager = None
 
-    def test_validate_payload(self):
-        data = {
-            "sampler_name": "k_lms",
-            "cfg_scale": 5,
-            "denoising_strength": 0.75,
-            "seed": "23113",
-            "height": 512,
-            "width": 512,
-            "karras": True,
-            "tiling": False,
-            "hires_fix": False,
-            "clip_skip": 1,
-            "control_type": None,
-            "image_is_control": False,
-            "return_control_map": False,
-            "prompt": "a dog ### cat, mouse, lion",
-            "ddim_steps": 30,
-            "n_iter": 1,
-            "model": "Deliberate",
-        }
-
-        assert self.horde is not None
-
-        # Missing key
-        result = data.copy()
-        self.horde._check_payload(result)
-        assert "loras" in result, "Failed to fix missing lora attribute in payload"
-
-        # Bad and good lora
-        data["loras"] = [
-            {"clip": "this is bad"},
-            {
-                "name": "briscou's gingers",
-                "model": 0.5,
-                "clip": 0.4,
-            },
-        ]
-        result = data.copy()
-        self.horde._check_payload(result)
-        assert "loras" in result, "Lost the lora attribute in our payload"
-        assert len(result["loras"]) == 1, "Unexpected number of loras in payload"
-        assert result["loras"][0]["name"] == "briscou's gingers", "We lost Briscou's gingers"
-        assert result["loras"][0]["model"] == 0.5, "Unexpected lora model weight"
-        assert result["loras"][0]["clip"] == 0.4, "Unexpected lora model clip"
-
     def test_text_to_image_lora_red(self):
 
         # Red
         data = {
             "sampler_name": "k_euler",
             "cfg_scale": 8.0,
             "denoising_strength": 1.0,
@@ -89,15 +44,15 @@
             "ddim_steps": 20,
             "n_iter": 1,
             "model": "Deliberate",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
-        pil_image.save("images/horde_lora_red.webp", quality=90)
+        pil_image.save("images/lora_red.webp", quality=90)
 
     def test_text_to_image_lora_blue(self):
 
         # Blue
         data = {
             "sampler_name": "k_euler",
             "cfg_scale": 8.0,
@@ -117,15 +72,15 @@
             "ddim_steps": 20,
             "n_iter": 1,
             "model": "Deliberate",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
-        pil_image.save("images/horde_lora_blue.webp", quality=90)
+        pil_image.save("images/lora_blue.webp", quality=90)
 
     def test_text_to_image_lora_chained(self):
 
         data = {
             "sampler_name": "k_euler",
             "cfg_scale": 8.0,
             "denoising_strength": 1.0,
@@ -147,8 +102,8 @@
             "ddim_steps": 20,
             "n_iter": 1,
             "model": "Deliberate",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
-        pil_image.save("images/horde_lora_multiple.webp", quality=90)
+        pil_image.save("images/lora_multiple.webp", quality=90)
```

### Comparing `hordelib-1.1.2/tests/test_horde_pp.py` & `hordelib-1.2.0/tests/test_horde_pp.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,57 +43,57 @@
         }
         assert self.horde is not None
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
         width, height = pil_image.size
         assert width == self.width * 4
         assert height == self.height * 4
-        pil_image.save("images/horde_image_upscale_RealESRGAN_x4plus.webp", quality=90)
+        pil_image.save("images/image_upscale_RealESRGAN_x4plus.webp", quality=90)
 
     @pytest.mark.mm_model("esrgan")
     def test_image_upscale_RealESRGAN_x2plus(self):
         SharedModelManager.manager.load("RealESRGAN_x2plus")
         assert SharedModelManager.manager.esrgan.is_model_loaded("RealESRGAN_x2plus") is True
         data = {
             "model": "RealESRGAN_x2plus",
             "source_image": self.image,
         }
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
         width, height = pil_image.size
         assert width == self.width * 2
         assert height == self.height * 2
-        pil_image.save("images/horde_image_upscale_RealESRGAN_x2plus.webp", quality=90)
+        pil_image.save("images/image_upscale_RealESRGAN_x2plus.webp", quality=90)
 
     @pytest.mark.mm_model("esrgan")
     def test_image_upscale_NMKD_Siax(self):
         SharedModelManager.manager.load("NMKD_Siax")
         assert SharedModelManager.manager.esrgan.is_model_loaded("NMKD_Siax") is True
         data = {
             "model": "NMKD_Siax",
             "source_image": self.image,
         }
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
         width, height = pil_image.size
         assert width == self.width * 4
         assert height == self.height * 4
-        pil_image.save("images/horde_image_upscale_NMKD_Siax.webp", quality=90)
+        pil_image.save("images/image_upscale_NMKD_Siax.webp", quality=90)
 
     @pytest.mark.mm_model("esrgan")
     def test_image_upscale_NMKD_Siax_resize(self):
         SharedModelManager.manager.load("NMKD_Siax")
         assert SharedModelManager.manager.esrgan.is_model_loaded("NMKD_Siax") is True
         data = {"model": "NMKD_Siax", "source_image": self.real_image, "width": 1280, "height": 1280}
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
         width, height = pil_image.size
         assert width == 1280
         assert height == 1280
-        pil_image.save("images/horde_image_upscale_NMKD_Siax_resize.webp", quality=90)
+        pil_image.save("images/image_upscale_NMKD_Siax_resize.webp", quality=90)
 
     @pytest.mark.mm_model("esrgan")
     def test_image_upscale_RealESRGAN_x4plus_anime_6B(self):
         SharedModelManager.manager.load("RealESRGAN_x4plus_anime_6B")
         assert (
             SharedModelManager.manager.esrgan.is_model_loaded(
                 "RealESRGAN_x4plus_anime_6B",
@@ -106,15 +106,15 @@
         }
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
         width, height = pil_image.size
         assert width == self.width * 4
         assert height == self.height * 4
         pil_image.save(
-            "images/horde_image_upscale_RealESRGAN_x4plus_anime_6B.webp",
+            "images/image_upscale_RealESRGAN_x4plus_anime_6B.webp",
             quality=90,
         )
 
     @pytest.mark.mm_model("esrgan")
     def test_image_upscale_4x_AnimeSharp(self):
         SharedModelManager.manager.load("4x_AnimeSharp")
         assert SharedModelManager.manager.esrgan.is_model_loaded("4x_AnimeSharp") is True
@@ -123,34 +123,34 @@
             "source_image": self.image,
         }
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
         width, height = pil_image.size
         assert width == self.width * 4
         assert height == self.height * 4
-        pil_image.save("images/horde_image_upscale_4x_AnimeSharp.webp", quality=90)
+        pil_image.save("images/image_upscale_4x_AnimeSharp.webp", quality=90)
 
     @pytest.mark.mm_model("codeformer")
     def test_image_facefix_codeformers(self):
         SharedModelManager.manager.load("CodeFormers")
         assert SharedModelManager.manager.codeformer.is_model_loaded("CodeFormers") is True
         data = {
             "model": "CodeFormers",
             "source_image": Image.open("images/test_facefix.png"),
         }
         pil_image = self.horde.image_facefix(data)
         assert pil_image is not None
         width, height = pil_image.size
-        pil_image.save("images/horde_image_facefix_codeformers.webp", quality=90)
+        pil_image.save("images/image_facefix_codeformers.webp", quality=90)
 
     @pytest.mark.mm_model("gfpgan")
     def test_image_facefix_gfpgan(self):
         SharedModelManager.manager.load("GFPGAN")
         assert SharedModelManager.manager.gfpgan.is_model_loaded("GFPGAN") is True
         data = {
             "model": "GFPGAN",
             "source_image": Image.open("images/test_facefix.png"),
         }
         pil_image = self.horde.image_facefix(data)
         assert pil_image is not None
         width, height = pil_image.size
-        pil_image.save("images/horde_image_facefix_gfpgan.webp", quality=90)
+        pil_image.save("images/image_facefix_gfpgan.webp", quality=90)
```

### Comparing `hordelib-1.1.2/tests/test_horde_samplers.py` & `hordelib-1.2.0/tests/test_horde_samplers.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,18 +43,18 @@
             ),
             "ddim_steps": 30,
             "n_iter": 1,
             "model": "Deliberate",
         }
         assert self.horde is not None
         for sampler in HordeLib.SAMPLERS_MAP.keys():
-            data["sampler_name"] = sampler
+            data["sampler_name"] = sampler.upper()  # force uppercase to ensure case insensitive
             pil_image = self.horde.basic_inference(data)
             assert pil_image is not None
-            pil_image.save(f"images/horde_sampler_30_steps_{sampler}.webp", quality=90)
+            pil_image.save(f"images/sampler_30_steps_{sampler}.webp", quality=90)
 
     def test_slow_samplers(self):
         data = {
             "sampler_name": "",
             "cfg_scale": 6.5,
             "denoising_strength": 1.0,
             "seed": 3688390309,
@@ -77,8 +77,8 @@
             "model": "Deliberate",
         }
         assert self.horde is not None
         for sampler in SLOW_SAMPLERS:
             data["sampler_name"] = sampler
             pil_image = self.horde.basic_inference(data)
             assert pil_image is not None
-            pil_image.save(f"images/horde_sampler_10_steps_{sampler}.webp", quality=90)
+            pil_image.save(f"images/sampler_10_steps_{sampler}.webp", quality=90)
```

### Comparing `hordelib-1.1.2/tests/test_image_metadata.py` & `hordelib-1.2.0/tests/test_image_metadata.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/test_inference.py` & `hordelib-1.2.0/tests/test_inference.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         SharedModelManager.manager.load("Deliberate")
         yield
         del TestInference.comfy
         SharedModelManager._instance = None
         SharedModelManager.manager = None
 
     def test_unknown_pipeline(self):
-        result = self.comfy.run_pipeline("non-existent-pipeline", {})
+        result = self.comfy.run_image_pipeline("non-existent-pipeline", {})
         assert result is None
 
     def test_stable_diffusion_pipeline(self):
         params = {
             "sampler.sampler_name": "dpmpp_2m",
             "sampler.cfg": 7.5,
             "sampler.denoise": 1.0,
@@ -35,14 +35,15 @@
             "empty_latent_image.batch_size": 1,
             "sampler.scheduler": "karras",
             "sampler.steps": 25,
             "prompt.text": "a closeup photo of a confused dog",
             "negative_prompt.text": "cat, black and white, deformed",
             "model_loader.model_name": "Deliberate",
             "clip_skip.stop_at_clip_layer": -1,
+            "model_loader.model_manager": SharedModelManager,
         }
         images = self.comfy.run_image_pipeline("stable_diffusion", params)
         assert images is not None
 
         image = Image.open(images[0]["imagedata"])
         image.save("images/pipeline_stable_diffusion.webp", quality=90)
 
@@ -57,91 +58,62 @@
             "empty_latent_image.batch_size": 1,
             "sampler.scheduler": "karras",
             "sampler.steps": 25,
             "prompt.text": "a closeup photo of a confused dog",
             "negative_prompt.text": "cat, black and white, deformed",
             "model_loader.model_name": "Deliberate",
             "clip_skip.stop_at_clip_layer": -2,
+            "model_loader.model_manager": SharedModelManager,
         }
         images = self.comfy.run_image_pipeline("stable_diffusion", params)
         assert images is not None
 
         image = Image.open(images[0]["imagedata"])
         image.save("images/pipeline_stable_diffusion_clip_skip_2.webp", quality=90)
 
     def test_stable_diffusion_hires_fix_pipeline(self):
         params = {
-            "sampler.seed": 1003,
+            "sampler.seed": 1014,
             "sampler.cfg": 7.5,
             "sampler.scheduler": "normal",
-            "sampler.sampler_name": "dpmpp_sde",
+            "sampler.sampler_name": "euler",
             "sampler.denoise": 1.0,
-            "sampler.steps": 20,
+            "sampler.steps": 30,
             "prompt.text": (
-                "photograph of medusa, reverence princesss, cinematic, realistic, "
+                "photograph of medusa, snakes in hair, reverence princesss, cinematic, realistic, "
                 "hyperrealistic, very realistic, extremely detailed, detailed, sharp focus, "
                 "establishing shot, 8k resolution, dramatic lighting, award winning "
                 "photograph, masterpiece, very detailed, sharp focus, very realistic lighting"
             ),
             "negative_prompt.text": (
                 "render, cg, drawing, painting, artist, graphics, deformed, black and white, deformed eyes"
             ),
             "model_loader.model_name": "Deliberate",
-            "empty_latent_image.width": 256,
-            "empty_latent_image.height": 256,
-            "latent_upscale.width": 512,
-            "latent_upscale.height": 512,
+            "model_loader.model_manager": SharedModelManager,
+            "empty_latent_image.width": 512,
+            "empty_latent_image.height": 512,
+            "latent_upscale.width": 768,
+            "latent_upscale.height": 768,
             "latent_upscale.crop": "disabled",
             "latent_upscale.upscale_method": "nearest-exact",
             "upscale_sampler.seed": 450089106307460,
-            "upscale_sampler.steps": 20,
+            "upscale_sampler.steps": 30,
             "upscale_sampler.cfg": 8.0,
-            "upscale_sampler.sampler_name": "dpmpp_2m",
+            "upscale_sampler.sampler_name": "euler",
             "upscale_sampler.scheduler": "simple",
-            "upscale_sampler.denoise": 0.5,
+            "upscale_sampler.denoise": 0.65,
             "clip_skip.stop_at_clip_layer": -1,
         }
         images = self.comfy.run_image_pipeline("stable_diffusion_hires_fix", params)
         assert images is not None
 
         image = Image.open(images[0]["imagedata"])
         image.save("images/pipeline_stable_diffusion_hires_fix.webp", quality=90)
 
-    def test_stable_diffusion_hires_fix_pipeline_clip_skip_2(self):
-        params = {
-            "sampler.seed": 1003,
-            "sampler.cfg": 7.5,
-            "sampler.scheduler": "normal",
-            "sampler.sampler_name": "dpmpp_sde",
-            "sampler.denoise": 1.0,
-            "sampler.steps": 20,
-            "prompt.text": (
-                "photograph of medusa, reverence princesss, cinematic, realistic, "
-                "hyperrealistic, very realistic, extremely detailed, detailed, sharp focus, "
-                "establishing shot, 8k resolution, dramatic lighting, award winning "
-                "photograph, masterpiece, very detailed, sharp focus, very realistic lighting"
-            ),
-            "negative_prompt.text": (
-                "render, cg, drawing, painting, artist, graphics, deformed, black and white, deformed eyes"
-            ),
-            "model_loader.model_name": "Deliberate",
-            "empty_latent_image.width": 256,
-            "empty_latent_image.height": 256,
-            "latent_upscale.width": 512,
-            "latent_upscale.height": 512,
-            "latent_upscale.crop": "disabled",
-            "latent_upscale.upscale_method": "nearest-exact",
-            "upscale_sampler.seed": 450089106307460,
-            "upscale_sampler.steps": 20,
-            "upscale_sampler.cfg": 8.0,
-            "upscale_sampler.sampler_name": "dpmpp_2m",
-            "upscale_sampler.scheduler": "simple",
-            "upscale_sampler.denoise": 0.5,
-            "clip_skip.stop_at_clip_layer": -1,
-        }
+        params["clip_skip.stop_at_clip_layer"] = -2
         images = self.comfy.run_image_pipeline("stable_diffusion_hires_fix", params)
         assert images is not None
 
         image = Image.open(images[0]["imagedata"])
         image.save(
             "images/pipeline_stable_diffusion_hires_fix_clip_skip_2.webp",
             quality=90,
```

### Comparing `hordelib-1.1.2/tests/test_safety_checker.py` & `hordelib-1.2.0/tests/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/test_shared_model_manager.py` & `hordelib-1.2.0/tests/test_shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tests/test_utils.py` & `hordelib-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.1.2/tox.ini` & `hordelib-1.2.0/tox.ini`

 * *Files identical despite different names*

