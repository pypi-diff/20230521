# Comparing `tmp/amino.fix-2.3.5.5.tar.gz` & `tmp/amino.fix-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.fix-2.3.5.5.tar", last modified: Thu Apr  6 18:06:10 2023, max compression
+gzip compressed data, was "amino.fix-2.3.6.tar", last modified: Sun May 21 21:01:51 2023, max compression
```

## Comparing `amino.fix-2.3.5.5.tar` & `amino.fix-2.3.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 18:06:10.073481 amino.fix-2.3.5.5/
--rw-rw-rw-   0        0        0     1089 2023-01-20 11:16:36.000000 amino.fix-2.3.5.5/LICENSE
--rw-rw-rw-   0        0        0      620 2023-04-06 18:06:10.073481 amino.fix-2.3.5.5/PKG-INFO
--rw-rw-rw-   0        0        0      212 2022-03-19 07:48:20.000000 amino.fix-2.3.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 18:06:09.889481 amino.fix-2.3.5.5/amino.fix.egg-info/
--rw-rw-rw-   0        0        0      620 2023-04-06 18:06:09.000000 amino.fix-2.3.5.5/amino.fix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2023-04-06 18:06:09.000000 amino.fix-2.3.5.5/amino.fix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 18:06:09.000000 amino.fix-2.3.5.5/amino.fix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-06 18:06:09.000000 amino.fix-2.3.5.5/amino.fix.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 18:06:09.000000 amino.fix-2.3.5.5/amino.fix.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-06 18:06:09.963482 amino.fix-2.3.5.5/aminofix/
--rw-rw-rw-   0        0        0      715 2023-04-06 18:03:23.000000 amino.fix-2.3.5.5/aminofix/__init__.py
--rw-rw-rw-   0        0        0    12887 2023-01-20 09:14:27.000000 amino.fix-2.3.5.5/aminofix/acm.py
-drwxrwxrwx   0        0        0        0 2023-04-06 18:06:10.015482 amino.fix-2.3.5.5/aminofix/asyncfix/
--rw-rw-rw-   0        0        0      256 2023-01-20 07:25:50.000000 amino.fix-2.3.5.5/aminofix/asyncfix/__init__.py
--rw-rw-rw-   0        0        0    13760 2023-01-20 07:25:50.000000 amino.fix-2.3.5.5/aminofix/asyncfix/acm.py
--rw-rw-rw-   0        0        0    98032 2023-01-20 10:04:40.000000 amino.fix-2.3.5.5/aminofix/asyncfix/client.py
--rw-rw-rw-   0        0        0    13192 2023-01-20 09:24:56.000000 amino.fix-2.3.5.5/aminofix/asyncfix/socket.py
--rw-rw-rw-   0        0        0   110680 2023-04-06 18:02:18.000000 amino.fix-2.3.5.5/aminofix/asyncfix/sub_client.py
--rw-rw-rw-   0        0        0   100219 2023-01-26 19:52:08.000000 amino.fix-2.3.5.5/aminofix/client.py
-drwxrwxrwx   0        0        0        0 2023-04-06 18:06:10.018481 amino.fix-2.3.5.5/aminofix/lib/
--rw-rw-rw-   0        0        0        0 2023-01-20 07:25:50.000000 amino.fix-2.3.5.5/aminofix/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 18:06:10.070482 amino.fix-2.3.5.5/aminofix/lib/util/
--rw-rw-rw-   0        0        0       99 2023-01-20 09:15:29.000000 amino.fix-2.3.5.5/aminofix/lib/util/__init__.py
--rw-rw-rw-   0        0        0    31646 2023-01-20 07:25:50.000000 amino.fix-2.3.5.5/aminofix/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     3884 2023-01-23 16:21:31.000000 amino.fix-2.3.5.5/aminofix/lib/util/headers.py
--rw-rw-rw-   0        0        0     1215 2023-01-20 09:10:25.000000 amino.fix-2.3.5.5/aminofix/lib/util/helpers.py
--rw-rw-rw-   0        0        0   198051 2023-01-20 07:25:50.000000 amino.fix-2.3.5.5/aminofix/lib/util/objects.py
--rw-rw-rw-   0        0        0    13190 2023-01-20 09:13:24.000000 amino.fix-2.3.5.5/aminofix/socket.py
--rw-rw-rw-   0        0        0   117552 2023-04-06 18:02:18.000000 amino.fix-2.3.5.5/aminofix/sub_client.py
--rw-rw-rw-   0        0        0       42 2023-04-06 18:06:10.074482 amino.fix-2.3.5.5/setup.cfg
--rw-rw-rw-   0        0        0      920 2023-04-06 18:05:08.000000 amino.fix-2.3.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 21:01:51.270260 amino.fix-2.3.6/
+-rw-rw-rw-   0        0        0     1089 2023-01-20 11:16:36.000000 amino.fix-2.3.6/LICENSE
+-rw-rw-rw-   0        0        0      618 2023-05-21 21:01:51.270260 amino.fix-2.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2022-03-19 07:48:20.000000 amino.fix-2.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 21:01:51.115270 amino.fix-2.3.6/amino.fix.egg-info/
+-rw-rw-rw-   0        0        0      618 2023-05-21 21:01:51.000000 amino.fix-2.3.6/amino.fix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2023-05-21 21:01:51.000000 amino.fix-2.3.6/amino.fix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 21:01:51.000000 amino.fix-2.3.6/amino.fix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-05-21 21:01:51.000000 amino.fix-2.3.6/amino.fix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-21 21:01:51.000000 amino.fix-2.3.6/amino.fix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 21:01:51.169650 amino.fix-2.3.6/aminofix/
+-rw-rw-rw-   0        0        0      713 2023-05-21 21:00:58.000000 amino.fix-2.3.6/aminofix/__init__.py
+-rw-rw-rw-   0        0        0    12887 2023-01-20 09:14:27.000000 amino.fix-2.3.6/aminofix/acm.py
+drwxrwxrwx   0        0        0        0 2023-05-21 21:01:51.228265 amino.fix-2.3.6/aminofix/asyncfix/
+-rw-rw-rw-   0        0        0      256 2023-01-20 07:25:50.000000 amino.fix-2.3.6/aminofix/asyncfix/__init__.py
+-rw-rw-rw-   0        0        0    13760 2023-01-20 07:25:50.000000 amino.fix-2.3.6/aminofix/asyncfix/acm.py
+-rw-rw-rw-   0        0        0    98035 2023-05-21 20:55:10.000000 amino.fix-2.3.6/aminofix/asyncfix/client.py
+-rw-rw-rw-   0        0        0    13192 2023-01-20 09:24:56.000000 amino.fix-2.3.6/aminofix/asyncfix/socket.py
+-rw-rw-rw-   0        0        0   110680 2023-04-06 18:02:18.000000 amino.fix-2.3.6/aminofix/asyncfix/sub_client.py
+-rw-rw-rw-   0        0        0   100222 2023-05-21 20:55:10.000000 amino.fix-2.3.6/aminofix/client.py
+drwxrwxrwx   0        0        0        0 2023-05-21 21:01:51.230259 amino.fix-2.3.6/aminofix/lib/
+-rw-rw-rw-   0        0        0        0 2023-01-20 07:25:50.000000 amino.fix-2.3.6/aminofix/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 21:01:51.268259 amino.fix-2.3.6/aminofix/lib/util/
+-rw-rw-rw-   0        0        0       99 2023-01-20 09:15:29.000000 amino.fix-2.3.6/aminofix/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    31646 2023-01-20 07:25:50.000000 amino.fix-2.3.6/aminofix/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     3884 2023-01-23 16:21:31.000000 amino.fix-2.3.6/aminofix/lib/util/headers.py
+-rw-rw-rw-   0        0        0     1215 2023-01-20 09:10:25.000000 amino.fix-2.3.6/aminofix/lib/util/helpers.py
+-rw-rw-rw-   0        0        0   198051 2023-01-20 07:25:50.000000 amino.fix-2.3.6/aminofix/lib/util/objects.py
+-rw-rw-rw-   0        0        0    13190 2023-01-20 09:13:24.000000 amino.fix-2.3.6/aminofix/socket.py
+-rw-rw-rw-   0        0        0   117552 2023-04-06 18:02:18.000000 amino.fix-2.3.6/aminofix/sub_client.py
+-rw-rw-rw-   0        0        0       42 2023-05-21 21:01:51.271260 amino.fix-2.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      918 2023-05-21 21:01:08.000000 amino.fix-2.3.6/setup.py
```

### Comparing `amino.fix-2.3.5.5/LICENSE` & `amino.fix-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/PKG-INFO` & `amino.fix-2.3.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix
-Version: 2.3.5.5
+Version: 2.3.6
 Summary: Library for Amino. Discord - https://discord.gg/Bf3dpBRJHj
 Home-page: https://github.com/Minori100/Amino.fix
 Author: Minori
 Author-email: minorigithub@gmail.com
 License: MIT
 Keywords: aminoapps,amino.fix,amino,amino-bot,narvii,api,python,python3,python3.x,minori
 Platform: UNKNOWN
