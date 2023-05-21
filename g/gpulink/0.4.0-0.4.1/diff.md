# Comparing `tmp/gpulink-0.4.0.tar.gz` & `tmp/gpulink-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpulink-0.4.0.tar", last modified: Sun May 21 15:03:54 2023, max compression
+gzip compressed data, was "gpulink-0.4.1.tar", last modified: Sun May 21 15:26:41 2023, max compression
```

## Comparing `gpulink-0.4.0.tar` & `gpulink-0.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.754887 gpulink-0.4.0/
--rw-rw-rw-   0        0        0     1088 2022-07-18 07:04:47.000000 gpulink-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       15 2022-07-18 07:04:47.000000 gpulink-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5180 2023-05-21 15:03:54.753887 gpulink-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4653 2023-05-21 15:01:56.000000 gpulink-0.4.0/PYPI.md
--rw-rw-rw-   0        0        0     7303 2023-05-21 15:01:53.000000 gpulink-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.705715 gpulink-0.4.0/gpulink/
--rw-rw-rw-   0        0        0      387 2023-05-21 14:59:07.000000 gpulink-0.4.0/gpulink/__init__.py
--rw-rw-rw-   0        0        0      402 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.725714 gpulink-0.4.0/gpulink/cli/
--rw-rw-rw-   0        0        0        0 2022-07-18 07:04:47.000000 gpulink-0.4.0/gpulink/cli/__init__.py
--rw-rw-rw-   0        0        0     5440 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/cli/cmd_record.py
--rw-rw-rw-   0        0        0     3486 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/cli/cmd_sensors.py
--rw-rw-rw-   0        0        0      209 2023-05-21 15:00:12.000000 gpulink-0.4.0/gpulink/cli/console.py
--rw-rw-rw-   0        0        0       79 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/consts.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.734887 gpulink-0.4.0/gpulink/devices/
--rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/devices/__init__.py
--rw-rw-rw-   0        0        0     1427 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/devices/base_device.py
--rw-rw-rw-   0        0        0     4253 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/devices/devicectx.py
--rw-rw-rw-   0        0        0      799 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/devices/gpu.py
--rw-rw-rw-   0        0        0      751 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/devices/nvml_defines.py
--rw-rw-rw-   0        0        0     4469 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/devices/nvml_device.py
--rw-rw-rw-   0        0        0      597 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/devices/query.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.738886 gpulink-0.4.0/gpulink/plotting/
--rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/plotting/__init__.py
--rw-rw-rw-   0        0        0     2941 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/plotting/plot.py
--rw-rw-rw-   0        0        0      659 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/plotting/plot_options.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.744891 gpulink-0.4.0/gpulink/recording/
--rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/recording/__init__.py
--rw-rw-rw-   0        0        0     1858 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/recording/gpu_recording.py
--rw-rw-rw-   0        0        0     8079 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/recording/recorder.py
--rw-rw-rw-   0        0        0      774 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/recording/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.746891 gpulink-0.4.0/gpulink/threading/
--rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/threading/__init__.py
--rw-rw-rw-   0        0        0      377 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/threading/stoppable_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.717714 gpulink-0.4.0/gpulink.egg-info/
--rw-rw-rw-   0        0        0     5180 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1011 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      130 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-07-18 07:04:47.000000 gpulink-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 15:03:54.754887 gpulink-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1912 2023-05-21 14:49:27.000000 gpulink-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.752887 gpulink-0.4.0/tests/
--rw-rw-rw-   0        0        0      510 2022-07-21 20:40:05.000000 gpulink-0.4.0/tests/test_dataclasses.py
--rw-rw-rw-   0        0        0     4071 2022-07-21 20:40:05.000000 gpulink-0.4.0/tests/test_device_context.py
--rw-rw-rw-   0        0        0     4983 2022-07-21 20:40:05.000000 gpulink-0.4.0/tests/test_nvml_device.py
--rw-rw-rw-   0        0        0     3105 2022-07-21 20:40:05.000000 gpulink-0.4.0/tests/test_plot.py
--rw-rw-rw-   0        0        0     1951 2023-05-21 14:49:23.000000 gpulink-0.4.0/tests/test_recorder.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:26:41.167887 gpulink-0.4.1/
+-rw-rw-rw-   0        0        0     1088 2022-07-18 07:04:47.000000 gpulink-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0       15 2022-07-18 07:04:47.000000 gpulink-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5180 2023-05-21 15:26:41.166887 gpulink-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4653 2023-05-21 15:01:56.000000 gpulink-0.4.1/PYPI.md
+-rw-rw-rw-   0        0        0     7398 2023-05-21 15:19:01.000000 gpulink-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 15:26:41.126894 gpulink-0.4.1/gpulink/
+-rw-rw-rw-   0        0        0      387 2023-05-21 15:17:42.000000 gpulink-0.4.1/gpulink/__init__.py
+-rw-rw-rw-   0        0        0      402 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:26:41.138892 gpulink-0.4.1/gpulink/cli/
+-rw-rw-rw-   0        0        0        0 2022-07-18 07:04:47.000000 gpulink-0.4.1/gpulink/cli/__init__.py
+-rw-rw-rw-   0        0        0     5440 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/cli/cmd_record.py
+-rw-rw-rw-   0        0        0     3486 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/cli/cmd_sensors.py
+-rw-rw-rw-   0        0        0      209 2023-05-21 15:00:12.000000 gpulink-0.4.1/gpulink/cli/console.py
+-rw-rw-rw-   0        0        0       79 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/consts.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:26:41.147889 gpulink-0.4.1/gpulink/devices/
+-rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.1/gpulink/devices/__init__.py
+-rw-rw-rw-   0        0        0     1427 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/devices/base_device.py
+-rw-rw-rw-   0        0        0     4253 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/devices/devicectx.py
+-rw-rw-rw-   0        0        0      799 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/devices/gpu.py
+-rw-rw-rw-   0        0        0      751 2022-07-21 20:40:05.000000 gpulink-0.4.1/gpulink/devices/nvml_defines.py
+-rw-rw-rw-   0        0        0     4453 2023-05-21 15:16:12.000000 gpulink-0.4.1/gpulink/devices/nvml_device.py
+-rw-rw-rw-   0        0        0      597 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/devices/query.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:26:41.151893 gpulink-0.4.1/gpulink/plotting/
+-rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.1/gpulink/plotting/__init__.py
+-rw-rw-rw-   0        0        0     2941 2022-07-21 20:40:05.000000 gpulink-0.4.1/gpulink/plotting/plot.py
+-rw-rw-rw-   0        0        0      659 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/plotting/plot_options.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:26:41.157889 gpulink-0.4.1/gpulink/recording/
+-rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.1/gpulink/recording/__init__.py
+-rw-rw-rw-   0        0        0     1858 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/recording/gpu_recording.py
+-rw-rw-rw-   0        0        0     8079 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/recording/recorder.py
+-rw-rw-rw-   0        0        0      774 2023-05-21 14:49:23.000000 gpulink-0.4.1/gpulink/recording/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:26:41.159888 gpulink-0.4.1/gpulink/threading/
+-rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.1/gpulink/threading/__init__.py
+-rw-rw-rw-   0        0        0      377 2022-07-21 20:40:05.000000 gpulink-0.4.1/gpulink/threading/stoppable_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:26:41.133890 gpulink-0.4.1/gpulink.egg-info/
+-rw-rw-rw-   0        0        0     5180 2023-05-21 15:26:41.000000 gpulink-0.4.1/gpulink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1011 2023-05-21 15:26:41.000000 gpulink-0.4.1/gpulink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 15:26:41.000000 gpulink-0.4.1/gpulink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-21 15:26:41.000000 gpulink-0.4.1/gpulink.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-05-21 15:26:41.000000 gpulink-0.4.1/gpulink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 15:26:41.000000 gpulink-0.4.1/gpulink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-07-18 07:04:47.000000 gpulink-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 15:26:41.167887 gpulink-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1912 2023-05-21 15:12:33.000000 gpulink-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:26:41.165887 gpulink-0.4.1/tests/
+-rw-rw-rw-   0        0        0      510 2022-07-21 20:40:05.000000 gpulink-0.4.1/tests/test_dataclasses.py
+-rw-rw-rw-   0        0        0     4071 2022-07-21 20:40:05.000000 gpulink-0.4.1/tests/test_device_context.py
+-rw-rw-rw-   0        0        0     4982 2023-05-21 15:23:13.000000 gpulink-0.4.1/tests/test_nvml_device.py
+-rw-rw-rw-   0        0        0     3105 2022-07-21 20:40:05.000000 gpulink-0.4.1/tests/test_plot.py
+-rw-rw-rw-   0        0        0     1951 2023-05-21 14:49:23.000000 gpulink-0.4.1/tests/test_recorder.py
```

### Comparing `gpulink-0.4.0/LICENSE` & `gpulink-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/PKG-INFO` & `gpulink-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpulink
-Version: 0.4.0
+Version: 0.4.1
 Summary: A simple tool for monitoring and displaying GPU stats
 Home-page: https://github.com/PhilipKlaus/gpu-link
 Author: Philip Klaus
 Project-URL: Bug Tracker, https://github.com/PhilipKlaus/gpu-link/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gpulink-0.4.0/PYPI.md` & `gpulink-0.4.1/PYPI.md`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/README.md` & `gpulink-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -156,12 +156,14 @@
   typing `nvidia-smi --version` into a terminal:  
   ```pynvml.nvml.NVMLError_LibraryNotFound: NVML Shared Library Not Found```.  
 
 ## Planned features
 - Live-plotting of GPU stats
 
 ## Changelog 
