# Comparing `tmp/sensors_connectivity-1.4.0.tar.gz` & `tmp/sensors_connectivity-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensors_connectivity-1.4.0.tar", max compression
+gzip compressed data, was "sensors_connectivity-1.4.1.tar", max compression
```

## Comparing `sensors_connectivity-1.4.0.tar` & `sensors_connectivity-1.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1507 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/LICENSE
--rw-r--r--   0        0        0     6281 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/README.md
--rw-r--r--   0        0        0       24 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/__init__.py
--rw-r--r--   0        0        0     9099 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/config/README.md
--rw-r--r--   0        0        0       36 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/config/__init__.py
--rw-r--r--   0        0        0     1006 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/config/default.json
--rw-r--r--   0        0        0      938 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/config/logging.py
--rw-r--r--   0        0        0      824 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/config/logging_template.py
--rw-r--r--   0        0        0       94 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/constants.py
--rw-r--r--   0        0        0     5975 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/main.py
--rw-r--r--   0        0        0       51 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/drivers/__init__.py
--rw-r--r--   0        0        0      477 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/drivers/ping.py
--rw-r--r--   0        0        0     5754 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/drivers/sds011.py
--rw-r--r--   0        0        0      189 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/feeders/__init__.py
--rw-r--r--   0        0        0     8956 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/feeders/datalog_feeder.py
--rw-r--r--   0        0        0     1280 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/feeders/frontier_datalog.py
--rw-r--r--   0        0        0     1088 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/feeders/ifeeder.py
--rw-r--r--   0        0        0     3166 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/feeders/robonomics_feeder.py
--rw-r--r--   0        0        0      224 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/base.py
--rw-r--r--   0        0        0     2046 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/environmental_box.py
--rw-r--r--   0        0        0      643 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/lora_sensors.py
--rw-r--r--   0        0        0     1443 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/mobile_lab.py
--rw-r--r--   0        0        0     1427 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/sensor_sds011.py
--rw-r--r--   0        0        0      771 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/sensor_template.py
--rw-r--r--   0        0        0     2572 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/sensors/trackagro_sensor.py
--rw-r--r--   0        0        0      212 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/__init__.py
--rw-r--r--   0        0        0     2238 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/comstation.py
--rw-r--r--   0        0        0     4380 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/httpstation.py
--rw-r--r--   0        0        0     1639 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/istation.py
--rw-r--r--   0        0        0     4055 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/mqttstation.py
--rw-r--r--   0        0        0     3089 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/src/stations/trackargostation.py
--rw-r--r--   0        0        0       55 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/__init__.py
--rw-r--r--   0        0        0     2705 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/database.py
--rwxr-xr-x   0        0        0     3207 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/flash_firmware.py
--rwxr-xr-x   0        0        0     1825 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/generate_secrets.py
--rw-r--r--   0        0        0      391 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/get_mac.py
--rwxr-xr-x   0        0        0      553 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/py_generate_secrets.py
--rwxr-xr-x   0        0        0     2502 2023-04-11 13:26:12.141418 sensors_connectivity-1.4.0/connectivity/utils/virtual-sensor.py
--rw-r--r--   0        0        0     1174 2023-04-11 13:26:12.145418 sensors_connectivity-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     7507 1970-01-01 00:00:00.000000 sensors_connectivity-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1507 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/LICENSE
+-rw-r--r--   0        0        0     6281 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/README.md
+-rw-r--r--   0        0        0       24 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/__init__.py
+-rw-r--r--   0        0        0     9099 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/config/README.md
+-rw-r--r--   0        0        0       36 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/config/__init__.py
+-rw-r--r--   0        0        0     1006 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/config/default.json
+-rw-r--r--   0        0        0      938 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/config/logging.py
+-rw-r--r--   0        0        0      824 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/config/logging_template.py
+-rw-r--r--   0        0        0       94 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/constants.py
+-rw-r--r--   0        0        0     5975 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/main.py
+-rw-r--r--   0        0        0       51 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/drivers/__init__.py
+-rw-r--r--   0        0        0      477 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/drivers/ping.py
+-rw-r--r--   0        0        0     5754 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/drivers/sds011.py
+-rw-r--r--   0        0        0      189 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/feeders/__init__.py
+-rw-r--r--   0        0        0     9105 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/feeders/datalog_feeder.py
+-rw-r--r--   0        0        0     1280 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/feeders/frontier_datalog.py
+-rw-r--r--   0        0        0     1088 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/feeders/ifeeder.py
+-rw-r--r--   0        0        0     3166 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/feeders/robonomics_feeder.py
+-rw-r--r--   0        0        0      224 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/__init__.py
+-rw-r--r--   0        0        0     1461 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/base.py
+-rw-r--r--   0        0        0     2077 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/environmental_box.py
+-rw-r--r--   0        0        0      643 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/lora_sensors.py
+-rw-r--r--   0        0        0     1474 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/mobile_lab.py
+-rw-r--r--   0        0        0     1427 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/sensor_sds011.py
+-rw-r--r--   0        0        0      771 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/sensor_template.py
+-rw-r--r--   0        0        0     2603 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/trackagro_sensor.py
+-rw-r--r--   0        0        0      212 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/stations/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/stations/comstation.py
+-rw-r--r--   0        0        0     4380 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/stations/httpstation.py
+-rw-r--r--   0        0        0     1639 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/stations/istation.py
+-rw-r--r--   0        0        0     4055 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/stations/mqttstation.py
+-rw-r--r--   0        0        0     3089 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/src/stations/trackargostation.py
+-rw-r--r--   0        0        0       55 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/__init__.py
+-rw-r--r--   0        0        0     2705 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/database.py
+-rwxr-xr-x   0        0        0     3207 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/flash_firmware.py
+-rwxr-xr-x   0        0        0     1825 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/generate_secrets.py
+-rw-r--r--   0        0        0      391 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/get_mac.py
+-rwxr-xr-x   0        0        0      553 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/py_generate_secrets.py
+-rwxr-xr-x   0        0        0     2502 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/virtual-sensor.py
+-rw-r--r--   0        0        0     1174 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7507 1970-01-01 00:00:00.000000 sensors_connectivity-1.4.1/PKG-INFO
```

### Comparing `sensors_connectivity-1.4.0/LICENSE` & `sensors_connectivity-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/README.md` & `sensors_connectivity-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/config/README.md` & `sensors_connectivity-1.4.1/connectivity/config/README.md`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/config/default.json` & `sensors_connectivity-1.4.1/connectivity/config/default.json`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/config/logging.py` & `sensors_connectivity-1.4.1/connectivity/config/logging.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/config/logging_template.py` & `sensors_connectivity-1.4.1/connectivity/config/logging_template.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/main.py` & `sensors_connectivity-1.4.1/connectivity/main.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/drivers/sds011.py` & `sensors_connectivity-1.4.1/connectivity/src/drivers/sds011.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/feeders/datalog_feeder.py` & `sensors_connectivity-1.4.1/connectivity/src/feeders/datalog_feeder.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,22 +64,26 @@
     :param db: Database class object.
     :param endpoint: Endpoint for IPFS node. Default is local.
     :return: IPFS hash of the file and path to the temp file.
     """
 
     payload = {}
     for m in buf:
-        if m.public in payload:
-            payload[m.public]["measurements"].append(m.measurement)
-        else:
-            payload[m.public] = {
-                "model": m.model,
-                "geo": "{},{}".format(m.geo_lat, m.geo_lon),
-                "measurements": [m.measurement],
-            }
+        try:
+            if m.public in payload:
+                payload[m.public]["measurements"].append(m.measurement)
+            else:
+                payload[m.public] = {
+                    "model": m.model,
+                    "geo": "{},{}".format(m.geo_lat, m.geo_lon),
+                    "measurements": [m.measurement],
+                }
+        except Exception as e:
+            logger.warning(f"Datalog Feeder: Couldn't store data: {e}")
+
 
     logger.debug(f"Payload before sorting: {payload}")
     payload = _sort_payload(payload)
     logger.debug(f"Payload sorted: {payload}")
     try:
         temp = NamedTemporaryFile(mode="w", delete=False)
         logger.debug(f"Created temp file: {temp.name}")
```

### Comparing `sensors_connectivity-1.4.0/connectivity/src/feeders/frontier_datalog.py` & `sensors_connectivity-1.4.1/connectivity/src/feeders/frontier_datalog.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/feeders/ifeeder.py` & `sensors_connectivity-1.4.1/connectivity/src/feeders/ifeeder.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/feeders/robonomics_feeder.py` & `sensors_connectivity-1.4.1/connectivity/src/feeders/robonomics_feeder.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/sensors/base.py` & `sensors_connectivity-1.4.1/connectivity/src/sensors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     geo_lon: float = field(init=False)
     model: int = field(init=False)
     timestamp: float = field(init=False)
     measurement: dict = field(init=False)
 
     def __post_init__(self) -> None:
         self.timestamp = int(time.time())
+        self.geo_lat = 0.0
+        self.geo_lon = 0.0
+        self.measurement = {}
         self.measurement.update({"timestamp": self.timestamp})
 
     def generate_pubkey(self, id: str) -> str:
         """Generate public key for a sensor based on its id.
         
         :param id: Unique id of a sensor.
         :return: Public key of a sensor.
