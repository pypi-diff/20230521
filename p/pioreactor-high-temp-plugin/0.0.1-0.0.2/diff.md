# Comparing `tmp/pioreactor_high_temp_plugin-0.0.1-py3-none-any.whl.zip` & `tmp/pioreactor_high_temp_plugin-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2879 bytes, number of entries: 7
--rw-r--r--  2.0 unx      338 b- defN 23-May-20 00:35 pioreactor_high_temp_plugin/__init__.py
--rw-r--r--  2.0 unx     1079 b- defN 23-May-20 00:40 pioreactor_high_temp_plugin-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      580 b- defN 23-May-20 00:40 pioreactor_high_temp_plugin-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-20 00:40 pioreactor_high_temp_plugin-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 23-May-20 00:40 pioreactor_high_temp_plugin-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-May-20 00:40 pioreactor_high_temp_plugin-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      695 b- defN 23-May-20 00:40 pioreactor_high_temp_plugin-0.0.1.dist-info/RECORD
-7 files, 2891 bytes uncompressed, 1609 bytes compressed:  44.3%
+Zip file size: 2953 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      453 b- defN 23-May-21 16:09 pioreactor_high_temp_plugin/__init__.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-May-21 16:10 pioreactor_high_temp_plugin-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      580 b- defN 23-May-21 16:10 pioreactor_high_temp_plugin-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 16:10 pioreactor_high_temp_plugin-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-May-21 16:10 pioreactor_high_temp_plugin-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-May-21 16:10 pioreactor_high_temp_plugin-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      695 b- defN 23-May-21 16:10 pioreactor_high_temp_plugin-0.0.2.dist-info/RECORD
+7 files, 3006 bytes uncompressed, 1683 bytes compressed:  44.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pioreactor_high_temp_plugin/__init__.py
 Comment: 
 
-Filename: pioreactor_high_temp_plugin-0.0.1.dist-info/LICENSE
+Filename: pioreactor_high_temp_plugin-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: pioreactor_high_temp_plugin-0.0.1.dist-info/METADATA
+Filename: pioreactor_high_temp_plugin-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pioreactor_high_temp_plugin-0.0.1.dist-info/WHEEL
+Filename: pioreactor_high_temp_plugin-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pioreactor_high_temp_plugin-0.0.1.dist-info/entry_points.txt
+Filename: pioreactor_high_temp_plugin-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioreactor_high_temp_plugin-0.0.1.dist-info/top_level.txt
+Filename: pioreactor_high_temp_plugin-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pioreactor_high_temp_plugin-0.0.1.dist-info/RECORD
+Filename: pioreactor_high_temp_plugin-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioreactor_high_temp_plugin/__init__.py

```diff
@@ -1,9 +1,11 @@
 from pioreactor.background_jobs.monitor import Monitor
 from pioreactor.background_jobs.temperature_control import TemperatureController
 
 
 TemperatureController.MAX_TEMP_TO_REDUCE_HEATING = 81.5
 TemperatureController.MAX_TEMP_TO_DISABLE_HEATING = 83.5
 TemperatureController.MAX_TEMP_TO_SHUTDOWN = 85.0
+TemperatureController.INTERENCE_EVERY_N_SECONDS = 5 * 60 # PWM is on for just over half the time, instead of ~1/3
+
 
 Monitor.MAX_TEMP_TO_SHUTDOWN = 85.0
```

## Comparing `pioreactor_high_temp_plugin-0.0.1.dist-info/LICENSE` & `pioreactor_high_temp_plugin-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pioreactor_high_temp_plugin-0.0.1.dist-info/METADATA` & `pioreactor_high_temp_plugin-0.0.2.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pioreactor-high-temp-plugin
-Version: 0.0.1
+Version: 0.0.2
 Summary: Do not use this. Using this risks damaging your Pioreactor or harming yourself. All responsibility is on you.
 Home-page: https://github.com/Pioreactor/pioreactor-high-temp-plugin
 Author: Cam Davidson Pilon
 Author-email: cam@pioreactor.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