-- 0.4.0
+- **0.4.0**
     - Recording arbitrary GPU stats (clock, fan-speed, memory, power-usage, temp)
     - Display GPU name and power usage within `sensors` command
     - Replaced `arparse` library by [click](https://click.palletsprojects.com/en/8.1.x/)
     - Aborting a `watch` or `recording` command can be done by pressing any instead of `ctrl+c`
+- **0.4.1**
+    - Fix error when calling `nvmlDeviceGetName` in `pynvml` version *11.5.0*
```

### Comparing `gpulink-0.4.0/gpulink/cli/cmd_record.py` & `gpulink-0.4.1/gpulink/cli/cmd_record.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/cli/cmd_sensors.py` & `gpulink-0.4.1/gpulink/cli/cmd_sensors.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/devices/base_device.py` & `gpulink-0.4.1/gpulink/devices/base_device.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/devices/devicectx.py` & `gpulink-0.4.1/gpulink/devices/devicectx.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/devices/gpu.py` & `gpulink-0.4.1/gpulink/devices/gpu.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/devices/nvml_defines.py` & `gpulink-0.4.1/gpulink/devices/nvml_defines.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/devices/nvml_device.py` & `gpulink-0.4.1/gpulink/devices/nvml_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._device_ids = []
 
     def _get_device_handles(self):
         self._device_ids = [i for i in range(nvmlDeviceGetCount())]
         for dev in self._device_ids:
             handle = nvmlDeviceGetHandleByIndex(dev)
             self._device_handles.append(handle)
-            self._device_names.append(nvmlDeviceGetName(handle).decode("utf-8"))
+            self._device_names.append(nvmlDeviceGetName(handle))
 
     def _execute(self, query, type: Type, gpus: List[int], *args, **kwargs) -> List[QueryResult]:
         if not gpus or len(gpus) == 0:
             gpus = self._device_ids
             handles = self._device_handles
             gpu_names = self._device_names
         else:
```

### Comparing `gpulink-0.4.0/gpulink/devices/query.py` & `gpulink-0.4.1/gpulink/devices/query.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/plotting/plot.py` & `gpulink-0.4.1/gpulink/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/plotting/plot_options.py` & `gpulink-0.4.1/gpulink/plotting/plot_options.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/recording/gpu_recording.py` & `gpulink-0.4.1/gpulink/recording/gpu_recording.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/recording/recorder.py` & `gpulink-0.4.1/gpulink/recording/recorder.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink/recording/timeseries.py` & `gpulink-0.4.1/gpulink/recording/timeseries.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/gpulink.egg-info/PKG-INFO` & `gpulink-0.4.1/gpulink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpulink
-Version: 0.4.0
+Version: 0.4.1
 Summary: A simple tool for monitoring and displaying GPU stats
 Home-page: https://github.com/PhilipKlaus/gpu-link
 Author: Philip Klaus
 Project-URL: Bug Tracker, https://github.com/PhilipKlaus/gpu-link/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gpulink-0.4.0/gpulink.egg-info/SOURCES.txt` & `gpulink-0.4.1/gpulink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/setup.py` & `gpulink-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,19 +44,19 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=['gpulink', 'gpulink.cli', 'gpulink.devices', 'gpulink.plotting', 'gpulink.recording',
               'gpulink.threading'],
     python_requires=">=3.7",
     install_requires=[
-        "pynvml >= 11.4.1",
-        "matplotlib >= 3.5.1",
-        "numpy >= 1.22.2",
-        "tabulate >= 0.8.9",
-        "colorama >= 0.4.4",
+        "pynvml == 11.5.0",
+        "matplotlib >= 3.7.1",
+        "numpy >= 1.24.3",
+        "tabulate >= 0.9.0",
+        "colorama >= 0.4.6",
         "click >= 8.1.3"
     ],
     tests_require=tests_require,
     extras_require={"test": tests_require},
     entry_points={
         'console_scripts': ['gpulink=gpulink.__main__:main'],
     },
