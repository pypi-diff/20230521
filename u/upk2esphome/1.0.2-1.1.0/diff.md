# Comparing `tmp/upk2esphome-1.0.2.tar.gz` & `tmp/upk2esphome-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upk2esphome-1.0.2.tar", max compression
+gzip compressed data, was "upk2esphome-1.1.0.tar", max compression
```

## Comparing `upk2esphome-1.0.2.tar` & `upk2esphome-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1076 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/LICENSE
--rw-r--r--   0        0        0      531 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/README.md
--rw-r--r--   0        0        0      455 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      256 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/__init__.py
--rw-r--r--   0        0        0     1650 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/generator.py
--rw-r--r--   0        0        0     1442 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/input.py
--rw-r--r--   0        0        0      400 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/opts.py
--rw-r--r--   0        0        0       48 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/__init__.py
--rw-r--r--   0        0        0     8367 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/bulb.py
--rw-r--r--   0        0        0     1406 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/module.py
--rw-r--r--   0        0        0     3403 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/monitor.py
--rw-r--r--   0        0        0      775 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/netled.py
--rw-r--r--   0        0        0     1355 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/static.py
--rw-r--r--   0        0        0     3009 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/switch.py
--rw-r--r--   0        0        0     1834 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/result.py
--rw-r--r--   0        0        0      651 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/test.py
--rw-r--r--   0        0        0      444 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_cw_pwm.txt
--rw-r--r--   0        0        0      563 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbc_2135_2.txt
--rw-r--r--   0        0        0      430 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_2135.txt
--rw-r--r--   0        0        0      543 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt
--rw-r--r--   0        0        0      599 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_2235.txt
--rw-r--r--   0        0        0      496 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_5758d.txt
--rw-r--r--   0        0        0        0 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/empty.txt
--rw-r--r--   0        0        0     2936 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/plug_monitor_bl0937.txt
--rw-r--r--   0        0        0      476 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/plug_monitor_bl0942.txt
--rw-r--r--   0        0        0      497 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/plug_monitor_hlw8032.txt
--rw-r--r--   0        0        0      914 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/plug_total.txt
--rw-r--r--   0        0        0      777 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/switch_monitor.txt
--rw-r--r--   0        0        0      922 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/web.py
--rw-r--r--   0        0        0     1029 1970-01-01 00:00:00.000000 upk2esphome-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/LICENSE
+-rw-r--r--   0        0        0      531 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/README.md
+-rw-r--r--   0        0        0      475 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      256 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/__init__.py
+-rw-r--r--   0        0        0     1650 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/generator.py
+-rw-r--r--   0        0        0     1442 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/input.py
+-rw-r--r--   0        0        0      400 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/opts.py
+-rw-r--r--   0        0        0       48 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/parts/__init__.py
+-rw-r--r--   0        0        0     8367 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/parts/bulb.py
+-rw-r--r--   0        0        0     1406 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/parts/module.py
+-rw-r--r--   0        0        0     3403 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/parts/monitor.py
+-rw-r--r--   0        0        0      775 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/parts/netled.py
+-rw-r--r--   0        0        0     1355 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/parts/static.py
+-rw-r--r--   0        0        0     3009 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/parts/switch.py
+-rw-r--r--   0        0        0     1834 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/result.py
+-rw-r--r--   0        0        0      651 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/test.py
+-rw-r--r--   0        0        0      444 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/bulb_cw_pwm.txt
+-rw-r--r--   0        0        0      563 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/bulb_rgbc_2135_2.txt
+-rw-r--r--   0        0        0      430 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/bulb_rgbcw_2135.txt
+-rw-r--r--   0        0        0      543 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt
+-rw-r--r--   0        0        0      599 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/bulb_rgbcw_2235.txt
+-rw-r--r--   0        0        0      496 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/bulb_rgbcw_5758d.txt
+-rw-r--r--   0        0        0        0 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/empty.txt
+-rw-r--r--   0        0        0     2936 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/plug_monitor_bl0937.txt
+-rw-r--r--   0        0        0      476 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/plug_monitor_bl0942.txt
+-rw-r--r--   0        0        0      497 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/plug_monitor_hlw8032.txt
+-rw-r--r--   0        0        0      914 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/plug_total.txt
+-rw-r--r--   0        0        0      777 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/tests/switch_monitor.txt
+-rw-r--r--   0        0        0      922 2023-05-20 16:29:21.105016 upk2esphome-1.1.0/upk2esphome/web.py
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 upk2esphome-1.1.0/PKG-INFO
```

### Comparing `upk2esphome-1.0.2/LICENSE` & `upk2esphome-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/README.md` & `upk2esphome-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/generator.py` & `upk2esphome-1.1.0/upk2esphome/generator.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/input.py` & `upk2esphome-1.1.0/upk2esphome/input.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/parts/bulb.py` & `upk2esphome-1.1.0/upk2esphome/parts/bulb.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/parts/module.py` & `upk2esphome-1.1.0/upk2esphome/parts/module.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/parts/monitor.py` & `upk2esphome-1.1.0/upk2esphome/parts/monitor.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/parts/netled.py` & `upk2esphome-1.1.0/upk2esphome/parts/netled.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/parts/static.py` & `upk2esphome-1.1.0/upk2esphome/parts/static.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/parts/switch.py` & `upk2esphome-1.1.0/upk2esphome/parts/switch.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/result.py` & `upk2esphome-1.1.0/upk2esphome/result.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/test.py` & `upk2esphome-1.1.0/upk2esphome/test.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbc_2135_2.txt` & `upk2esphome-1.1.0/upk2esphome/tests/bulb_rgbc_2135_2.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt` & `upk2esphome-1.1.0/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_2235.txt` & `upk2esphome-1.1.0/upk2esphome/tests/bulb_rgbcw_2235.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/tests/plug_monitor_bl0937.txt` & `upk2esphome-1.1.0/upk2esphome/tests/plug_monitor_bl0937.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/tests/plug_total.txt` & `upk2esphome-1.1.0/upk2esphome/tests/plug_total.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/tests/switch_monitor.txt` & `upk2esphome-1.1.0/upk2esphome/tests/switch_monitor.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/upk2esphome/web.py` & `upk2esphome-1.1.0/upk2esphome/web.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.2/PKG-INFO` & `upk2esphome-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: upk2esphome
-Version: 1.0.2
-Summary: Convert Tuya device configuration to ESPHome YAML
+Version: 1.1.0
+Summary: Convert Tuya device configuration to ESPHome YAML (ltchiptool plugin)
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

