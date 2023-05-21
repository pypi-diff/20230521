# Comparing `tmp/python-mystrom-2.1.0.tar.gz` & `tmp/python-mystrom-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mystrom-2.1.0.tar", last modified: Sat Nov 26 08:15:20 2022, max compression
+gzip compressed data, was "python-mystrom-2.2.0.tar", last modified: Sun May 21 18:49:56 2023, max compression
```

## Comparing `python-mystrom-2.1.0.tar` & `python-mystrom-2.2.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxr-x   0 fab       (1000) fab       (1000)        0 2022-11-26 08:15:20.934958 python-mystrom-2.1.0/
--rw-rw-r--   0 fab       (1000) fab       (1000)     1011 2022-11-26 08:06:41.000000 python-mystrom-2.1.0/CHANGELOG.rst
--rw-rw-r--   0 fab       (1000) fab       (1000)     1120 2022-11-26 08:06:41.000000 python-mystrom-2.1.0/LICENSE
--rw-r--r--   0 fab       (1000) fab       (1000)       45 2020-11-09 19:08:18.000000 python-mystrom-2.1.0/MANIFEST.in
--rw-rw-r--   0 fab       (1000) fab       (1000)     8163 2022-11-26 08:15:20.934958 python-mystrom-2.1.0/PKG-INFO
--rw-rw-r--   0 fab       (1000) fab       (1000)     7384 2022-09-25 20:34:46.000000 python-mystrom-2.1.0/README.rst
-drwxrwxr-x   0 fab       (1000) fab       (1000)        0 2022-11-26 08:15:20.933958 python-mystrom-2.1.0/examples/
--rw-rw-r--   0 fab       (1000) fab       (1000)      411 2022-09-25 20:47:23.000000 python-mystrom-2.1.0/examples/example-bulb-hsv.py
--rw-rw-r--   0 fab       (1000) fab       (1000)     2253 2022-09-25 20:34:36.000000 python-mystrom-2.1.0/examples/example-bulb.py
--rw-r--r--   0 fab       (1000) fab       (1000)      382 2021-08-31 12:11:15.000000 python-mystrom-2.1.0/examples/example-discovery.py
--rw-r--r--   0 fab       (1000) fab       (1000)      454 2022-09-25 20:47:33.000000 python-mystrom-2.1.0/examples/example-get-data-bulb.py
--rw-rw-r--   0 fab       (1000) fab       (1000)     1165 2020-11-10 16:06:57.000000 python-mystrom-2.1.0/examples/example-pir.py
--rw-rw-r--   0 fab       (1000) fab       (1000)     1025 2022-11-26 08:01:47.000000 python-mystrom-2.1.0/examples/example-switch.py
-drwxrwxr-x   0 fab       (1000) fab       (1000)        0 2022-11-26 08:15:20.933958 python-mystrom-2.1.0/pymystrom/
--rw-rw-r--   0 fab       (1000) fab       (1000)     1790 2022-09-25 20:47:47.000000 python-mystrom-2.1.0/pymystrom/__init__.py
--rw-rw-r--   0 fab       (1000) fab       (1000)     5783 2022-11-26 08:06:41.000000 python-mystrom-2.1.0/pymystrom/bulb.py
--rw-rw-r--   0 fab       (1000) fab       (1000)     8719 2022-11-26 08:06:41.000000 python-mystrom-2.1.0/pymystrom/cli.py
--rw-rw-r--   0 fab       (1000) fab       (1000)     3515 2022-11-26 08:06:41.000000 python-mystrom-2.1.0/pymystrom/discovery.py
--rw-rw-r--   0 fab       (1000) fab       (1000)      366 2020-08-15 11:57:45.000000 python-mystrom-2.1.0/pymystrom/exceptions.py
--rw-rw-r--   0 fab       (1000) fab       (1000)     5395 2022-11-26 08:06:41.000000 python-mystrom-2.1.0/pymystrom/pir.py
--rw-rw-r--   0 fab       (1000) fab       (1000)     3518 2022-11-26 08:06:41.000000 python-mystrom-2.1.0/pymystrom/switch.py
-drwxrwxr-x   0 fab       (1000) fab       (1000)        0 2022-11-26 08:15:20.934958 python-mystrom-2.1.0/python_mystrom.egg-info/
--rw-rw-r--   0 fab       (1000) fab       (1000)     8163 2022-11-26 08:15:20.000000 python-mystrom-2.1.0/python_mystrom.egg-info/PKG-INFO
--rw-rw-r--   0 fab       (1000) fab       (1000)      626 2022-11-26 08:15:20.000000 python-mystrom-2.1.0/python_mystrom.egg-info/SOURCES.txt
--rw-rw-r--   0 fab       (1000) fab       (1000)        1 2022-11-26 08:15:20.000000 python-mystrom-2.1.0/python_mystrom.egg-info/dependency_links.txt
--rw-rw-r--   0 fab       (1000) fab       (1000)       47 2022-11-26 08:15:20.000000 python-mystrom-2.1.0/python_mystrom.egg-info/entry_points.txt
--rw-rw-r--   0 fab       (1000) fab       (1000)       34 2022-11-26 08:15:20.000000 python-mystrom-2.1.0/python_mystrom.egg-info/requires.txt
--rw-rw-r--   0 fab       (1000) fab       (1000)       10 2022-11-26 08:15:20.000000 python-mystrom-2.1.0/python_mystrom.egg-info/top_level.txt
--rw-rw-r--   0 fab       (1000) fab       (1000)        1 2020-08-15 11:57:46.000000 python-mystrom-2.1.0/python_mystrom.egg-info/zip-safe
--rw-rw-r--   0 fab       (1000) fab       (1000)       38 2022-11-26 08:15:20.934958 python-mystrom-2.1.0/setup.cfg
--rw-rw-r--   0 fab       (1000) fab       (1000)     1389 2022-11-26 08:06:41.000000 python-mystrom-2.1.0/setup.py
+drwxr-xr-x   0 fab       (1000) users      (100)        0 2023-05-21 18:49:56.297261 python-mystrom-2.2.0/
+-rw-r--r--   0 fab       (1000) users      (100)     1120 2023-05-21 18:41:23.000000 python-mystrom-2.2.0/LICENSE
+-rw-r--r--   0 fab       (1000) users      (100)       45 2023-03-29 14:29:35.000000 python-mystrom-2.2.0/MANIFEST.in
+-rw-r--r--   0 fab       (1000) users      (100)     8162 2023-05-21 18:49:56.297261 python-mystrom-2.2.0/PKG-INFO
+-rw-r--r--   0 fab       (1000) users      (100)     7383 2023-03-29 16:31:13.000000 python-mystrom-2.2.0/README.rst
+drwxr-xr-x   0 fab       (1000) users      (100)        0 2023-05-21 18:49:56.294261 python-mystrom-2.2.0/examples/
+-rw-r--r--   0 fab       (1000) users      (100)      411 2023-03-29 14:29:35.000000 python-mystrom-2.2.0/examples/example-bulb-hsv.py
+-rw-r--r--   0 fab       (1000) users      (100)     2253 2023-03-29 14:29:35.000000 python-mystrom-2.2.0/examples/example-bulb.py
+-rw-r--r--   0 fab       (1000) users      (100)      382 2021-08-31 12:11:15.000000 python-mystrom-2.2.0/examples/example-discovery.py
+-rw-r--r--   0 fab       (1000) users      (100)      454 2023-03-29 14:29:35.000000 python-mystrom-2.2.0/examples/example-get-data-bulb.py
+-rw-r--r--   0 fab       (1000) users      (100)     1164 2023-05-21 18:41:23.000000 python-mystrom-2.2.0/examples/example-pir.py
+-rw-r--r--   0 fab       (1000) users      (100)     1024 2023-05-21 18:41:23.000000 python-mystrom-2.2.0/examples/example-switch.py
+drwxr-xr-x   0 fab       (1000) users      (100)        0 2023-05-21 18:49:56.295261 python-mystrom-2.2.0/pymystrom/
+-rw-r--r--   0 fab       (1000) users      (100)     3174 2023-05-21 18:43:32.000000 python-mystrom-2.2.0/pymystrom/__init__.py
+-rw-r--r--   0 fab       (1000) users      (100)     5759 2023-05-21 18:41:23.000000 python-mystrom-2.2.0/pymystrom/bulb.py
+-rw-r--r--   0 fab       (1000) users      (100)     8639 2023-05-21 18:41:23.000000 python-mystrom-2.2.0/pymystrom/cli.py
+-rw-r--r--   0 fab       (1000) users      (100)     3729 2023-05-21 18:41:23.000000 python-mystrom-2.2.0/pymystrom/discovery.py
+-rw-r--r--   0 fab       (1000) users      (100)      366 2023-03-29 14:29:35.000000 python-mystrom-2.2.0/pymystrom/exceptions.py
+-rw-r--r--   0 fab       (1000) users      (100)     5381 2023-05-21 18:41:23.000000 python-mystrom-2.2.0/pymystrom/pir.py
+-rw-r--r--   0 fab       (1000) users      (100)     4112 2023-03-29 16:31:13.000000 python-mystrom-2.2.0/pymystrom/switch.py
+drwxr-xr-x   0 fab       (1000) users      (100)        0 2023-05-21 18:49:56.296261 python-mystrom-2.2.0/python_mystrom.egg-info/
+-rw-rw-r--   0 fab       (1000) users      (100)     8162 2023-05-21 18:49:56.000000 python-mystrom-2.2.0/python_mystrom.egg-info/PKG-INFO
+-rw-rw-r--   0 fab       (1000) users      (100)      612 2023-05-21 18:49:56.000000 python-mystrom-2.2.0/python_mystrom.egg-info/SOURCES.txt
+-rw-rw-r--   0 fab       (1000) users      (100)        1 2023-05-21 18:49:56.000000 python-mystrom-2.2.0/python_mystrom.egg-info/dependency_links.txt
+-rw-rw-r--   0 fab       (1000) users      (100)       47 2023-05-21 18:49:56.000000 python-mystrom-2.2.0/python_mystrom.egg-info/entry_points.txt
+-rw-rw-r--   0 fab       (1000) users      (100)       34 2023-05-21 18:49:56.000000 python-mystrom-2.2.0/python_mystrom.egg-info/requires.txt
+-rw-rw-r--   0 fab       (1000) users      (100)       10 2023-05-21 18:49:56.000000 python-mystrom-2.2.0/python_mystrom.egg-info/top_level.txt
+-rw-rw-r--   0 fab       (1000) users      (100)        1 2020-08-15 11:57:46.000000 python-mystrom-2.2.0/python_mystrom.egg-info/zip-safe
+-rw-r--r--   0 fab       (1000) users      (100)       38 2023-05-21 18:49:56.297261 python-mystrom-2.2.0/setup.cfg
+-rw-r--r--   0 fab       (1000) users      (100)     1389 2023-05-21 18:46:24.000000 python-mystrom-2.2.0/setup.py
```

### Comparing `python-mystrom-2.1.0/LICENSE` & `python-mystrom-2.2.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2015-2022 Fabian Affolter <fabian@affolter-engineering.ch>
+Copyright (c) 2015-2023 Fabian Affolter <fabian@affolter-engineering.ch>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `python-mystrom-2.1.0/PKG-INFO` & `python-mystrom-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mystrom
-Version: 2.1.0
+Version: 2.2.0
 Summary: Asynchronous Python API client for interacting with myStrom devices
 Home-page: https://github.com/home-assistant-ecosystem/python-mystrom
 Author: Fabian Affolter
 Author-email: fabian@affolter-engineering.ch
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -59,15 +59,15 @@
     $ sudo dnf -y install python3-mystrom
 
 For Nix or NixOS users is a package available. Keep in mind that the lastest releases might only
 be present in the ``unstable`` channel.
 
 .. code:: bash
 
-    $ nix-env -iA nixos.python39Packages.python-mystrom
+    $ nix-env -iA nixos.python3Packages.python-mystrom
 
 
 Plug/switch
 -----------
 
 At the moment the following endpoints are covered according `https://api.mystrom.ch <https://api.mystrom.ch>`_:
