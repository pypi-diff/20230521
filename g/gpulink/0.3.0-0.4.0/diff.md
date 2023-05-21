# Comparing `tmp/gpulink-0.3.0.tar.gz` & `tmp/gpulink-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpulink-0.3.0.tar", last modified: Sat Oct 15 13:27:13 2022, max compression
+gzip compressed data, was "gpulink-0.4.0.tar", last modified: Sun May 21 15:03:54 2023, max compression
```

## Comparing `gpulink-0.3.0.tar` & `gpulink-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,51 @@
-drwxrwxrwx   0        0        0        0 2022-10-15 13:27:13.261797 gpulink-0.3.0/
--rw-rw-rw-   0        0        0     1088 2022-07-18 07:04:47.000000 gpulink-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       15 2022-07-18 07:04:47.000000 gpulink-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4887 2022-10-15 13:27:13.261797 gpulink-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4360 2022-10-15 12:40:21.000000 gpulink-0.3.0/PYPI.md
--rw-rw-rw-   0        0        0     6387 2022-10-15 12:40:21.000000 gpulink-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-15 13:27:13.178797 gpulink-0.3.0/gpulink/
--rw-rw-rw-   0        0        0      364 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/__init__.py
--rw-rw-rw-   0        0        0     1809 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/__main__.py
-drwxrwxrwx   0        0        0        0 2022-10-15 13:27:13.234795 gpulink-0.3.0/gpulink/cli/
--rw-rw-rw-   0        0        0        0 2022-07-18 07:04:47.000000 gpulink-0.3.0/gpulink/cli/__init__.py
--rw-rw-rw-   0        0        0      472 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/cli/console.py
--rw-rw-rw-   0        0        0     1427 2022-10-15 12:40:21.000000 gpulink-0.3.0/gpulink/cli/record.py
--rw-rw-rw-   0        0        0     2952 2022-10-15 12:40:21.000000 gpulink-0.3.0/gpulink/cli/sensors.py
--rw-rw-rw-   0        0        0      980 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/cli/tools.py
--rw-rw-rw-   0        0        0       33 2022-07-18 07:04:47.000000 gpulink-0.3.0/gpulink/consts.py
-drwxrwxrwx   0        0        0        0 2022-10-15 13:27:13.248795 gpulink-0.3.0/gpulink/devices/
--rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/devices/__init__.py
--rw-rw-rw-   0        0        0     1427 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/devices/base_device.py
--rw-rw-rw-   0        0        0     4253 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/devices/devicectx.py
--rw-rw-rw-   0        0        0      795 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/devices/gpu.py
--rw-rw-rw-   0        0        0      751 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/devices/nvml_defines.py
--rw-rw-rw-   0        0        0     4303 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/devices/nvml_device.py
--rw-rw-rw-   0        0        0      595 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/devices/query.py
-drwxrwxrwx   0        0        0        0 2022-10-15 13:27:13.252798 gpulink-0.3.0/gpulink/plotting/
--rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/plotting/__init__.py
--rw-rw-rw-   0        0        0     2941 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/plotting/plot.py
--rw-rw-rw-   0        0        0      657 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/plotting/plot_options.py
-drwxrwxrwx   0        0        0        0 2022-10-15 13:27:13.257797 gpulink-0.3.0/gpulink/recording/
--rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/recording/__init__.py
--rw-rw-rw-   0        0        0     1738 2022-10-15 13:21:27.000000 gpulink-0.3.0/gpulink/recording/gpu_recording.py
--rw-rw-rw-   0        0        0     2577 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/recording/recorder.py
--rw-rw-rw-   0        0        0      772 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/recording/timeseries.py
-drwxrwxrwx   0        0        0        0 2022-10-15 13:27:13.260797 gpulink-0.3.0/gpulink/threading/
--rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/threading/__init__.py
--rw-rw-rw-   0        0        0      377 2022-07-21 20:40:05.000000 gpulink-0.3.0/gpulink/threading/stoppable_thread.py
-drwxrwxrwx   0        0        0        0 2022-10-15 13:27:13.221796 gpulink-0.3.0/gpulink.egg-info/
--rw-rw-rw-   0        0        0     4887 2022-10-15 13:27:13.000000 gpulink-0.3.0/gpulink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      901 2022-10-15 13:27:13.000000 gpulink-0.3.0/gpulink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-15 13:27:13.000000 gpulink-0.3.0/gpulink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-10-15 13:27:13.000000 gpulink-0.3.0/gpulink.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      117 2022-10-15 13:27:13.000000 gpulink-0.3.0/gpulink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-10-15 13:27:13.000000 gpulink-0.3.0/gpulink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-07-18 07:04:47.000000 gpulink-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-15 13:27:13.261797 gpulink-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1375 2022-10-15 13:22:50.000000 gpulink-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.754887 gpulink-0.4.0/
+-rw-rw-rw-   0        0        0     1088 2022-07-18 07:04:47.000000 gpulink-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       15 2022-07-18 07:04:47.000000 gpulink-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5180 2023-05-21 15:03:54.753887 gpulink-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4653 2023-05-21 15:01:56.000000 gpulink-0.4.0/PYPI.md
+-rw-rw-rw-   0        0        0     7303 2023-05-21 15:01:53.000000 gpulink-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.705715 gpulink-0.4.0/gpulink/
+-rw-rw-rw-   0        0        0      387 2023-05-21 14:59:07.000000 gpulink-0.4.0/gpulink/__init__.py
+-rw-rw-rw-   0        0        0      402 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.725714 gpulink-0.4.0/gpulink/cli/
+-rw-rw-rw-   0        0        0        0 2022-07-18 07:04:47.000000 gpulink-0.4.0/gpulink/cli/__init__.py
+-rw-rw-rw-   0        0        0     5440 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/cli/cmd_record.py
+-rw-rw-rw-   0        0        0     3486 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/cli/cmd_sensors.py
+-rw-rw-rw-   0        0        0      209 2023-05-21 15:00:12.000000 gpulink-0.4.0/gpulink/cli/console.py
+-rw-rw-rw-   0        0        0       79 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/consts.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.734887 gpulink-0.4.0/gpulink/devices/
+-rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/devices/__init__.py
+-rw-rw-rw-   0        0        0     1427 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/devices/base_device.py
+-rw-rw-rw-   0        0        0     4253 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/devices/devicectx.py
+-rw-rw-rw-   0        0        0      799 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/devices/gpu.py
+-rw-rw-rw-   0        0        0      751 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/devices/nvml_defines.py
+-rw-rw-rw-   0        0        0     4469 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/devices/nvml_device.py
+-rw-rw-rw-   0        0        0      597 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/devices/query.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.738886 gpulink-0.4.0/gpulink/plotting/
+-rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/plotting/__init__.py
+-rw-rw-rw-   0        0        0     2941 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/plotting/plot.py
+-rw-rw-rw-   0        0        0      659 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/plotting/plot_options.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.744891 gpulink-0.4.0/gpulink/recording/
+-rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/recording/__init__.py
+-rw-rw-rw-   0        0        0     1858 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/recording/gpu_recording.py
+-rw-rw-rw-   0        0        0     8079 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/recording/recorder.py
+-rw-rw-rw-   0        0        0      774 2023-05-21 14:49:23.000000 gpulink-0.4.0/gpulink/recording/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.746891 gpulink-0.4.0/gpulink/threading/
+-rw-rw-rw-   0        0        0        0 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/threading/__init__.py
+-rw-rw-rw-   0        0        0      377 2022-07-21 20:40:05.000000 gpulink-0.4.0/gpulink/threading/stoppable_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.717714 gpulink-0.4.0/gpulink.egg-info/
+-rw-rw-rw-   0        0        0     5180 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1011 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 15:03:54.000000 gpulink-0.4.0/gpulink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-07-18 07:04:47.000000 gpulink-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 15:03:54.754887 gpulink-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1912 2023-05-21 14:49:27.000000 gpulink-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:03:54.752887 gpulink-0.4.0/tests/
+-rw-rw-rw-   0        0        0      510 2022-07-21 20:40:05.000000 gpulink-0.4.0/tests/test_dataclasses.py
+-rw-rw-rw-   0        0        0     4071 2022-07-21 20:40:05.000000 gpulink-0.4.0/tests/test_device_context.py
+-rw-rw-rw-   0        0        0     4983 2022-07-21 20:40:05.000000 gpulink-0.4.0/tests/test_nvml_device.py
+-rw-rw-rw-   0        0        0     3105 2022-07-21 20:40:05.000000 gpulink-0.4.0/tests/test_plot.py
+-rw-rw-rw-   0        0        0     1951 2023-05-21 14:49:23.000000 gpulink-0.4.0/tests/test_recorder.py
```

### Comparing `gpulink-0.3.0/LICENSE` & `gpulink-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpulink-0.3.0/PKG-INFO` & `gpulink-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpulink
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple tool for monitoring and displaying GPU stats
 Home-page: https://github.com/PhilipKlaus/gpu-link
 Author: Philip Klaus
 Project-URL: Bug Tracker, https://github.com/PhilipKlaus/gpu-link/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,29 +46,30 @@
 3. Install requirements: `pip install -r requirements.txt`
 
 ## Command-line usage
 
 **gpulink** can either be imported as a library or can be used from the command line:
 
 ```
-usage: gpulink [-h] {sensors,record} ...
+Usage: GPU-Link: Monitor NVIDIA GPUs [OPTIONS] COMMAND [ARGS]...
 
-GPU-Link: Monitor NVIDIA GPU status
-
-positional arguments:
-  {sensors,record}
-
-optional arguments:
-  -h, --help        show this help message and exit
+Options:
+  --version  Show the version and exit.
+  --help     Show this message and exit.
+
+Commands:
+  record   Record GPU properties.
+  sensors  Fetch and print the GPU sensor status.
 ```
 
 ### Examples
 
 - View GPU sensor status: `gpulink sensors`
