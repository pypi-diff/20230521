# Comparing `tmp/amino.li-0.8.tar.gz` & `tmp/amino.li-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.li-0.8.tar", last modified: Sat Apr  1 06:35:21 2023, max compression
+gzip compressed data, was "amino.li-1.1.tar", last modified: Sun May 21 18:44:51 2023, max compression
```

## Comparing `amino.li-0.8.tar` & `amino.li-1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 06:35:21.203277 amino.li-0.8/
--rw-rw-rw-   0        0        0      402 2023-04-01 06:35:21.204276 amino.li-0.8/PKG-INFO
--rw-rw-rw-   0        0        0       90 2023-02-05 06:12:12.000000 amino.li-0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-01 06:35:21.052681 amino.li-0.8/amino.li.egg-info/
--rw-rw-rw-   0        0        0      402 2023-04-01 06:35:20.000000 amino.li-0.8/amino.li.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-04-01 06:35:20.000000 amino.li-0.8/amino.li.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 06:35:20.000000 amino.li-0.8/amino.li.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-01 06:35:20.000000 amino.li-0.8/amino.li.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-01 06:35:20.000000 amino.li-0.8/amino.li.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-01 06:35:21.080610 amino.li-0.8/aminoli/
--rw-rw-rw-   0        0        0      672 2023-04-01 06:34:58.000000 amino.li-0.8/aminoli/__init__.py
--rw-rw-rw-   0        0        0    12645 2023-04-01 06:34:13.000000 amino.li-0.8/aminoli/acm.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:35:21.138453 amino.li-0.8/aminoli/asyncfix/
--rw-rw-rw-   0        0        0      232 2023-02-05 04:28:06.000000 amino.li-0.8/aminoli/asyncfix/__init__.py
--rw-rw-rw-   0        0        0    13502 2023-01-26 19:53:12.000000 amino.li-0.8/aminoli/asyncfix/acm.py
--rw-rw-rw-   0        0        0    95643 2023-04-01 06:34:17.000000 amino.li-0.8/aminoli/asyncfix/client.py
--rw-rw-rw-   0        0        0    13789 2023-02-13 03:47:02.000000 amino.li-0.8/aminoli/asyncfix/socket.py
--rw-rw-rw-   0        0        0   108461 2023-04-01 06:34:21.000000 amino.li-0.8/aminoli/asyncfix/sub_client.py
--rw-rw-rw-   0        0        0    98585 2023-04-01 06:27:49.000000 amino.li-0.8/aminoli/client.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:35:21.152414 amino.li-0.8/aminoli/lib/
--rw-rw-rw-   0        0        0        0 2023-01-26 19:53:12.000000 amino.li-0.8/aminoli/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:35:21.197559 amino.li-0.8/aminoli/lib/util/
--rw-rw-rw-   0        0        0       95 2023-01-26 19:53:12.000000 amino.li-0.8/aminoli/lib/util/__init__.py
--rw-rw-rw-   0        0        0    30690 2023-01-26 19:53:12.000000 amino.li-0.8/aminoli/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     3784 2023-04-01 06:27:27.000000 amino.li-0.8/aminoli/lib/util/headers.py
--rw-rw-rw-   0        0        0     1184 2023-01-26 19:53:12.000000 amino.li-0.8/aminoli/lib/util/helpers.py
--rw-rw-rw-   0        0        0   193750 2023-01-26 19:53:12.000000 amino.li-0.8/aminoli/lib/util/objects.py
--rw-rw-rw-   0        0        0    14008 2023-03-11 22:44:20.000000 amino.li-0.8/aminoli/socket.py
--rw-rw-rw-   0        0        0   117288 2023-04-01 06:34:24.000000 amino.li-0.8/aminoli/sub_client.py
--rw-rw-rw-   0        0        0       42 2023-04-01 06:35:21.218238 amino.li-0.8/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-04-01 06:34:58.000000 amino.li-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 18:44:51.144091 amino.li-1.1/
+-rw-rw-rw-   0        0        0      402 2023-05-21 18:44:51.144091 amino.li-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       90 2023-02-05 06:12:12.000000 amino.li-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 18:44:49.864508 amino.li-1.1/amino.li.egg-info/
+-rw-rw-rw-   0        0        0      402 2023-05-21 18:44:49.000000 amino.li-1.1/amino.li.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-05-21 18:44:49.000000 amino.li-1.1/amino.li.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 18:44:49.000000 amino.li-1.1/amino.li.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-05-21 18:44:49.000000 amino.li-1.1/amino.li.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 18:44:49.000000 amino.li-1.1/amino.li.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 18:44:50.152738 amino.li-1.1/aminoli/
+-rw-rw-rw-   0        0        0      672 2023-05-21 18:39:43.000000 amino.li-1.1/aminoli/__init__.py
+-rw-rw-rw-   0        0        0    12645 2023-04-01 06:34:13.000000 amino.li-1.1/aminoli/acm.py
+drwxrwxrwx   0        0        0        0 2023-05-21 18:44:50.524743 amino.li-1.1/aminoli/asyncfix/
+-rw-rw-rw-   0        0        0      232 2023-02-05 04:28:06.000000 amino.li-1.1/aminoli/asyncfix/__init__.py
+-rw-rw-rw-   0        0        0    13502 2023-01-26 19:53:12.000000 amino.li-1.1/aminoli/asyncfix/acm.py
+-rw-rw-rw-   0        0        0    95646 2023-05-21 18:36:01.000000 amino.li-1.1/aminoli/asyncfix/client.py
+-rw-rw-rw-   0        0        0    13792 2023-05-21 18:39:00.000000 amino.li-1.1/aminoli/asyncfix/socket.py
+-rw-rw-rw-   0        0        0   108461 2023-04-01 06:34:21.000000 amino.li-1.1/aminoli/asyncfix/sub_client.py
+-rw-rw-rw-   0        0        0    98588 2023-05-21 18:34:40.000000 amino.li-1.1/aminoli/client.py
+drwxrwxrwx   0        0        0        0 2023-05-21 18:44:50.634451 amino.li-1.1/aminoli/lib/
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:53:12.000000 amino.li-1.1/aminoli/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 18:44:50.966563 amino.li-1.1/aminoli/lib/util/
+-rw-rw-rw-   0        0        0       95 2023-01-26 19:53:12.000000 amino.li-1.1/aminoli/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    30690 2023-01-26 19:53:12.000000 amino.li-1.1/aminoli/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     3784 2023-04-01 06:27:27.000000 amino.li-1.1/aminoli/lib/util/headers.py
+-rw-rw-rw-   0        0        0     1184 2023-01-26 19:53:12.000000 amino.li-1.1/aminoli/lib/util/helpers.py
+-rw-rw-rw-   0        0        0   193750 2023-01-26 19:53:12.000000 amino.li-1.1/aminoli/lib/util/objects.py
+-rw-rw-rw-   0        0        0    14011 2023-05-21 18:39:32.000000 amino.li-1.1/aminoli/socket.py
+-rw-rw-rw-   0        0        0   117288 2023-04-01 06:34:24.000000 amino.li-1.1/aminoli/sub_client.py
+-rw-rw-rw-   0        0        0       42 2023-05-21 18:44:51.147085 amino.li-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-05-21 18:39:55.000000 amino.li-1.1/setup.py
```

### Comparing `amino.li-0.8/amino.li.egg-info/SOURCES.txt` & `amino.li-1.1/amino.li.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.li-0.8/aminoli/__init__.py` & `amino.li-1.1/aminoli/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'Amino.li'
 __author__ = 'Lucas'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023'
