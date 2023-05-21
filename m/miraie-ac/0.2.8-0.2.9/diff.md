# Comparing `tmp/miraie-ac-0.2.8.tar.gz` & `tmp/miraie-ac-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miraie-ac-0.2.8.tar", last modified: Mon Nov 14 14:50:25 2022, max compression
+gzip compressed data, was "miraie-ac-0.2.9.tar", last modified: Mon Nov 14 14:53:57 2022, max compression
```

## Comparing `miraie-ac-0.2.8.tar` & `miraie-ac-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-14 14:50:25.366813 miraie-ac-0.2.8/
--rw-rw-rw-   0        0        0     1089 2022-11-14 08:12:24.000000 miraie-ac-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      738 2022-11-14 14:50:25.365813 miraie-ac-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      471 2022-11-14 11:24:06.000000 miraie-ac-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2022-11-14 14:50:25.355251 miraie-ac-0.2.8/miraie_ac/
--rw-rw-rw-   0        0        0      295 2022-11-14 13:55:24.000000 miraie-ac-0.2.8/miraie_ac/__init__.py
--rw-rw-rw-   0        0        0     4629 2022-11-14 14:33:23.000000 miraie-ac-0.2.8/miraie_ac/broker.py
--rw-rw-rw-   0        0        0      649 2022-11-14 08:12:24.000000 miraie-ac-0.2.8/miraie_ac/constants.py
--rw-rw-rw-   0        0        0     4568 2022-11-14 14:50:13.000000 miraie-ac-0.2.8/miraie_ac/device.py
--rw-rw-rw-   0        0        0      770 2022-11-14 14:02:53.000000 miraie-ac-0.2.8/miraie_ac/enums.py
--rw-rw-rw-   0        0        0      351 2022-11-14 08:12:24.000000 miraie-ac-0.2.8/miraie_ac/home.py
--rw-rw-rw-   0        0        0     7002 2022-11-14 14:48:42.000000 miraie-ac-0.2.8/miraie_ac/hub.py
--rw-rw-rw-   0        0        0      363 2022-11-14 08:12:24.000000 miraie-ac-0.2.8/miraie_ac/topic.py
--rw-rw-rw-   0        0        0      368 2022-11-14 08:12:24.000000 miraie-ac-0.2.8/miraie_ac/user.py
-drwxrwxrwx   0        0        0        0 2022-11-14 14:50:25.365813 miraie-ac-0.2.8/miraie_ac.egg-info/
--rw-rw-rw-   0        0        0      738 2022-11-14 14:50:25.000000 miraie-ac-0.2.8/miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2022-11-14 14:50:25.000000 miraie-ac-0.2.8/miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-14 14:50:25.000000 miraie-ac-0.2.8/miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-11-14 14:50:25.000000 miraie-ac-0.2.8/miraie_ac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-14 14:50:25.366813 miraie-ac-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      972 2022-11-14 14:50:22.000000 miraie-ac-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-14 14:53:57.654069 miraie-ac-0.2.9/
+-rw-rw-rw-   0        0        0     1089 2022-11-14 08:12:24.000000 miraie-ac-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      738 2022-11-14 14:53:57.654069 miraie-ac-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2022-11-14 11:24:06.000000 miraie-ac-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2022-11-14 14:53:57.636007 miraie-ac-0.2.9/miraie_ac/
+-rw-rw-rw-   0        0        0      295 2022-11-14 13:55:24.000000 miraie-ac-0.2.9/miraie_ac/__init__.py
+-rw-rw-rw-   0        0        0     4629 2022-11-14 14:33:23.000000 miraie-ac-0.2.9/miraie_ac/broker.py
+-rw-rw-rw-   0        0        0      649 2022-11-14 08:12:24.000000 miraie-ac-0.2.9/miraie_ac/constants.py
+-rw-rw-rw-   0        0        0     4568 2022-11-14 14:50:13.000000 miraie-ac-0.2.9/miraie_ac/device.py
+-rw-rw-rw-   0        0        0      770 2022-11-14 14:02:53.000000 miraie-ac-0.2.9/miraie_ac/enums.py
+-rw-rw-rw-   0        0        0      351 2022-11-14 08:12:24.000000 miraie-ac-0.2.9/miraie_ac/home.py
+-rw-rw-rw-   0        0        0     6903 2022-11-14 14:53:33.000000 miraie-ac-0.2.9/miraie_ac/hub.py
+-rw-rw-rw-   0        0        0      363 2022-11-14 08:12:24.000000 miraie-ac-0.2.9/miraie_ac/topic.py
+-rw-rw-rw-   0        0        0      368 2022-11-14 08:12:24.000000 miraie-ac-0.2.9/miraie_ac/user.py
+drwxrwxrwx   0        0        0        0 2022-11-14 14:53:57.653057 miraie-ac-0.2.9/miraie_ac.egg-info/
+-rw-rw-rw-   0        0        0      738 2022-11-14 14:53:57.000000 miraie-ac-0.2.9/miraie_ac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2022-11-14 14:53:57.000000 miraie-ac-0.2.9/miraie_ac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-14 14:53:57.000000 miraie-ac-0.2.9/miraie_ac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2022-11-14 14:53:57.000000 miraie-ac-0.2.9/miraie_ac.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-14 14:53:57.655068 miraie-ac-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      972 2022-11-14 14:53:52.000000 miraie-ac-0.2.9/setup.py
```

### Comparing `miraie-ac-0.2.8/LICENSE` & `miraie-ac-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `miraie-ac-0.2.8/PKG-INFO` & `miraie-ac-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miraie-ac
-Version: 0.2.8
+Version: 0.2.9
 Summary: MirAIe-AC API for Python
 Home-page: https://github.com/Kir4Kun/miraie-ac
 Author: Kir4Kun
 Author-email: rkbl4ze@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `miraie-ac-0.2.8/miraie_ac/broker.py` & `miraie-ac-0.2.9/miraie_ac/broker.py`

 * *Files identical despite different names*

### Comparing `miraie-ac-0.2.8/miraie_ac/constants.py` & `miraie-ac-0.2.9/miraie_ac/constants.py`

 * *Files identical despite different names*

### Comparing `miraie-ac-0.2.8/miraie_ac/device.py` & `miraie-ac-0.2.9/miraie_ac/device.py`

 * *Files identical despite different names*

### Comparing `miraie-ac-0.2.8/miraie_ac/enums.py` & `miraie-ac-0.2.9/miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `miraie-ac-0.2.8/miraie_ac/hub.py` & `miraie-ac-0.2.9/miraie_ac/hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,26 +155,24 @@
 
         for index in range(0, len(statuses)):
             device = self.home.devices[index]
             status = statuses[index]
 
             status_obj: DeviceStatus
             if "ty" not in status:
-                status_obj = device.set_status(
-                    DeviceStatus(
-                        is_online=False,
-                        temperature=24.0,
-                        room_temperature=24.0,
-                        power_mode=PowerMode.OFF,
-                        fan_mode=FanMode.AUTO,
-                        swing_mode=SwingMode.AUTO,
-                        display_mode=DisplayMode.ON,
-                        hvac_mode=HVACMode.AUTO,
-                        preset_mode=PresetMode.NONE,
-                    )
+                status_obj = DeviceStatus(
+                    is_online=False,
+                    temperature=24.0,
+                    room_temperature=24.0,
+                    power_mode=PowerMode.OFF,
+                    fan_mode=FanMode.AUTO,
+                    swing_mode=SwingMode.AUTO,
+                    display_mode=DisplayMode.ON,
+                    hvac_mode=HVACMode.AUTO,
+                    preset_mode=PresetMode.NONE,
                 )
             else:
                 status_obj = DeviceStatus(
                     is_online=status["onlineStatus"] == "true",
                     temperature=float(status["actmp"]),
                     room_temperature=float(status["rmtmp"]),
                     power_mode=PowerMode(status["ps"]),
```

### Comparing `miraie-ac-0.2.8/miraie_ac.egg-info/PKG-INFO` & `miraie-ac-0.2.9/miraie_ac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miraie-ac
-Version: 0.2.8
+Version: 0.2.9
 Summary: MirAIe-AC API for Python
 Home-page: https://github.com/Kir4Kun/miraie-ac
 Author: Kir4Kun
 Author-email: rkbl4ze@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `miraie-ac-0.2.8/setup.py` & `miraie-ac-0.2.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Always prefer setuptools over distutils
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="miraie-ac",
-    version="0.2.8",
+    version="0.2.9",
     description="MirAIe-AC API for Python",
     long_description="MirAIe-AC API for Python",
     long_description_content_type="text/markdown",
     url="https://github.com/Kir4Kun/miraie-ac",
     author="Kir4Kun",
     author_email="rkbl4ze@gmail.com",
     license="MIT",
```

