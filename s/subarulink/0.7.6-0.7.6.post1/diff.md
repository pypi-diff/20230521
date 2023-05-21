# Comparing `tmp/subarulink-0.7.6.tar.gz` & `tmp/subarulink-0.7.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subarulink-0.7.6.tar", last modified: Fri Apr  7 05:06:35 2023, max compression
+gzip compressed data, was "subarulink-0.7.6.post1.tar", last modified: Sun May 21 15:46:10 2023, max compression
```

## Comparing `subarulink-0.7.6.tar` & `subarulink-0.7.6.post1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-04-07 05:06:35.117887 subarulink-0.7.6/
--rw-r--r--   0 gg         (501) wheel        (0)      195 2022-02-12 17:50:33.000000 subarulink-0.7.6/AUTHORS.md
--rw-r--r--   0 gg         (501) wheel        (0)     6362 2022-03-30 01:34:05.000000 subarulink-0.7.6/DEVELOPERS.md
--rw-r--r--   0 gg         (501) wheel        (0)    11358 2020-10-11 22:38:54.000000 subarulink-0.7.6/LICENSE
--rw-r--r--   0 gg         (501) wheel        (0)       30 2022-02-12 17:49:18.000000 subarulink-0.7.6/MANIFEST.in
--rw-r--r--   0 gg         (501) wheel        (0)     8286 2023-04-07 05:06:35.117973 subarulink-0.7.6/PKG-INFO
--rw-r--r--   0 gg         (501) wheel        (0)     7680 2022-12-08 02:51:09.000000 subarulink-0.7.6/README.md
--rw-r--r--   0 gg         (501) wheel        (0)     2479 2022-12-18 23:12:31.000000 subarulink-0.7.6/pyproject.toml
--rw-r--r--   0 gg         (501) wheel        (0)      509 2023-04-07 05:06:35.118271 subarulink-0.7.6/setup.cfg
--rw-r--r--   0 gg         (501) wheel        (0)     3971 2022-12-08 02:51:09.000000 subarulink-0.7.6/setup.py
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-04-07 05:06:35.114945 subarulink-0.7.6/subarulink/
--rw-r--r--   0 gg         (501) wheel        (0)      808 2022-12-03 21:57:17.000000 subarulink-0.7.6/subarulink/__init__.py
--rw-r--r--   0 gg         (501) wheel        (0)      264 2023-04-07 04:54:03.000000 subarulink-0.7.6/subarulink/__version__.py
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-04-07 05:06:35.116036 subarulink-0.7.6/subarulink/_subaru_api/
--rw-r--r--   0 gg         (501) wheel        (0)      204 2022-12-08 02:51:09.000000 subarulink-0.7.6/subarulink/_subaru_api/__init__.py
--rw-r--r--   0 gg         (501) wheel        (0)     7266 2023-04-07 04:49:31.000000 subarulink-0.7.6/subarulink/_subaru_api/const.py
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-04-07 05:06:35.116476 subarulink-0.7.6/subarulink/app/
--rw-r--r--   0 gg         (501) wheel        (0)      219 2022-02-12 17:50:33.000000 subarulink-0.7.6/subarulink/app/__init__.py
--rw-r--r--   0 gg         (501) wheel        (0)    29784 2023-02-18 01:13:37.000000 subarulink-0.7.6/subarulink/app/cli.py
--rw-r--r--   0 gg         (501) wheel        (0)    13768 2023-01-21 17:52:41.000000 subarulink-0.7.6/subarulink/connection.py
--rw-r--r--   0 gg         (501) wheel        (0)     7433 2023-01-21 17:52:41.000000 subarulink-0.7.6/subarulink/const.py
--rw-r--r--   0 gg         (501) wheel        (0)    56482 2023-01-21 17:55:31.000000 subarulink-0.7.6/subarulink/controller.py
--rw-r--r--   0 gg         (501) wheel        (0)     1187 2020-12-24 00:13:12.000000 subarulink-0.7.6/subarulink/exceptions.py
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-04-07 05:06:35.115706 subarulink-0.7.6/subarulink.egg-info/
--rw-r--r--   0 gg         (501) wheel        (0)     8286 2023-04-07 05:06:35.000000 subarulink-0.7.6/subarulink.egg-info/PKG-INFO
--rw-r--r--   0 gg         (501) wheel        (0)      656 2023-04-07 05:06:35.000000 subarulink-0.7.6/subarulink.egg-info/SOURCES.txt
--rw-r--r--   0 gg         (501) wheel        (0)        1 2023-04-07 05:06:35.000000 subarulink-0.7.6/subarulink.egg-info/dependency_links.txt
--rw-r--r--   0 gg         (501) wheel        (0)       55 2023-04-07 05:06:35.000000 subarulink-0.7.6/subarulink.egg-info/entry_points.txt
--rw-r--r--   0 gg         (501) wheel        (0)       18 2023-04-07 05:06:35.000000 subarulink-0.7.6/subarulink.egg-info/requires.txt
--rw-r--r--   0 gg         (501) wheel        (0)       11 2023-04-07 05:06:35.000000 subarulink-0.7.6/subarulink.egg-info/top_level.txt
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-04-07 05:06:35.117750 subarulink-0.7.6/tests/
--rw-r--r--   0 gg         (501) wheel        (0)     4575 2023-01-21 17:52:41.000000 subarulink-0.7.6/tests/test_cli.py
--rw-r--r--   0 gg         (501) wheel        (0)    15062 2023-01-21 17:52:41.000000 subarulink-0.7.6/tests/test_connection.py
--rw-r--r--   0 gg         (501) wheel        (0)    15911 2022-12-18 20:24:35.000000 subarulink-0.7.6/tests/test_remote_commands.py
--rw-r--r--   0 gg         (501) wheel        (0)     9684 2023-01-21 17:52:41.000000 subarulink-0.7.6/tests/test_vehicle_status.py
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-05-21 15:46:10.524129 subarulink-0.7.6.post1/
+-rw-r--r--   0 gg         (501) wheel        (0)      195 2022-02-12 17:50:33.000000 subarulink-0.7.6.post1/AUTHORS.md
+-rw-r--r--   0 gg         (501) wheel        (0)     6362 2022-03-30 01:34:05.000000 subarulink-0.7.6.post1/DEVELOPERS.md
+-rw-r--r--   0 gg         (501) wheel        (0)    11358 2020-10-11 22:38:54.000000 subarulink-0.7.6.post1/LICENSE
+-rw-r--r--   0 gg         (501) wheel        (0)       30 2022-02-12 17:49:18.000000 subarulink-0.7.6.post1/MANIFEST.in
+-rw-r--r--   0 gg         (501) wheel        (0)     8203 2023-05-21 15:46:10.524201 subarulink-0.7.6.post1/PKG-INFO
+-rw-r--r--   0 gg         (501) wheel        (0)     7591 2023-05-21 15:44:58.000000 subarulink-0.7.6.post1/README.md
+-rw-r--r--   0 gg         (501) wheel        (0)     2479 2022-12-18 23:12:31.000000 subarulink-0.7.6.post1/pyproject.toml
+-rw-r--r--   0 gg         (501) wheel        (0)      509 2023-05-21 15:46:10.524511 subarulink-0.7.6.post1/setup.cfg
+-rw-r--r--   0 gg         (501) wheel        (0)     3971 2022-12-08 02:51:09.000000 subarulink-0.7.6.post1/setup.py
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-05-21 15:46:10.520447 subarulink-0.7.6.post1/subarulink/
+-rw-r--r--   0 gg         (501) wheel        (0)      808 2022-12-03 21:57:17.000000 subarulink-0.7.6.post1/subarulink/__init__.py
+-rw-r--r--   0 gg         (501) wheel        (0)      266 2023-05-21 15:45:55.000000 subarulink-0.7.6.post1/subarulink/__version__.py
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-05-21 15:46:10.521929 subarulink-0.7.6.post1/subarulink/_subaru_api/
+-rw-r--r--   0 gg         (501) wheel        (0)      204 2022-12-08 02:51:09.000000 subarulink-0.7.6.post1/subarulink/_subaru_api/__init__.py
+-rw-r--r--   0 gg         (501) wheel        (0)     7266 2023-04-07 05:56:35.000000 subarulink-0.7.6.post1/subarulink/_subaru_api/const.py
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-05-21 15:46:10.522491 subarulink-0.7.6.post1/subarulink/app/
+-rw-r--r--   0 gg         (501) wheel        (0)      219 2022-02-12 17:50:33.000000 subarulink-0.7.6.post1/subarulink/app/__init__.py
+-rw-r--r--   0 gg         (501) wheel        (0)    29784 2023-02-18 01:13:37.000000 subarulink-0.7.6.post1/subarulink/app/cli.py
+-rw-r--r--   0 gg         (501) wheel        (0)    13734 2023-04-08 01:17:29.000000 subarulink-0.7.6.post1/subarulink/connection.py
+-rw-r--r--   0 gg         (501) wheel        (0)     7433 2023-01-21 17:52:41.000000 subarulink-0.7.6.post1/subarulink/const.py
+-rw-r--r--   0 gg         (501) wheel        (0)    56337 2023-04-08 01:17:38.000000 subarulink-0.7.6.post1/subarulink/controller.py
+-rw-r--r--   0 gg         (501) wheel        (0)     1187 2020-12-24 00:13:12.000000 subarulink-0.7.6.post1/subarulink/exceptions.py
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-05-21 15:46:10.521528 subarulink-0.7.6.post1/subarulink.egg-info/
+-rw-r--r--   0 gg         (501) wheel        (0)     8203 2023-05-21 15:46:10.000000 subarulink-0.7.6.post1/subarulink.egg-info/PKG-INFO
+-rw-r--r--   0 gg         (501) wheel        (0)      656 2023-05-21 15:46:10.000000 subarulink-0.7.6.post1/subarulink.egg-info/SOURCES.txt
+-rw-r--r--   0 gg         (501) wheel        (0)        1 2023-05-21 15:46:10.000000 subarulink-0.7.6.post1/subarulink.egg-info/dependency_links.txt
+-rw-r--r--   0 gg         (501) wheel        (0)       55 2023-05-21 15:46:10.000000 subarulink-0.7.6.post1/subarulink.egg-info/entry_points.txt
+-rw-r--r--   0 gg         (501) wheel        (0)       18 2023-05-21 15:46:10.000000 subarulink-0.7.6.post1/subarulink.egg-info/requires.txt
+-rw-r--r--   0 gg         (501) wheel        (0)       11 2023-05-21 15:46:10.000000 subarulink-0.7.6.post1/subarulink.egg-info/top_level.txt
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-05-21 15:46:10.523972 subarulink-0.7.6.post1/tests/
+-rw-r--r--   0 gg         (501) wheel        (0)     4575 2023-01-21 17:52:41.000000 subarulink-0.7.6.post1/tests/test_cli.py
+-rw-r--r--   0 gg         (501) wheel        (0)    15062 2023-01-21 17:52:41.000000 subarulink-0.7.6.post1/tests/test_connection.py
+-rw-r--r--   0 gg         (501) wheel        (0)    15911 2022-12-18 20:24:35.000000 subarulink-0.7.6.post1/tests/test_remote_commands.py
+-rw-r--r--   0 gg         (501) wheel        (0)     9684 2023-01-21 17:52:41.000000 subarulink-0.7.6.post1/tests/test_vehicle_status.py
```

### Comparing `subarulink-0.7.6/DEVELOPERS.md` & `subarulink-0.7.6.post1/DEVELOPERS.md`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/LICENSE` & `subarulink-0.7.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/PKG-INFO` & `subarulink-0.7.6.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subarulink
-Version: 0.7.6
+Version: 0.7.6.post1
 Summary: A package for interacting with Subaru Starlink Remote Services API.
 Home-page: https://github.com/G-Two/subarulink
 Author: G-Two
 Author-email: 
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -25,21 +25,22 @@
 
 This package supports Subaru STARLINK equipped vehicles with active service plans. A [MySubaru](https://www.mysubaru.com) account must be setup prior to using this package. The features available will depend on the model year and type of service plan (Safety Plus or Safety/Security Plus).
 
 
 | Model Year   | Safety Plus | Security Plus |
 |--------------|-------------|---------------|
 | 2016-2018    |  No Support | Remote Lock/Unlock <br> Remote Horn and/or Lights <br> Remote Vehicle Locator <br> Odometer (updated every 500 miles) 
-| 2019+        |  Tire Pressure# <br> Fuel Economy# <br> Fuel Range# <br> Odometer#     |Remote Lock/Unlock <br> Remote Horn and/or Lights <br> Remote Vehicle Locator <br> Remote Engine Start w/ Climate Control <br> PHEV Start Charge* <br> Door/Window Status** <br> Tire Pressure <br> Fuel Economy <br> Fuel Range <br> Odometer
+| 2019+        |  Tire Pressure# <br> Fuel Economy# <br> Fuel Range# <br> Odometer#     |Remote Lock/Unlock <br> Remote Horn and/or Lights <br> Remote Vehicle Locator <br> Remote Engine Start w/ Climate Control <br> EV Start Charge* <br> Door/Window/Sunroof Status** <br> Tire Pressure <br> Fuel Economy <br> Fuel Range <br> Odometer
 
 \# Unclear how often this is updated <br>
-\* Plug-In hybrid only <br>
-\*\* Support varies by model
+\* EV/PHEV only <br>
+\*\* Support varies by model/year
 
-**NOTE:**  This project was developed based upon analysis of the official MySubaru Android app. Subaru has no official public API; therefore, this library may stop working at any time without warning.  Use at your own risk.
+> **NOTE:**
+> This project was developed based upon analysis of the official MySubaru Android app. Subaru has no official public API; therefore, this library may stop working at any time without warning.  Use at your own risk.
 
 
 ## Home Assistant Integration
 
 There is a Home Assistant [custom component](https://github.com/G-Two/homeassistant-subaru) that uses this package and allows users to add Subaru STARLINK integration to their Home Assistant instance.
 
 In addition, as of 2021.3, Home Assistant Core includes the [Subaru integration](https://www.home-assistant.io/integrations/subaru/) that uses this package. Due to the required incremental additions required by Home Assistant Core, only the sensor and lock platforms are supported at this time. Additional PRs are pending to add full functionality. Users that desire the most recent features should continue using the custom component.
@@ -87,15 +88,15 @@
 Accounts with only one vehicle do not need to specify a VIN
 
 ## Configuration
 A JSON file is used for configuration. A user provided file can be passed to the CLI via the `--config`. If no config file is provided, two default locations are searched for. First is `~/.subarulink.cfg` and if that is not found, `$XDG_CONFIG_HOME/subarulink/subarulink.cfg` will be used.
 
 ## Known Issues
 ### Battery Discharge
-Aggressively polling the vehicle location with subarulink.Controller.update(vin) may discharge the auxiliary battery (in a PHEV).  Intermittent (every 2 hours) use isn't a problem, but polling at 5 minute intervals will drain the auxiliary battery fully after a few consecutive non-driving days.  The vehicle does report the auxiliary battery voltage with every update, so this can be avoided.  
+Aggressively polling the vehicle location with subarulink.Controller.update(vin) may discharge the auxiliary 12V battery (in a PHEV).  Intermittent (every 2 hours) use isn't a problem, but polling at 5 minute intervals will drain the auxiliary battery fully after a few consecutive non-driving days.
 
 Effects of aggressive polling on the battery of a gasoline-only vehicle are unknown.
 
 ### Stale Data
 Sensor data is only sent by the vehicle during certain events (e.g. engine shutdown or a user requested location update) and should not be relied on to indicate a vehicle's real time status. If more recent data is desired, then the user must initiate a location update which will update the data for all sensors (exception: tire pressures will only be updated if the vehicle is in motion).
 
 ### Remote climate control preset options vary by model
```

