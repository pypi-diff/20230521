# Comparing `tmp/aliot-py-0.5.0.tar.gz` & `tmp/aliot-py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliot-py-0.5.0.tar", last modified: Wed Oct  5 19:46:24 2022, max compression
+gzip compressed data, was "aliot-py-1.0.0.tar", last modified: Sun May 21 20:57:41 2023, max compression
```

## Comparing `aliot-py-0.5.0.tar` & `aliot-py-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-10-05 19:46:24.244568 aliot-py-0.5.0/
--rw-rw-rw-   0        0        0     2858 2022-10-05 19:46:24.243566 aliot-py-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2328 2022-07-04 22:20:06.000000 aliot-py-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-05 19:46:24.100069 aliot-py-0.5.0/aliot/
--rw-rw-rw-   0        0        0      100 2022-10-05 19:44:46.000000 aliot-py-0.5.0/aliot/__init__.py
--rw-rw-rw-   0        0        0    18355 2022-10-05 19:24:06.000000 aliot-py-0.5.0/aliot/aliot_obj.py
--rw-rw-rw-   0        0        0     2784 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/constants.py
-drwxrwxrwx   0        0        0        0 2022-10-05 19:46:24.101570 aliot-py-0.5.0/aliot/core/
--rw-rw-rw-   0        0        0        0 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-05 19:46:24.135566 aliot-py-0.5.0/aliot/core/_cli/
--rw-rw-rw-   0        0        0        0 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/core/_cli/__init__.py
--rw-rw-rw-   0        0        0     4444 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/core/_cli/aliot_cli.py
--rw-rw-rw-   0        0        0     2102 2022-07-05 22:02:17.000000 aliot-py-0.5.0/aliot/core/_cli/cli_service.py
--rw-rw-rw-   0        0        0      970 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/core/_cli/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-05 19:46:24.171069 aliot-py-0.5.0/aliot/core/_config/
--rw-rw-rw-   0        0        0        0 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/core/_config/__init__.py
--rw-rw-rw-   0        0        0     1804 2022-10-05 18:50:18.000000 aliot-py-0.5.0/aliot/core/_config/config.py
--rw-rw-rw-   0        0        0      530 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/core/_config/constants.py
--rw-rw-rw-   0        0        0     2215 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/core/_config/templates.py
--rw-rw-rw-   0        0        0      386 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/decoder.py
--rw-rw-rw-   0        0        0      377 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/encoder.py
-drwxrwxrwx   0        0        0        0 2022-10-05 19:46:24.183069 aliot-py-0.5.0/aliot/exceptions/
--rw-rw-rw-   0        0        0        0 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/exceptions/__init__.py
--rw-rw-rw-   0        0        0      309 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/exceptions/should_not_call_error.py
--rw-rw-rw-   0        0        0      872 2022-07-04 22:20:06.000000 aliot-py-0.5.0/aliot/state.py
-drwxrwxrwx   0        0        0        0 2022-10-05 19:46:24.219569 aliot-py-0.5.0/aliot_py.egg-info/
--rw-rw-rw-   0        0        0     2858 2022-10-05 19:46:23.000000 aliot-py-0.5.0/aliot_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      680 2022-10-05 19:46:23.000000 aliot-py-0.5.0/aliot_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-05 19:46:23.000000 aliot-py-0.5.0/aliot_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2022-10-05 19:46:23.000000 aliot-py-0.5.0/aliot_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       86 2022-10-05 19:46:23.000000 aliot-py-0.5.0/aliot_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-10-05 19:46:23.000000 aliot-py-0.5.0/aliot_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-05 19:46:24.245070 aliot-py-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1547 2022-07-05 21:53:31.000000 aliot-py-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-05 19:46:24.241066 aliot-py-0.5.0/test/
--rw-rw-rw-   0        0        0      576 2022-07-05 22:02:54.000000 aliot-py-0.5.0/test/test.py
--rw-rw-rw-   0        0        0      186 2022-07-05 22:02:54.000000 aliot-py-0.5.0/test/test_state.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:57:41.293867 aliot-py-1.0.0/
+-rw-rw-rw-   0        0        0     2899 2023-05-21 20:57:41.286676 aliot-py-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2328 2022-10-07 01:57:50.000000 aliot-py-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 20:57:41.237261 aliot-py-1.0.0/aliot/
+-rw-rw-rw-   0        0        0      100 2023-05-21 20:55:08.000000 aliot-py-1.0.0/aliot/__init__.py
+-rw-rw-rw-   0        0        0    18353 2023-05-21 20:50:20.000000 aliot-py-1.0.0/aliot/aliot_obj.py
+-rw-rw-rw-   0        0        0     2784 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:57:41.239515 aliot-py-1.0.0/aliot/core/
+-rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:57:41.251309 aliot-py-1.0.0/aliot/core/_cli/
+-rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/core/_cli/__init__.py
+-rw-rw-rw-   0        0        0     4442 2023-05-21 19:59:44.000000 aliot-py-1.0.0/aliot/core/_cli/aliot_cli.py
+-rw-rw-rw-   0        0        0     2102 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/core/_cli/cli_service.py
+-rw-rw-rw-   0        0        0      970 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/core/_cli/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:57:41.257477 aliot-py-1.0.0/aliot/core/_config/
+-rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/core/_config/__init__.py
+-rw-rw-rw-   0        0        0     1834 2023-05-21 19:57:00.000000 aliot-py-1.0.0/aliot/core/_config/config.py
+-rw-rw-rw-   0        0        0      530 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/core/_config/constants.py
+-rw-rw-rw-   0        0        0     2215 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/core/_config/templates.py
+-rw-rw-rw-   0        0        0      386 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/decoder.py
+-rw-rw-rw-   0        0        0      377 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:57:41.262585 aliot-py-1.0.0/aliot/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      309 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/exceptions/should_not_call_error.py
+-rw-rw-rw-   0        0        0      872 2022-10-07 01:57:50.000000 aliot-py-1.0.0/aliot/state.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:57:41.286676 aliot-py-1.0.0/aliot_py.egg-info/
+-rw-rw-rw-   0        0        0     2899 2023-05-21 20:57:40.000000 aliot-py-1.0.0/aliot_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      680 2023-05-21 20:57:41.000000 aliot-py-1.0.0/aliot_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 20:57:40.000000 aliot-py-1.0.0/aliot_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-21 20:57:40.000000 aliot-py-1.0.0/aliot_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       86 2023-05-21 20:57:40.000000 aliot-py-1.0.0/aliot_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-21 20:57:41.000000 aliot-py-1.0.0/aliot_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 20:57:41.294378 aliot-py-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2022-10-07 01:57:50.000000 aliot-py-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:57:41.286676 aliot-py-1.0.0/test/
+-rw-rw-rw-   0        0        0      576 2022-10-07 01:57:50.000000 aliot-py-1.0.0/test/test.py
+-rw-rw-rw-   0        0        0      186 2022-10-07 01:57:50.000000 aliot-py-1.0.0/test/test_state.py
```

### Comparing `aliot-py-0.5.0/PKG-INFO` & `aliot-py-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: aliot-py
-Version: 0.5.0
+Version: 1.0.0
 Summary: Aliot-py is the python implementation of the Aliot library, an IOT library made to work with the ALIVEIoT ecosystem (see https://alivecode.ca/iot)
 Home-page: https://github.com/ALIVEcode/aliot/tree/aliot2
 Author: Mathis Laroche, Enric Soldevila
 Author-email: alivecode.developers@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ### ALIOT-PY: The python implementation of the Aliot library!
 
@@ -79,7 +81,9 @@
     3. controller.handle_event(event: AliotEvent) -> None
     4. decoder.decode_data<T>(data: dict) -> T
 * On send:
     1. encoder.encode_data(data: Any) -> dict
     2. encode.encode_event()
     3. obj.__send_event() -> None
 
+
+
```

### Comparing `aliot-py-0.5.0/README.md` & `aliot-py-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aliot-py-0.5.0/aliot/aliot_obj.py` & `aliot-py-1.0.0/aliot/aliot_obj.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 import warnings
 from functools import wraps
 from threading import Thread
 from typing import TYPE_CHECKING
+from time import ctime, sleep
 
 import requests
 
 from aliot.exceptions.should_not_call_error import ShouldNotCallError
 
 if TYPE_CHECKING:
     from encoder import Encoder
@@ -392,20 +393,15 @@
             print("the message received does not have a valid structure")
             return
 
         msg_id = msg["id"]
         protocol = self.protocols.get(msg_id)
 
         if protocol is None:
-            if self.connected_to_alivecode:
-                self.connected_to_alivecode = False
             print_err(f"The protocol with the id {msg_id!r} is not implemented")
-
-            # magic of python
-            print_info("Connection CLOSED")
         else:
             protocol(msg["value"])
 
     def __connect_success(self):
         if len(self.__listeners) == 0:
             print_success(f"Object {self.name!r}", success_name="Connected")
             self.connected_to_alivecode = True
@@ -474,14 +470,18 @@
 
     def __on_close(self, ws: WebSocketApp, *_):
         self.__connected = False
         self.__connected_to_alivecode = False
         print_info(info_name="Connection closed")
         self.__on_end and self.__on_end[0](*self.__on_end[1], **self.__on_end[2])
 
+        print ("Retrying connection in 5 seconds. Current time : %s" % ctime())
+        sleep(5)
+        self.run() # retry per 5 seconds
+
     def __on_open(self, ws):
         # Register IoTObject on ALIVEcode
         self.__connected = True
         token = self.auth_token
         if token is None:
             self.__handle_error(
                 "IoTObjects now require an AuthToken to securely connect to ALIVEiot. Please make sure to register an AuthToken on your IoTObject on ALIVEcode from your IoT Dashboard and add in your config.ini: auth_token = <your_auth_token>",
```

### Comparing `aliot-py-0.5.0/aliot/constants.py` & `aliot-py-1.0.0/aliot/constants.py`

 * *Files identical despite different names*

### Comparing `aliot-py-0.5.0/aliot/core/_cli/aliot_cli.py` & `aliot-py-1.0.0/aliot/core/_cli/aliot_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 @main.command()
 @click.argument("object-name")
 @click.option("--obj-id", default=None)
 @click.option("--main", default=None)
 @click.option("-t", "--template", type=click.Choice(["blank", "minimal", "normal", "complete"], case_sensitive=False),
-              default="complete", prompt="Choose a template")
+              default="normal", prompt="Choose a template")
 def new(object_name: str, obj_id: str, main: str, template: str):
     fields_to_overwrite = {}
     if obj_id is not None:
         fields_to_overwrite["obj_id"] = obj_id
     if main is not None:
         fields_to_overwrite["main"] = main
     success = print_result(
```

### Comparing `aliot-py-0.5.0/aliot/core/_cli/cli_service.py` & `aliot-py-1.0.0/aliot/core/_cli/cli_service.py`

 * *Files identical despite different names*

### Comparing `aliot-py-0.5.0/aliot/core/_cli/utils.py` & `aliot-py-1.0.0/aliot/core/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `aliot-py-0.5.0/aliot/core/_config/config.py` & `aliot-py-1.0.0/aliot/core/_config/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,16 +41,16 @@
             raise IOError(f"Cannot read {config_file_path}")
         __updated = False
     return __config
 
 
 def make_config_section(obj_name: str):
     return {
-        "obj_id": f"Paste the id of {obj_name} here :)",
-        "auth_token": f"Paste the auth_token of {obj_name} here :)",
+        "obj_id": f"Paste the id of {obj_name} from ALIVEcode here :)",
+        "auth_token": f"Paste the auth_token of {obj_name} from ALIVEcode here :)",
         "main": f"{obj_name}.py"
     }
 
 
 def get_default_code(obj_name: str) -> str:
     variable = obj_name.replace('-', '_')
```

### Comparing `aliot-py-0.5.0/aliot/core/_config/constants.py` & `aliot-py-1.0.0/aliot/core/_config/constants.py`

 * *Files identical despite different names*

### Comparing `aliot-py-0.5.0/aliot/core/_config/templates.py` & `aliot-py-1.0.0/aliot/core/_config/templates.py`

 * *Files identical despite different names*

### Comparing `aliot-py-0.5.0/aliot/state.py` & `aliot-py-1.0.0/aliot/state.py`

 * *Files identical despite different names*

### Comparing `aliot-py-0.5.0/aliot_py.egg-info/PKG-INFO` & `aliot-py-1.0.0/aliot_py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: aliot-py
-Version: 0.5.0
+Version: 1.0.0
 Summary: Aliot-py is the python implementation of the Aliot library, an IOT library made to work with the ALIVEIoT ecosystem (see https://alivecode.ca/iot)
 Home-page: https://github.com/ALIVEcode/aliot/tree/aliot2
 Author: Mathis Laroche, Enric Soldevila
 Author-email: alivecode.developers@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ### ALIOT-PY: The python implementation of the Aliot library!
 
@@ -79,7 +81,9 @@
     3. controller.handle_event(event: AliotEvent) -> None
     4. decoder.decode_data<T>(data: dict) -> T
 * On send:
     1. encoder.encode_data(data: Any) -> dict
     2. encode.encode_event()
     3. obj.__send_event() -> None
 
+
+
```

### Comparing `aliot-py-0.5.0/aliot_py.egg-info/SOURCES.txt` & `aliot-py-1.0.0/aliot_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliot-py-0.5.0/setup.py` & `aliot-py-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `aliot-py-0.5.0/test/test.py` & `aliot-py-1.0.0/test/test.py`

 * *Files identical despite different names*