```

### Comparing `sensors_connectivity-1.4.0/connectivity/src/sensors/environmental_box.py` & `sensors_connectivity-1.4.1/connectivity/src/sensors/environmental_box.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     :param data: Unparsed data from the sensor.
     """
 
     data: dict = field(repr=False)
 
     def __post_init__(self) -> None:
         """Parse data from sensor and store into the corresponding variables."""
-
+        super().__post_init__()
         self.id = str(self.data["esp8266id"])
         self.model = SDS011_MODEL
         self.public = self.generate_pubkey(str(self.id))
         sensors_data = self.data["sensordatavalues"]
         for d in sensors_data:
             if d["value_type"] == "GPS_lat":
                 self.geo_lat = d["value"]
```

### Comparing `sensors_connectivity-1.4.0/connectivity/src/sensors/lora_sensors.py` & `sensors_connectivity-1.4.1/connectivity/src/sensors/lora_sensors.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/sensors/mobile_lab.py` & `sensors_connectivity-1.4.1/connectivity/src/sensors/mobile_lab.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     :param data: Unparsed data from the sensor.
     """
 
     data: dict = field(repr=False)
 
     def __post_init__(self) -> None:
         """Parse data from sensor and store into the corresponding variables."""
-
+        super().__post_init__()
         self.id = self.data["ID"]
         self.model = MOBILE_GPS
         self.public = self.generate_pubkey(str(self.id))
         self.geo_lat = float(self.data.get("GPS_lat"))
         self.geo_lon = float(self.data.get("GPS_lon"))
         self.measurement = reduce(self._mobile_sensor_data_saver, self.data.items(), {})
         self.timestamp = int(time.time())
