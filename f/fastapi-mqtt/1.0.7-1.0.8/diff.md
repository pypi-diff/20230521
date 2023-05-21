# Comparing `tmp/fastapi_mqtt-1.0.7.tar.gz` & `tmp/fastapi_mqtt-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mqtt-1.0.7.tar", max compression
+gzip compressed data, was "fastapi_mqtt-1.0.8.tar", max compression
```

## Comparing `fastapi_mqtt-1.0.7.tar` & `fastapi_mqtt-1.0.8.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-02-05 12:08:06.629155 fastapi_mqtt-1.0.7/LICENSE
--rw-r--r--   0        0        0     3465 2023-02-05 12:08:06.629155 fastapi_mqtt-1.0.7/README.md
--rw-r--r--   0        0        0      319 2023-02-05 12:08:06.629155 fastapi_mqtt-1.0.7/fastapi_mqtt/__init__.py
--rw-r--r--   0        0        0     2223 2023-02-05 12:08:06.629155 fastapi_mqtt-1.0.7/fastapi_mqtt/config.py
--rw-r--r--   0        0        0     9538 2023-02-05 12:08:06.629155 fastapi_mqtt-1.0.7/fastapi_mqtt/fastmqtt.py
--rw-r--r--   0        0        0     1573 2023-02-05 12:08:06.629155 fastapi_mqtt-1.0.7/fastapi_mqtt/handlers.py
--rw-r--r--   0        0        0        1 2023-02-05 12:08:06.629155 fastapi_mqtt-1.0.7/fastapi_mqtt/py.typed
--rw-r--r--   0        0        0     1069 2023-02-05 12:08:19.933439 fastapi_mqtt-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 fastapi_mqtt-1.0.7/setup.py
--rw-r--r--   0        0        0     4667 1970-01-01 00:00:00.000000 fastapi_mqtt-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-20 10:54:55.172911 fastapi_mqtt-1.0.8/LICENSE
+-rw-r--r--   0        0        0     3465 2023-05-20 10:54:55.172911 fastapi_mqtt-1.0.8/README.md
+-rw-r--r--   0        0        0      319 2023-05-20 10:54:55.172911 fastapi_mqtt-1.0.8/fastapi_mqtt/__init__.py
+-rw-r--r--   0        0        0     2217 2023-05-20 10:54:55.172911 fastapi_mqtt-1.0.8/fastapi_mqtt/config.py
+-rw-r--r--   0        0        0     9460 2023-05-20 10:54:55.172911 fastapi_mqtt-1.0.8/fastapi_mqtt/fastmqtt.py
+-rw-r--r--   0        0        0     1573 2023-05-20 10:54:55.172911 fastapi_mqtt-1.0.8/fastapi_mqtt/handlers.py
+-rw-r--r--   0        0        0        1 2023-05-20 10:54:55.172911 fastapi_mqtt-1.0.8/fastapi_mqtt/py.typed
+-rw-r--r--   0        0        0     1069 2023-05-20 10:55:13.281057 fastapi_mqtt-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 fastapi_mqtt-1.0.8/PKG-INFO
```

### Comparing `fastapi_mqtt-1.0.7/LICENSE` & `fastapi_mqtt-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_mqtt-1.0.7/README.md` & `fastapi_mqtt-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_mqtt-1.0.7/fastapi_mqtt/config.py` & `fastapi_mqtt-1.0.8/fastapi_mqtt/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,13 +45,13 @@
     port: int = 1883
     ssl: Union[bool, SSLContext] = False
     keepalive: int = 60
     username: Optional[str] = None
     password: Optional[str] = None
     version: int = MQTTv50
 
-    reconnect_retries: Optional[int] = None
-    reconnect_delay: Optional[int] = None
+    reconnect_retries: Optional[int] = 1
+    reconnect_delay: Optional[int] = 6
 
     will_message_topic: Optional[str] = None
     will_message_payload: Optional[str] = None