```

### Comparing `python-mystrom-2.1.0/README.rst` & `python-mystrom-2.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     $ sudo dnf -y install python3-mystrom
 
 For Nix or NixOS users is a package available. Keep in mind that the lastest releases might only
 be present in the ``unstable`` channel.
 
 .. code:: bash
 
-    $ nix-env -iA nixos.python39Packages.python-mystrom
+    $ nix-env -iA nixos.python3Packages.python-mystrom
 
 
 Plug/switch
 -----------
 
 At the moment the following endpoints are covered according `https://api.mystrom.ch <https://api.mystrom.ch>`_:
```

### Comparing `python-mystrom-2.1.0/examples/example-bulb.py` & `python-mystrom-2.2.0/examples/example-bulb.py`

 * *Files identical despite different names*

### Comparing `python-mystrom-2.1.0/examples/example-pir.py` & `python-mystrom-2.2.0/examples/example-pir.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 IP_ADDRESS = "192.168.1.225"
 
 
 async def main():
     """Sample code to work with a myStrom PIR."""
     async with MyStromPir(IP_ADDRESS) as pir:
-
         # Get the PIR settings
         await pir.get_settings()
         print("Settings:", pir.settings)
 
         # Get the PIR settings
         await pir.get_pir()
         print("PIR settings:", pir.pir)
