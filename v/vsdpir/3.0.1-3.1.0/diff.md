# Comparing `tmp/vsdpir-3.0.1-py3-none-any.whl.zip` & `tmp/vsdpir-3.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13520 bytes, number of entries: 12
--rw-r--r--  2.0 fat    14653 b- defN 20-Feb-02 00:00 vsdpir/__init__.py
+Zip file size: 13151 bytes, number of entries: 12
+-rw-r--r--  2.0 fat    12297 b- defN 20-Feb-02 00:00 vsdpir/__init__.py
 -rw-r--r--  2.0 fat      912 b- defN 20-Feb-02 00:00 vsdpir/__main__.py
 -rw-r--r--  2.0 fat    21548 b- defN 20-Feb-02 00:00 vsdpir/basicblock.py
--rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/drunet_color.pth
--rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/drunet_deblocking_color.pth
--rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/drunet_deblocking_gray.pth
--rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/drunet_gray.pth
 -rw-r--r--  2.0 fat     2757 b- defN 20-Feb-02 00:00 vsdpir/network_unet.py
-?rw-r--r--  2.0 fat     3055 b- defN 20-Feb-02 00:00 vsdpir-3.0.1.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 vsdpir-3.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1089 b- defN 20-Feb-02 00:00 vsdpir-3.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat      934 b- defN 20-Feb-02 00:00 vsdpir-3.0.1.dist-info/RECORD
-12 files, 45035 bytes uncompressed, 11952 bytes compressed:  73.5%
+-rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_color.pth
+-rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_deblocking_color.pth
+-rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_deblocking_gray.pth
+-rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_gray.pth
+?rw-r--r--  2.0 fat     3100 b- defN 20-Feb-02 00:00 vsdpir-3.1.0.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 vsdpir-3.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1089 b- defN 20-Feb-02 00:00 vsdpir-3.1.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat      962 b- defN 20-Feb-02 00:00 vsdpir-3.1.0.dist-info/RECORD
+12 files, 42752 bytes uncompressed, 11527 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -3,35 +3,35 @@
 
 Filename: vsdpir/__main__.py
 Comment: 
 
 Filename: vsdpir/basicblock.py
 Comment: 
 
-Filename: vsdpir/drunet_color.pth
+Filename: vsdpir/network_unet.py
 Comment: 
 
-Filename: vsdpir/drunet_deblocking_color.pth
+Filename: vsdpir/models/drunet_color.pth
 Comment: 
 
-Filename: vsdpir/drunet_deblocking_gray.pth
+Filename: vsdpir/models/drunet_deblocking_color.pth
 Comment: 
 
-Filename: vsdpir/drunet_gray.pth
+Filename: vsdpir/models/drunet_deblocking_gray.pth
 Comment: 
 
-Filename: vsdpir/network_unet.py
+Filename: vsdpir/models/drunet_gray.pth
 Comment: 
 
-Filename: vsdpir-3.0.1.dist-info/METADATA
+Filename: vsdpir-3.1.0.dist-info/METADATA
 Comment: 
 
-Filename: vsdpir-3.0.1.dist-info/WHEEL
+Filename: vsdpir-3.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: vsdpir-3.0.1.dist-info/licenses/LICENSE
+Filename: vsdpir-3.1.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: vsdpir-3.0.1.dist-info/RECORD
+Filename: vsdpir-3.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vsdpir/__init__.py