-__version__ = '0.8'
+__version__ = '1.1'
 
 from .acm import ACM
 from .client import Client
 from .sub_client import SubClient
 from .lib.util import exceptions, helpers, objects, headers
 from .asyncfix import acm, client, sub_client, socket
 from .socket import Callbacks, SocketHandler
```

### Comparing `amino.li-0.8/aminoli/acm.py` & `amino.li-1.1/aminoli/acm.py`

 * *Files identical despite different names*

### Comparing `amino.li-0.8/aminoli/asyncfix/acm.py` & `amino.li-1.1/aminoli/asyncfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.li-0.8/aminoli/asyncfix/client.py` & `amino.li-1.1/aminoli/asyncfix/client.py`

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

### Comparing `amino.li-0.8/aminoli/asyncfix/socket.py` & `amino.li-1.1/aminoli/asyncfix/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sys import _getframe as getframe
 
 from ..lib.util import objects, helpers
 from ..lib.util.helpers import gen_deviceId
 
 class SocketHandler:
     def __init__(self, client, socket_trace = False, debug = False):
-        self.socket_url = "wss://ws1.narvii.com"
+        self.socket_url = "wss://ws1.aminoapps.com"
         self.client = client
         self.debug = debug
         self.active = False
         self.headers = None
         self.socket = None
         self.socket_thread = None
         self.reconnectTime = 180
```

### Comparing `amino.li-0.8/aminoli/asyncfix/sub_client.py` & `amino.li-1.1/aminoli/asyncfix/sub_client.py`

 * *Files identical despite different names*

### Comparing `amino.li-0.8/aminoli/client.py` & `amino.li-1.1/aminoli/client.py`

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

### Comparing `amino.li-0.8/aminoli/lib/util/exceptions.py` & `amino.li-1.1/aminoli/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.li-0.8/aminoli/lib/util/headers.py` & `amino.li-1.1/aminoli/lib/util/headers.py`

 * *Files identical despite different names*

### Comparing `amino.li-0.8/aminoli/lib/util/helpers.py` & `amino.li-1.1/aminoli/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.li-0.8/aminoli/lib/util/objects.py` & `amino.li-1.1/aminoli/lib/util/objects.py`

 * *Files identical despite different names*

### Comparing `amino.li-0.8/aminoli/socket.py` & `amino.li-1.1/aminoli/socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sys import _getframe as getframe
 
 from .lib.util.helpers import gen_deviceId
 from .lib.util import objects, helpers
 
 class SocketHandler:
     def __init__(self, client, socket_trace = False, debug = False):
-        self.socket_url = "wss://ws1.narvii.com"
+        self.socket_url = "wss://ws1.aminoapps.com"
         self.client = client
         self.debug = debug
         self.active = False
         self.headers = None
         self.socket = None
         self.socket_thread = None
         self.reconnectTime = 180
```

### Comparing `amino.li-0.8/aminoli/sub_client.py` & `amino.li-1.1/aminoli/sub_client.py`

 * *Files identical despite different names*