```

### Comparing `amino.fix-2.3.5.5/amino.fix.egg-info/PKG-INFO` & `amino.fix-2.3.6/amino.fix.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix
-Version: 2.3.5.5
+Version: 2.3.6
 Summary: Library for Amino. Discord - https://discord.gg/Bf3dpBRJHj
 Home-page: https://github.com/Minori100/Amino.fix
 Author: Minori
 Author-email: minorigithub@gmail.com
 License: MIT
 Keywords: aminoapps,amino.fix,amino,amino-bot,narvii,api,python,python3,python3.x,minori
 Platform: UNKNOWN
```

### Comparing `amino.fix-2.3.5.5/amino.fix.egg-info/SOURCES.txt` & `amino.fix-2.3.6/amino.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/aminofix/__init__.py` & `amino.fix-2.3.6/aminofix/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'Amino.fix'
 __author__ = 'Minori'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2021-2023 Minori'
-__version__ = '2.3.5.5'
+__version__ = '2.3.6'
 
 from .acm import ACM
 from .client import Client
 from .sub_client import SubClient
 from .lib.util import exceptions, helpers, objects, headers
 from .asyncfix import acm, client, sub_client, socket
 from .socket import Callbacks, SocketHandler
```

### Comparing `amino.fix-2.3.5.5/aminofix/acm.py` & `amino.fix-2.3.6/aminofix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/aminofix/asyncfix/acm.py` & `amino.fix-2.3.6/aminofix/asyncfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/aminofix/asyncfix/client.py` & `amino.fix-2.3.6/aminofix/asyncfix/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ..lib.util.helpers import gen_deviceId
 from .socket import Callbacks, SocketHandler
 
 #@dorthegra/IDörthe#8835 thanks for support!
 
 class Client(Callbacks, SocketHandler):
     def __init__(self, deviceId: str = None, userAgent: str = "Apple iPhone12,1 iOS v15.5 Main/3.12.2", socket_trace = False, socketDebugging = False, socket_enabled = True, autoDevice = False, sub: bool = False):
