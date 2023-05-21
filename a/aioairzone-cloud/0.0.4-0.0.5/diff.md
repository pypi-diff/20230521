# Comparing `tmp/aioairzone-cloud-0.0.4.tar.gz` & `tmp/aioairzone-cloud-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.0.4.tar", last modified: Thu May 18 16:30:20 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.0.5.tar", last modified: Sun May 21 08:37:26 2023, max compression
```

## Comparing `aioairzone-cloud-0.0.4.tar` & `aioairzone-cloud-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 16:30:20.793392 aioairzone-cloud-0.0.4/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.4/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.4/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-18 16:30:20.793392 aioairzone-cloud-0.0.4/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      320 2023-05-18 08:06:51.000000 aioairzone-cloud-0.0.4/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 16:30:20.793392 aioairzone-cloud-0.0.4/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    13337 2023-05-18 16:26:53.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4225 2022-04-06 19:26:33.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2890 2022-04-06 19:36:15.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      731 2023-05-18 16:12:10.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1168 2022-04-06 10:44:53.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3775 2022-04-06 08:42:41.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    17976 2022-04-06 19:27:54.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 16:30:20.793392 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      593 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      963 2023-05-18 16:27:43.000000 aioairzone-cloud-0.0.4/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.4/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-18 16:30:20.793392 aioairzone-cloud-0.0.4/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-21 08:37:26.532835 aioairzone-cloud-0.0.5/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.5/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.5/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-21 08:37:26.532835 aioairzone-cloud-0.0.5/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      320 2023-05-18 08:06:51.000000 aioairzone-cloud-0.0.5/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-21 08:37:26.532835 aioairzone-cloud-0.0.5/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    15463 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     5888 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-21 08:37:26.532835 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      593 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      963 2023-05-21 08:35:30.000000 aioairzone-cloud-0.0.5/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.5/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-21 08:37:26.532835 aioairzone-cloud-0.0.5/setup.cfg
```

### Comparing `aioairzone-cloud-0.0.4/LICENSE` & `aioairzone-cloud-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.4/PKG-INFO` & `aioairzone-cloud-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.0.4/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.0.5/aioairzone_cloud/cloudapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Airzone Cloud API."""
 from __future__ import annotations
 
 import logging
 import urllib.parse
+from datetime import datetime
 from typing import Any, cast
 
 from aiohttp import ClientConnectorError, ClientResponseError, ClientSession
 from aiohttp.client_reqrep import ClientResponse
 
 from .common import ConnectionOptions
 from .const import (
@@ -15,37 +16,42 @@
     API_AZ_SYSTEM,
     API_AZ_ZONE,
     API_CONFIG,
     API_DEVICE_ID,
     API_DEVICE_TYPE,
     API_DEVICES,
     API_EMAIL,
+    API_GROUPS,
     API_INSTALLATION_ID,
     API_INSTALLATIONS,
     API_PASSWORD,
     API_REFRESH_TOKEN,
     API_STATUS,
     API_TOKEN,
+    API_TYPE,
     API_URL,
     API_USER,
     API_USER_LOGOUT,
     API_V1,
     API_WS,
+    API_WS_ID,
     AZD_INSTALLATIONS,
     AZD_SYSTEMS,
     AZD_WEBSERVERS,
     AZD_ZONES,
     HEADER_AUTHORIZATION,
     HEADER_BEARER,
     HTTP_CALL_TIMEOUT,
+    TOKEN_REFRESH_PERIOD,
 )
 from .device import Device
 from .exceptions import (
     AirzoneCloudError,
     APIError,
+    AuthError,
     LoginError,
     TokenRefreshError,
     TooManyRequests,
 )
 from .installation import Installation
 from .system import System
 from .webserver import WebServer
@@ -62,14 +68,15 @@
         aiohttp_session: ClientSession,
         options: ConnectionOptions,
     ):
         """Airzone Cloud API init."""
         self.aiohttp_session = aiohttp_session
         self.installations: list[Installation] = []
         self.options = options
+        self.refresh_time: datetime
         self.refresh_token: str | None = None
         self.systems: list[System] = []
         self.token: str | None = None
         self.webservers: list[WebServer] = []
         self.zones: list[Zone] = []
 
     async def api_request(
@@ -87,28 +94,35 @@
                 method,
                 f"{API_URL}/{path}",
                 headers=headers,
                 json=json,
                 raise_for_status=True,
                 timeout=HTTP_CALL_TIMEOUT,
             )
+        except ClientConnectorError as err:
+            raise AirzoneCloudError from err
         except ClientResponseError as err:
             if path.endswith(API_AUTH_LOGIN):
                 raise LoginError from err
+            if path.endswith(API_AUTH_REFRESH_TOKEN):
+                raise TokenRefreshError from err
 
             if err.status == 400:
                 raise APIError from err
+            if err.status == 401:
+                raise AuthError from err
             if err.status == 429:
                 raise TooManyRequests from err
+
             raise AirzoneCloudError from err
 
         resp_json = await resp.json(content_type=None)
         _LOGGER.debug("aiohttp response: %s", resp_json)
 
-        return cast(dict, resp_json)
+        return cast(dict[str, Any], resp_json)
 
     async def api_get_device_config(self, device: Device) -> dict[str, Any]:
         """Request API device config data."""
         dev_id = urllib.parse.quote(device.get_id())
 
         params = {
             API_INSTALLATION_ID: device.get_installation(),
@@ -184,45 +198,44 @@
             {
                 API_EMAIL: self.options.username,
                 API_PASSWORD: self.options.password,
             },
         )
         _LOGGER.debug("login resp: %s", resp)
         if resp.keys() < {API_TOKEN, API_REFRESH_TOKEN}:
-            raise LoginError
+            raise LoginError("Invalid API response")
         self.token = resp[API_TOKEN]
+        self.refresh_time = datetime.now()
         self.refresh_token = resp[API_REFRESH_TOKEN]
 
     async def logout(self) -> None:
         """Perform Airzone Cloud API logout."""
         try:
             if self.token:
                 await self.api_request(
                     "GET",
                     f"{API_V1}/{API_USER_LOGOUT}",
                 )
-        except ClientConnectorError:
+        except AirzoneCloudError:
             pass
         finally:
             self.refresh_token = None
             self.token = None
 
     async def token_refresh(self) -> None:
         """Perform Airzone Cloud API token refresh."""
         if self.token and self.refresh_token:
+            refresh_token = urllib.parse.quote(self.refresh_token)
             resp = await self.api_request(
-                "POST",
-                f"{API_V1}/{API_AUTH_REFRESH_TOKEN}",
-                {
-                    API_REFRESH_TOKEN: self.refresh_token,
-                },
+                "GET",
+                f"{API_V1}/{API_AUTH_REFRESH_TOKEN}/{refresh_token}",
             )
             _LOGGER.debug("refresh resp: %s", resp)
             if resp.keys() < {API_TOKEN, API_REFRESH_TOKEN}:
-                raise TokenRefreshError
+                raise TokenRefreshError("Invalid API response")
             self.token = resp[API_TOKEN]
             self.refresh_token = resp[API_REFRESH_TOKEN]
 
     def data(self) -> dict[str, Any]:
         """Return Airzone Cloud data."""
         data: dict[str, Any] = {}
 
@@ -294,15 +307,15 @@
         """Select single Airzone Cloud installation."""
         self.installations = [inst]
         for ws_id in inst.get_webservers():
             if not self.get_webserver_id(ws_id):
                 ws = WebServer(inst.get_id(), ws_id)
                 self.webservers.append(ws)
 
-    def set_system_zones_data(self, system: System):
+    def set_system_zones_data(self, system: System) -> None:
         """Set slave zones modes from master zone."""
         modes = system.get_modes()
         installation_id = system.get_installation()
         system_id = system.get_id()
         system_num = system.get_system()
         for zone in self.zones:
             zone.set_system_id(system_id)
@@ -311,14 +324,32 @@
                 is_slave
                 and modes
                 and zone.get_installation() == installation_id
                 and zone.get_system() == system_num
             ):
                 zone.set_modes(modes)
 
+    async def update_installation(self, inst: Installation) -> None:
+        """Update Airzone Cloud installation from API."""
+        installation_data = await self.api_get_installation(inst)
+        for group in installation_data[API_GROUPS]:
+            for device_data in group[API_DEVICES]:
+                if API_AZ_ZONE == device_data[API_TYPE]:
+                    if not self.get_zone_id(device_data[API_DEVICE_ID]):
+                        zone = Zone(inst.get_id(), device_data[API_WS_ID], device_data)
+                        if zone:
+                            self.zones.append(zone)
+                elif API_AZ_SYSTEM == device_data[API_TYPE]:
+                    if not self.get_system_id(device_data[API_DEVICE_ID]):
+                        system = System(
+                            inst.get_id(), device_data[API_WS_ID], device_data
+                        )
+                        if system:
+                            self.systems.append(system)
+
     async def update_installations(self) -> None:
         """Update Airzone Cloud installations from API."""
         installations_data = await self.api_get_installations()
         for installation_data in installations_data[API_INSTALLATIONS]:
             if not self.get_installation_id(installation_data[API_INSTALLATION_ID]):
                 installation = Installation(installation_data)
                 if installation:
@@ -352,26 +383,26 @@
             for device_data in ws_data[API_DEVICES]:
                 if API_AZ_ZONE == device_data[API_DEVICE_TYPE]:
                     if not self.get_zone_id(device_data[API_DEVICE_ID]):
                         zone = Zone(ws.get_installation(), ws.get_id(), device_data)
                         if zone:
                             self.zones.append(zone)
                 elif API_AZ_SYSTEM == device_data[API_DEVICE_TYPE]:
-                    if not self.get_zone_id(device_data[API_DEVICE_ID]):
+                    if not self.get_system_id(device_data[API_DEVICE_ID]):
                         system = System(ws.get_installation(), ws.get_id(), device_data)
                         if system:
                             self.systems.append(system)
 
-    async def update_webserver_id(self, ws_id: str, devices: bool = False) -> None:
+    async def update_webserver_id(self, ws_id: str, devices: bool) -> None:
         """Update Airzone Cloud WebServer by ID."""
         ws = self.get_webserver_id(ws_id)
         if ws:
             await self.update_webserver(ws, devices)
 
-    async def update_webservers(self, devices: bool = True) -> None:
+    async def update_webservers(self, devices: bool) -> None:
         """Update all Airzone Cloud WebServers."""
         for ws in self.webservers:
             await self.update_webserver(ws, devices)
 
     async def update_zone(self, zone: Zone) -> None:
         """Update Airzone Cloud Zone from API."""
         device_data = await self.api_get_device_status(zone)
@@ -386,7 +417,32 @@
     async def update_zones(self) -> None:
         """Update all Airzone Cloud Zones."""
         for zone in self.zones:
             await self.update_zone(zone)
 
         for system in self.systems:
             self.set_system_zones_data(system)
+
+    async def _update(self) -> None:
+        tasks = [
+            self.update_webservers(False),
+            self.update_systems(),
+            self.update_zones(),
+        ]
+
+        for task in tasks:
+            await task
+
+    async def update(self) -> None:
+        """Update all Airzone Cloud data."""
+
+        if (datetime.now() - self.refresh_time) > TOKEN_REFRESH_PERIOD:
+            try:
+                await self.token_refresh()
+            except TokenRefreshError:
+                await self.login()
+
+        try:
+            await self._update()
+        except LoginError:
+            await self.login()
+            await self._update()
```

### Comparing `aioairzone-cloud-0.0.4/aioairzone_cloud/common.py` & `aioairzone-cloud-0.0.5/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.4/aioairzone_cloud/device.py` & `aioairzone-cloud-0.0.5/aioairzone_cloud/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any
 
 from .common import OperationMode
 from .const import (
     API_CONFIG,
     API_DEVICE_ID,
     API_IS_CONNECTED,
+    API_META,
     API_MODE,
     API_MODE_AVAIL,
     API_SYSTEM_NUMBER,
     AZD_CONNECTED,
     AZD_ID,
     AZD_INSTALLATION,
     AZD_MODE,
@@ -30,17 +31,21 @@
 
     def __init__(self, inst_id: str, ws_id: str, device_data: dict[str, Any]):
         """Airzone Cloud Device init."""
         self.id = str(device_data[API_DEVICE_ID])
         self.installation_id = inst_id
         self.mode: OperationMode | None = None
         self.modes: list[OperationMode] = []
-        self.system_number = int(device_data[API_CONFIG][API_SYSTEM_NUMBER])
         self.webserver_id = ws_id
 
+        if API_CONFIG in device_data:
+            self.system_number = int(device_data[API_CONFIG][API_SYSTEM_NUMBER])
+        else:
+            self.system_number = int(device_data[API_META][API_SYSTEM_NUMBER])
+
         if API_IS_CONNECTED in device_data:
             self.connected = bool(device_data[API_IS_CONNECTED])
 
     def data(self) -> dict[str, Any]:
         """Return Device data."""
         data = {
             AZD_CONNECTED: self.get_connected(),
```

### Comparing `aioairzone-cloud-0.0.4/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.0.5/aioairzone_cloud/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,19 @@
     """Exception raised when API fails."""
 
 
 class LoginError(AirzoneCloudError):
     """Exception raised when login fails."""
 
 
-class TokenRefreshError(AirzoneCloudError):
+class AuthError(LoginError):
+    """Exception raised when API denies access."""
+
+
+class TokenRefreshError(LoginError):
     """Exception raised when token refresh fails."""
 
 
 class InvalidParam(AirzoneCloudError):
     """Exception raised when invalid param is requested."""
```

### Comparing `aioairzone-cloud-0.0.4/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.0.5/aioairzone_cloud/installation.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     AZD_WEBSERVERS,
 )
 
 
 class Installation:
     """Airzone Cloud Installation."""
 
-    def __init__(self, inst_data):
+    def __init__(self, inst_data: dict[str, Any]):
         """Airzone Cloud Installation init."""
         self.id = str(inst_data[API_INSTALLATION_ID])
         self.name = str(inst_data[API_NAME])
         self.webservers: list[str] = []
 
         for ws_id in inst_data[API_WS_IDS]:
             self.webservers.append(ws_id)
```

### Comparing `aioairzone-cloud-0.0.4/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.0.5/aioairzone_cloud/webserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self.stat_quality: int | None = None
         self.type: str | None = None
         self.wifi_channel: int | None = None
         self.wifi_mac: str | None = None
         self.wifi_quality: int | None = None
         self.wifi_ssid: str | None = None
 
-    def update(self, data) -> None:
+    def update(self, data: dict[str, Any]) -> None:
         """Update WebServer data."""
         self.connected = bool(data[API_STATUS][API_IS_CONNECTED])
         self.connection_date = str(data[API_STATUS][API_CONNECTION_DATE])
         self.disconnection_date = str(data[API_STATUS][API_DISCONNECTION_DATE])
         self.firmware = str(data[API_CONFIG][API_WS_FW])
         self.type = str(data[API_WS_TYPE])
         self.wifi_channel = int(data[API_CONFIG][API_STAT_CHANNEL])
```

### Comparing `aioairzone-cloud-0.0.4/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.0.5/aioairzone_cloud/zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from .const import (
     API_CELSIUS,
     API_CONFIG,
     API_DEFAULT_TEMP_STEP,
     API_HUMIDITY,
     API_LOCAL_TEMP,
+    API_META,
     API_MODE_AVAIL,
     API_NAME,
     API_POWER,
     API_RANGE_SP_MAX_COOL_AIR,
     API_RANGE_SP_MAX_DRY_AIR,
     API_RANGE_SP_MAX_EMERHEAT_AIR,
     API_RANGE_SP_MAX_HOT_AIR,
@@ -91,15 +92,19 @@
         self.temp_set_cool_air: float | None = None
         self.temp_set_dry_air: float | None = None
         self.temp_set_hot_air: float | None = None
         self.temp_set_stop_air: float | None = None
         self.temp_set_vent_air: float | None = None
         self.temp: float | None = None
         self.temp_step: float | None = None
-        self.zone_number = int(device_data[API_CONFIG][API_ZONE_NUMBER])
+
+        if API_CONFIG in device_data:
+            self.zone_number = int(device_data[API_CONFIG][API_ZONE_NUMBER])
+        else:
+            self.zone_number = int(device_data[API_META][API_ZONE_NUMBER])
 
     def data(self) -> dict[str, Any]:
         """Return Zone data."""
         data = super().data()
 
         data[AZD_HUMIDITY] = self.get_humidity()
         data[AZD_MASTER] = self.get_master()
@@ -358,15 +363,15 @@
             return round(self.temp_step, 1)
         return API_DEFAULT_TEMP_STEP
 
     def get_zone(self) -> int:
         """Return Zone number."""
         return self.zone_number
 
-    def set_modes(self, modes: list[OperationMode]):
+    def set_modes(self, modes: list[OperationMode]) -> None:
         """Set slave zone modes."""
         self.modes = modes
 
     def set_system_id(self, system_id: str) -> None:
         """Set System ID."""
         self.system_id = system_id
```

### Comparing `aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