```

### Comparing `gpulink-0.4.0/tests/test_device_context.py` & `gpulink-0.4.1/tests/test_device_context.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/tests/test_nvml_device.py` & `gpulink-0.4.1/tests/test_nvml_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 def patch_nvcontext(mocker):
     time = 0
     mocker.patch("gpulink.devices.nvml_device.time_ns", return_value=time)
     mocker.patch("gpulink.devices.nvml_device.nvmlInit")
     mocker.patch("gpulink.devices.nvml_device.nvmlShutdown")
     mocker.patch("gpulink.devices.nvml_device.nvmlDeviceGetCount", return_value=2)
     mocker.patch("gpulink.devices.nvml_device.nvmlDeviceGetHandleByIndex")
-    mocker.patch("gpulink.devices.nvml_device.nvmlDeviceGetName", return_value=b"GPU_TEST")
+    mocker.patch("gpulink.devices.nvml_device.nvmlDeviceGetName", return_value="GPU_TEST")
     mocker.patch("gpulink.devices.nvml_device.nvmlDeviceGetMemoryInfo",
                  return_value=MemoryInfo(total=_GB, used=_GB // 2, free=_GB // 2))
     mocker.patch("gpulink.devices.nvml_device.nvmlDeviceGetFanSpeed", return_value=_FAN_SPEED_PCT)
     mocker.patch("gpulink.devices.nvml_device.nvmlDeviceGetFanSpeed_v2", return_value=_FAN_SPEED_PCT // 2)
     mocker.patch("gpulink.devices.nvml_device.nvmlDeviceGetTemperature", return_value=_TMP)
     mocker.patch("gpulink.devices.nvml_device.nvmlDeviceGetTemperatureThreshold", return_value=_TMP // 2)
     mocker.patch("gpulink.devices.nvml_device.nvmlDeviceGetClock", return_value=_CLOCK // 2)
```

### Comparing `gpulink-0.4.0/tests/test_plot.py` & `gpulink-0.4.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.4.0/tests/test_recorder.py` & `gpulink-0.4.1/tests/test_recorder.py`

 * *Files identical despite different names*