-        self.api = "https://service.narvii.com/api/v1"
+        self.api = "https://service.aminoapps.com/api/v1"
         self.authenticated = False
         self.configured = False
 
         self.socket_enabled = socket_enabled
         self.autoDevice = autoDevice
 
         if sub:
```

### Comparing `amino.fix-2.3.5.5/aminofix/asyncfix/socket.py` & `amino.fix-2.3.6/aminofix/asyncfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/aminofix/asyncfix/sub_client.py` & `amino.fix-2.3.6/aminofix/asyncfix/sub_client.py`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/aminofix/client.py` & `amino.fix-2.3.6/aminofix/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .socket import Callbacks, SocketHandler
 from .lib.util.helpers import gen_deviceId
 
 #@dorthegra/IDörthe#8835 thanks for support!
 
 class Client(Callbacks, SocketHandler):
     def __init__(self, deviceId: str = None, userAgent: str = "Apple iPhone12,1 iOS v15.5 Main/3.12.2", proxies: dict = None, certificatePath = None, socket_trace = False, socketDebugging = False, socket_enabled = True, autoDevice = False, sub: bool = False):
-        self.api = "https://service.narvii.com/api/v1"
+        self.api = "https://service.aminoapps.com/api/v1"
         self.authenticated = False
         self.configured = False
         self.session = requests.Session()
         self.autoDevice = autoDevice
 
         if sub:
             if deviceId:
```

### Comparing `amino.fix-2.3.5.5/aminofix/lib/util/exceptions.py` & `amino.fix-2.3.6/aminofix/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/aminofix/lib/util/headers.py` & `amino.fix-2.3.6/aminofix/lib/util/headers.py`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/aminofix/lib/util/helpers.py` & `amino.fix-2.3.6/aminofix/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/aminofix/lib/util/objects.py` & `amino.fix-2.3.6/aminofix/lib/util/objects.py`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/aminofix/socket.py` & `amino.fix-2.3.6/aminofix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/aminofix/sub_client.py` & `amino.fix-2.3.6/aminofix/sub_client.py`

 * *Files identical despite different names*

### Comparing `amino.fix-2.3.5.5/setup.py` & `amino.fix-2.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 setup(
     name="amino.fix",
     license="MIT",
     author="Minori",
-    version="2.3.5.5",
+    version="2.3.6",
     author_email="minorigithub@gmail.com",
     description="Library for Amino. Discord - https://discord.gg/Bf3dpBRJHj",
     url="https://github.com/Minori100/Amino.fix",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