```

### Comparing `python-mystrom-2.1.0/examples/example-switch.py` & `python-mystrom-2.2.0/examples/example-switch.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 IP_ADDRESS = "192.168.0.40"
 
 
 async def main():
     """Sample code to work with a myStrom switch."""
     async with MyStromSwitch(IP_ADDRESS) as switch:
-
         # Collect the data of the current state
         await switch.get_state()
 
         print("Power consumption:", switch.consumption)
         print("Energy consumed:", switch.consumedWs)
         print("Relay state:", switch.relay)
         print("Temperature:", switch.temperature)
```

### Comparing `python-mystrom-2.1.0/pymystrom/bulb.py` & `python-mystrom-2.2.0/pymystrom/bulb.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,15 @@
         self._consumption = 0
         self.data = None
         self._firmware = None
         self._mode = None
         self._bulb_type = None
         self._state = None
         self._transition_time = 0
-        self.uri = (
-            URL.build(scheme="http", host=self._host).join(URI_BULB) / self._mac
-        )
+        self.uri = URL.build(scheme="http", host=self._host).join(URI_BULB) / self._mac
 
     async def get_state(self) -> object:
         """Get the state of the bulb."""
         response = await request(self, uri=self.uri)
         self._consumption = response[self._mac]["power"]
         self._firmware = response[self._mac]["fw_version"]
         self._color = response[self._mac]["color"]
