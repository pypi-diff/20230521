# Comparing `tmp/TeslaPy-2.7.0.tar.gz` & `tmp/TeslaPy-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TeslaPy-2.7.0.tar", last modified: Sun Dec 11 18:17:33 2022, max compression
+gzip compressed data, was "TeslaPy-2.8.0.tar", last modified: Sun May 21 10:03:50 2023, max compression
```

## Comparing `TeslaPy-2.7.0.tar` & `TeslaPy-2.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-12-11 18:17:33.203373 TeslaPy-2.7.0/
--rw-rw-rw-   0        0        0     1069 2021-02-20 17:11:36.000000 TeslaPy-2.7.0/LICENSE
--rw-rw-rw-   0        0        0       24 2021-02-21 16:17:41.000000 TeslaPy-2.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0    39717 2022-12-11 18:17:33.204370 TeslaPy-2.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    38872 2022-09-24 13:09:47.000000 TeslaPy-2.7.0/README.md
-drwxrwxrwx   0        0        0        0 2022-12-11 18:17:33.189410 TeslaPy-2.7.0/TeslaPy.egg-info/
--rw-rw-rw-   0        0        0    39717 2022-12-11 18:17:33.000000 TeslaPy-2.7.0/TeslaPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2022-12-11 18:17:33.000000 TeslaPy-2.7.0/TeslaPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-11 18:17:33.000000 TeslaPy-2.7.0/TeslaPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2022-12-11 18:17:33.000000 TeslaPy-2.7.0/TeslaPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-12-11 18:17:33.000000 TeslaPy-2.7.0/TeslaPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1046 2022-12-11 18:17:33.206364 TeslaPy-2.7.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2021-02-21 16:07:51.000000 TeslaPy-2.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-11 18:17:33.199386 TeslaPy-2.7.0/teslapy/
--rw-rw-rw-   0        0        0    43772 2022-12-11 18:16:39.000000 TeslaPy-2.7.0/teslapy/__init__.py
--rw-rw-rw-   0        0        0    61026 2022-12-11 17:31:38.000000 TeslaPy-2.7.0/teslapy/endpoints.json
--rw-rw-rw-   0        0        0    24057 2022-06-04 10:06:46.000000 TeslaPy-2.7.0/teslapy/option_codes.json
+drwxrwxrwx   0        0        0        0 2023-05-21 10:03:50.121472 TeslaPy-2.8.0/
+-rw-rw-rw-   0        0        0     1069 2021-02-20 17:11:36.000000 TeslaPy-2.8.0/LICENSE
+-rw-rw-rw-   0        0        0       24 2021-02-21 16:17:41.000000 TeslaPy-2.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    39240 2023-05-21 10:03:50.121472 TeslaPy-2.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0    38343 2023-05-12 18:00:35.000000 TeslaPy-2.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 10:03:50.115270 TeslaPy-2.8.0/TeslaPy.egg-info/
+-rw-rw-rw-   0        0        0    39240 2023-05-21 10:03:50.000000 TeslaPy-2.8.0/TeslaPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-21 10:03:50.000000 TeslaPy-2.8.0/TeslaPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 10:03:50.000000 TeslaPy-2.8.0/TeslaPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-21 10:03:50.000000 TeslaPy-2.8.0/TeslaPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 10:03:50.000000 TeslaPy-2.8.0/TeslaPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-05-21 10:03:50.121472 TeslaPy-2.8.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2021-02-21 16:07:51.000000 TeslaPy-2.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 10:03:50.121472 TeslaPy-2.8.0/teslapy/
+-rw-rw-rw-   0        0        0    42761 2023-05-21 09:57:41.000000 TeslaPy-2.8.0/teslapy/__init__.py
+-rw-rw-rw-   0        0        0    70663 2023-04-26 17:06:19.000000 TeslaPy-2.8.0/teslapy/endpoints.json
+-rw-rw-rw-   0        0        0    24057 2022-06-04 10:06:46.000000 TeslaPy-2.8.0/teslapy/option_codes.json
```

### Comparing `TeslaPy-2.7.0/LICENSE` & `TeslaPy-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TeslaPy-2.7.0/PKG-INFO` & `TeslaPy-2.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: TeslaPy
-Version: 2.7.0
+Version: 2.8.0
 Summary: A Python module to use the Tesla Motors Owner API
 Home-page: https://github.com/tdorssers/TeslaPy
 Author: Tim Dorssers
 Author-email: tim.dorssers@xs4all.nl
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TeslaPy
 
 A Python implementation based on [unofficial documentation](https://tesla-api.timdorr.com/) of the client side interface to the Tesla Motors Owner API, which provides functionality to monitor and control Tesla products remotely.
@@ -73,47 +74,42 @@
 | `refresh_token()` | requests an SSO token using [Refresh Token](https://oauth.net/2/grant-types/refresh-token/) grant |
 | `close()` | remove all requests adapter instances |
 | `logout()` | removes token from cache, returns logout URL and optionally signs out using system's default web browser |
 | `vehicle_list()` | returns a list of Vehicle objects |
 | `battery_list()` | returns a list of Battery objects |
 | `solar_list()` | returns a list of SolarPanel objects |
 
-The `Vehicle` class extends `dict` and stores vehicle data returned by the Owner API, which is a pull API. The `get_vehicle_summary()`, `get_vehicle_data()` and `get_latest_vehicle_data()` calls update the `Vehicle` instance, merging data. The streaming API pushes vehicle data on-change after subscription. The `stream()` method takes an optional argument, a callback function that is called with one argument, a dict holding the changed data. The `Vehicle` object is always updated with the pushed data. If there are no changes within 10 seconds, the vehicle stops streaming data. The `stream()` method has two more optional arguments to control restarting. Additionally, the class implements the following methods:
+The `Vehicle` class extends `dict` and stores vehicle data returned by the Owner API, which is a pull API. The `get_vehicle_summary()` and `get_vehicle_data()` calls update the `Vehicle` instance, merging data. The streaming API pushes vehicle data on-change after subscription. The `stream()` method takes an optional argument, a callback function that is called with one argument, a dict holding the changed data. The `Vehicle` object is always updated with the pushed data. If there are no changes within 10 seconds, the vehicle stops streaming data. The `stream()` method has two more optional arguments to control restarting. Additionally, the class implements the following methods:
 
 | Call | Online | Description |
 | --- | --- | --- |
 | `api()` | Yes | performs an API call to named endpoint requiring vehicle_id with optional arguments |
 | `get_vehicle_summary()` | No | gets the state of the vehicle (online, asleep, offline) |
 | `available()` | No | checks if the vehicle is online based on cached data or refreshed status when aged out |
 | `sync_wake_up()` | No | wakes up and waits for the vehicle to come online |
 | `decode_option()` | No | lookup option code description (read from *option_codes.json*) |
 | `option_code_list()` <sup>1</sup> | No | lists known descriptions of the vehicle option codes |
 | `get_vehicle_data()` | Yes | gets a rollup of all the data request endpoints plus vehicle config |
-| `get_latest_vehicle_data()` | No <sup>2</sup> | gets cached data, pushed by the vehicle on sleep, wake and around OTA |
 | `get_nearby_charging_sites()` | Yes | lists nearby Tesla-operated charging stations |
 | `get_service_scheduling_data()` | No | retrieves next service appointment for this vehicle |
-| `get_charge_history()` <sup>3</sup> | No | lists vehicle charging history data points |
-| `get_user()` | No | gets user account data |
-| `get_user_details()` | No | get user account details |
+| `get_charge_history()` <sup>2</sup> | No | lists vehicle charging history data points |
 | `mobile_enabled()` | Yes | checks if the Mobile Access setting is enabled in the car |
-| `compose_image()` <sup>4</sup> | No | composes a vehicle image based on vehicle option codes |
+| `compose_image()` <sup>3</sup> | No | composes a vehicle image based on vehicle option codes |
 | `dist_units()` | No | converts distance or speed units to GUI setting of the vehicle |
 | `temp_units()` | No | converts temperature units to GUI setting of the vehicle |
 | `gui_time()` | No | returns timestamp or current time formatted to GUI setting |
 | `last_seen()` | No | returns vehicle last seen natural time |
 | `decode_vin()` | No | decodes the vehicle identification number to a dict |
 | `command()` | Yes | wrapper around `api()` for vehicle command response error handling |
 
-<sup>1</sup> Option codes appear to be deprecated. Vehicles return a generic set of codes related to a Model 3.
+<sup>1</sup> Option codes appear to be deprecated.
 
-<sup>2</sup> Vehicle should still be online if there is no cached data available.
+<sup>2</sup> Car software version 2021.44.25 or higher required, Data Sharing must be enabled and you must be the primary vehicle owner.
 
-<sup>3</sup> Car software version 2021.44.25 or higher required, Data Sharing must be enabled and you must be the primary vehicle owner.
-
-<sup>4</sup> Pass vehicle option codes to this method or the image may not be accurate.
+<sup>3</sup> Pass vehicle option codes to this method now options codes are deprecated.
 
 Only methods with *No* in the *Online* column are available when the vehicle is asleep or offline. These methods will not prevent your vehicle from sleeping. Other methods and API calls require the vehicle to be brought online by using `sync_wake_up()` and can prevent your vehicle from sleeping if called within too short a period.
 
 The `Product` class extends `dict` and is initialized with product data of Powerwalls and solar panels returned by the API. Additionally, the class implements the following methods:
 
 | Call | Description |
 | --- | --- |
@@ -373,15 +369,15 @@
 | HONK_HORN | | |
 | FLASH_LIGHTS | | |
 | CLIMATE_ON | | |
 | CLIMATE_OFF | | |
 | MAX_DEFROST | `on` | `true` or `false` |
 | CHANGE_CLIMATE_TEMPERATURE_SETTING | `driver_temp`, `passenger_temp` | temperature in celcius |
 | SET_CLIMATE_KEEPER_MODE | `climate_keeper_mode` | 0=off, 1=on, 2=dog, 3=camp |
-| HVAC_BIOWEAPON_MODE | |
+| HVAC_BIOWEAPON_MODE | `on` | `true` or `false` |
 | SCHEDULED_DEPARTURE <sup>1</sup> | `enable`, `departure_time`, `preconditioning_enabled`, `preconditioning_weekdays_only`, `off_peak_charging_enabled`, `off_peak_charging_weekdays_only`, `end_off_peak_time` | `true` or `false`, minutes past midnight |
 | SCHEDULED_CHARGING <sup>1</sup> | `enable`, `time` | `true` or `false`, minutes past midnight |
 | CHARGING_AMPS <sup>1</sup> | `charging_amps` | between 0-32 |
 | SET_CABIN_OVERHEAT_PROTECTION | `on`, `fan_only` | `true` or `false` |
 | CHANGE_CHARGE_LIMIT | `percent` | percentage |
 | SET_VEHICLE_NAME | `vehicle_name` | name |
 | CHANGE_SUNROOF_STATE | `state` | `vent` or `close` |
@@ -389,14 +385,15 @@
 | ACTUATE_TRUNK | `which_trunk` | `rear` or `front` |
 | REMOTE_START | | |
 | TRIGGER_HOMELINK | `lat`, `lon` | current lattitude and logitude |
 | CHARGE_PORT_DOOR_OPEN | | |
 | CHARGE_PORT_DOOR_CLOSE | | |
 | START_CHARGE | | |
 | STOP_CHARGE | | |
+| SET_COP_TEMP | `temp` | temperature in celcius |
 | MEDIA_TOGGLE_PLAYBACK | | |
 | MEDIA_NEXT_TRACK | | |
 | MEDIA_PREVIOUS_TRACK | | |
 | MEDIA_NEXT_FAVORITE | | |
 | MEDIA_PREVIOUS_FAVORITE | | |
 | MEDIA_VOLUME_UP | | |
 | MEDIA_VOLUME_DOWN | | |
@@ -516,15 +513,15 @@
 
 ```json
 {
     "id": 12345678901234567,
     "vehicle_id": 1234567890,
     "vin": "5YJ3E111111111111",
     "display_name": "Tim's Tesla",
-    "option_codes": "AD15,MDL3,PBSB,RENA,BT37,ID3W,RF3G,S3PB,DRLH,DV2W,W39B,APF0,COUS,BC3B,CH07,PC30,FC3P,FG31,GLFR,HL31,HM31,IL31,LTPB,MR31,FM3B,RS3H,SA3P,STCP,SC04,SU3C,T3CA,TW00,TM00,UT3P,WR00,AU3P,APH3,AF00,ZCST,MI00,CDM0",
+    "option_codes": null,
     "color": null,
     "tokens": [
         "1234567890abcdef",
         "abcdef1234567890"
     ],
     "state": "online",
     "in_service": false,
```

### Comparing `TeslaPy-2.7.0/README.md` & `TeslaPy-2.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,47 +52,42 @@
 | `refresh_token()` | requests an SSO token using [Refresh Token](https://oauth.net/2/grant-types/refresh-token/) grant |
 | `close()` | remove all requests adapter instances |
 | `logout()` | removes token from cache, returns logout URL and optionally signs out using system's default web browser |
 | `vehicle_list()` | returns a list of Vehicle objects |
 | `battery_list()` | returns a list of Battery objects |
 | `solar_list()` | returns a list of SolarPanel objects |
 
-The `Vehicle` class extends `dict` and stores vehicle data returned by the Owner API, which is a pull API. The `get_vehicle_summary()`, `get_vehicle_data()` and `get_latest_vehicle_data()` calls update the `Vehicle` instance, merging data. The streaming API pushes vehicle data on-change after subscription. The `stream()` method takes an optional argument, a callback function that is called with one argument, a dict holding the changed data. The `Vehicle` object is always updated with the pushed data. If there are no changes within 10 seconds, the vehicle stops streaming data. The `stream()` method has two more optional arguments to control restarting. Additionally, the class implements the following methods:
+The `Vehicle` class extends `dict` and stores vehicle data returned by the Owner API, which is a pull API. The `get_vehicle_summary()` and `get_vehicle_data()` calls update the `Vehicle` instance, merging data. The streaming API pushes vehicle data on-change after subscription. The `stream()` method takes an optional argument, a callback function that is called with one argument, a dict holding the changed data. The `Vehicle` object is always updated with the pushed data. If there are no changes within 10 seconds, the vehicle stops streaming data. The `stream()` method has two more optional arguments to control restarting. Additionally, the class implements the following methods:
 
 | Call | Online | Description |
 | --- | --- | --- |
 | `api()` | Yes | performs an API call to named endpoint requiring vehicle_id with optional arguments |
 | `get_vehicle_summary()` | No | gets the state of the vehicle (online, asleep, offline) |
 | `available()` | No | checks if the vehicle is online based on cached data or refreshed status when aged out |
 | `sync_wake_up()` | No | wakes up and waits for the vehicle to come online |
 | `decode_option()` | No | lookup option code description (read from *option_codes.json*) |
 | `option_code_list()` <sup>1</sup> | No | lists known descriptions of the vehicle option codes |
 | `get_vehicle_data()` | Yes | gets a rollup of all the data request endpoints plus vehicle config |
-| `get_latest_vehicle_data()` | No <sup>2</sup> | gets cached data, pushed by the vehicle on sleep, wake and around OTA |
 | `get_nearby_charging_sites()` | Yes | lists nearby Tesla-operated charging stations |
 | `get_service_scheduling_data()` | No | retrieves next service appointment for this vehicle |
-| `get_charge_history()` <sup>3</sup> | No | lists vehicle charging history data points |
-| `get_user()` | No | gets user account data |
-| `get_user_details()` | No | get user account details |
+| `get_charge_history()` <sup>2</sup> | No | lists vehicle charging history data points |
 | `mobile_enabled()` | Yes | checks if the Mobile Access setting is enabled in the car |
-| `compose_image()` <sup>4</sup> | No | composes a vehicle image based on vehicle option codes |
+| `compose_image()` <sup>3</sup> | No | composes a vehicle image based on vehicle option codes |
 | `dist_units()` | No | converts distance or speed units to GUI setting of the vehicle |
 | `temp_units()` | No | converts temperature units to GUI setting of the vehicle |
 | `gui_time()` | No | returns timestamp or current time formatted to GUI setting |
 | `last_seen()` | No | returns vehicle last seen natural time |
 | `decode_vin()` | No | decodes the vehicle identification number to a dict |
 | `command()` | Yes | wrapper around `api()` for vehicle command response error handling |
 
-<sup>1</sup> Option codes appear to be deprecated. Vehicles return a generic set of codes related to a Model 3.
+<sup>1</sup> Option codes appear to be deprecated.
 
-<sup>2</sup> Vehicle should still be online if there is no cached data available.
+<sup>2</sup> Car software version 2021.44.25 or higher required, Data Sharing must be enabled and you must be the primary vehicle owner.
 
-<sup>3</sup> Car software version 2021.44.25 or higher required, Data Sharing must be enabled and you must be the primary vehicle owner.
-
-<sup>4</sup> Pass vehicle option codes to this method or the image may not be accurate.
+<sup>3</sup> Pass vehicle option codes to this method now options codes are deprecated.
 
 Only methods with *No* in the *Online* column are available when the vehicle is asleep or offline. These methods will not prevent your vehicle from sleeping. Other methods and API calls require the vehicle to be brought online by using `sync_wake_up()` and can prevent your vehicle from sleeping if called within too short a period.
 
 The `Product` class extends `dict` and is initialized with product data of Powerwalls and solar panels returned by the API. Additionally, the class implements the following methods:
 
 | Call | Description |
 | --- | --- |
@@ -352,15 +347,15 @@
 | HONK_HORN | | |
 | FLASH_LIGHTS | | |
 | CLIMATE_ON | | |
 | CLIMATE_OFF | | |
 | MAX_DEFROST | `on` | `true` or `false` |
 | CHANGE_CLIMATE_TEMPERATURE_SETTING | `driver_temp`, `passenger_temp` | temperature in celcius |
 | SET_CLIMATE_KEEPER_MODE | `climate_keeper_mode` | 0=off, 1=on, 2=dog, 3=camp |
-| HVAC_BIOWEAPON_MODE | |
+| HVAC_BIOWEAPON_MODE | `on` | `true` or `false` |
 | SCHEDULED_DEPARTURE <sup>1</sup> | `enable`, `departure_time`, `preconditioning_enabled`, `preconditioning_weekdays_only`, `off_peak_charging_enabled`, `off_peak_charging_weekdays_only`, `end_off_peak_time` | `true` or `false`, minutes past midnight |
 | SCHEDULED_CHARGING <sup>1</sup> | `enable`, `time` | `true` or `false`, minutes past midnight |
 | CHARGING_AMPS <sup>1</sup> | `charging_amps` | between 0-32 |
 | SET_CABIN_OVERHEAT_PROTECTION | `on`, `fan_only` | `true` or `false` |
 | CHANGE_CHARGE_LIMIT | `percent` | percentage |
 | SET_VEHICLE_NAME | `vehicle_name` | name |
 | CHANGE_SUNROOF_STATE | `state` | `vent` or `close` |
@@ -368,14 +363,15 @@
 | ACTUATE_TRUNK | `which_trunk` | `rear` or `front` |
 | REMOTE_START | | |
 | TRIGGER_HOMELINK | `lat`, `lon` | current lattitude and logitude |
 | CHARGE_PORT_DOOR_OPEN | | |
 | CHARGE_PORT_DOOR_CLOSE | | |
 | START_CHARGE | | |
 | STOP_CHARGE | | |
+| SET_COP_TEMP | `temp` | temperature in celcius |
 | MEDIA_TOGGLE_PLAYBACK | | |
 | MEDIA_NEXT_TRACK | | |
 | MEDIA_PREVIOUS_TRACK | | |
 | MEDIA_NEXT_FAVORITE | | |
 | MEDIA_PREVIOUS_FAVORITE | | |
 | MEDIA_VOLUME_UP | | |
 | MEDIA_VOLUME_DOWN | | |
@@ -495,15 +491,15 @@
 
 ```json
 {
     "id": 12345678901234567,
     "vehicle_id": 1234567890,
     "vin": "5YJ3E111111111111",
     "display_name": "Tim's Tesla",
-    "option_codes": "AD15,MDL3,PBSB,RENA,BT37,ID3W,RF3G,S3PB,DRLH,DV2W,W39B,APF0,COUS,BC3B,CH07,PC30,FC3P,FG31,GLFR,HL31,HM31,IL31,LTPB,MR31,FM3B,RS3H,SA3P,STCP,SC04,SU3C,T3CA,TW00,TM00,UT3P,WR00,AU3P,APH3,AF00,ZCST,MI00,CDM0",
+    "option_codes": null,
     "color": null,
     "tokens": [
         "1234567890abcdef",
         "abcdef1234567890"
     ],
     "state": "online",
     "in_service": false,
```

### Comparing `TeslaPy-2.7.0/TeslaPy.egg-info/PKG-INFO` & `TeslaPy-2.8.0/TeslaPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: TeslaPy
-Version: 2.7.0
+Version: 2.8.0
 Summary: A Python module to use the Tesla Motors Owner API
 Home-page: https://github.com/tdorssers/TeslaPy
 Author: Tim Dorssers
 Author-email: tim.dorssers@xs4all.nl
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TeslaPy
 
 A Python implementation based on [unofficial documentation](https://tesla-api.timdorr.com/) of the client side interface to the Tesla Motors Owner API, which provides functionality to monitor and control Tesla products remotely.
@@ -73,47 +74,42 @@
 | `refresh_token()` | requests an SSO token using [Refresh Token](https://oauth.net/2/grant-types/refresh-token/) grant |
 | `close()` | remove all requests adapter instances |
 | `logout()` | removes token from cache, returns logout URL and optionally signs out using system's default web browser |
 | `vehicle_list()` | returns a list of Vehicle objects |
 | `battery_list()` | returns a list of Battery objects |
 | `solar_list()` | returns a list of SolarPanel objects |
 
-The `Vehicle` class extends `dict` and stores vehicle data returned by the Owner API, which is a pull API. The `get_vehicle_summary()`, `get_vehicle_data()` and `get_latest_vehicle_data()` calls update the `Vehicle` instance, merging data. The streaming API pushes vehicle data on-change after subscription. The `stream()` method takes an optional argument, a callback function that is called with one argument, a dict holding the changed data. The `Vehicle` object is always updated with the pushed data. If there are no changes within 10 seconds, the vehicle stops streaming data. The `stream()` method has two more optional arguments to control restarting. Additionally, the class implements the following methods:
+The `Vehicle` class extends `dict` and stores vehicle data returned by the Owner API, which is a pull API. The `get_vehicle_summary()` and `get_vehicle_data()` calls update the `Vehicle` instance, merging data. The streaming API pushes vehicle data on-change after subscription. The `stream()` method takes an optional argument, a callback function that is called with one argument, a dict holding the changed data. The `Vehicle` object is always updated with the pushed data. If there are no changes within 10 seconds, the vehicle stops streaming data. The `stream()` method has two more optional arguments to control restarting. Additionally, the class implements the following methods:
 
 | Call | Online | Description |
 | --- | --- | --- |
 | `api()` | Yes | performs an API call to named endpoint requiring vehicle_id with optional arguments |
 | `get_vehicle_summary()` | No | gets the state of the vehicle (online, asleep, offline) |
 | `available()` | No | checks if the vehicle is online based on cached data or refreshed status when aged out |
 | `sync_wake_up()` | No | wakes up and waits for the vehicle to come online |
 | `decode_option()` | No | lookup option code description (read from *option_codes.json*) |
 | `option_code_list()` <sup>1</sup> | No | lists known descriptions of the vehicle option codes |
 | `get_vehicle_data()` | Yes | gets a rollup of all the data request endpoints plus vehicle config |
-| `get_latest_vehicle_data()` | No <sup>2</sup> | gets cached data, pushed by the vehicle on sleep, wake and around OTA |
 | `get_nearby_charging_sites()` | Yes | lists nearby Tesla-operated charging stations |
 | `get_service_scheduling_data()` | No | retrieves next service appointment for this vehicle |
-| `get_charge_history()` <sup>3</sup> | No | lists vehicle charging history data points |
-| `get_user()` | No | gets user account data |
-| `get_user_details()` | No | get user account details |
+| `get_charge_history()` <sup>2</sup> | No | lists vehicle charging history data points |
 | `mobile_enabled()` | Yes | checks if the Mobile Access setting is enabled in the car |
-| `compose_image()` <sup>4</sup> | No | composes a vehicle image based on vehicle option codes |
+| `compose_image()` <sup>3</sup> | No | composes a vehicle image based on vehicle option codes |
 | `dist_units()` | No | converts distance or speed units to GUI setting of the vehicle |
 | `temp_units()` | No | converts temperature units to GUI setting of the vehicle |
 | `gui_time()` | No | returns timestamp or current time formatted to GUI setting |
 | `last_seen()` | No | returns vehicle last seen natural time |
 | `decode_vin()` | No | decodes the vehicle identification number to a dict |
 | `command()` | Yes | wrapper around `api()` for vehicle command response error handling |
 
-<sup>1</sup> Option codes appear to be deprecated. Vehicles return a generic set of codes related to a Model 3.
+<sup>1</sup> Option codes appear to be deprecated.
 
-<sup>2</sup> Vehicle should still be online if there is no cached data available.
+<sup>2</sup> Car software version 2021.44.25 or higher required, Data Sharing must be enabled and you must be the primary vehicle owner.
 
-<sup>3</sup> Car software version 2021.44.25 or higher required, Data Sharing must be enabled and you must be the primary vehicle owner.
-
-<sup>4</sup> Pass vehicle option codes to this method or the image may not be accurate.
+<sup>3</sup> Pass vehicle option codes to this method now options codes are deprecated.
 
 Only methods with *No* in the *Online* column are available when the vehicle is asleep or offline. These methods will not prevent your vehicle from sleeping. Other methods and API calls require the vehicle to be brought online by using `sync_wake_up()` and can prevent your vehicle from sleeping if called within too short a period.
 
 The `Product` class extends `dict` and is initialized with product data of Powerwalls and solar panels returned by the API. Additionally, the class implements the following methods:
 
 | Call | Description |
 | --- | --- |
@@ -373,15 +369,15 @@
 | HONK_HORN | | |
 | FLASH_LIGHTS | | |
 | CLIMATE_ON | | |
 | CLIMATE_OFF | | |
 | MAX_DEFROST | `on` | `true` or `false` |
 | CHANGE_CLIMATE_TEMPERATURE_SETTING | `driver_temp`, `passenger_temp` | temperature in celcius |
 | SET_CLIMATE_KEEPER_MODE | `climate_keeper_mode` | 0=off, 1=on, 2=dog, 3=camp |
-| HVAC_BIOWEAPON_MODE | |
+| HVAC_BIOWEAPON_MODE | `on` | `true` or `false` |
 | SCHEDULED_DEPARTURE <sup>1</sup> | `enable`, `departure_time`, `preconditioning_enabled`, `preconditioning_weekdays_only`, `off_peak_charging_enabled`, `off_peak_charging_weekdays_only`, `end_off_peak_time` | `true` or `false`, minutes past midnight |
 | SCHEDULED_CHARGING <sup>1</sup> | `enable`, `time` | `true` or `false`, minutes past midnight |
 | CHARGING_AMPS <sup>1</sup> | `charging_amps` | between 0-32 |
 | SET_CABIN_OVERHEAT_PROTECTION | `on`, `fan_only` | `true` or `false` |
 | CHANGE_CHARGE_LIMIT | `percent` | percentage |
 | SET_VEHICLE_NAME | `vehicle_name` | name |
 | CHANGE_SUNROOF_STATE | `state` | `vent` or `close` |
@@ -389,14 +385,15 @@
 | ACTUATE_TRUNK | `which_trunk` | `rear` or `front` |
 | REMOTE_START | | |
 | TRIGGER_HOMELINK | `lat`, `lon` | current lattitude and logitude |
 | CHARGE_PORT_DOOR_OPEN | | |
 | CHARGE_PORT_DOOR_CLOSE | | |
 | START_CHARGE | | |
 | STOP_CHARGE | | |
+| SET_COP_TEMP | `temp` | temperature in celcius |
 | MEDIA_TOGGLE_PLAYBACK | | |
 | MEDIA_NEXT_TRACK | | |
 | MEDIA_PREVIOUS_TRACK | | |
 | MEDIA_NEXT_FAVORITE | | |
 | MEDIA_PREVIOUS_FAVORITE | | |
 | MEDIA_VOLUME_UP | | |
 | MEDIA_VOLUME_DOWN | | |
@@ -516,15 +513,15 @@
 
 ```json
 {
     "id": 12345678901234567,
     "vehicle_id": 1234567890,
     "vin": "5YJ3E111111111111",
     "display_name": "Tim's Tesla",
-    "option_codes": "AD15,MDL3,PBSB,RENA,BT37,ID3W,RF3G,S3PB,DRLH,DV2W,W39B,APF0,COUS,BC3B,CH07,PC30,FC3P,FG31,GLFR,HL31,HM31,IL31,LTPB,MR31,FM3B,RS3H,SA3P,STCP,SC04,SU3C,T3CA,TW00,TM00,UT3P,WR00,AU3P,APH3,AF00,ZCST,MI00,CDM0",
+    "option_codes": null,
     "color": null,
     "tokens": [
         "1234567890abcdef",
         "abcdef1234567890"
     ],
     "state": "online",
     "in_service": false,
```

### Comparing `TeslaPy-2.7.0/setup.cfg` & `TeslaPy-2.8.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b62 6469 7374 5f77 6865 656c 5d0d 0a75  [bdist_wheel]..u
 00000010: 6e69 7665 7273 616c 203d 2031 0d0a 0d0a  niversal = 1....
 00000020: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000030: 203d 2054 6573 6c61 5079 0d0a 7665 7273   = TeslaPy..vers
-00000040: 696f 6e20 3d20 322e 372e 300d 0a61 7574  ion = 2.7.0..aut
+00000040: 696f 6e20 3d20 322e 382e 300d 0a61 7574  ion = 2.8.0..aut
 00000050: 686f 7220 3d20 5469 6d20 446f 7273 7365  hor = Tim Dorsse
 00000060: 7273 0d0a 6175 7468 6f72 5f65 6d61 696c  rs..author_email
 00000070: 203d 2074 696d 2e64 6f72 7373 6572 7340   = tim.dorssers@
 00000080: 7873 3461 6c6c 2e6e 6c0d 0a64 6573 6372  xs4all.nl..descr
 00000090: 6970 7469 6f6e 203d 2041 2050 7974 686f  iption = A Pytho
 000000a0: 6e20 6d6f 6475 6c65 2074 6f20 7573 6520  n module to use 
 000000b0: 7468 6520 5465 736c 6120 4d6f 746f 7273  the Tesla Motors
@@ -40,27 +40,29 @@
 00000270: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
 00000280: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
 00000290: 3a3a 2033 2e38 0d0a 0950 726f 6772 616d  :: 3.8...Program
 000002a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
 000002b0: 2050 7974 686f 6e20 3a3a 2033 2e39 0d0a   Python :: 3.9..
 000002c0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
 000002d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002e0: 3a3a 2033 2e31 300d 0a09 4f70 6572 6174  :: 3.10...Operat
-000002f0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000300: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
-00000310: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
-00000320: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-00000330: 686f 6e5f 7265 7175 6972 6573 203e 203d  hon_requires > =
-00000340: 2032 2e37 2c20 213d 332e 302e 2a2c 2021   2.7, !=3.0.*, !
-00000350: 3d33 2e31 2e2a 2c20 213d 332e 322e 2a2c  =3.1.*, !=3.2.*,
-00000360: 2021 3d33 2e33 2e2a 2c20 213d 332e 342e   !=3.3.*, !=3.4.
-00000370: 2a0d 0a69 6e63 6c75 6465 5f70 6163 6b61  *..include_packa
-00000380: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
-00000390: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-000003a0: 203d 200d 0a09 7265 7175 6573 7473 203e   = ...requests >
-000003b0: 3d20 322e 342e 320d 0a09 7265 7175 6573  = 2.4.2...reques
-000003c0: 7473 5f6f 6175 7468 6c69 620d 0a09 7765  ts_oauthlib...we
-000003d0: 6273 6f63 6b65 742d 636c 6965 6e74 203e  bsocket-client >
-000003e0: 3d20 302e 3539 2e30 0d0a 0d0a 5b65 6767  = 0.59.0....[egg
-000003f0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000400: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000410: 2030 0d0a 0d0a                            0....
+000002e0: 3a3a 2033 2e31 300d 0a09 5072 6f67 7261  :: 3.10...Progra
+000002f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000300: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
+00000310: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+00000320: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000330: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
+00000340: 735d 0d0a 7061 636b 6167 6573 203d 2066  s]..packages = f
+00000350: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
+00000360: 7569 7265 7320 3e20 3d20 322e 372c 2021  uires > = 2.7, !
+00000370: 3d33 2e30 2e2a 2c20 213d 332e 312e 2a2c  =3.0.*, !=3.1.*,
+00000380: 2021 3d33 2e32 2e2a 2c20 213d 332e 332e   !=3.2.*, !=3.3.
+00000390: 2a2c 2021 3d33 2e34 2e2a 0d0a 696e 636c  *, !=3.4.*..incl
+000003a0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+000003b0: 203d 2054 7275 650d 0a69 6e73 7461 6c6c   = True..install
+000003c0: 5f72 6571 7569 7265 7320 3d20 0d0a 0972  _requires = ...r
+000003d0: 6571 7565 7374 7320 3e3d 2032 2e34 2e32  equests >= 2.4.2
+000003e0: 0d0a 0972 6571 7565 7374 735f 6f61 7574  ...requests_oaut
+000003f0: 686c 6962 0d0a 0977 6562 736f 636b 6574  hlib...websocket
+00000400: 2d63 6c69 656e 7420 3e3d 2030 2e35 392e  -client >= 0.59.
+00000410: 300d 0a0d 0a5b 6567 675f 696e 666f 5d0d  0....[egg_info].
+00000420: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000430: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `TeslaPy-2.7.0/teslapy/__init__.py` & `TeslaPy-2.8.0/teslapy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 RFC compliant OAuth 2 Single Sign-On service. Tokens are saved to 'cache.json'
 for reuse and refreshed automatically. The vehicle option codes are loaded from
 'option_codes.json' and the API endpoints are loaded from 'endpoints.json'.
 """
 
 # Author: Tim Dorssers
 
-__version__ = '2.7.0'
+__version__ = '2.8.0'
 
 import os
 import ast
 import json
 import time
 import base64
 import hashlib
@@ -532,32 +532,25 @@
                 cls.codes = {}
                 logger.error('No option codes loaded')
         # Lookup option code title
         return cls.codes.get(code)
 
     def option_code_list(self):
         """ Returns a list of known vehicle option code titles """
+        codes = self['option_codes'] if self['option_codes'] else ''
         return list(filter(None, [self.decode_option(code)
-                                  for code in self['option_codes'].split(',')]))
+                                  for code in codes.split(',')]))
 
     def get_vehicle_data(self):
         """ A rollup of all the data request endpoints plus vehicle config.
         Raises HTTPError when vehicle is not online. """
         self.update(self.api('VEHICLE_DATA')['response'])
         self.timestamp = time.time()
         return self
 
-    def get_latest_vehicle_data(self):
-        """ Cached data, pushed by the vehicle on sleep, wake and around OTA.
-        Raises HTTPError if no data is available and vehicle is not online. """
-        response = self.api('CACHED_PROTO_VEHICLE_DATA')['response']
-        self.update(response['data'] if 'data' in response else response)
-        self.timestamp = time.time()
-        return self
-
     def get_nearby_charging_sites(self):
         """ Lists nearby Tesla-operated charging stations. Raises HTTPError when
         vehicle is in service or not online. """
         return self.api('NEARBY_CHARGING_SITES')['response']
 
     def get_service_scheduling_data(self):
         """ Retrieves next service appointment for this vehicle """
@@ -565,53 +558,40 @@
         return next((enabled for enabled in response['enabled_vins']
                      if enabled['vin'] == self['vin']), {})
 
     def get_charge_history(self):
         """ Lists vehicle charging history data points """
         return self.api('VEHICLE_CHARGE_HISTORY')['response']
 
-    def get_user(self, device_country='US', device_language='EN'):
-        """ Retrieve user account data """
-        return self.tesla.api('USER', vin=self['vin'],
-                              deviceCountry=device_country,
-                              deviceLanguage=device_language)['data']
-
-    def get_user_details(self, device_country='US', device_language='EN'):
-        """ Retrieve user account details """
-        return self.tesla.api('USER_ACCOUNT_GET_DETAILS', vin=self['vin'],
-                              deviceCountry=device_country,
-                              deviceLanguage=device_language)['data']
-
     def mobile_enabled(self):
         """ Checks if the Mobile Access setting is enabled in the car. Raises
         HTTPError when vehicle is in service or not online. """
         # Construct URL and send request
         uri = 'api/1/vehicles/%s/mobile_enabled' % self['id_s']
         return self.tesla.get(uri)['response']
 
     def compose_image(self, view='STUD_3QTR', size=640, options=None):
         """ Returns a PNG formatted composed vehicle image. Valid views are:
         STUD_3QTR, STUD_SEAT, STUD_SIDE, STUD_REAR and STUD_WHEEL """
-        if options is None:
-            logger.warning('`compose_image` requires `options` to be set for '
-                           'an accurate image')
+        if options is None and self['option_codes'] is None:
+            raise ValueError('`compose_image` requires `options` to be set')
         # Derive model from VIN and other properties from (given) option codes
         params = {'model': 'm' + self['vin'][3].lower(),
                   'bkba_opt': 1, 'view': view, 'size': size,
                   'options': options or self['option_codes']}
         # Retrieve image from compositor
         url = 'https://static-assets.tesla.com/v1/compositor/'
         response = requests.get(url, params=params, verify=self.tesla.verify,
                                 proxies=self.tesla.proxies)
         response.raise_for_status()  # Raise HTTPError, if one occurred
         return response.content
 
     def __missing__(self, key):
         """ Get cached data when accessed. Raises KeyError on invalid key. """
-        if key not in self.get_latest_vehicle_data():
+        if key not in self.get_vehicle_data():
             raise KeyError(key)
         return self[key]
 
     def dist_units(self, miles, speed=False):
         """ Format and convert distance or speed to GUI setting units """
         if miles is None:
             return None
```

### Comparing `TeslaPy-2.7.0/teslapy/endpoints.json` & `TeslaPy-2.8.0/teslapy/endpoints.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8657844990548204%*

 * *Differences: {"'ADD_MANAGED_CHARGING_SITE'": "OrderedDict([('TYPE', 'POST'), ('URI', "*

 * *                                "'api/1/vehicles/{vehicle_id}/command/add_managed_charging_site'), "*

 * *                                "('AUTH', True)])",*

 * * "'CHARGE_STATE'": "OrderedDict([('TYPE', 'GET'), ('URI', "*

 * *                   "'api/1/vehicles/{vehicle_id}/data_request/charge_state'), ('AUTH', True)])",*

 * * "'CHARGING_BALANCE_GET_CTA'": "OrderedDict([('TYPE', 'GET'), ('URI', "*

 * *                               "'bff/v2/mobile-app/charg […]*

```diff
@@ -5,14 +5,19 @@
         "URI": "api/1/vehicles/{vehicle_id}/command/actuate_trunk"
     },
     "ADD_KEY": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/add_key"
     },
+    "ADD_MANAGED_CHARGING_SITE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/vehicles/{vehicle_id}/command/add_managed_charging_site"
+    },
     "ADJUST_VOLUME": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/adjust_volume"
     },
     "APP_FEEDBACK_ENTITLEMENTS": {
         "AUTH": true,
@@ -131,14 +136,19 @@
         "URI": "api/1/vehicles/{vehicle_id}/command/charge_port_door_close"
     },
     "CHARGE_PORT_DOOR_OPEN": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/charge_port_door_open"
     },
+    "CHARGE_STATE": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "api/1/vehicles/{vehicle_id}/data_request/charge_state"
+    },
     "CHARGING_AMPS": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/set_charging_amps"
     },
     "CHARGING_BALANCE": {
         "AUTH": true,
@@ -151,14 +161,19 @@
         "URI": "bff/v2/mobile-app/feature-flag/tao-9296-filter-by-charge-type"
     },
     "CHARGING_BALANCE_CREATE_OFFLINE_ORDER": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/charging/payment"
     },
+    "CHARGING_BALANCE_GET_CTA": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/charging-cn/supercharger-balance-cta"
+    },
     "CHARGING_BALANCE_GET_IS_BLOCKED": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/charging-cn/supercharger-status"
     },
     "CHARGING_BALANCE_PAYMENT": {
         "AUTH": true,
@@ -436,14 +451,19 @@
         "URI": "bff/v2/mobile-app/contact-us/classify-narrative"
     },
     "CONTACT_US_CONTENT_CATALOG": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "mobile-app/contact-us/content-catalog"
     },
+    "CREATE_ENERGY_SITE_SHARE_INVITE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/energy_sites/{site_id}/invitations"
+    },
     "CREATE_VEHICLE_SHARE_INVITE": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/invitations"
     },
     "DASHCAM_SAVE_CLIP": {
         "AUTH": true,
@@ -451,14 +471,24 @@
         "URI": "api/1/vehicles/{vehicle_id}/command/dashcam_save_clip"
     },
     "DEACTIVATE_DEVICE_TOKEN": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/device/{device_token}/deactivate"
     },
+    "DOCUMENTS_DOWNLOAD_FAPIAO": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/documents/fapiao/{fapiaoId}"
+    },
+    "DOCUMENTS_DOWNLOAD_INSPECTION": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/service/documents/inspection/{serviceVisitID}"
+    },
     "DOCUMENTS_DOWNLOAD_INVOICE": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/documents/invoices/{invoiceId}"
     },
     "DOWNLOAD_CHARGING_INVOICE": {
         "AUTH": true,
@@ -489,75 +519,75 @@
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/energy_sites/energy_event"
     },
     "ENERGY_GET_TROUBLESHOOTING_GUIDE": {
         "AUTH": true,
         "TYPE": "GET",
-        "URI": "bff/v2/mobile-app/energy-service/troubleshooting/{troubleshootingFlow}?version=3"
+        "URI": "bff/v2/mobile-app/energy-support/troubleshooting/{troubleshootingFlow}?version=3"
     },
     "ENERGY_OWNERSHIP_GET_TOGGLES": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/energy/feature-flags"
     },
     "ENERGY_REGISTER_PRODUCT": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/users/register_product"
     },
     "ENERGY_SERVICE_CANCEL_APPOINTMENT": {
         "AUTH": true,
         "TYPE": "PUT",
-        "URI": "bff/v2/mobile-app/energy-service/appointments"
+        "URI": "bff/v2/mobile-app/energy-support/appointments"
     },
     "ENERGY_SERVICE_CANCEL_GRID_SERVICE_CASE": {
         "AUTH": true,
         "TYPE": "PUT",
-        "URI": "bff/v2/mobile-app/energy-service/service-case"
+        "URI": "bff/v2/mobile-app/energy-support/service-case"
     },
     "ENERGY_SERVICE_CANCEL_SUPPORT_CASE": {
         "AUTH": true,
         "TYPE": "PUT",
         "URI": "bff/v2/mobile-app/energy-support/support-cases"
     },
     "ENERGY_SERVICE_CONFIRM_APPOINTMENT": {
         "AUTH": true,
         "TYPE": "PUT",
-        "URI": "bff/v2/mobile-app/energy-service/confirm-appointment"
+        "URI": "bff/v2/mobile-app/energy-support/confirm-appointment"
     },
     "ENERGY_SERVICE_GET_APPOINTMENT_SUGGESTIONS": {
         "AUTH": true,
         "TYPE": "GET",
-        "URI": "bff/v2/mobile-app/energy-service/appointment-suggestions"
+        "URI": "bff/v2/mobile-app/energy-support/appointment-suggestions"
     },
     "ENERGY_SERVICE_GET_CHAT_AVAILABILITY": {
         "AUTH": true,
         "TYPE": "GET",
-        "URI": "bff/v2/mobile-app/energy-service/chat-availability"
+        "URI": "bff/v2/mobile-app/energy-support/chat-availability"
     },
     "ENERGY_SERVICE_GET_POWERWALL_WARRANTY_DETAILS": {
         "AUTH": true,
         "TYPE": "GET",
-        "URI": "bff/v2/mobile-app/energy-service/warranty-details"
+        "URI": "bff/v2/mobile-app/energy-support/warranty-details"
     },
     "ENERGY_SERVICE_GET_SITE_INFORMATION": {
         "AUTH": true,
         "TYPE": "GET",
-        "URI": "bff/v2/mobile-app/energy-service/site-information"
+        "URI": "bff/v2/mobile-app/energy-support/site-information"
     },
     "ENERGY_SERVICE_GET_SUPPORT_CASES": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/energy-support/support-cases"
     },
     "ENERGY_SERVICE_POST_GRID_SERVICE_CASE": {
         "AUTH": true,
         "TYPE": "POST",
-        "URI": "bff/v2/mobile-app/energy-service/appointments"
+        "URI": "bff/v2/mobile-app/energy-support/appointments"
     },
     "ENERGY_SERVICE_POST_SUPPORT_CASE": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/energy-support/support-cases"
     },
     "ENERGY_SITE_BACKUP_TIME_REMAINING": {
@@ -661,14 +691,19 @@
         "URI": "api/1/wall_connectors/firmware"
     },
     "ESA_CREATE_OFFLINE_ORDER": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/esa/payment/offline-order"
     },
+    "ESA_DOWNLOAD_AGREEMENT": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/esa-documents/agreement"
+    },
     "ESA_FETCH_ELIGIBLE": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/esa/eligible"
     },
     "ESA_FETCH_PURCHASED": {
         "AUTH": true,
@@ -676,29 +711,109 @@
         "URI": "bff/v2/mobile-app/esa/purchased"
     },
     "ESA_OFFLINE_ORDER_COMPLETE": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/esa/payment/offline-purchase-complete"
     },
+    "ESA_V2_CREATE_OFFLINE_ORDER": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/esa/v2/payment/offline-order"
+    },
+    "ESA_V2_FETCH_ELIGIBLE": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/esa/v2/eligible"
+    },
+    "ESA_V2_FETCH_PURCHASED": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/esa/v2/purchased"
+    },
+    "ESA_V2_OFFLINE_ORDER_COMPLETE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/esa/v2/payment/offline-purchase-complete"
+    },
+    "FAPIAO_FETCH_DETAILS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "mobile-app/fapiao/{id}/details"
+    },
+    "FAPIAO_FETCH_HISTORIES": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "mobile-app/fapiao/history"
+    },
+    "FAPIAO_FETCH_MENUS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/fapiao/menus"
+    },
+    "FAPIAO_FETCH_ORDERS": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/fapiao/orders"
+    },
+    "FAPIAO_POST_ORDERS": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/fapiao"
+    },
     "FEATURE_CONFIG": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "api/1/users/feature_config"
     },
+    "FETCH_ENERGY_SITE_SHARED_USERS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "api/1/energy_sites/{site_id}/users"
+    },
+    "FETCH_ENERGY_SITE_SHARE_INVITES": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "api/1/energy_sites/{site_id}/invitations"
+    },
     "FETCH_VEHICLE_SHARED_DRIVERS": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "api/1/vehicles/{vehicle_id}/drivers"
     },
     "FETCH_VEHICLE_SHARE_INVITES": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "api/1/vehicles/{vehicle_id}/invitations"
     },
+    "FINANCING_BUYOUT_APPLY_ESIGN": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/financing/buyout-apply-esign"
+    },
+    "FINANCING_BUYOUT_ELIGIBLE": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/financing/buyout-eligible"
+    },
+    "FINANCING_BUYOUT_ESIGN_STATUS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/financing/buyout-esign-status"
+    },
+    "FINANCING_BUYOUT_NEW_QUOTE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/financing/new-buyout-quote"
+    },
+    "FINANCING_BUYOUT_QUOTE": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/financing/buyout-quote"
+    },
     "FINANCING_CANCEL_APPOINTMENT": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/financing/appointment/cancel"
     },
     "FINANCING_DOWNLOAD_DOCUMENT": {
         "AUTH": true,
@@ -736,18 +851,23 @@
         "URI": "bff/v2/mobile-app/financing/acquisition/file"
     },
     "FINANCING_GET_ACQUISITION_FILE_LIST": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/financing/acquisition/files"
     },
+    "FINANCING_GET_AGREEMENT_DOCS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/financing/agreement-docs"
+    },
     "FINANCING_GET_AMORTIZATION": {
         "AUTH": true,
         "TYPE": "GET",
-        "URI": "bff/v2/mobile-app/financing/amortization-info"
+        "URI": "bff/v2/mobile-app/financing/amortization-info-v2"
     },
     "FINANCING_GET_APPOINTMENT_DETAILS": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/financing/appointment/details"
     },
     "FINANCING_GET_APPOINTMENT_LOCATION": {
@@ -766,14 +886,24 @@
         "URI": "bff/v2/mobile-app/financing/car-details"
     },
     "FINANCING_GET_COMMERCIAL_SIGNED_TOKEN": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/financing/commercial-signed-token"
     },
+    "FINANCING_GET_DELIVERY_LINK": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "mobile-app/financing/delivery-link"
+    },
+    "FINANCING_GET_ELIGIBLE_DELIVERY_LINKS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "mobile-app/financing/eligible-delivery-links"
+    },
     "FINANCING_GET_EXTENSION_QUOTE": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/financing/extension-quote"
     },
     "FINANCING_GET_E_SIGN_DOCUMENT": {
         "AUTH": true,
@@ -876,14 +1006,24 @@
         "URI": "bff/v2/mobile-app/financing/acquisition/file"
     },
     "FINANCING_REQUEST_INSPECTION_APPOINTMENT": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/financing/appointment/inspection-request"
     },
+    "FINANCING_SAVE_DELIVERY_LINK_INTENT": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "mobile-app/financing/delivery-link-intent"
+    },
+    "FINANCING_SAVE_INSPECTION": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/financing/acquisition/save-inspection"
+    },
     "FINANCING_STATUS_UPDATE_ACQUISITION": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/financing/acquisition/status-update"
     },
     "FINANCING_SUBMIT_ACQUISITION": {
         "AUTH": true,
@@ -926,14 +1066,29 @@
         "URI": "bff/v2/mobile-app/financing/esign-validate-details"
     },
     "FLASH_LIGHTS": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/flash_lights"
     },
+    "GET_CHARGE_ON_SOLAR_FEATURE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/vehicles/{vehicle_id}/command/get_charge_on_solar_feature"
+    },
+    "GET_FILE_LIST_BY_METADATA": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/mobile-app/files/product-files/files-by-metadata"
+    },
+    "GET_MANAGED_CHARGING_SITES": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/vehicles/{vehicle_id}/command/get_managed_charging_sites"
+    },
     "GET_MANAGE_DRIVER_FLAG": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/feature-flag/TAO-14025-add-driver-flow"
     },
     "GET_OWNERSHIP_XP_CONFIG": {
         "AUTH": true,
@@ -971,14 +1126,89 @@
         "URI": "api/1/vehicles/{vehicle_id}/command/honk_horn"
     },
     "HVAC_BIOWEAPON_MODE": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/set_bioweapon_mode"
     },
+    "INBOX_GET_FILE": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/mobile-app/files/product-files/{uuid}"
+    },
+    "INBOX_UPLOAD_FILE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/mobile-app/files/product-files"
+    },
+    "INSURANCE_CN_DELETE_SELF_INSURANCE_INFO": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/insurance-cn/self-insurance/delete"
+    },
+    "INSURANCE_CN_DISMISS_EXPIRE_MESSAGE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/insurance-cn/expiry-status-dismiss"
+    },
+    "INSURANCE_CN_GET_CLAIMS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/insurance-cn/claims"
+    },
+    "INSURANCE_CN_GET_CLAIM_PHOTOS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/insurance-cn/claim-photos"
+    },
+    "INSURANCE_CN_GET_CLAIM_SERVICE_INFO": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/insurance-cn/claim-service-info"
+    },
+    "INSURANCE_CN_GET_INSURANCE_STATUS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/insurance-cn/status"
+    },
+    "INSURANCE_CN_GET_INSURER_LIST": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/insurance-cn/insurers"
+    },
+    "INSURANCE_CN_GET_SELF_INSURANCE_INFO": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/insurance-cn/self-insurance/get-insurance"
+    },
+    "INSURANCE_CN_SAVE_CLAIM_GET_PHOTO": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/insurance-cn/claim-photo/{uuid}"
+    },
+    "INSURANCE_CN_SAVE_CLAIM_PHOTOS": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/insurance-cn/claim-photos"
+    },
+    "INSURANCE_CN_SAVE_CLAIM_UPLOAD_PHOTO": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/insurance-cn/upload-claim-photo"
+    },
+    "INSURANCE_CN_SAVE_SELF_INSURANCE_INFO": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/insurance-cn/self-insurance/save"
+    },
+    "INSURANCE_CN_SUBMIT_CLAIMS": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "mobile-app/insurance-cn/report-claim"
+    },
     "LOCK": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/door_lock"
     },
     "LOOTBOX_GET_ONBOARDING_COPY": {
         "AUTH": true,
@@ -1112,14 +1342,19 @@
         "URI": "api/1/messages/count"
     },
     "MESSAGE_CENTER_MESSAGE_LIST": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "api/1/messages"
     },
+    "NAVIGATION_ROUTE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/vehicles/{vehicle_id}/command/get_active_route"
+    },
     "NEARBY_CHARGING_SITES": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "api/1/vehicles/{vehicle_id}/nearby_charging_sites"
     },
     "NON_OWNER_SUPPORTED_PRODUCTS": {
         "AUTH": true,
@@ -1158,14 +1393,29 @@
         "URI": "api/1/energy_sites/{site_id}/operation"
     },
     "OWNERSHIP_RESERVATION_DETAILS_REQUEST": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/ownership/reservation-details/{rn}"
     },
+    "OWNERSHIP_TRANSFER_REQUEST_APPROVE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/mobile-app/transfer/transfer-request-approve"
+    },
+    "OWNERSHIP_TRANSFER_REQUEST_INITIATE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/mobile-app/transfer/transfer-request-initiate"
+    },
+    "OWNERSHIP_TRANSFER_REQUEST_REJECT": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/mobile-app/transfer/transfer-request-reject"
+    },
     "OWNERSHIP_TRANSFER_TOOL_ADD_INITIATE": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/mobile-app/transfer/add-initiate"
     },
     "OWNERSHIP_TRANSFER_TOOL_ADD_PROCESS": {
         "AUTH": true,
@@ -1176,15 +1426,15 @@
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/mobile-app/transfer/assets"
     },
     "OWNERSHIP_TRANSFER_TOOL_REMOVAL_ELIGIBILITY": {
         "AUTH": true,
         "TYPE": "GET",
-        "URI": "bff/mobile-app/transfer/remove-car-eligibility"
+        "URI": "bff/mobile-app/transfer/remove-car-eligibility-v2"
     },
     "OWNERSHIP_TRANSFER_TOOL_REMOVE_INITIATE": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/mobile-app/transfer/remove-car"
     },
     "OWNERSHIP_TRANSFER_TOOL_SECURITY_CODE": {
@@ -1208,24 +1458,34 @@
         "URI": "bff/mobile-app/transfer/user-signed-token"
     },
     "OWNERSHIP_TRANSFER_TOOL_VALIDATE_CAR_NAME": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/mobile-app/transfer/check-name"
     },
+    "OWNERSHIP_TRANSFER_VIEW_REQUEST": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/mobile-app/transfer/view-transfer-request"
+    },
     "OWNERSHIP_TRANSLATIONS": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/static/protected/translations/{path}"
     },
     "OWNERSHIP_VEHICLE_SPECS_REQUEST": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/ownership/vehicle-details"
     },
+    "OWNERSHIP_VERIFY_ID": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "mobile-app/financing/validate-identity-card"
+    },
     "OWNERSHIP_WARRANTY_DETAILS_REQUEST": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/ownership/warranty-details"
     },
     "PAYMENTS_FETCH_CN_ENTITY": {
         "AUTH": true,
@@ -1266,14 +1526,19 @@
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/place_suggestions"
     },
     "PLAN_TRIP": {
         "AUTH": true,
         "TYPE": "POST",
+        "URI": "trip-planner/api/v1/tripplan"
+    },
+    "PLAN_TRIP_CN": {
+        "AUTH": true,
+        "TYPE": "POST",
         "URI": "api/1/vehicles/plan_trip"
     },
     "POWERWALL_ORDER_PAGE": {
         "AUTH": true,
         "CONTENT": "HTML",
         "TYPE": "GET",
         "URI": "powerwall_order_page"
@@ -1289,14 +1554,19 @@
         "URI": "api/1/products"
     },
     "RATE_TARIFFS": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "api/1/energy_sites/rate_tariffs"
     },
+    "REDEEM_ENERGY_SITE_SHARE_INVITE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/invitations/redeem"
+    },
     "REDEEM_VEHICLE_SHARE_INVITE": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/invitations/redeem"
     },
     "REFERRAL_DATA": {
         "AUTH": true,
@@ -1360,14 +1630,19 @@
         "URI": "api/1/vehicles/{vehicle_id}/release_notes"
     },
     "REMOTE_AUTO_SEAT_CLIMATE_REQUEST": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/remote_auto_seat_climate_request"
     },
+    "REMOTE_AUTO_STEERING_WHEEL_HEAT_CLIMATE_REQUEST": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/vehicles/{vehicle_id}/command/remote_auto_steering_wheel_heat_climate_request"
+    },
     "REMOTE_BOOMBOX": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/remote_boombox"
     },
     "REMOTE_SEAT_COOLING_REQUEST": {
         "AUTH": true,
@@ -1385,14 +1660,29 @@
         "URI": "api/1/vehicles/{vehicle_id}/command/remote_start_drive"
     },
     "REMOTE_STEERING_WHEEL_HEATER_REQUEST": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/remote_steering_wheel_heater_request"
     },
+    "REMOTE_STEERING_WHEEL_HEAT_LEVEL_REQUEST": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/vehicles/{vehicle_id}/command/remote_steering_wheel_heat_level_request"
+    },
+    "REMOVE_ENERGY_SITE_SHARE_USER": {
+        "AUTH": true,
+        "TYPE": "DELETE",
+        "URI": "api/1/energy_sites/{site_id}/users/{user_id}"
+    },
+    "REMOVE_MANAGED_CHARGING_SITE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/vehicles/{vehicle_id}/command/remove_managed_charging_site"
+    },
     "REMOVE_VEHICLE_SHARE_DRIVER": {
         "AUTH": true,
         "TYPE": "DELETE",
         "URI": "api/1/vehicles/{vehicle_id}/drivers/{share_user_id}"
     },
     "RESET_VALET_PIN": {
         "AUTH": true,
@@ -1410,14 +1700,19 @@
         "URI": "api/1/subscriptions"
     },
     "REVERSE_GEOCODING": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "maps/reverse_geocoding/v3/"
     },
+    "REVOKE_ENERGY_SITE_SHARE_INVITE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/energy_sites/{site_id}/invitations/{invite_id}/revoke"
+    },
     "REVOKE_VEHICLE_SHARE_INVITE": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/invitations/{invite_id}/revoke"
     },
     "ROADSIDE_ASSISTANCE_DATA": {
         "AUTH": true,
@@ -1441,29 +1736,54 @@
         "URI": "bff/v2/mobile-app/roadside/countries"
     },
     "ROADSIDE_CREATE_INCIDENT": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/roadside/incidents"
     },
+    "ROADSIDE_CREATE_MOBILE_TIRE_VISIT": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "mobile-app/roadside/visit"
+    },
     "ROADSIDE_INCIDENTS": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/roadside/incidents"
     },
     "ROADSIDE_LOCATIONS": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/roadside/locations"
     },
+    "ROADSIDE_MOBILE_TIRE_SLOTS": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/roadside/tire/slots"
+    },
+    "ROADSIDE_STATIC_CONTENT": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/roadside/static-content"
+    },
+    "ROADSIDE_UPDATE_MOBILE_TIRE_VISIT": {
+        "AUTH": true,
+        "TYPE": "PATCH",
+        "URI": "mobile-app/roadside/visit/{serviceVisitID}"
+    },
     "ROADSIDE_WARRANTY": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/roadside/warranty"
     },
+    "ROADSIDE_WARRANTY_QUALIFICATION": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/roadside/warranty/qualify"
+    },
     "SAFETY_RATING_GET_DAILY_BREAKDOWN": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/insurance/daily-breakdown"
     },
     "SAFETY_RATING_GET_ELIGIBLE_FOR_TELEMATICS": {
         "AUTH": true,
@@ -1501,14 +1821,19 @@
         "URI": "bff/mobile-app/security-privacy/assets"
     },
     "SEND_DEVICE_KEY": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/users/keys"
     },
+    "SEND_DOCUMENTS_EMAIL": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "bff/v2/mobile-app/insurance-cn/send-mail"
+    },
     "SEND_GPS_TO_VEHICLE": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/navigation_gps_request"
     },
     "SEND_NOTIFICATION_CONFIRMATION": {
         "AUTH": true,
@@ -1731,14 +2056,24 @@
         "URI": "bff/v2/mobile-app/service/service-appointments"
     },
     "SERVICE_GET_SERVICE_VISITS": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/service/appointments"
     },
+    "SERVICE_GET_SERVICE_VISIT_AMOUNT_DUE": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/v2/mobile-app/service/payment/amount-due/{serviceVisitID}"
+    },
+    "SERVICE_GET_TESLA_INSURANCE_OPEN_CLAIMS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "mobile-app/service/insurance/claims"
+    },
     "SERVICE_HISTORY": {
         "AUTH": true,
         "TYPE": "GET",
         "URI": "bff/v2/mobile-app/service/history"
     },
     "SERVICE_IPOS": {
         "AUTH": true,
@@ -1841,19 +2176,29 @@
         "URI": "mobile-app/service/reschedule-disclaimer"
     },
     "SERVICE_SAVE_CENTER_APPOINTMENT": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/service/center"
     },
+    "SERVICE_SAVE_LOCATION": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "mobile-app/service/appointments/{serviceVisitID}/save-address"
+    },
     "SERVICE_SEND_MESSAGE": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/service/messages/{serviceVisitID}"
     },
+    "SERVICE_STEPS": {
+        "AUTH": true,
+        "TYPE": "GET",
+        "URI": "bff/mobile-app/service/steps/{serviceVisitID}"
+    },
     "SERVICE_SURVEY_ANSWER_QUESTIONS": {
         "AUTH": true,
         "TYPE": "PUT",
         "URI": "bff/v2/mobile-app/service/surveys"
     },
     "SERVICE_SURVEY_ELIGIBILITY": {
         "AUTH": true,
@@ -2121,14 +2466,19 @@
         "URI": "api/1/vehicles/{vehicle_id}/screenshot"
     },
     "UNLOCK": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/door_unlock"
     },
+    "UPDATE_CHARGE_ON_SOLAR_FEATURE": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/vehicles/{vehicle_id}/command/update_charge_on_solar_feature"
+    },
     "UPGRADES_COMPLETE_OFFLINE_ORDER": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "bff/v2/mobile-app/upgrades/payment/offline-purchase-complete/v2"
     },
     "UPGRADES_CREATE_OFFLINE_ORDER": {
         "AUTH": true,
```

### Comparing `TeslaPy-2.7.0/teslapy/option_codes.json` & `TeslaPy-2.8.0/teslapy/option_codes.json`

 * *Files identical despite different names*