```

### Comparing `sensors_connectivity-1.4.0/connectivity/src/sensors/sensor_sds011.py` & `sensors_connectivity-1.4.1/connectivity/src/sensors/sensor_sds011.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/sensors/sensor_template.py` & `sensors_connectivity-1.4.1/connectivity/src/sensors/sensor_template.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/sensors/trackagro_sensor.py` & `sensors_connectivity-1.4.1/connectivity/src/sensors/trackagro_sensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """
 
     data: tp.List[tp.Dict[str, tp.Union[str, int, float]]]
     _time_from: int
 
     def __post_init__(self) -> None:
         """Parse data from sensor and store into the corresponding variables."""
-
+        super().__post_init__()
         self.model = SDS011_MODEL
         meas = self._parse_data()
         if meas:
             self.measurement = meas
             self.public = self.generate_pubkey(self.id)
 
     @property
```

### Comparing `sensors_connectivity-1.4.0/connectivity/src/stations/comstation.py` & `sensors_connectivity-1.4.1/connectivity/src/stations/comstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/stations/httpstation.py` & `sensors_connectivity-1.4.1/connectivity/src/stations/httpstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/stations/istation.py` & `sensors_connectivity-1.4.1/connectivity/src/stations/istation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/stations/mqttstation.py` & `sensors_connectivity-1.4.1/connectivity/src/stations/mqttstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/src/stations/trackargostation.py` & `sensors_connectivity-1.4.1/connectivity/src/stations/trackargostation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/utils/database.py` & `sensors_connectivity-1.4.1/connectivity/utils/database.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/utils/flash_firmware.py` & `sensors_connectivity-1.4.1/connectivity/utils/flash_firmware.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/utils/generate_secrets.py` & `sensors_connectivity-1.4.1/connectivity/utils/generate_secrets.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/utils/py_generate_secrets.py` & `sensors_connectivity-1.4.1/connectivity/utils/py_generate_secrets.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/connectivity/utils/virtual-sensor.py` & `sensors_connectivity-1.4.1/connectivity/utils/virtual-sensor.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.0/pyproject.toml` & `sensors_connectivity-1.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sensors_connectivity"
-version = "1.4.0"
+version = "1.4.1"
 description = "Robonomics package to read data from sensors and publish to different output channels"
 authors = [
     "Vadim Manaenko <vadim.razorq@gmail.com>",
     "Mariia Bystramovich <m.bystramovich@gmail.com>",
 ]
 license = "BSD 3-Clause License"
```

### Comparing `sensors_connectivity-1.4.0/PKG-INFO` & `sensors_connectivity-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensors-connectivity
-Version: 1.4.0
+Version: 1.4.1
 Summary: Robonomics package to read data from sensors and publish to different output channels
 Home-page: https://github.com/airalab/sensors-connectivity
 License: BSD 3-Clause License
 Author: Vadim Manaenko
 Author-email: vadim.razorq@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