```

### Comparing `python-mystrom-2.1.0/pymystrom/cli.py` & `python-mystrom-2.2.0/pymystrom/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,15 @@
     prompt="MAC address of the device",
     help="MAC address of the device.",
 )
 def read_config(ip, mac):
     """Read the current configuration of a myStrom device."""
     click.echo("Read configuration from %s" % ip)
     try:
-        request = requests.get(
-            "http://{}/{}/{}/".format(ip, URI, mac), timeout=TIMEOUT
-        )
+        request = requests.get("http://{}/{}/{}/".format(ip, URI, mac), timeout=TIMEOUT)
         click.echo(request.json())
     except requests.exceptions.ConnectionError:
         click.echo("Communication issue with the device")
 
 
 @main.group("button")
 def button():
@@ -83,17 +81,15 @@
     prompt="URL for a double tap",
     default="",
     help="URL for a double tap.",
 )
 @click.option(
     "--long", prompt="URL for a long tab", default="", help="URL for a long tab."
 )
-@click.option(
-    "--touch", prompt="URL for a touch", default="", help="URL for a touch."
-)
+@click.option("--touch", prompt="URL for a touch", default="", help="URL for a touch.")
 def write_config(ip, mac, single, double, long, touch):
     """Write the current configuration of a myStrom button."""
     click.echo("Write configuration to device %s" % ip)
     data = {
         "single": single,
         "double": double,
         "long": long,
@@ -204,46 +200,40 @@
     prompt="MAC address of the button",
     help="MAC address of the Wifi Button.",
 )
 def read_config(ip, mac):
     """Read the current configuration of a myStrom WiFi Button."""
     click.echo("Read the configuration of button %s..." % ip)
     try:
-        request = requests.get(
-            "http://{}/{}/{}/".format(ip, URI, mac), timeout=TIMEOUT
-        )
+        request = requests.get("http://{}/{}/{}/".format(ip, URI, mac), timeout=TIMEOUT)
         click.echo(request.json())
     except requests.exceptions.ConnectionError:
         click.echo("Communication issue with the device. No action performed")
 
 
 @main.group("bulb")
 def bulb():
     """Get and set details of a myStrom bulb."""
 
 
 @bulb.command("on")
 @coro
-@click.option(
-    "--ip", prompt="IP address of the bulb", help="IP address of the bulb."
-)
+@click.option("--ip", prompt="IP address of the bulb", help="IP address of the bulb.")
 @click.option(
     "--mac", prompt="MAC address of the bulb", help="MAC address of the bulb."
 )
 async def on(ip, mac):
     """Switch the bulb on."""
     async with MyStromBulb(ip, mac) as bulb:
         await bulb.set_color_hex("00FFFFFF")
 
 
 @bulb.command("color")
 @coro