-- Record the memory usage over time, generate a plot and save it as a png image: `gpulink record -o memory.png`
+- Watch GPU sensor status: `gpulink sensors -w`
+- Record the memory usage over time, generate a plot and save it as a png image: `gpulink record -o memory.png memory`
 
 ## Library usage
 
 **gpulink** can be simply used from within Python. Just import `gpulink` and create a `DeviceCtx`. This context manages
 device access and provides an API for fetching GPU properties
 (see [API example](https://github.com/PhilipKlaus/gpu-link/blob/main/example/example_api.py)):
 
@@ -133,19 +134,22 @@
 ```
 import gpulink as gpu
 
 with gpu.DeviceCtx(device=DeviceMock) as ctx:
    ...
 ```
 
-## Currently planned features
-
-- Recording arbitrary GPU stats
-- [Curses](https://docs.python.org/3/howto/curses.html) based ui (
-  using [windows-curses](https://pypi.org/project/windows-curses/))
-- Live-plotting of GPU stats
-
 ## Troubleshooting
 
 - If you get the error message below, please ensure that the NVIDIA Management Library is installed on you system by
   typing `nvidia-smi --version` into a terminal:  
   ```pynvml.nvml.NVMLError_LibraryNotFound: NVML Shared Library Not Found```.  
+
+## Planned features
+- Live-plotting of GPU stats
+
+## Changelog 
+- 0.4.0
+    - Recording arbitrary GPU stats (clock, fan-speed, memory, power-usage, temp)
+    - Display GPU name and power usage within `sensors` command
+    - Replaced `arparse` library by [click](https://click.palletsprojects.com/en/8.1.x/)
+    - Aborting a `watch` or `recording` command can be done by pressing any instead of `ctrl+c`
```

### Comparing `gpulink-0.3.0/PYPI.md` & `gpulink-0.4.0/PYPI.md`

 * *Files 7% similar despite different names*

```diff
@@ -31,29 +31,30 @@
 3. Install requirements: `pip install -r requirements.txt`
 
 ## Command-line usage
 
 **gpulink** can either be imported as a library or can be used from the command line:
 
 ```
-usage: gpulink [-h] {sensors,record} ...
+Usage: GPU-Link: Monitor NVIDIA GPUs [OPTIONS] COMMAND [ARGS]...
 
-GPU-Link: Monitor NVIDIA GPU status
-
-positional arguments:
-  {sensors,record}
-
-optional arguments:
-  -h, --help        show this help message and exit
+Options:
+  --version  Show the version and exit.
+  --help     Show this message and exit.
+
+Commands:
+  record   Record GPU properties.
+  sensors  Fetch and print the GPU sensor status.
 ```
 
 ### Examples
 
 - View GPU sensor status: `gpulink sensors`
-- Record the memory usage over time, generate a plot and save it as a png image: `gpulink record -o memory.png`
+- Watch GPU sensor status: `gpulink sensors -w`
+- Record the memory usage over time, generate a plot and save it as a png image: `gpulink record -o memory.png memory`
 
 ## Library usage
 
 **gpulink** can be simply used from within Python. Just import `gpulink` and create a `DeviceCtx`. This context manages
 device access and provides an API for fetching GPU properties
 (see [API example](https://github.com/PhilipKlaus/gpu-link/blob/main/example/example_api.py)):
 
@@ -118,19 +119,22 @@
 ```
 import gpulink as gpu
 
 with gpu.DeviceCtx(device=DeviceMock) as ctx:
    ...
 ```
 
-## Currently planned features
-
-- Recording arbitrary GPU stats
-- [Curses](https://docs.python.org/3/howto/curses.html) based ui (
-  using [windows-curses](https://pypi.org/project/windows-curses/))
-- Live-plotting of GPU stats
-
 ## Troubleshooting
 
 - If you get the error message below, please ensure that the NVIDIA Management Library is installed on you system by
   typing `nvidia-smi --version` into a terminal:  
   ```pynvml.nvml.NVMLError_LibraryNotFound: NVML Shared Library Not Found```.  
+
+## Planned features
+- Live-plotting of GPU stats
+
+## Changelog 
+- 0.4.0
+    - Recording arbitrary GPU stats (clock, fan-speed, memory, power-usage, temp)
+    - Display GPU name and power usage within `sensors` command
+    - Replaced `arparse` library by [click](https://click.palletsprojects.com/en/8.1.x/)
+    - Aborting a `watch` or `recording` command can be done by pressing any instead of `ctrl+c`
```

### Comparing `gpulink-0.3.0/README.md` & `gpulink-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 A library and command-line tool for monitoring NVIDIA GPU stats.  
 **gpulink** uses [pynvml](https://github.com/gpuopenanalytics/pynvml) - a Python wrapper for
 the [NVIDIA Management Library](https://developer.nvidia.com/nvidia-management-library-nvml) (NVML).
 
 ## Current status
 
-**⚠ This project is in a very early state and under heavy development - breaking changes between versions are possible
-⚠**
+⚠ gpulink is in a very early state - breaking changes between versions are possible!
 
 ## Requirements
 
 **gpulink** requires the NVIDIA Management Library to be installed which is shipped together
 with [nvidia-smi](https://developer.nvidia.com/nvidia-system-management-interface).
 
 ## Installation
@@ -31,41 +30,45 @@
 3. Install requirements: `pip install -r requirements.txt`
 
 ## Command-line usage
 
 **gpulink** can either be imported as a library or can be used from the command line:
 
 ```
-usage: gpulink [-h] {sensors,record} ...
+Usage: GPU-Link: Monitor NVIDIA GPUs [OPTIONS] COMMAND [ARGS]...
 
-GPU-Link: Monitor NVIDIA GPU status
-
-positional arguments:
-  {sensors,record}
-
-optional arguments:
-  -h, --help        show this help message and exit
+Options:
+  --version  Show the version and exit.
+  --help     Show this message and exit.
+
+Commands:
+  record   Record GPU properties.
+  sensors  Fetch and print the GPU sensor status.
 ```
 
 ### Examples
 
 - View GPU sensor status: `gpulink sensors`
 
 ```
-╒════════╤═════════════════════╤═════════════╤═════════════════╤═══════════════╕
-│ GPU    │ Memory [MB]         │   Temp [°C] │   Fan speed [%] │ Clock [MHz]   │
-╞════════╪═════════════════════╪═════════════╪═════════════════╪═══════════════╡
-│ 0      │ 1588 / 25769 (6.2%) │          34 │              41 │ Graph.: 173   │
-│        │                     │             │                 │ Memory: 403   │
-│        │                     │             │                 │ SM: 173       │
-│        │                     │             │                 │ Video: 539    │
-╘════════╧═════════════════════╧═════════════╧═════════════════╧═══════════════╛
+╒═══════╤══════════════════╤═════════════════════╤═════════════╤═════════════════╤═══════════════╤═══════════════════╕
+│   GPU │ Name             │ Memory [MB]         │   Temp [°C] │   Fan speed [%] │ Clock [MHz]   │   Power Usage [W] │
+╞═══════╪══════════════════╪═════════════════════╪═════════════╪═════════════════╪═══════════════╪═══════════════════╡
+│     0 │ NVIDIA TITAN RTX │ 1809 / 25769 (7.0%) │          34 │              41 │ Graph.: 173   │            26.583 │
+│       │                  │                     │             │                 │ Memory: 403   │                   │
+│       │                  │                     │             │                 │ SM: 173       │                   │
+│       │                  │                     │             │                 │ Video: 540    │                   │
+╘═══════╧══════════════════╧═════════════════════╧═════════════╧═════════════════╧═══════════════╧═══════════════════╛
 ```
+- Watch GPU sensor status: `gpulink sensors -w`  
+
+![Watch sensor status](https://github.com/PhilipKlaus/gpu-link/blob/main/docs/gpulink_sensors_watch.gif)
 
-- Record the memory usage over time, generate a plot and save it as a png image: `gpulink record -o memory.png`
+
+- Record the memory usage over time, generate a plot and save it as a png image: `gpulink record -o memory.png memory`
 
 ```
 ╒═════╤══════════════════╤══════════════════════╕
 │ GPU │ Name             │ Memory used [MB]     │
 ├─────┼──────────────────┼──────────────────────┤
 │ 0   │ NVIDIA TITAN RTX │ minimum: 1584.754688 │
 │     │                  │ maximum: 2204.585984 │
@@ -143,19 +146,22 @@
 ```
 import gpulink as gpu
 
 with gpu.DeviceCtx(device=DeviceMock) as ctx:
    ...
 ```
 
-## Currently planned features
-
-- Recording arbitrary GPU stats
-- [Curses](https://docs.python.org/3/howto/curses.html) based ui (
-  using [windows-curses](https://pypi.org/project/windows-curses/))
-- Live-plotting of GPU stats
-
 ## Troubleshooting
 
 - If you get the error message below, please ensure that the NVIDIA Management Library is installed on you system by
   typing `nvidia-smi --version` into a terminal:  
   ```pynvml.nvml.NVMLError_LibraryNotFound: NVML Shared Library Not Found```.  
+
+## Planned features
+- Live-plotting of GPU stats
+
+## Changelog 
+- 0.4.0
+    - Recording arbitrary GPU stats (clock, fan-speed, memory, power-usage, temp)
+    - Display GPU name and power usage within `sensors` command
+    - Replaced `arparse` library by [click](https://click.palletsprojects.com/en/8.1.x/)
+    - Aborting a `watch` or `recording` command can be done by pressing any instead of `ctrl+c`
```

### Comparing `gpulink-0.3.0/gpulink/cli/sensors.py` & `gpulink-0.4.0/gpulink/cli/cmd_sensors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import time
 from dataclasses import dataclass
 from typing import List, Iterator
 
+import click
 from tabulate import tabulate
 
 from gpulink import DeviceCtx
-from gpulink.cli.console import cls, set_cursor, get_spinner
-from gpulink.cli.tools import start_in_background
-from gpulink.consts import MB
+from gpulink.cli.console import get_spinner, set_cursor
+from gpulink.consts import MB, WATTS
 from gpulink.devices.gpu import GpuSet
-from gpulink.threading.stoppable_thread import StoppableThread
 from gpulink.devices.nvml_defines import TemperatureSensorType, ClockType
 from gpulink.devices.query import SimpleResult, MemInfo
+from gpulink.threading.stoppable_thread import StoppableThread
 
 
 class SensorWatcher(StoppableThread):
     def __init__(self, ctx: DeviceCtx):
         super().__init__()
         self._ctx = ctx
 
@@ -29,56 +29,64 @@
             temperature=self._ctx.get_temperature(TemperatureSensorType.GPU, gpus=gpus.ids),
             fan_speed=self._ctx.get_fan_speed(gpus=gpus.ids),
             clock=zip(
                 self._ctx.get_clock(ClockType.CLOCK_GRAPHICS, gpus=gpus.ids),
                 self._ctx.get_clock(ClockType.CLOCK_MEM, gpus=gpus.ids),
                 self._ctx.get_clock(ClockType.CLOCK_SM, gpus=gpus.ids),
                 self._ctx.get_clock(ClockType.CLOCK_VIDEO, gpus=gpus.ids),
-            )
+            ),
+            power_usage=self._ctx.get_power_usage(gpus.ids)
         )
 
     def run(self) -> None:
-        cls()
+        click.clear()
         spinner = get_spinner()
         while not self.should_stop:
-            print(f"{self.get_sensor_status()}\n[WATCHING] {next(spinner)}{set_cursor(1, 1)}", end="")
-            time.sleep(0.5)
-        cls()
-
+            click.echo(f"{self.get_sensor_status()}\nPress any key to abort...\n[WATCHING] ", nl=False)
+            click.secho(f"{next(spinner)}{set_cursor(1, 1)}", nl=False, fg="green")
+            time.sleep(0.1)
+        click.clear()
 
-def sensors(args):
-    """Print GPU sensor output"""
 
+@click.command(name="sensors")
+@click.option('--watch', '-w', is_flag=True, help="Poll and print GPU sensor status.")
+def sensors(watch: bool):
+    """
+    Fetch and print the GPU sensor status.
+    :param watch: Set too bool if the sensor status should be polled and printed continuously.
+    """
     with DeviceCtx() as ctx:
         watcher = SensorWatcher(ctx)
-
-        if args.watch:
-            start_in_background(watcher)
-        else:
-            print(watcher.get_sensor_status())
+        if watch:
+            watcher.start()
+            click.pause("")
+            watcher.stop(auto_join=True)
+        click.echo(watcher.get_sensor_status())
 
 
 @dataclass
 class SensorStatus:
     """
     A container for storing several sensor status.
     """
     gpus: GpuSet
     memory: List[MemInfo]
     temperature: List[SimpleResult]
     fan_speed: List[SimpleResult]
     clock: Iterator
+    power_usage: List[SimpleResult]
 
     def __str__(self):
-        header = ["GPU", "Name", "Memory [MB]", "Temp [°C]", "Fan speed [%]", "Clock [MHz]"]
+        header = ["GPU", "Name", "Memory [MB]", "Temp [°C]", "Fan speed [%]", "Clock [MHz]", "Power Usage [W]"]
         table = [header]
-        for data in zip(self.gpus, self.memory, self.temperature, self.fan_speed, self.clock):
+        for data in zip(self.gpus, self.memory, self.temperature, self.fan_speed, self.clock, self.power_usage):
             table.append([
                 f"{data[0].id}",
                 f"{data[0].name}",
                 f"{int(data[1].used / MB)} / {int(data[1].total / MB)} ({(data[1].used / data[1].total) * 100:.1f}%)",
                 f"{data[2].value}",
                 f"{data[3].value}",
                 f"Graph.: {data[4][0].value}\nMemory: {data[4][1].value}\n"
-                f"SM: {data[4][2].value}\nVideo: {data[4][3].value} "
+                f"SM: {data[4][2].value}\nVideo: {data[4][3].value}",
+                f"{data[5].value / WATTS}"
             ])
-        return tabulate(table, headers='firstrow', tablefmt='fancy_grid')
+        return tabulate(table, headers='firstrow', tablefmt='fancy_grid')
```

### Comparing `gpulink-0.3.0/gpulink/devices/base_device.py` & `gpulink-0.4.0/gpulink/devices/base_device.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, List
 
+from gpulink.devices.gpu import GpuSet
 from gpulink.devices.nvml_defines import ClockType, ClockId, TemperatureThreshold, \
     TemperatureSensorType
 from gpulink.devices.query import SimpleResult, MemInfo
-from gpulink.devices.gpu import GpuSet
 
 
 class BaseDevice:
 
     def setup(self) -> None:
         raise NotImplementedError()
```

### Comparing `gpulink-0.3.0/gpulink/devices/devicectx.py` & `gpulink-0.4.0/gpulink/devices/devicectx.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from functools import wraps
 from typing import List, Optional, Type
 
 from gpulink.devices.base_device import BaseDevice
-from gpulink.devices.nvml_device import LocalNvmlGpu
+from gpulink.devices.gpu import GpuSet
 from gpulink.devices.nvml_defines import TemperatureThreshold, ClockId, \
     ClockType, TemperatureSensorType
+from gpulink.devices.nvml_device import LocalNvmlGpu
 from gpulink.devices.query import SimpleResult, MemInfo
-from gpulink.devices.gpu import GpuSet
 
 
 def ctx_guard(fn):
     @wraps(fn)
     def guard(ref, *args, **kwargs):
         if not ref.valid_ctx:
             raise RuntimeError("Cannot execute query in an invalid NVContext")
```

### Comparing `gpulink-0.3.0/gpulink/devices/gpu.py` & `gpulink-0.4.0/gpulink/devices/gpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     name: str
 
 
 class GpuSet:
     """
     A set of GPUs.
     """
+
     def __init__(self, gpus: List[Gpu]):
         self._gpus = gpus
 
     def __getitem__(self, key) -> Gpu:
         return self._gpus[key]
 
     def __len__(self) -> int:
@@ -31,8 +32,8 @@
 
     @property
     def ids(self) -> List[int]:
         return [gpu.id for gpu in self._gpus]
 
     @property
     def names(self) -> List[str]:
-        return [gpu.name for gpu in self._gpus]
+        return [gpu.name for gpu in self._gpus]
```

### Comparing `gpulink-0.3.0/gpulink/devices/nvml_defines.py` & `gpulink-0.4.0/gpulink/devices/nvml_defines.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.3.0/gpulink/devices/nvml_device.py` & `gpulink-0.4.0/gpulink/devices/nvml_device.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from time import time_ns
 from typing import Type, Optional, cast, List
 
+import pynvml
 from pynvml import nvmlDeviceGetCount, nvmlDeviceGetHandleByIndex, nvmlDeviceGetName, nvmlDeviceGetClock, \
     nvmlDeviceGetTemperatureThreshold, nvmlDeviceGetClockInfo, nvmlDeviceGetPowerUsage, nvmlDeviceGetTemperature, \
     nvmlDeviceGetMemoryInfo, nvmlDeviceGetFanSpeed_v2, nvmlDeviceGetFanSpeed, nvmlInit, nvmlShutdown
 
 from gpulink.devices.base_device import BaseDevice
+from gpulink.devices.gpu import Gpu, GpuSet
 from gpulink.devices.nvml_defines import ClockType, ClockId, TemperatureSensorType, \
     TemperatureThreshold
 from gpulink.devices.query import QueryResult, SimpleResult, MemInfo
-from gpulink.devices.gpu import Gpu, GpuSet
 
 
 class LocalNvmlGpu(BaseDevice):
 
     def __init__(self):
         self._device_handles = []
         self._device_names = []
@@ -46,16 +47,19 @@
             else:
                 for key in type.__annotations__:
                     tmp[key] = getattr(query_result, key)
             res.append(type(**tmp))
         return res
 
     def setup(self) -> None:
-        nvmlInit()
-        self._get_device_handles()
+        try:
+            nvmlInit()
+            self._get_device_handles()
+        except pynvml.nvml.NVMLError as e:
+            raise RuntimeError("Cannot initialize NVML library - Is it installed?")
 
     def shutdown(self) -> None:
         nvmlShutdown()
 
     def get_gpus(self) -> GpuSet:
         gpus = []
         for id, name in zip(self._device_ids, self._device_names):
```

### Comparing `gpulink-0.3.0/gpulink/devices/query.py` & `gpulink-0.4.0/gpulink/devices/query.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 @dataclass
 class MemInfo(QueryResult):
     """
     Stores the result of a nvmlDeviceGetMemoryInfo query.
     """
     total: int
     used: int
-    free: int
+    free: int
```

### Comparing `gpulink-0.3.0/gpulink/plotting/plot.py` & `gpulink-0.4.0/gpulink/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `gpulink-0.3.0/gpulink/plotting/plot_options.py` & `gpulink-0.4.0/gpulink/plotting/plot_options.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     y_axis_divider: Optional[DATA] = None
     auto_scale: Optional[bool] = None
 
     def patch(self, other: PlotOptions):
         for field in fields(PlotOptions):
             value = other.__getattribute__(field.name)
             if value:
-                self.__setattr__(field.name, value)
+                self.__setattr__(field.name, value)
```

### Comparing `gpulink-0.3.0/gpulink/recording/gpu_recording.py` & `gpulink-0.4.0/gpulink/recording/gpu_recording.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
+import sys
 from dataclasses import dataclass
 from typing import List, Optional
 
 import numpy as np
 from tabulate import tabulate
 
-from gpulink.consts import MB, SEC
+from gpulink.consts import SEC
 from gpulink.devices.gpu import GpuSet
 from gpulink.plotting.plot_options import PlotOptions
 from gpulink.recording.timeseries import TimeSeries
 
 
 @dataclass
 class Recording:
@@ -24,25 +25,26 @@
     def _create_data_table(self):
         table = [["GPU", "Name", f"{self.plot_options.y_axis_label} [{self.plot_options.y_axis_unit}]"]]
         for gpu, timeseries in zip(self.gpus, self.timeseries):
             data = timeseries.data
             table.append(
                 [gpu.id,
                  gpu.name,
-                 f"minimum: {np.min(data) / MB}\nmaximum: {np.max(data) / MB}"
+                 f"minimum: {np.min(data) / self.plot_options.y_axis_divider}\n"
+                 f"maximum: {np.max(data) / self.plot_options.y_axis_divider} "
                  ]
             )
         return tabulate(table, tablefmt='fancy_grid')
 
     def _get_duration(self):
         timestamps = [t.timestamps for t in self.timeseries]
         min_time = min([np.min(t) for t in timestamps])
         max_time = min([np.max(t) for t in timestamps])
         return (max_time - min_time) / SEC
 
     def __str__(self):
         data_table = self._create_data_table()
         duration = f"{self._get_duration():.3f}"
-        sampling_rate = f"{self.timeseries[0].data.size / self._get_duration():.3f}"
+        sampling_rate = f"{self.timeseries[0].data.size / max(self._get_duration(), sys.float_info.epsilon):.3f}"
         return f"{data_table}\n" \
                f"{'Duration:':25}{duration} [s]\n" \
                f"{'Sampling rate:':25}{sampling_rate} [Hz]"
```

### Comparing `gpulink-0.3.0/gpulink/recording/timeseries.py` & `gpulink-0.4.0/gpulink/recording/timeseries.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
     @property
     def timestamps(self) -> np.ndarray:
         return np.array(self._timestamps)
 
     @property
     def data(self) -> np.ndarray:
-        return np.array(self._data)
+        return np.array(self._data)
```

### Comparing `gpulink-0.3.0/gpulink.egg-info/PKG-INFO` & `gpulink-0.4.0/gpulink.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpulink
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple tool for monitoring and displaying GPU stats
 Home-page: https://github.com/PhilipKlaus/gpu-link
 Author: Philip Klaus
 Project-URL: Bug Tracker, https://github.com/PhilipKlaus/gpu-link/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,29 +46,30 @@
 3. Install requirements: `pip install -r requirements.txt`
 
 ## Command-line usage
 
 **gpulink** can either be imported as a library or can be used from the command line:
 
 ```
-usage: gpulink [-h] {sensors,record} ...
+Usage: GPU-Link: Monitor NVIDIA GPUs [OPTIONS] COMMAND [ARGS]...
 
-GPU-Link: Monitor NVIDIA GPU status
-
-positional arguments:
-  {sensors,record}
-
-optional arguments:
-  -h, --help        show this help message and exit
+Options:
+  --version  Show the version and exit.
+  --help     Show this message and exit.
+
+Commands:
+  record   Record GPU properties.
+  sensors  Fetch and print the GPU sensor status.
 ```
 
 ### Examples
 
 - View GPU sensor status: `gpulink sensors`
-- Record the memory usage over time, generate a plot and save it as a png image: `gpulink record -o memory.png`
+- Watch GPU sensor status: `gpulink sensors -w`
+- Record the memory usage over time, generate a plot and save it as a png image: `gpulink record -o memory.png memory`
 
 ## Library usage
 
 **gpulink** can be simply used from within Python. Just import `gpulink` and create a `DeviceCtx`. This context manages
 device access and provides an API for fetching GPU properties
 (see [API example](https://github.com/PhilipKlaus/gpu-link/blob/main/example/example_api.py)):
 
@@ -133,19 +134,22 @@
 ```
 import gpulink as gpu
 
 with gpu.DeviceCtx(device=DeviceMock) as ctx:
    ...
 ```
 
-## Currently planned features
-
-- Recording arbitrary GPU stats
-- [Curses](https://docs.python.org/3/howto/curses.html) based ui (
-  using [windows-curses](https://pypi.org/project/windows-curses/))
-- Live-plotting of GPU stats
-
 ## Troubleshooting
 
 - If you get the error message below, please ensure that the NVIDIA Management Library is installed on you system by
   typing `nvidia-smi --version` into a terminal:  
   ```pynvml.nvml.NVMLError_LibraryNotFound: NVML Shared Library Not Found```.  
+
+## Planned features
+- Live-plotting of GPU stats
+
+## Changelog 
+- 0.4.0
+    - Recording arbitrary GPU stats (clock, fan-speed, memory, power-usage, temp)
+    - Display GPU name and power usage within `sensors` command
+    - Replaced `arparse` library by [click](https://click.palletsprojects.com/en/8.1.x/)
+    - Aborting a `watch` or `recording` command can be done by pressing any instead of `ctrl+c`
```

### Comparing `gpulink-0.3.0/gpulink.egg-info/SOURCES.txt` & `gpulink-0.4.0/gpulink.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 gpulink.egg-info/PKG-INFO
 gpulink.egg-info/SOURCES.txt
 gpulink.egg-info/dependency_links.txt
 gpulink.egg-info/entry_points.txt
 gpulink.egg-info/requires.txt
 gpulink.egg-info/top_level.txt
 gpulink/cli/__init__.py
+gpulink/cli/cmd_record.py
+gpulink/cli/cmd_sensors.py
 gpulink/cli/console.py
-gpulink/cli/record.py
-gpulink/cli/sensors.py
-gpulink/cli/tools.py
 gpulink/devices/__init__.py
 gpulink/devices/base_device.py
 gpulink/devices/devicectx.py
 gpulink/devices/gpu.py
 gpulink/devices/nvml_defines.py
 gpulink/devices/nvml_device.py
 gpulink/devices/query.py
@@ -29,8 +28,13 @@
 gpulink/plotting/plot.py
 gpulink/plotting/plot_options.py
 gpulink/recording/__init__.py
 gpulink/recording/gpu_recording.py
 gpulink/recording/recorder.py
 gpulink/recording/timeseries.py
 gpulink/threading/__init__.py
-gpulink/threading/stoppable_thread.py
+gpulink/threading/stoppable_thread.py
+tests/test_dataclasses.py
+tests/test_device_context.py
+tests/test_nvml_device.py
+tests/test_plot.py
+tests/test_recorder.py
```