### Comparing `subarulink-0.7.6/README.md` & `subarulink-0.7.6.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 
 This package supports Subaru STARLINK equipped vehicles with active service plans. A [MySubaru](https://www.mysubaru.com) account must be setup prior to using this package. The features available will depend on the model year and type of service plan (Safety Plus or Safety/Security Plus).
 
 
 | Model Year   | Safety Plus | Security Plus |
 |--------------|-------------|---------------|
 | 2016-2018    |  No Support | Remote Lock/Unlock <br> Remote Horn and/or Lights <br> Remote Vehicle Locator <br> Odometer (updated every 500 miles) 
-| 2019+        |  Tire Pressure# <br> Fuel Economy# <br> Fuel Range# <br> Odometer#     |Remote Lock/Unlock <br> Remote Horn and/or Lights <br> Remote Vehicle Locator <br> Remote Engine Start w/ Climate Control <br> PHEV Start Charge* <br> Door/Window Status** <br> Tire Pressure <br> Fuel Economy <br> Fuel Range <br> Odometer
+| 2019+        |  Tire Pressure# <br> Fuel Economy# <br> Fuel Range# <br> Odometer#     |Remote Lock/Unlock <br> Remote Horn and/or Lights <br> Remote Vehicle Locator <br> Remote Engine Start w/ Climate Control <br> EV Start Charge* <br> Door/Window/Sunroof Status** <br> Tire Pressure <br> Fuel Economy <br> Fuel Range <br> Odometer
 
 \# Unclear how often this is updated <br>
-\* Plug-In hybrid only <br>
-\*\* Support varies by model
+\* EV/PHEV only <br>
+\*\* Support varies by model/year
 
-**NOTE:**  This project was developed based upon analysis of the official MySubaru Android app. Subaru has no official public API; therefore, this library may stop working at any time without warning.  Use at your own risk.
+> **NOTE:**
+> This project was developed based upon analysis of the official MySubaru Android app. Subaru has no official public API; therefore, this library may stop working at any time without warning.  Use at your own risk.
 
 
 ## Home Assistant Integration
 
 There is a Home Assistant [custom component](https://github.com/G-Two/homeassistant-subaru) that uses this package and allows users to add Subaru STARLINK integration to their Home Assistant instance.
 
 In addition, as of 2021.3, Home Assistant Core includes the [Subaru integration](https://www.home-assistant.io/integrations/subaru/) that uses this package. Due to the required incremental additions required by Home Assistant Core, only the sensor and lock platforms are supported at this time. Additional PRs are pending to add full functionality. Users that desire the most recent features should continue using the custom component.
@@ -67,15 +68,15 @@
 Accounts with only one vehicle do not need to specify a VIN
 
 ## Configuration
 A JSON file is used for configuration. A user provided file can be passed to the CLI via the `--config`. If no config file is provided, two default locations are searched for. First is `~/.subarulink.cfg` and if that is not found, `$XDG_CONFIG_HOME/subarulink/subarulink.cfg` will be used.
 
 ## Known Issues
 ### Battery Discharge
-Aggressively polling the vehicle location with subarulink.Controller.update(vin) may discharge the auxiliary battery (in a PHEV).  Intermittent (every 2 hours) use isn't a problem, but polling at 5 minute intervals will drain the auxiliary battery fully after a few consecutive non-driving days.  The vehicle does report the auxiliary battery voltage with every update, so this can be avoided.  
+Aggressively polling the vehicle location with subarulink.Controller.update(vin) may discharge the auxiliary 12V battery (in a PHEV).  Intermittent (every 2 hours) use isn't a problem, but polling at 5 minute intervals will drain the auxiliary battery fully after a few consecutive non-driving days.
 
 Effects of aggressive polling on the battery of a gasoline-only vehicle are unknown.
 
 ### Stale Data
 Sensor data is only sent by the vehicle during certain events (e.g. engine shutdown or a user requested location update) and should not be relied on to indicate a vehicle's real time status. If more recent data is desired, then the user must initiate a location update which will update the data for all sensors (exception: tire pressures will only be updated if the vehicle is in motion).
 
 ### Remote climate control preset options vary by model
```

### Comparing `subarulink-0.7.6/pyproject.toml` & `subarulink-0.7.6.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/setup.py` & `subarulink-0.7.6.post1/setup.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/subarulink/__init__.py` & `subarulink-0.7.6.post1/subarulink/__init__.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/subarulink/_subaru_api/const.py` & `subarulink-0.7.6.post1/subarulink/_subaru_api/const.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/subarulink/app/cli.py` & `subarulink-0.7.6.post1/subarulink/app/cli.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/subarulink/connection.py` & `subarulink-0.7.6.post1/subarulink/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from __future__ import annotations
 
 import asyncio
 import logging
 import pprint
 import time
-from typing import Any, Dict, List, Optional
+from typing import Any
 
 import aiohttp
 from yarl import URL
 
 from subarulink.exceptions import (
     IncompleteCredentials,
     InvalidCredentials,
@@ -68,32 +68,32 @@
         """
         self._username = username
         self._password = password
         self._device_id = device_id
         self._country = country
         self._lock = asyncio.Lock()
         self._device_name = device_name
-        self._vehicles: List[Dict] = []
+        self._vehicles: list[dict] = []
         self._head = {
             "User-Agent": "Mozilla/5.0 (Linux; Android 10; Android SDK built for x86 Build/QSR1.191030.002; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/74.0.3729.185 Mobile Safari/537.36",
             "Origin": "file://",
             "X-Requested-With": API_MOBILE_APP[self._country],
             "Accept-Language": "en-US,en;q=0.9",
             "Accept-Encoding": "gzip, deflate",
             "Accept": "*/*",
         }
         self._websession = websession
         self._authenticated = False
         self._registered = False
         self._current_vin = ""
-        self._list_of_vins: List[str] = []
+        self._list_of_vins: list[str] = []
         self._session_login_time = 0.0
-        self._auth_contact_options: Dict[str, str] | Any = {}
+        self._auth_contact_options: dict[str, str] | Any = {}
 
-    async def connect(self) -> List[Dict[str, Any]]:
+    async def connect(self) -> list[dict[str, Any]]:
         """
         Connect to and establish session with Subaru Starlink mobile app API.
 
         Returns:
             List: A list of dicts containing information about each vehicle registered in the Subaru account.
 
         Raises:
@@ -110,15 +110,15 @@
 
     @property
     def device_registered(self) -> bool:
         """Device is registered."""
         return self._registered
 
     @property
-    def auth_contact_methods(self) -> Dict[str, str]:
+    def auth_contact_methods(self) -> dict[str, str]:
         """Contact methods for 2FA."""
         return self._auth_contact_options
 
     async def request_auth_code(self, contact_method: str) -> bool:
         """Request 2FA code be sent via specified contact method."""
         if contact_method not in self.auth_contact_methods:
             _LOGGER.error("Invalid 2FA contact method requested")
@@ -206,15 +206,15 @@
         """Return number of minutes since last authentication."""
         return (time.time() - self._session_login_time) // 60
 
     def reset_session(self):
         """Clear session cookies."""
         self._websession.cookie_jar.clear()
 
-    async def get(self, url: str, params: Optional[Dict] = None) -> Dict[str, Any]:
+    async def get(self, url: str, params: dict | None = None) -> dict[str, Any]:
         """
         Send HTTPS GET request to Subaru Remote Services API.
 
         Args:
             url (str): URL path that will be concatenated after `subarulink.const.MOBILE_API_BASE_URL`
             params (Dict, optional): HTTP GET request parameters
 
@@ -225,15 +225,15 @@
             SubaruException: If request fails.
         """
         js_resp = {}
         if self._authenticated:
             js_resp = await self.__open(url, method=GET, headers=self._head, params=params)
         return js_resp
 
-    async def post(self, url: str, params: Optional[Dict] = None, json_data: Optional[Dict] = None) -> Dict[str, Any]:
+    async def post(self, url: str, params: dict | None = None, json_data: dict | None = None) -> dict[str, Any]:
         """
         Send HTTPS POST request to Subaru Remote Services API.
 
         Args:
             url (str): URL path that will be concatenated after `subarulink.const.MOBILE_API_BASE_URL`
             params (Dict, optional): HTTP POST request parameters
             json_data (Dict, optional): HTTP POST request JSON data as a Dict
@@ -245,15 +245,15 @@
             SubaruException: If request fails.
         """
         js_resp = {}
         if self._authenticated:
             js_resp = await self.__open(url, method=POST, headers=self._head, params=params, json_data=json_data)
         return js_resp
 
-    async def _authenticate(self, vin: Optional[str] = None) -> bool:
+    async def _authenticate(self, vin: str | None = None) -> bool:
         """Authenticate to Subaru Remote Services API."""
         if self._username and self._password and self._device_id:
             post_data = {
                 "env": "cloudprod",
                 "loginUsername": self._username,
                 "password": self._password,
                 "deviceId": self._device_id,
@@ -283,15 +283,15 @@
                     raise InvalidCredentials(error)
                 if error == API_ERROR_PASSWORD_WARNING:
                     _LOGGER.error("Multiple Password Failures.")
                     raise InvalidCredentials(error)
                 raise SubaruException(error)
         raise IncompleteCredentials("Connection requires email and password and device id.")
 
-    async def _select_vehicle(self, vin: str) -> Dict[str, Any] | None:
+    async def _select_vehicle(self, vin: str) -> dict[str, Any] | None:
         """Select active vehicle for accounts with multiple VINs."""
         params = {"vin": vin, "_": int(time.time())}
         js_resp = await self.get(API_SELECT_VEHICLE, params=params)
         _LOGGER.debug(pprint.pformat(js_resp))
         if js_resp.get("success"):
             self._current_vin = vin
             _LOGGER.debug("Current vehicle: vin=%s", js_resp["data"]["vin"])
@@ -325,15 +325,15 @@
         url,
         method=GET,
         headers=None,
         data=None,
         json_data=None,
         params=None,
         baseurl="",
-    ) -> Dict:
+    ) -> dict:
         """Open url."""
         if not baseurl:
             baseurl = f"https://{API_SERVER[self._country]}{API_VERSION}"
         endpoint: URL = URL(baseurl + url)
 
         _LOGGER.debug("%s: %s, params=%s, json_data=%s", method.upper(), endpoint, params, json_data)
         async with self._lock:
```

### Comparing `subarulink-0.7.6/subarulink/const.py` & `subarulink-0.7.6.post1/subarulink/const.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/subarulink/controller.py` & `subarulink-0.7.6.post1/subarulink/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import asyncio
 from datetime import datetime, timedelta
 import json
 import logging
 import pprint
 import time
-from typing import Any, Dict, List, Optional, Tuple, TypedDict, Union
+from typing import Any, TypedDict
 
 from aiohttp.client import ClientSession
 
 import subarulink
 from subarulink.connection import Connection
 import subarulink.const as sc
 from subarulink.exceptions import (
@@ -34,20 +34,20 @@
 
 class VehicleInfo(TypedDict):
     """TypedDict to store information for each vehicle."""
 
     model_year: str
     model_name: str
     vehicle_name: str
-    vehicle_features: List[str]
-    subscription_features: List[str]
+    vehicle_features: list[str]
+    subscription_features: list[str]
     subscription_status: str
-    vehicle_status: Dict[str, Any]
-    vehicle_health: Dict[str, Any]
-    climate: List[Dict]
+    vehicle_status: dict[str, Any]
+    vehicle_health: dict[str, Any]
+    climate: list[dict]
     last_fetch: datetime
     last_update: datetime
 
 
 class Controller:
     """Controller to interact with Subaru Starlink mobile app API."""
 
@@ -77,20 +77,20 @@
             fetch_interval (int, optional): Seconds between fetches of Subaru's cached vehicle information
 
         """
         self._connection = Connection(websession, username, password, device_id, device_name, country)
         self._country = country
         self._update_interval = update_interval
         self._fetch_interval = fetch_interval
-        self._vehicles: Dict[str, VehicleInfo] = {}
-        self._vehicle_asyncio_lock: Dict[str, asyncio.Lock] = {}
+        self._vehicles: dict[str, VehicleInfo] = {}
+        self._vehicle_asyncio_lock: dict[str, asyncio.Lock] = {}
         self._pin = pin
         self._controller_lock = asyncio.Lock()
         self._pin_lockout = False
-        self._raw_api_data: Dict[str, Dict] = {}
+        self._raw_api_data: dict[str, dict] = {}
         self.version = subarulink.__version__
 
     async def connect(self) -> bool:
         """
         Connect to Subaru Remote Services API.
 
         Returns:
@@ -116,15 +116,15 @@
 
     @property
     def device_registered(self) -> bool:
         """Device is registered."""
         return self._connection.device_registered
 
     @property
-    def contact_methods(self) -> Dict[str, str]:
+    def contact_methods(self) -> dict[str, str]:
         """Email address for 2FA."""
         return self._connection.auth_contact_methods
 
     async def request_auth_code(self, contact_method: str) -> bool:
         """Request 2FA code be sent via email."""
         return await self._connection.request_auth_code(contact_method)
 
@@ -169,15 +169,15 @@
                     _LOGGER.debug(pprint.pformat(js_resp))
                     if js_resp["success"]:
                         _LOGGER.info("PIN is valid for Subaru remote services")
                         return True
         _LOGGER.info("No active vehicles with remote services subscription - PIN not required")
         return False
 
-    def get_vehicles(self) -> List[str]:
+    def get_vehicles(self) -> list[str]:
         """
         Return list of VINs available to user on Subaru Remote Services API.
 
         Returns:
             List: A list containing the VINs of all vehicles registered to the Subaru account.
         """
         return list(self._vehicles.keys())
@@ -395,15 +395,15 @@
         vehicle = self._vehicles.get(vin.upper())
         if vehicle:
             if len(vehicle[sc.VEHICLE_STATUS]) == 0:
                 await self.fetch(vin)
             return self._vehicles[vin.upper()]
         raise SubaruException("Invalid VIN")
 
-    def get_raw_data(self, vin: str) -> Dict[str, Dict[str, Any]]:
+    def get_raw_data(self, vin: str) -> dict[str, dict[str, Any]]:
         """
         Get locally cached vehicle data as received by the Subaru API without processing.  Fetch from Subaru API if not present.
 
         Args:
             vin (str): The VIN to get.
 
         Returns:
@@ -414,15 +414,15 @@
         """
         vehicle = self._vehicles.get(vin.upper())
         if vehicle:
             result = self._raw_api_data[vin.upper()]
             return result
         raise SubaruException("Invalid VIN")
 
-    async def list_climate_preset_names(self, vin: str) -> List[str]:
+    async def list_climate_preset_names(self, vin: str) -> list[str]:
         """
         Get list of climate control presets.
 
         Args:
             vin (str): The VIN of the vehicle.
 
         Returns:
@@ -433,15 +433,15 @@
             VehicleNotSupported: if vehicle/subscription not supported
         """
         self._validate_remote_capability(vin)
         if len(self._vehicles[vin][sc.VEHICLE_CLIMATE]) == 0:
             await self._fetch_climate_presets(vin)
         return [i[sc.PRESET_NAME] for i in self._vehicles[vin][sc.VEHICLE_CLIMATE]]
 
-    async def get_climate_preset_by_name(self, vin: str, preset_name: str) -> Dict[str, Union[int, str]] | None:
+    async def get_climate_preset_by_name(self, vin: str, preset_name: str) -> dict[str, int | str] | None:
         """
         Get climate control preset by name.
 
         Args:
             vin (str): The VIN of the vehicle.
             preset_name (str): Name of climate settings preset.
 
@@ -456,15 +456,15 @@
         if len(self._vehicles[vin][sc.VEHICLE_CLIMATE]) == 0:
             await self._fetch_climate_presets(vin)
         for preset in self._vehicles[vin][sc.VEHICLE_CLIMATE]:
             if preset["name"] == preset_name:
                 return preset
         return None
 
-    async def get_user_climate_preset_data(self, vin: str) -> List[Dict[str, Union[int, str]]]:
+    async def get_user_climate_preset_data(self, vin: str) -> list[dict[str, int | str]]:
         """
         Get user climate control preset data.
 
         Args:
             vin (str): The VIN of the vehicle.
 
         Returns:
@@ -498,15 +498,15 @@
         preset = await self.get_climate_preset_by_name(vin, preset_name)
         if preset and preset["presetType"] == "userPreset":
             user_presets = [i for i in self._vehicles[vin][sc.VEHICLE_CLIMATE] if i["presetType"] == "userPreset"]
             user_presets.remove(preset)
             return await self.update_user_climate_presets(vin, user_presets)
         raise SubaruException(f"User preset name '{preset_name}' not found")
 
-    async def update_user_climate_presets(self, vin: str, preset_data: List[Dict[str, Union[int, str]]]) -> bool:
+    async def update_user_climate_presets(self, vin: str, preset_data: list[dict[str, int | str]]) -> bool:
         """
         Save user defined climate control settings to Subaru.
 
         Args:
             vin (str): The VIN to save climate settings to.
             preset_data (list): List of Climate settings dicts to save.
 
@@ -890,25 +890,25 @@
         """
         if new_pin != self._pin:
             self._pin = new_pin
             self._pin_lockout = False
             return True
         return False
 
-    async def _get(self, url: str, params: Optional[Dict[str, str]] = None) -> Dict[str, Any]:
+    async def _get(self, url: str, params: dict[str, str] | None = None) -> dict[str, Any]:
         js_resp = await self._connection.get(url, params)
         self._check_error_code(js_resp)
         return js_resp
 
-    async def _post(self, url: str, params: None = None, json_data: Optional[Any] = None) -> Dict[str, Any]:
+    async def _post(self, url: str, params: None = None, json_data: Any | None = None) -> dict[str, Any]:
         js_resp = await self._connection.post(url, params, json_data)
         self._check_error_code(js_resp)
         return js_resp
 
-    def _check_error_code(self, js_resp: Dict[str, Any]) -> None:
+    def _check_error_code(self, js_resp: dict[str, Any]) -> None:
         error = js_resp.get("errorCode")
         if error in [api.API_ERROR_SOA_403, api.API_ERROR_INVALID_TOKEN]:
             _LOGGER.debug("SOA 403 error - clearing session cookie")
             self._connection.reset_session()
         elif error in [api.API_ERROR_INVALID_CREDENTIALS, "SXM40006"]:
             _LOGGER.error("PIN is not valid for Subaru remote services")
             self._pin_lockout = True
@@ -918,15 +918,15 @@
             api.API_ERROR_G1_SERVICE_ALREADY_STARTED,
         ]:
             pass
         elif error:
             _LOGGER.error("Unhandled API error code %s", error)
             raise SubaruException(f"Unhandled API error: {error} - {js_resp}")
 
-    def _parse_vehicle(self, vehicle: Dict[str, Any]) -> None:
+    def _parse_vehicle(self, vehicle: dict[str, Any]) -> None:
         vin = vehicle["vin"].upper()
         _LOGGER.debug("Parsing vehicle: %s", vin)
         self._vehicle_asyncio_lock[vin] = asyncio.Lock()
         self._raw_api_data[vin] = {}
         self._raw_api_data[vin]["switchVehicle"] = vehicle
         self._vehicles[vin] = VehicleInfo(
             {
@@ -943,15 +943,15 @@
                 sc.VEHICLE_LAST_UPDATE: datetime(1980, 1, 2, 1, 0, 0),
             }
         )
         self._vehicles[vin][sc.VEHICLE_HEALTH][
             sc.HEALTH_RECOMMENDED_TIRE_PRESSURE
         ] = self._parse_recommended_tire_pressure(vin)
 
-    async def _remote_query(self, vin: str, cmd: str) -> Dict[str, Any]:
+    async def _remote_query(self, vin: str, cmd: str) -> dict[str, Any]:
         tries_left = 2
         js_resp = None
         while tries_left > 0:
             await self._connection.validate_session(vin)
 
             # G3 uses G2 API for now
             api_gen = (
@@ -968,16 +968,16 @@
                 if js_resp["errorCode"] == api.API_ERROR_SOA_403:
                     tries_left -= 1
                 else:
                     tries_left = 0
         raise SubaruException("Remote query failed. Response: %s " % js_resp)
 
     async def _remote_command(
-        self, vin: str, cmd: str, poll_url: str, data: Optional[Dict[str, Any]] = None
-    ) -> Tuple[bool, Dict[str, Any]]:
+        self, vin: str, cmd: str, poll_url: str, data: dict[str, Any] | None = None
+    ) -> tuple[bool, dict[str, Any]]:
         try_again = True
         vin = vin.upper()
         while try_again:
             if not self._pin_lockout:
                 # There is some sort of token expiration with the telematics provider that is checked after
                 # a successful remote command is sent causing the status polling to fail and making it seem the
                 # command failed. Workaround is to force a reauth before the command is issued.
@@ -989,16 +989,16 @@
                     if success:
                         return success, js_resp
             else:
                 raise PINLockoutProtect("Remote command with invalid PIN cancelled to prevent account lockout")
         raise SubaruException("Unexpected error received from Subaru API during remote command")
 
     async def _execute_remote_command(
-        self, vin: str, cmd: str, data: Optional[Dict[str, Union[int, str, bool]]], poll_url: str
-    ) -> Tuple[bool, bool, Dict[str, Any]]:
+        self, vin: str, cmd: str, data: dict[str, int | str | bool] | None, poll_url: str
+    ) -> tuple[bool, bool, dict[str, Any]]:
         try_again = False
         success = False
 
         # G3 uses G2 API for now
         api_gen = (
             api.API_FEATURE_G1_TELEMATICS
             if self.get_api_gen(vin) == api.API_FEATURE_G1_TELEMATICS
@@ -1020,26 +1020,24 @@
             try_again = True
         if js_resp["success"]:
             req_id = js_resp["data"][api.API_SERVICE_REQ_ID]
             success, js_resp = await self._wait_request_status(vin, req_id, poll_url)
         return try_again, success, js_resp
 
     async def _actuate(
-        self, vin: str, cmd: str, data: Optional[Dict[str, Any]] = None, poll_url: str = api.API_REMOTE_SVC_STATUS
-    ) -> Tuple[bool, Dict[str, Any]]:
+        self, vin: str, cmd: str, data: dict[str, Any] | None = None, poll_url: str = api.API_REMOTE_SVC_STATUS
+    ) -> tuple[bool, dict[str, Any]]:
         form_data = {"delay": 0, "vin": vin}
         if data:
             form_data.update(data)
         if self.get_remote_status(vin):
             return await self._remote_command(vin, cmd, poll_url, data=form_data)
         raise VehicleNotSupported("Active STARLINK Security Plus subscription required.")
 
-    async def _get_vehicle_status(
-        self, vin: str
-    ) -> Dict[str, Optional[Union[bool, Dict[str, Optional[Union[int, str, float]]]]]]:
+    async def _get_vehicle_status(self, vin: str) -> dict[str, bool | dict[str, int | str | float | None] | None]:
         await self._connection.validate_session(vin)
         js_resp = await self._get(api.API_VEHICLE_STATUS)
         _LOGGER.debug(pprint.pformat(js_resp))
         return js_resp
 
     async def _fetch_status(self, vin: str) -> bool:
         _LOGGER.debug("Fetching vehicle status from Subaru")
@@ -1109,15 +1107,15 @@
             success = js_resp.get("success", False)
 
         if success and js_resp.get("success"):
             self._parse_location(vin, js_resp["data"]["result"])
             return True
         return False
 
-    def _parse_location(self, vin: str, result: Dict[str, Optional[Union[float, int]]]) -> None:
+    def _parse_location(self, vin: str, result: dict[str, float | int | None]) -> None:
         if result[api.API_LONGITUDE] == sc.BAD_LONGITUDE and result[api.API_LATITUDE] == sc.BAD_LATITUDE:
             # After car shutdown, some vehicles will push an update to Subaru with an invalid location. In this case keep previous and set flag so app knows to request update.
             self._vehicles[vin][sc.VEHICLE_STATUS][api.API_LONGITUDE] = self._vehicles[vin][sc.VEHICLE_STATUS].get(
                 api.API_LONGITUDE
             )
             self._vehicles[vin][sc.VEHICLE_STATUS][api.API_LATITUDE] = self._vehicles[vin][sc.VEHICLE_STATUS].get(
                 api.API_LATITUDE
@@ -1130,15 +1128,15 @@
             self._vehicles[vin][sc.VEHICLE_STATUS][sc.LONGITUDE] = result.get(api.API_LONGITUDE)
             self._vehicles[vin][sc.VEHICLE_STATUS][sc.LATITUDE] = result.get(api.API_LATITUDE)
             self._vehicles[vin][sc.VEHICLE_STATUS][sc.HEADING] = result.get(api.API_HEADING)
             self._vehicles[vin][sc.VEHICLE_STATUS][sc.LOCATION_VALID] = True
 
     async def _wait_request_status(
         self, vin: str, req_id: str, poll_url: str, attempts: int = 20
-    ) -> Tuple[bool, Dict[str, Any]]:
+    ) -> tuple[bool, dict[str, Any]]:
         params = {api.API_SERVICE_REQ_ID: req_id}
         attempts_left = attempts
         _LOGGER.debug("Polling for remote service request completion: serviceRequestId=%s", req_id)
 
         # G3 uses G2 API for now
         api_gen = (
             api.API_FEATURE_G1_TELEMATICS
@@ -1200,15 +1198,15 @@
                 for i in json.loads(data):
                     presets.append(i)
 
             self._vehicles[vin][sc.VEHICLE_CLIMATE] = presets
             return True
         raise VehicleNotSupported("Active STARLINK Security Plus subscription required.")
 
-    def _validate_remote_start_params(self, vin: str, preset_data: Dict[str, Union[int, str]]) -> bool:
+    def _validate_remote_start_params(self, vin: str, preset_data: dict[str, int | str]) -> bool:
         is_valid = True
         err_msg = None
         try:
             for item in preset_data:
                 if preset_data[item] not in sc.VALID_CLIMATE_OPTIONS[item]:
                     if item == "name" and isinstance(preset_data[item], str):
                         continue
@@ -1230,19 +1228,19 @@
     def _validate_remote_capability(self, vin: str) -> bool:
         if not self.get_res_status(vin) and not self.get_ev_status(vin):
             raise VehicleNotSupported(
                 "Active STARLINK Security Plus subscription and remote start capable vehicle required."
             )
         return True
 
-    def _parse_vehicle_status(self, js_resp: Dict, vin: str) -> Dict[str, Union[int, float, datetime, str, bool, None]]:
+    def _parse_vehicle_status(self, js_resp: dict, vin: str) -> dict[str, int | float | datetime | str | bool | None]:
         """Parse fields from vehicleStatus.json."""
         data = js_resp["data"]
         old_status = self._vehicles[vin][sc.VEHICLE_STATUS]
-        status: Dict[str, Union[int, float, datetime, str, bool, None]] = {}
+        status: dict[str, int | float | datetime | str | bool | None] = {}
 
         # These values seem to always be valid
         status[sc.ODOMETER] = int(data.get(api.API_ODOMETER))
         status[sc.TIMESTAMP] = datetime.strptime(data.get(api.API_TIMESTAMP), api.API_VS_TIMESTAMP_FMT)
 
         # These values are either valid or None. If None and we have a previous value, keep previous, otherwise None.
         status[sc.AVG_FUEL_CONSUMPTION] = data.get(api.API_AVG_FUEL_CONSUMPTION) or (
@@ -1274,17 +1272,15 @@
             status[sc.LONGITUDE] = data.get(api.API_LONGITUDE)
             status[sc.LATITUDE] = data.get(api.API_LATITUDE)
             status[sc.HEADING] = int(data.get(api.API_HEADING))
             status[sc.LOCATION_VALID] = True
 
         return status
 
-    def _parse_condition(
-        self, js_resp: Dict[str, Any], vin: str
-    ) -> Dict[str, Optional[Union[str, datetime, int, float]]]:
+    def _parse_condition(self, js_resp: dict[str, Any], vin: str) -> dict[str, str | datetime | int | float | None]:
         """Parse fields from condition/execute.json."""
         data = js_resp["data"]["result"]
         keep_data = {
             sc.DOOR_BOOT_POSITION: data[api.API_DOOR_BOOT_POSITION],
             sc.DOOR_ENGINE_HOOD_POSITION: data[api.API_DOOR_ENGINE_HOOD_POSITION],
             sc.DOOR_FRONT_LEFT_POSITION: data[api.API_DOOR_FRONT_LEFT_POSITION],
             sc.DOOR_FRONT_RIGHT_POSITION: data[api.API_DOOR_FRONT_RIGHT_POSITION],
```

### Comparing `subarulink-0.7.6/subarulink/exceptions.py` & `subarulink-0.7.6.post1/subarulink/exceptions.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/subarulink.egg-info/PKG-INFO` & `subarulink-0.7.6.post1/subarulink.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subarulink
-Version: 0.7.6
+Version: 0.7.6.post1
 Summary: A package for interacting with Subaru Starlink Remote Services API.
 Home-page: https://github.com/G-Two/subarulink
 Author: G-Two
 Author-email: 
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -25,21 +25,22 @@
 
 This package supports Subaru STARLINK equipped vehicles with active service plans. A [MySubaru](https://www.mysubaru.com) account must be setup prior to using this package. The features available will depend on the model year and type of service plan (Safety Plus or Safety/Security Plus).
 
 
 | Model Year   | Safety Plus | Security Plus |
 |--------------|-------------|---------------|
 | 2016-2018    |  No Support | Remote Lock/Unlock <br> Remote Horn and/or Lights <br> Remote Vehicle Locator <br> Odometer (updated every 500 miles) 
-| 2019+        |  Tire Pressure# <br> Fuel Economy# <br> Fuel Range# <br> Odometer#     |Remote Lock/Unlock <br> Remote Horn and/or Lights <br> Remote Vehicle Locator <br> Remote Engine Start w/ Climate Control <br> PHEV Start Charge* <br> Door/Window Status** <br> Tire Pressure <br> Fuel Economy <br> Fuel Range <br> Odometer
+| 2019+        |  Tire Pressure# <br> Fuel Economy# <br> Fuel Range# <br> Odometer#     |Remote Lock/Unlock <br> Remote Horn and/or Lights <br> Remote Vehicle Locator <br> Remote Engine Start w/ Climate Control <br> EV Start Charge* <br> Door/Window/Sunroof Status** <br> Tire Pressure <br> Fuel Economy <br> Fuel Range <br> Odometer
 
 \# Unclear how often this is updated <br>
-\* Plug-In hybrid only <br>
-\*\* Support varies by model
+\* EV/PHEV only <br>
+\*\* Support varies by model/year
 
-**NOTE:**  This project was developed based upon analysis of the official MySubaru Android app. Subaru has no official public API; therefore, this library may stop working at any time without warning.  Use at your own risk.
+> **NOTE:**
+> This project was developed based upon analysis of the official MySubaru Android app. Subaru has no official public API; therefore, this library may stop working at any time without warning.  Use at your own risk.
 
 
 ## Home Assistant Integration
 
 There is a Home Assistant [custom component](https://github.com/G-Two/homeassistant-subaru) that uses this package and allows users to add Subaru STARLINK integration to their Home Assistant instance.
 
 In addition, as of 2021.3, Home Assistant Core includes the [Subaru integration](https://www.home-assistant.io/integrations/subaru/) that uses this package. Due to the required incremental additions required by Home Assistant Core, only the sensor and lock platforms are supported at this time. Additional PRs are pending to add full functionality. Users that desire the most recent features should continue using the custom component.
@@ -87,15 +88,15 @@
 Accounts with only one vehicle do not need to specify a VIN
 
 ## Configuration
 A JSON file is used for configuration. A user provided file can be passed to the CLI via the `--config`. If no config file is provided, two default locations are searched for. First is `~/.subarulink.cfg` and if that is not found, `$XDG_CONFIG_HOME/subarulink/subarulink.cfg` will be used.
 
 ## Known Issues
 ### Battery Discharge
-Aggressively polling the vehicle location with subarulink.Controller.update(vin) may discharge the auxiliary battery (in a PHEV).  Intermittent (every 2 hours) use isn't a problem, but polling at 5 minute intervals will drain the auxiliary battery fully after a few consecutive non-driving days.  The vehicle does report the auxiliary battery voltage with every update, so this can be avoided.  
+Aggressively polling the vehicle location with subarulink.Controller.update(vin) may discharge the auxiliary 12V battery (in a PHEV).  Intermittent (every 2 hours) use isn't a problem, but polling at 5 minute intervals will drain the auxiliary battery fully after a few consecutive non-driving days.
 
 Effects of aggressive polling on the battery of a gasoline-only vehicle are unknown.
 
 ### Stale Data
 Sensor data is only sent by the vehicle during certain events (e.g. engine shutdown or a user requested location update) and should not be relied on to indicate a vehicle's real time status. If more recent data is desired, then the user must initiate a location update which will update the data for all sensors (exception: tire pressures will only be updated if the vehicle is in motion).
 
 ### Remote climate control preset options vary by model
```

### Comparing `subarulink-0.7.6/subarulink.egg-info/SOURCES.txt` & `subarulink-0.7.6.post1/subarulink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/tests/test_cli.py` & `subarulink-0.7.6.post1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/tests/test_connection.py` & `subarulink-0.7.6.post1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/tests/test_remote_commands.py` & `subarulink-0.7.6.post1/tests/test_remote_commands.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.6/tests/test_vehicle_status.py` & `subarulink-0.7.6.post1/tests/test_vehicle_status.py`

 * *Files identical despite different names*