```diff
@@ -5,71 +5,58 @@
 from dataclasses import dataclass
 from threading import Lock
 
 import numpy as np
 import tensorrt
 import torch
 import torch.nn.functional as F
-import vapoursynth as vs
-from functorch.compile import memory_efficient_fusion
 from torch_tensorrt.fx import LowerSetting
 from torch_tensorrt.fx.lower import Lowerer
 from torch_tensorrt.fx.utils import LowerPrecision
-from vsutil import fallback
+from vstools import check_variable, fallback, vs
 
 from .network_unet import UNetRes
 
-__version__ = "3.0.1"
+__version__ = "3.1.0"
 
 os.environ["CUDA_MODULE_LOADING"] = "LAZY"
 
-package_dir = os.path.dirname(os.path.realpath(__file__))
+model_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "models")
 
 
 class Backend:
     @dataclass
     class Eager:
         module: torch.nn.Module
 
     @dataclass
-    class CUDAGraphs:
-        graph: list[torch.cuda.CUDAGraph]
-        static_input: list[torch.Tensor]
-        static_output: list[torch.Tensor]
-
-    @dataclass
     class TensorRT:
         module: list[torch.nn.Module]
 
 
 @torch.inference_mode()
 def dpir(
     clip: vs.VideoNode,
     device_index: int | None = None,
     num_streams: int = 1,
-    nvfuser: bool = False,
-    cuda_graphs: bool = False,
     trt: bool = False,
     trt_max_workspace_size: int = 1 << 30,
-    trt_cache_path: str = package_dir,
+    trt_cache_path: str = model_dir,
     task: str = "deblock",
     strength: float | vs.VideoNode | None = None,
     tile_w: int = 0,
     tile_h: int = 0,
     tile_pad: int = 8,
 ) -> vs.VideoNode:
     """Deep Plug-and-Play Image Restoration
 
     :param clip:                    Clip to process. Only RGBH/RGBS/GRAYH/GRAYS formats are supported. RGBH/GRAYH
                                     performs inference in FP16 mode while RGBS/GRAYS performs inference in FP32 mode.
     :param device_index:            Device ordinal of the GPU.
     :param num_streams:             Number of CUDA streams to enqueue the kernels.
-    :param nvfuser:                 Enable fusion through nvFuser. Not allowed in TensorRT. (experimental)
-    :param cuda_graphs:             Use CUDA Graphs to remove CPU overhead associated with launching CUDA kernels
-                                    sequentially. Not allowed in TensorRT.
     :param trt:                     Use TensorRT for high-performance inference.
     :param trt_max_workspace_size:  Maximum workspace size for TensorRT engine.
     :param trt_cache_path:          Path for TensorRT engine file. Engine will be cached when it's built for the first
                                     time. Note each engine is created for specific settings such as model path/name,
                                     precision, workspace etc, and specific GPUs and it's not portable.
     :param task:                    Task to perform. Must be 'deblock' or 'denoise'.
     :param strength:                Strength for deblocking/denoising.
@@ -77,49 +64,43 @@
                                     Also accepts a clip of GRAY format for varying strength.
     :param tile_w:                  Tile width. As too large images result in the out of GPU memory issue, so this tile
                                     option will first crop input images into tiles, and then process each of them.
                                     Finally, they will be merged into one image. 0 denotes for do not use tile.
     :param tile_h:                  Tile height.
     :param tile_pad:                Pad size for each tile, to remove border artifacts.
     """
-    if not isinstance(clip, vs.VideoNode):
-        raise vs.Error("dpir: this is not a clip")
+    assert check_variable(clip, dpir)
 
     if clip.format.id not in [vs.RGBH, vs.RGBS, vs.GRAYH, vs.GRAYS]:
         raise vs.Error("dpir: only RGBH/RGBS/GRAYH/GRAYS formats are supported")
 
     if not torch.cuda.is_available():
         raise vs.Error("dpir: CUDA is not available")
 
     if num_streams < 1:
         raise vs.Error("dpir: num_streams must be at least 1")
 
     if num_streams > vs.core.num_threads:
         raise vs.Error("dpir: setting num_streams greater than `core.num_threads` is useless")
 
-    if trt:
-        if nvfuser:
-            raise vs.Error("dpir: nvfuser and trt are mutually exclusive")
-
-        if cuda_graphs:
-            raise vs.Error("dpir: cuda_graphs and trt are mutually exclusive")
-
     task = task.lower()
 
     if task not in ["deblock", "denoise"]:
         raise vs.Error("dpir: task must be 'deblock' or 'denoise'")
 
     if isinstance(strength, vs.VideoNode):
+        assert check_variable(strength, dpir)
+
         if strength.format.color_family != vs.GRAY:
             raise vs.Error("dpir: strength must be of GRAY format")
 
         if strength.width != clip.width or strength.height != clip.height or strength.num_frames != clip.num_frames:
             raise vs.Error("dpir: strength must have the same dimensions and number of frames as main clip")
 
-    if os.path.getsize(os.path.join(package_dir, "drunet_color.pth")) == 0:
+    if os.path.getsize(os.path.join(model_dir, "drunet_color.pth")) == 0:
         raise vs.Error("dpir: model files have not been downloaded. run 'python -m vsdpir' first")
 
     torch.set_float32_matmul_precision("high")
 
     color_or_gray = "color" if clip.format.color_family == vs.RGB else "gray"
 
     fp16 = clip.format.bits_per_sample == 16
@@ -146,57 +127,30 @@
         model_name = f"drunet_{color_or_gray}.pth"
 
         if isinstance(strength, vs.VideoNode):
             noise = strength.std.Expr("x 255 /", format=noise_format)
         else:
             noise = clip.std.BlankClip(format=noise_format, color=fallback(strength, 5.0) / 255, keep=True)
 
-    model_path = os.path.join(package_dir, model_name)
+    model_path = os.path.join(model_dir, model_name)
 
     module = UNetRes(in_nc=clip.format.num_planes + 1, out_nc=clip.format.num_planes)
     module.load_state_dict(torch.load(model_path, map_location="cpu"))
     module.eval().to(device, memory_format=torch.channels_last)
     if fp16:
         module.half()
 
     if tile_w > 0 and tile_h > 0:
         pad_w = math.ceil(min(tile_w + 2 * tile_pad, clip.width) / 8) * 8
         pad_h = math.ceil(min(tile_h + 2 * tile_pad, clip.height) / 8) * 8
     else:
         pad_w = math.ceil(clip.width / 8) * 8
         pad_h = math.ceil(clip.height / 8) * 8
 
-    if nvfuser:
-        module = memory_efficient_fusion(module)
-
-    if cuda_graphs:
-        graph: list[torch.cuda.CUDAGraph] = []
-        static_input: list[torch.Tensor] = []
-        static_output: list[torch.Tensor] = []
-
-        for i in range(num_streams):
-            static_input.append(
-                torch.zeros((1, clip.format.num_planes + 1, pad_h, pad_w), dtype=dtype, device=device).to(
-                    memory_format=torch.channels_last
-                )
-            )
-
-            torch.cuda.synchronize(device=device)
-            stream[i].wait_stream(torch.cuda.current_stream(device=device))
-            with torch.cuda.stream(stream[i]):
-                module(static_input[i])
-            torch.cuda.current_stream(device=device).wait_stream(stream[i])
-            torch.cuda.synchronize(device=device)
-
-            graph.append(torch.cuda.CUDAGraph())
-            with torch.cuda.graph(graph[i], stream=stream[i]):
-                static_output.append(module(static_input[i]))
-
-        backend = Backend.CUDAGraphs(graph, static_input, static_output)
-    elif trt:
+    if trt:
         device_name = torch.cuda.get_device_name(device)
         trt_version = tensorrt.__version__
         dimensions = f"{pad_w}x{pad_h}"
         precision = "fp16" if fp16 else "fp32"
         trt_engine_path = os.path.join(
             os.path.realpath(trt_cache_path),
             (
@@ -254,19 +208,15 @@
 
             if tile_w > 0 and tile_h > 0:
                 output = tile_process(img, tile_w, tile_h, tile_pad, pad_w, pad_h, backend, local_index)
             else:
                 h, w = img.shape[2:]
                 img = F.pad(img, (0, pad_w - w, 0, pad_h - h), "reflect")
 
-                if cuda_graphs:
-                    static_input[local_index].copy_(img)
-                    graph[local_index].replay()
-                    output = static_output[local_index]
-                elif trt:
+                if trt:
                     output = module[local_index](img)
                 else:
                     output = module(img)
 
                 output = output[:, :, :h, :w]
 
             return tensor_to_frame(output, f[0].copy())
@@ -289,15 +239,15 @@
 def tile_process(
     img: torch.Tensor,
     tile_w: int,
     tile_h: int,
     tile_pad: int,
     pad_w: int,
     pad_h: int,
-    backend: Backend.Eager | Backend.CUDAGraphs | Backend.TensorRT,
+    backend: Backend.Eager | Backend.TensorRT,
     index: int,
 ) -> torch.Tensor:
     batch, channel, height, width = img.shape
     output_shape = (batch, channel - 1, height, width)
 
     # start with black image
     output = img.new_zeros(output_shape)
@@ -331,19 +281,15 @@
             input_tile = img[:, :, input_start_y_pad:input_end_y_pad, input_start_x_pad:input_end_x_pad]
 
             h, w = input_tile.shape[2:]
             mode = "reflect" if pad_w - w < w and pad_h - h < h else "replicate"
             input_tile = F.pad(input_tile, (0, pad_w - w, 0, pad_h - h), mode)
 
             # process tile
-            if isinstance(backend, Backend.CUDAGraphs):
-                backend.static_input[index].copy_(input_tile)
-                backend.graph[index].replay()
-                output_tile = backend.static_output[index]
-            elif isinstance(backend, Backend.TensorRT):
+            if isinstance(backend, Backend.TensorRT):
                 output_tile = backend.module[index](input_tile)
             else:
                 output_tile = backend.module(input_tile)
 
             output_tile = output_tile[:, :, :h, :w]
 
             # output tile area on total image
```