-    will_delay_interval: Optional[str] = None
+    will_delay_interval: Optional[int] = None
```

### Comparing `fastapi_mqtt-1.0.7/fastapi_mqtt/fastmqtt.py` & `fastapi_mqtt-1.0.8/fastapi_mqtt/fastmqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             self.config.will_message_topic
             and self.config.will_message_payload
             and self.config.will_delay_interval
         ):
             self.client._will_message = Message(
                 self.config.will_message_topic,
                 self.config.will_message_payload,
-                self.config.will_delay_interval,
+                will_delay_interval=self.config.will_delay_interval,
             )
             log_info.debug(
                 f'topic -> {self.config.will_message_topic} \n payload -> {self.config.will_message_payload} \n will_delay_interval -> {self.config.will_delay_interval}'  # noqa E501
             )
             log_info.debug('WILL MESSAGE INITIALIZED')
 
     @staticmethod
@@ -133,20 +133,18 @@
     async def __set_connetion_config(self) -> None:
         """
         The connected MQTT clients will always try to reconnect in case of lost connections.
         The number of reconnect attempts is unlimited.
         For changing this behavior, set reconnect_retries and reconnect_delay with its values.
         For more info: https://github.com/wialon/gmqtt#reconnects
         """
-        if self.config.reconnect_retries:
-            self.client.set_config(reconnect_retries=self.config.reconnect_retries)
-
-        if self.config.reconnect_delay:
-            self.client.set_config(reconnect_delay=self.config.reconnect_delay)
-
+        self.client.set_config({
+            "reconnect_retries":self.reconnect_retries, 
+            "reconnect_delay": self.reconnect_delay})
+     
     def __on_connect(self, client, flags, rc, properties) -> None:
         """
         Generic on connecting handler, it would call user handler if defined.
         Will perform subscription for given topics.
         It cannot be done earlier, since subscription relies on connection.
         """
         if self.mqtt_handlers.get_user_connect_handler:
```

### Comparing `fastapi_mqtt-1.0.7/fastapi_mqtt/handlers.py` & `fastapi_mqtt-1.0.8/fastapi_mqtt/handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_mqtt-1.0.7/pyproject.toml` & `fastapi_mqtt-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-mqtt"
-version = "1.0.7"
+version = "1.0.8"
 description = "fastapi-mqtt is extension for MQTT protocol"
 authors = ["sabuhish <sabuhi.shukurov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/sabuhish/fastapi-mqtt"
 repository = "https://github.com/sabuhish/fastapi-mqtt"
 classifiers = [
```

### Comparing `fastapi_mqtt-1.0.7/setup.py` & `fastapi_mqtt-1.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,155 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fastapi-mqtt
+Version: 1.0.8
+Summary: fastapi-mqtt is extension for MQTT protocol
+Home-page: https://github.com/sabuhish/fastapi-mqtt
+License: MIT
+Author: sabuhish
+Author-email: sabuhi.shukurov@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Requires-Dist: fastapi (==0.*)
+Requires-Dist: gmqtt (>=0.6.11,<0.7.0)
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: uvicorn (>=0.19.0)
+Project-URL: Repository, https://github.com/sabuhish/fastapi-mqtt
+Description-Content-Type: text/markdown
 
-packages = \
-['fastapi_mqtt']
+# fastapi-mqtt
 
-package_data = \
-{'': ['*']}
+MQTT is a lightweight publish/subscribe messaging protocol designed for M2M (machine to machine) telemetry in low bandwidth environments.
+Fastapi-mqtt is the client for working with MQTT.
 
-install_requires = \
-['fastapi<1.0.0',
- 'gmqtt>=0.6.11,<0.7.0',
- 'pydantic>=1.9.0,<2.0.0',
- 'uvicorn>=0.19.0']
-
-setup_kwargs = {
-    'name': 'fastapi-mqtt',
-    'version': '1.0.7',
-    'description': 'fastapi-mqtt is extension for MQTT protocol',
-    'long_description': '# fastapi-mqtt\n\nMQTT is a lightweight publish/subscribe messaging protocol designed for M2M (machine to machine) telemetry in low bandwidth environments.\nFastapi-mqtt is the client for working with MQTT.\n\nFor more information about MQTT, please refer to here: [MQTT](MQTT.md)\n\nFatapi-mqtt wraps around [gmqtt](https://github.com/wialon/gmqtt) module. Gmqtt Python async client for MQTT client implementation.\nModule has support of MQTT version 5.0 protocol\n\n[![MIT licensed](https://img.shields.io/github/license/sabuhish/fastapi-mqtt)](https://raw.githubusercontent.com/sabuhish/fastapi-mqtt/master/LICENSE)\n[![GitHub stars](https://img.shields.io/github/stars/sabuhish/fastapi-mqtt.svg)](https://github.com/sabuhish/fastapi-mqtt/stargazers)\n[![GitHub forks](https://img.shields.io/github/forks/sabuhish/fastapi-mqtt.svg)](https://github.com/sabuhish/fastapi-mqtt/network)\n[![GitHub issues](https://img.shields.io/github/issues-raw/sabuhish/fastapi-mqtt)](https://github.com/sabuhish/fastapi-mqtt/issues)\n[![Downloads](https://pepy.tech/badge/fastapi-mqtt)](https://pepy.tech/project/fastapi-mqtt)\n\n---\n\n## **Documentation**: [FastApi-MQTT](https://sabuhish.github.io/fastapi-mqtt/)\n\nThe key feature are:\n\nMQTT specification avaliable with help decarator methods using callbacks:\n\n- on_connect()\n- on_disconnect()\n- on_subscribe()\n- on_message()\n- subscribe(topic)\n\n- Base Settings available with `pydantic` class\n- Authetication to broker with credentials\n- unsubscribe certain topics and publish to certain topics\n\n### 🔨 Installation\n\n```sh\n $ pip install fastapi-mqtt\n```\n\n### 🕹 Guide\n\n```python\nfrom fastapi import FastAPI\nfrom fastapi_mqtt import FastMQTT, MQTTConfig\n\napp = FastAPI()\n\nmqtt_config = MQTTConfig()\n\nmqtt = FastMQTT(\n    config=mqtt_config\n)\n\nmqtt.init_app(app)\n\n\n\n@mqtt.on_connect()\ndef connect(client, flags, rc, properties):\n    mqtt.client.subscribe("/mqtt") #subscribing mqtt topic\n    print("Connected: ", client, flags, rc, properties)\n\n@mqtt.on_message()\nasync def message(client, topic, payload, qos, properties):\n    print("Received message: ",topic, payload.decode(), qos, properties)\n\n@mqtt.subscribe("my/mqtt/topic/#")\nasync def message_to_topic(client, topic, payload, qos, properties):\n    print("Received message to specific topic: ", topic, payload.decode(), qos, properties)\n\n@mqtt.on_disconnect()\ndef disconnect(client, packet, exc=None):\n    print("Disconnected")\n\n@mqtt.on_subscribe()\ndef subscribe(client, mid, qos, properties):\n    print("subscribed", client, mid, qos, properties)\n\n```\n\nPublish method:\n\n```python\nasync def func():\n    mqtt.publish("/mqtt", "Hello from Fastapi") #publishing mqtt topic\n\n    return {"result": True,"message":"Published" }\n\n\n```\n\nSubscribe method:\n\n```python\n\n@mqtt.on_connect()\ndef connect(client, flags, rc, properties):\n    mqtt.client.subscribe("/mqtt") #subscribing mqtt topic\n    print("Connected: ", client, flags, rc, properties)\n\n```\n\nChanging connection params\n\n```python\nmqtt_config = MQTTConfig(host = "mqtt.mosquito.org",\n    port= 1883,\n    keepalive = 60,\n    username="username",\n    password="strong_password")\n\n\nmqtt = FastMQTT(\n    config=mqtt_config)\n\n```\n\n# Contributing\n\nFell free to open issue and send pull request.\n\nThanks To [Contributors](https://github.com/sabuhish/fastapi-mqtt/graphs/contributors).\nContributions of any kind are welcome!\n\nBefore you start please read [CONTRIBUTING](https://github.com/sabuhish/fastapi-mqtt/blob/master/CONTRIBUTING.md)\n',
-    'author': 'sabuhish',
-    'author_email': 'sabuhi.shukurov@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/sabuhish/fastapi-mqtt',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+For more information about MQTT, please refer to here: [MQTT](MQTT.md)
 
+Fatapi-mqtt wraps around [gmqtt](https://github.com/wialon/gmqtt) module. Gmqtt Python async client for MQTT client implementation.
+Module has support of MQTT version 5.0 protocol
+
+[![MIT licensed](https://img.shields.io/github/license/sabuhish/fastapi-mqtt)](https://raw.githubusercontent.com/sabuhish/fastapi-mqtt/master/LICENSE)
+[![GitHub stars](https://img.shields.io/github/stars/sabuhish/fastapi-mqtt.svg)](https://github.com/sabuhish/fastapi-mqtt/stargazers)
+[![GitHub forks](https://img.shields.io/github/forks/sabuhish/fastapi-mqtt.svg)](https://github.com/sabuhish/fastapi-mqtt/network)
+[![GitHub issues](https://img.shields.io/github/issues-raw/sabuhish/fastapi-mqtt)](https://github.com/sabuhish/fastapi-mqtt/issues)
+[![Downloads](https://pepy.tech/badge/fastapi-mqtt)](https://pepy.tech/project/fastapi-mqtt)
+
+---
+
+## **Documentation**: [FastApi-MQTT](https://sabuhish.github.io/fastapi-mqtt/)
+
+The key feature are:
+
+MQTT specification avaliable with help decarator methods using callbacks:
+
+- on_connect()
+- on_disconnect()
+- on_subscribe()
+- on_message()
+- subscribe(topic)
+
+- Base Settings available with `pydantic` class
+- Authetication to broker with credentials
+- unsubscribe certain topics and publish to certain topics
+
+### 🔨 Installation
+
+```sh
+ $ pip install fastapi-mqtt
+```
+
+### 🕹 Guide
+
+```python
+from fastapi import FastAPI
+from fastapi_mqtt import FastMQTT, MQTTConfig
+
+app = FastAPI()
+
+mqtt_config = MQTTConfig()
+
+mqtt = FastMQTT(
+    config=mqtt_config
+)
+
+mqtt.init_app(app)
+
+
+
+@mqtt.on_connect()
+def connect(client, flags, rc, properties):
+    mqtt.client.subscribe("/mqtt") #subscribing mqtt topic
+    print("Connected: ", client, flags, rc, properties)
+
+@mqtt.on_message()
+async def message(client, topic, payload, qos, properties):
+    print("Received message: ",topic, payload.decode(), qos, properties)
+
+@mqtt.subscribe("my/mqtt/topic/#")
+async def message_to_topic(client, topic, payload, qos, properties):
+    print("Received message to specific topic: ", topic, payload.decode(), qos, properties)
+
+@mqtt.on_disconnect()
+def disconnect(client, packet, exc=None):
+    print("Disconnected")
+
+@mqtt.on_subscribe()
+def subscribe(client, mid, qos, properties):
+    print("subscribed", client, mid, qos, properties)
+
+```
+
+Publish method:
+
+```python
+async def func():
+    mqtt.publish("/mqtt", "Hello from Fastapi") #publishing mqtt topic
+
+    return {"result": True,"message":"Published" }
+
+
+```
+
+Subscribe method:
+
+```python
+
+@mqtt.on_connect()
+def connect(client, flags, rc, properties):
+    mqtt.client.subscribe("/mqtt") #subscribing mqtt topic
+    print("Connected: ", client, flags, rc, properties)
+
+```
+
+Changing connection params
+
+```python
+mqtt_config = MQTTConfig(host = "mqtt.mosquito.org",
+    port= 1883,
+    keepalive = 60,
+    username="username",
+    password="strong_password")
+
+
+mqtt = FastMQTT(
+    config=mqtt_config)
+
+```
+
+# Contributing
+
+Fell free to open issue and send pull request.
+
+Thanks To [Contributors](https://github.com/sabuhish/fastapi-mqtt/graphs/contributors).
+Contributions of any kind are welcome!
+
+Before you start please read [CONTRIBUTING](https://github.com/sabuhish/fastapi-mqtt/blob/master/CONTRIBUTING.md)
 
-setup(**setup_kwargs)
```