-@click.option(
-    "--ip", prompt="IP address of the bulb", help="IP address of the bulb."
-)
+@click.option("--ip", prompt="IP address of the bulb", help="IP address of the bulb.")
 @click.option(
     "--mac", prompt="MAC address of the bulb", help="MAC address of the bulb."
 )
 @click.option(
     "--hue", prompt="Set the hue of the bulb", help="Set the hue of the bulb."
 )
 @click.option(
@@ -260,31 +250,27 @@
     """Switch the bulb on with the given color."""
     async with MyStromBulb(ip, mac) as bulb:
         await bulb.set_color_hsv(hue, saturation, value)
 
 
 @bulb.command("off")
 @coro
-@click.option(
-    "--ip", prompt="IP address of the bulb", help="IP address of the bulb."
-)
+@click.option("--ip", prompt="IP address of the bulb", help="IP address of the bulb.")
 @click.option(
     "--mac", prompt="MAC address of the bulb", help="MAC address of the bulb."
 )
 async def off(ip, mac):
     """Switch the bulb off."""
     async with MyStromBulb(ip, mac) as bulb:
         await bulb.set_off()
 
 
 @bulb.command("flash")
 @coro
-@click.option(
-    "--ip", prompt="IP address of the bulb", help="IP address of the bulb."
-)
+@click.option("--ip", prompt="IP address of the bulb", help="IP address of the bulb.")
 @click.option(
     "--mac", prompt="MAC address of the bulb", help="MAC address of the bulb."
 )
 @click.option(
     "--time",
     prompt="Time to flash",
     help="Time to flash the bulb in seconds.",
@@ -294,17 +280,15 @@
     """Flash the bulb off."""
     async with MyStromBulb(ip, mac) as bulb:
         await bulb.set_flashing(time, [100, 50, 30], [200, 0, 71])
 
 
 @bulb.command("rainbow")
 @coro
-@click.option(
-    "--ip", prompt="IP address of the bulb", help="IP address of the bulb."
-)
+@click.option("--ip", prompt="IP address of the bulb", help="IP address of the bulb.")
 @click.option(
     "--mac", prompt="MAC address of the bulb", help="MAC address of the bulb."
 )
 @click.option(
     "--time",
     prompt="Time for the complete rainbow",
     help="Time to perform the rainbow in seconds.",
```

### Comparing `python-mystrom-2.1.0/pymystrom/discovery.py` & `python-mystrom-2.2.0/pymystrom/discovery.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 import asyncio
 import logging
 from typing import Optional, List
 
 _LOGGER = logging.getLogger(__name__)
 
 DEVICE_MAPPING = {
+    "101": "myStrom Switch v1",
     "102": "myStrom Bulb",
+    "103": "myStrom Button+",
+    "104": "myStrom Button",
+    "105": "myStrom LED strip",
+    "106": "myStzrom Switch v2",
+    "107": "myStrom Switch EU",
+    "110": "myStrom Motion sensor",
+    "120": "myStrom Switch Zero",
 }
 
 
 class DiscoveredDevice(object):
     """Representation of discovered device."""
 
     mac: str
@@ -19,23 +27,19 @@
     mystrom_registered: bool
     mystrom_online: bool
     restarted: bool
 
     @staticmethod
     def create_from_announce_msg(raw_addr, announce_msg):
         """Create announce message."""
-        _LOGGER.debug(
-            "Received announce message '%s' from %s ", announce_msg, raw_addr
-        )
+        _LOGGER.debug("Received announce message '%s' from %s ", announce_msg, raw_addr)
         if len(announce_msg) != 8:
             raise RuntimeError("Unexpected announcement, '%s'" % announce_msg)
 
-        device = DiscoveredDevice(
-            host=raw_addr[0], mac=announce_msg[0:6].hex(":")
-        )
+        device = DiscoveredDevice(host=raw_addr[0], mac=announce_msg[0:6].hex(":"))
         device.type = announce_msg[6]
 
         if device.type == "102":
             device.hardware = DEVICE_MAPPING[str(announce_msg[6])]
         else:
             device.hardware = "non_mystrom"
         status = announce_msg[7]
```

### Comparing `python-mystrom-2.1.0/pymystrom/pir.py` & `python-mystrom-2.2.0/pymystrom/pir.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 URI_PIR = URL("api/v1/")
 
 
 class MyStromPir:
     """A class for a myStrom PIR."""
 
-    def __init__(
-        self, host: str, session: aiohttp.client.ClientSession = None
-    ) -> None:
+    def __init__(self, host: str, session: aiohttp.client.ClientSession = None) -> None:
         """Initialize the switch."""
         self._close_session = False
         self._host = host
         self._session = session
         self._intensity = None
         self._day = None
         self._light_raw = None
```

### Comparing `python-mystrom-2.1.0/pymystrom/switch.py` & `python-mystrom-2.2.0/pymystrom/switch.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 from . import _request as request
 
 
 class MyStromSwitch:
     """A class for a myStrom switch/plug."""
 
-    def __init__(
-        self, host: str, session: aiohttp.client.ClientSession = None
-    ) -> None:
+    def __init__(self, host: str, session: aiohttp.client.ClientSession = None) -> None:
         """Initialize the switch."""
         self._close_session = False
         self._host = host
         self._session = session
         self._consumption = 0
         self._consumedWs = 0
         self._state = None
@@ -44,41 +42,59 @@
         await request(self, uri=url)
         await self.get_state()
 
     async def get_state(self) -> None:
         """Get the details from the switch/plug."""
         url = URL(self.uri).join(URL("report"))
         response = await request(self, uri=url)
-        self._consumption = response["power"]
-        self._consumedWs = response["Ws"]
+        try:
+            self._consumption = response["power"]
+        except KeyError:
+            self._consumption = None
+        try:
+            self._consumedWs = response["Ws"]
+        except KeyError:
+            self._consumedWs = None
         self._state = response["relay"]
         try:
             self._temperature = response["temperature"]
         except KeyError:
             self._temperature = None
 
-        url = URL(self.uri).join(URL("info.json"))
+        # Try the new API (Devices with newer firmware)
+        url = URL(self.uri).join(URL("api/v1/info"))
         response = await request(self, uri=url)
+        if not isinstance(response, dict):
+            # Fall back to the old API version if the device runs with old firmware
+            url = URL(self.uri).join(URL("info.json"))
+            response = await request(self, uri=url)
+
         self._firmware = response["version"]
         self._mac = response["mac"]
 
     @property
     def relay(self) -> bool:
         """Return the relay state."""
         return bool(self._state)
 
     @property
     def consumption(self) -> float:
         """Return the current power consumption in mWh."""
-        return round(self._consumption, 1)
+        if self._consumption is not None:
+            return round(self._consumption, 1)
+
+        return self._consumption
 
     @property
     def consumedWs(self) -> float:
         """The average of energy consumed per second since last report call."""
-        return round(self._consumedWs, 1)
+        if self._consumedWs is not None:
+            return round(self._consumedWs, 1)
+
+        return self._consumedWs
 
     @property
     def firmware(self) -> float:
         """Return the current firmware."""
         return self._firmware
 
     @property
```

### Comparing `python-mystrom-2.1.0/python_mystrom.egg-info/PKG-INFO` & `python-mystrom-2.2.0/python_mystrom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mystrom
-Version: 2.1.0
+Version: 2.2.0
 Summary: Asynchronous Python API client for interacting with myStrom devices
 Home-page: https://github.com/home-assistant-ecosystem/python-mystrom
 Author: Fabian Affolter
 Author-email: fabian@affolter-engineering.ch
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -59,15 +59,15 @@
     $ sudo dnf -y install python3-mystrom
 
 For Nix or NixOS users is a package available. Keep in mind that the lastest releases might only
 be present in the ``unstable`` channel.
 
 .. code:: bash
 
-    $ nix-env -iA nixos.python39Packages.python-mystrom
+    $ nix-env -iA nixos.python3Packages.python-mystrom
 
 
 Plug/switch
 -----------
 
 At the moment the following endpoints are covered according `https://api.mystrom.ch <https://api.mystrom.ch>`_:
```

### Comparing `python-mystrom-2.1.0/python_mystrom.egg-info/SOURCES.txt` & `python-mystrom-2.2.0/python_mystrom.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 examples/example-bulb-hsv.py
 examples/example-bulb.py
 examples/example-discovery.py
```

### Comparing `python-mystrom-2.1.0/setup.py` & `python-mystrom-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "README.rst"), encoding="utf-8") as readme:
     long_description = readme.read()
 
 setup(
     name="python-mystrom",
-    version="2.1.0",
+    version="2.2.0",
     description="Asynchronous Python API client for interacting with myStrom devices",
     long_description=long_description,
     url="https://github.com/home-assistant-ecosystem/python-mystrom",
     author="Fabian Affolter",
     author_email="fabian@affolter-engineering.ch",
     license="MIT",
     install_requires=[
```