## Comparing `vsdpir-3.0.1.dist-info/METADATA` & `vsdpir-3.1.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsdpir
-Version: 3.0.1
+Version: 3.1.0
 Summary: DPIR function for VapourSynth
 Project-URL: Homepage, https://github.com/HolyWu/vs-dpir
 Project-URL: Bug Tracker, https://github.com/HolyWu/vs-dpir/issues
 Author-email: HolyWu <holywu@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2023 HolyWu
@@ -26,40 +26,40 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Keywords: DPIR,VapourSynth
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia :: Video
 Requires-Python: >=3.10
-Requires-Dist: numpy
-Requires-Dist: requests
-Requires-Dist: tensorrt>=8.5.3.1
-Requires-Dist: torch-tensorrt-fx-only>=1.3.0
-Requires-Dist: torch>=1.13.0
-Requires-Dist: tqdm
-Requires-Dist: vapoursynth>=55
-Requires-Dist: vsutil
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: requests>=2.30.0
+Requires-Dist: tensorrt>=8.6.1
+Requires-Dist: torch-tensorrt-fx-only>=1.5.0.dev0
+Requires-Dist: torch>=2.0.1
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: vapoursynth>=60
+Requires-Dist: vstools>=2.1.0
 Description-Content-Type: text/markdown
 
 # DPIR
 Plug-and-Play Image Restoration with Deep Denoiser Prior, based on https://github.com/cszn/DPIR.
 
 
 ## Dependencies
 - [NumPy](https://numpy.org/install)
-- [PyTorch](https://pytorch.org/get-started) 1.13
-- [VapourSynth](http://www.vapoursynth.com/) R55+
+- [PyTorch](https://pytorch.org/get-started) >=2.0.1
+- [VapourSynth](http://www.vapoursynth.com/) >=R60
 
 `trt` requires additional runtime libraries:
-- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 11.7
-- [cuDNN](https://developer.nvidia.com/cudnn) 8.6
-- [TensorRT](https://developer.nvidia.com/tensorrt) 8.5.3.1
+- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 11.8
+- [cuDNN](https://developer.nvidia.com/cudnn) 8.9
+- [TensorRT](https://developer.nvidia.com/tensorrt) >=8.6.1.6
 
 For ease of installation on Windows, you can download the 7z file on [Releases](https://github.com/HolyWu/vs-dpir/releases) which contains required runtime libraries and Python wheel file. Either add the unzipped directory to your system `PATH` or copy the DLL files to a directory which is already in your system `PATH`. Finally pip install the Python wheel file.
 
 
 ## Installation
 ```
 pip install -U vsdpir
```

## Comparing `vsdpir-3.0.1.dist-info/licenses/LICENSE` & `vsdpir-3.1.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `vsdpir-3.0.1.dist-info/RECORD` & `vsdpir-3.1.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-vsdpir/__init__.py,sha256=p2179CzQpGOmH-I1scnOrxuNjnNLUjMFiIEluS3ZW28,14653
+vsdpir/__init__.py,sha256=EmxC5LFDgCsdC3OTCrNQyGeckm0hdDXBzBtAXxIh25A,12297
 vsdpir/__main__.py,sha256=2t6FJP1a3X8Ut4czODKF0qV9bUIHV_tT2FGS88ZE83E,912
 vsdpir/basicblock.py,sha256=JgSHEeEWi4t2x1ZlDzjbQA2PH5gSECaN83ql0cN3Ptw,21548
-vsdpir/drunet_color.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vsdpir/drunet_deblocking_color.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vsdpir/drunet_deblocking_gray.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vsdpir/drunet_gray.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsdpir/network_unet.py,sha256=4WzY7UAmfMlhYazd-tfeOOIz_mktNcU_OL4ZrgTJoY8,2757
-vsdpir-3.0.1.dist-info/METADATA,sha256=bnAXaJIoEYPF5qpUNVbap9TykWKbSpodl9w6zrukp5Y,3055
-vsdpir-3.0.1.dist-info/WHEEL,sha256=Fd6mP6ydyRguakwUJ05oBE7fh2IPxgtDN9IwHJ9OqJQ,87
-vsdpir-3.0.1.dist-info/licenses/LICENSE,sha256=cgEoXz2kbESametJVH_uTy_eWfVY2ZCwfL6SOyI63bM,1089
-vsdpir-3.0.1.dist-info/RECORD,,
+vsdpir/models/drunet_color.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+vsdpir/models/drunet_deblocking_color.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+vsdpir/models/drunet_deblocking_gray.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+vsdpir/models/drunet_gray.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+vsdpir-3.1.0.dist-info/METADATA,sha256=-p6-1hg8Y-axgtN71B4RR16oiEHfRs569l3_8Ir9VZA,3100
+vsdpir-3.1.0.dist-info/WHEEL,sha256=y1bSCq4r5i4nMmpXeUJMqs3ipKvkZObrIXSvJHm1qCI,87
+vsdpir-3.1.0.dist-info/licenses/LICENSE,sha256=cgEoXz2kbESametJVH_uTy_eWfVY2ZCwfL6SOyI63bM,1089
+vsdpir-3.1.0.dist-info/RECORD,,
```

