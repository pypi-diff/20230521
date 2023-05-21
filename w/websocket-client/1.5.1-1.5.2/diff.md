# Comparing `tmp/websocket-client-1.5.1.tar.gz` & `tmp/websocket-client-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websocket-client-1.5.1.tar", last modified: Sat Feb  4 17:58:33 2023, max compression
+gzip compressed data, was "websocket-client-1.5.2.tar", last modified: Sun May 21 19:29:25 2023, max compression
```

## Comparing `websocket-client-1.5.1.tar` & `websocket-client-1.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:58:33.124578 websocket-client-1.5.1/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    16842 2023-02-04 17:55:28.000000 websocket-client-1.5.1/ChangeLog
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11339 2023-02-04 17:51:20.000000 websocket-client-1.5.1/LICENSE
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       81 2023-02-04 17:51:20.000000 websocket-client-1.5.1/MANIFEST.in
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-02-04 17:58:33.128578 websocket-client-1.5.1/PKG-INFO
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5997 2023-02-04 17:51:20.000000 websocket-client-1.5.1/README.md
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:58:33.120578 websocket-client-1.5.1/examples/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      344 2023-02-04 17:51:20.000000 websocket-client-1.5.1/examples/echo_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1009 2023-02-04 17:51:20.000000 websocket-client-1.5.1/examples/echoapp_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      351 2023-02-04 17:51:20.000000 websocket-client-1.5.1/examples/rel_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       59 2023-02-04 17:58:33.128578 websocket-client-1.5.1/setup.cfg
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2641 2023-02-04 17:54:19.000000 websocket-client-1.5.1/setup.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:58:33.124578 websocket-client-1.5.1/websocket/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      801 2023-02-04 17:54:12.000000 websocket-client-1.5.1/websocket/__init__.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    13303 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_abnf.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    19097 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_app.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2118 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_cookiejar.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    19855 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_core.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2105 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_exceptions.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     6043 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_handshake.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11754 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_http.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2027 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_logging.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4860 2023-02-04 17:52:14.000000 websocket-client-1.5.1/websocket/_socket.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1122 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_ssl_compat.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4797 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_url.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     3516 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_utils.py
--rwxrwxr-x   0 drift3r   (1000) drift3r   (1000)     6909 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/_wsdump.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:58:33.124578 websocket-client-1.5.1/websocket/tests/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/__init__.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:58:33.124578 websocket-client-1.5.1/websocket/tests/data/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      163 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/data/header01.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      161 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/data/header02.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      216 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/data/header03.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      481 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/echo-server.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4175 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/test_abnf.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    12669 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/test_app.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4325 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/test_cookiejar.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     9623 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/test_http.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    14589 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/test_url.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    18072 2023-02-04 17:51:20.000000 websocket-client-1.5.1/websocket/tests/test_websocket.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:58:33.124578 websocket-client-1.5.1/websocket_client.egg-info/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-02-04 17:58:33.000000 websocket-client-1.5.1/websocket_client.egg-info/PKG-INFO
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1014 2023-02-04 17:58:33.000000 websocket-client-1.5.1/websocket_client.egg-info/SOURCES.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        1 2023-02-04 17:58:33.000000 websocket-client-1.5.1/websocket_client.egg-info/dependency_links.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       50 2023-02-04 17:58:33.000000 websocket-client-1.5.1/websocket_client.egg-info/entry_points.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       94 2023-02-04 17:58:33.000000 websocket-client-1.5.1/websocket_client.egg-info/requires.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       10 2023-02-04 17:58:33.000000 websocket-client-1.5.1/websocket_client.egg-info/top_level.txt
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.776701 websocket-client-1.5.2/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    17075 2023-05-21 19:26:03.000000 websocket-client-1.5.2/ChangeLog
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11339 2023-02-04 17:51:20.000000 websocket-client-1.5.2/LICENSE
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       81 2023-02-04 17:51:20.000000 websocket-client-1.5.2/MANIFEST.in
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-05-21 19:29:25.776701 websocket-client-1.5.2/PKG-INFO
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5997 2023-02-04 17:51:20.000000 websocket-client-1.5.2/README.md
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.772701 websocket-client-1.5.2/examples/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      344 2023-02-04 17:51:20.000000 websocket-client-1.5.2/examples/echo_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1009 2023-02-04 17:51:20.000000 websocket-client-1.5.2/examples/echoapp_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      351 2023-02-04 17:51:20.000000 websocket-client-1.5.2/examples/rel_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       59 2023-05-21 19:29:25.776701 websocket-client-1.5.2/setup.cfg
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2641 2023-05-21 19:21:24.000000 websocket-client-1.5.2/setup.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.776701 websocket-client-1.5.2/websocket/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      801 2023-05-21 19:21:14.000000 websocket-client-1.5.2/websocket/__init__.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    13619 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_abnf.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    20185 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_app.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2164 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_cookiejar.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    19872 2023-04-07 22:45:05.000000 websocket-client-1.5.2/websocket/_core.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2106 2023-04-07 22:59:49.000000 websocket-client-1.5.2/websocket/_exceptions.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     6515 2023-04-07 22:48:16.000000 websocket-client-1.5.2/websocket/_handshake.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11806 2023-04-07 22:47:13.000000 websocket-client-1.5.2/websocket/_http.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2220 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_logging.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4979 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_socket.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1122 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/_ssl_compat.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4932 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_url.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     3636 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_utils.py
+-rwxrwxr-x   0 drift3r   (1000) drift3r   (1000)     7120 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/_wsdump.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.776701 websocket-client-1.5.2/websocket/tests/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        0 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/__init__.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.776701 websocket-client-1.5.2/websocket/tests/data/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      163 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/data/header01.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      161 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/data/header02.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      216 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/data/header03.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      486 2023-05-21 19:20:24.000000 websocket-client-1.5.2/websocket/tests/echo-server.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4175 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_abnf.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    12669 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_app.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4325 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_cookiejar.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     9623 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_http.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    14589 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_url.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    18072 2023-02-04 17:51:20.000000 websocket-client-1.5.2/websocket/tests/test_websocket.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-05-21 19:29:25.776701 websocket-client-1.5.2/websocket_client.egg-info/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/PKG-INFO
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1014 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        1 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       50 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/entry_points.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       94 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/requires.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       10 2023-05-21 19:29:25.000000 websocket-client-1.5.2/websocket_client.egg-info/top_level.txt
```

### Comparing `websocket-client-1.5.1/ChangeLog` & `websocket-client-1.5.2/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 ChangeLog
 ============
 
+- 1.5.2
+  - Add typehints (#908)
+  - Fix pytype errors (#906)
+  - Fix args passed to logging function (#898)
+  - Standardize PEP 3101 formatting (c6a445f)
+  - Add more verbose exception for unsuccessful handshake for #900 (f85ae1f)
+
 - 1.5.1
   - Fix logic bug that can cause disconnects (#893)
 
 - 1.5.0
   - Refactor and improve ping/pong logic to resolve several issues, including an infinite loop issue during reconnect (#862)
   - Fix issue where `skip_utf8_validation = True` is ignored (#886)
   - Fix issue where sslopt `is_ssl` is ignored (#875)
```

### Comparing `websocket-client-1.5.1/LICENSE` & `websocket-client-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.1/PKG-INFO` & `websocket-client-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-client
-Version: 1.5.1
+Version: 1.5.2
 Summary: WebSocket client for Python with low level API options
 Home-page: https://github.com/websocket-client/websocket-client.git
 Download-URL: https://github.com/websocket-client/websocket-client/releases
 Author: liris
 Author-email: liris.pp@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://websocket-client.readthedocs.io/
```

### Comparing `websocket-client-1.5.1/README.md` & `websocket-client-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.1/examples/echoapp_client.py` & `websocket-client-1.5.2/examples/echoapp_client.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.1/setup.py` & `websocket-client-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-VERSION = "1.5.1"
+VERSION = "1.5.2"
 
 install_requires = []
 tests_require = []
 
 setup(
     name="websocket-client",
     version=VERSION,
```

### Comparing `websocket-client-1.5.1/websocket/__init__.py` & `websocket-client-1.5.2/websocket/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 from ._abnf import *
 from ._app import WebSocketApp, setReconnect
 from ._core import *
 from ._exceptions import *
 from ._logging import *
 from ._socket import *
 
-__version__ = "1.5.1"
+__version__ = "1.5.2"
```

### Comparing `websocket-client-1.5.1/websocket/_abnf.py` & `websocket-client-1.5.2/websocket/_abnf.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,22 +29,22 @@
 try:
     # If wsaccel is available, use compiled routines to mask data.
     # wsaccel only provides around a 10% speed boost compared
     # to the websocket-client _mask() implementation.
     # Note that wsaccel is unmaintained.
     from wsaccel.xormask import XorMaskerSimple
 
-    def _mask(_m, _d):
+    def _mask(_m, _d) -> bytes:
         return XorMaskerSimple(_m).process(_d)
 
 except ImportError:
     # wsaccel is not available, use websocket-client _mask()
     native_byteorder = sys.byteorder
 
-    def _mask(mask_value, data_value):
+    def _mask(mask_value: int, data_value: int) -> bytes:
         datalen = len(data_value)
         data_value = int.from_bytes(data_value, native_byteorder)
         mask_value = int.from_bytes(mask_value * (datalen // 4) + mask_value[: datalen % 4], native_byteorder)
         return (data_value ^ mask_value).to_bytes(datalen, native_byteorder)
 
 
 __all__ = [
@@ -127,31 +127,31 @@
     }
 
     # data length threshold.
     LENGTH_7 = 0x7e
     LENGTH_16 = 1 << 16
     LENGTH_63 = 1 << 63
 
-    def __init__(self, fin=0, rsv1=0, rsv2=0, rsv3=0,
-                 opcode=OPCODE_TEXT, mask=1, data=""):
+    def __init__(self, fin: int = 0, rsv1: int = 0, rsv2: int = 0, rsv3: int = 0,
+                 opcode: int = OPCODE_TEXT, mask: int = 1, data: str = "") -> None:
         """
         Constructor for ABNF. Please check RFC for arguments.
         """
         self.fin = fin
         self.rsv1 = rsv1
         self.rsv2 = rsv2
         self.rsv3 = rsv3
         self.opcode = opcode
         self.mask = mask
         if data is None:
             data = ""
         self.data = data
         self.get_mask_key = os.urandom
 
-    def validate(self, skip_utf8_validation=False) -> None:
+    def validate(self, skip_utf8_validation: bool = False) -> None:
         """
         Validate the ABNF frame.
 
         Parameters
         ----------
         skip_utf8_validation: skip utf8 validation.
         """
@@ -183,15 +183,15 @@
 
     def __str__(self) -> str:
         return "fin=" + str(self.fin) \
             + " opcode=" + str(self.opcode) \
             + " data=" + str(self.data)
 
     @staticmethod
-    def create_frame(data, opcode, fin=1):
+    def create_frame(data: str, opcode: int, fin: int = 1) -> 'ABNF':
         """
         Create frame to send text, binary and other data.
 
         Parameters
         ----------
         data: <type>
             data to send. This is string value(byte array).
@@ -233,24 +233,24 @@
 
         if not self.mask:
             return frame_header + self.data
         else:
             mask_key = self.get_mask_key(4)
             return frame_header + self._get_masked(mask_key)
 
-    def _get_masked(self, mask_key):
+    def _get_masked(self, mask_key: bytes) -> bytes:
         s = ABNF.mask(mask_key, self.data)
 
         if isinstance(mask_key, str):
             mask_key = mask_key.encode('utf-8')
 
         return mask_key + s
 
     @staticmethod
-    def mask(mask_key, data):
+    def mask(mask_key: bytes, data: bytes) -> bytes:
         """
         Mask or unmask data. Just do xor for each byte
 
         Parameters
         ----------
         mask_key: bytes or str
             4 byte mask.
@@ -269,72 +269,72 @@
         return _mask(array.array("B", mask_key), array.array("B", data))
 
 
 class frame_buffer:
     _HEADER_MASK_INDEX = 5
     _HEADER_LENGTH_INDEX = 6
 
-    def __init__(self, recv_fn, skip_utf8_validation):
+    def __init__(self, recv_fn: int, skip_utf8_validation: bool) -> None:
         self.recv = recv_fn
         self.skip_utf8_validation = skip_utf8_validation
         # Buffers over the packets from the layer beneath until desired amount
         # bytes of bytes are received.
         self.recv_buffer = []
         self.clear()
         self.lock = Lock()
 
-    def clear(self):
+    def clear(self) -> None:
         self.header = None
         self.length = None
         self.mask = None
 
     def has_received_header(self) -> bool:
         return self.header is None
 
-    def recv_header(self):
+    def recv_header(self) -> None:
         header = self.recv_strict(2)
         b1 = header[0]
         fin = b1 >> 7 & 1
         rsv1 = b1 >> 6 & 1
         rsv2 = b1 >> 5 & 1
         rsv3 = b1 >> 4 & 1
         opcode = b1 & 0xf
         b2 = header[1]
         has_mask = b2 >> 7 & 1
         length_bits = b2 & 0x7f
 
         self.header = (fin, rsv1, rsv2, rsv3, opcode, has_mask, length_bits)
 
-    def has_mask(self):
+    def has_mask(self) -> bool or int:
         if not self.header:
             return False
         return self.header[frame_buffer._HEADER_MASK_INDEX]
 
     def has_received_length(self) -> bool:
         return self.length is None
 
-    def recv_length(self):
+    def recv_length(self) -> None:
         bits = self.header[frame_buffer._HEADER_LENGTH_INDEX]
         length_bits = bits & 0x7f
         if length_bits == 0x7e:
             v = self.recv_strict(2)
             self.length = struct.unpack("!H", v)[0]
         elif length_bits == 0x7f:
             v = self.recv_strict(8)
             self.length = struct.unpack("!Q", v)[0]
         else:
             self.length = length_bits
 
     def has_received_mask(self) -> bool:
         return self.mask is None
 
-    def recv_mask(self):
+    def recv_mask(self) -> None:
         self.mask = self.recv_strict(4) if self.has_mask() else ""
 
-    def recv_frame(self):
+    def recv_frame(self) -> ABNF:
 
         with self.lock:
             # Header
             if self.has_received_header():
                 self.recv_header()
             (fin, rsv1, rsv2, rsv3, opcode, has_mask, _) = self.header
 
@@ -382,42 +382,42 @@
         else:
             self.recv_buffer = [unified[bufsize:]]
             return unified[:bufsize]
 
 
 class continuous_frame:
 
-    def __init__(self, fire_cont_frame, skip_utf8_validation):
+    def __init__(self, fire_cont_frame: bool, skip_utf8_validation: bool) -> None:
         self.fire_cont_frame = fire_cont_frame
         self.skip_utf8_validation = skip_utf8_validation
         self.cont_data = None
         self.recving_frames = None
 
-    def validate(self, frame):
+    def validate(self, frame: ABNF) -> None:
         if not self.recving_frames and frame.opcode == ABNF.OPCODE_CONT:
             raise WebSocketProtocolException("Illegal frame")
         if self.recving_frames and \
                 frame.opcode in (ABNF.OPCODE_TEXT, ABNF.OPCODE_BINARY):
             raise WebSocketProtocolException("Illegal frame")
 
-    def add(self, frame):
+    def add(self, frame: ABNF) -> None:
         if self.cont_data:
             self.cont_data[1] += frame.data
         else:
             if frame.opcode in (ABNF.OPCODE_TEXT, ABNF.OPCODE_BINARY):
                 self.recving_frames = frame.opcode
             self.cont_data = [frame.opcode, frame.data]
 
         if frame.fin:
             self.recving_frames = None
 
-    def is_fire(self, frame):
+    def is_fire(self, frame: ABNF) -> bool or int:
         return frame.fin or self.fire_cont_frame
 
-    def extract(self, frame):
+    def extract(self, frame: ABNF) -> list:
         data = self.cont_data
         self.cont_data = None
         frame.data = data[1]
         if not self.fire_cont_frame and data[0] == ABNF.OPCODE_TEXT and not self.skip_utf8_validation and not validate_utf8(frame.data):
             raise WebSocketPayloadException(
                 "cannot decode: " + repr(frame.data))
```

### Comparing `websocket-client-1.5.1/websocket/_app.py` & `websocket-client-1.5.2/websocket/_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import inspect
 import selectors
 import sys
 import threading
 import time
 import traceback
+import socket
+
+from typing import Callable, Any
 
 from . import _logging
 from ._abnf import ABNF
 from ._url import parse_url
 from ._core import WebSocket, getdefaulttimeout
 from ._exceptions import *
 
@@ -31,45 +34,46 @@
 """
 
 __all__ = ["WebSocketApp"]
 
 RECONNECT = 0
 
 
-def setReconnect(reconnectInterval):
+def setReconnect(reconnectInterval: int) -> None:
     global RECONNECT
     RECONNECT = reconnectInterval
 
 
 class DispatcherBase:
     """
     DispatcherBase
     """
-    def __init__(self, app, ping_timeout):
+    def __init__(self, app: Any, ping_timeout: int or float) -> None:
         self.app = app
         self.ping_timeout = ping_timeout
 
-    def timeout(self, seconds, callback):
+    def timeout(self, seconds: int, callback: Callable) -> None:
         time.sleep(seconds)
         callback()
 
-    def reconnect(self, seconds, reconnector):
+    def reconnect(self, seconds: int, reconnector: Callable) -> None:
         try:
-            _logging.info("reconnect() - retrying in %s seconds [%s frames in stack]" % (seconds, len(inspect.stack())))
+            _logging.info("reconnect() - retrying in {seconds_count} seconds [{frame_count} frames in stack]".format(
+                seconds_count=seconds, frame_count=len(inspect.stack())))
             time.sleep(seconds)
             reconnector(reconnecting=True)
         except KeyboardInterrupt as e:
-            _logging.info("User exited %s" % (e,))
+            _logging.info("User exited {err}".format(err=e))
 
 
 class Dispatcher(DispatcherBase):
     """
     Dispatcher
     """
-    def read(self, sock, read_callback, check_callback):
+    def read(self, sock: socket, read_callback: Callable, check_callback: Callable) -> None:
         while self.app.keep_running:
             sel = selectors.DefaultSelector()
             sel.register(self.app.sock.sock, selectors.EVENT_READ)
 
             r = sel.select(self.ping_timeout)
             if r:
                 if not read_callback():
@@ -78,23 +82,23 @@
             sel.close()
 
 
 class SSLDispatcher(DispatcherBase):
     """
     SSLDispatcher
     """
-    def read(self, sock, read_callback, check_callback):
+    def read(self, sock: socket, read_callback: Callable, check_callback: Callable) -> None:
         while self.app.keep_running:
             r = self.select()
             if r:
                 if not read_callback():
                     break
             check_callback()
 
-    def select(self):
+    def select(self) -> list:
         sock = self.app.sock.sock
         if sock.pending():
             return [sock,]
 
         sel = selectors.DefaultSelector()
         sel.register(sock, selectors.EVENT_READ)
 
@@ -105,44 +109,44 @@
             return r[0][0]
 
 
 class WrappedDispatcher:
     """
     WrappedDispatcher
     """
-    def __init__(self, app, ping_timeout, dispatcher):
+    def __init__(self, app, ping_timeout: int or float, dispatcher: Dispatcher) -> None:
         self.app = app
         self.ping_timeout = ping_timeout
         self.dispatcher = dispatcher
         dispatcher.signal(2, dispatcher.abort)  # keyboard interrupt
 
-    def read(self, sock, read_callback, check_callback):
+    def read(self, sock: socket, read_callback: Callable, check_callback: Callable) -> None:
         self.dispatcher.read(sock, read_callback)
         self.ping_timeout and self.timeout(self.ping_timeout, check_callback)
 
-    def timeout(self, seconds, callback):
+    def timeout(self, seconds: int, callback: Callable) -> None:
         self.dispatcher.timeout(seconds, callback)
 
-    def reconnect(self, seconds, reconnector):
+    def reconnect(self, seconds: int, reconnector: Callable) -> None:
         self.timeout(seconds, reconnector)
 
 
 class WebSocketApp:
     """
     Higher level of APIs are provided. The interface is like JavaScript WebSocket object.
     """
 
-    def __init__(self, url, header=None,
-                 on_open=None, on_message=None, on_error=None,
-                 on_close=None, on_ping=None, on_pong=None,
-                 on_cont_message=None,
-                 keep_running=True, get_mask_key=None, cookie=None,
-                 subprotocols=None,
-                 on_data=None,
-                 socket=None):
+    def __init__(self, url: str, header: list or dict = None,
+                 on_open: Callable = None, on_message: Callable = None, on_error: Callable = None,
+                 on_close: Callable = None, on_ping: Callable = None, on_pong: Callable = None,
+                 on_cont_message: Callable = None,
+                 keep_running: bool = True, get_mask_key: Callable = None, cookie: str = None,
+                 subprotocols: list = None,
+                 on_data: Callable = None,
+                 socket: socket = None) -> None:
         """
         WebSocketApp initialization
 
         Parameters
         ----------
         url: str
             Websocket url.
@@ -219,15 +223,15 @@
         self.ping_interval = 0
         self.ping_timeout = None
         self.ping_payload = ""
         self.subprotocols = subprotocols
         self.prepared_socket = socket
         self.has_errored = False
 
-    def send(self, data, opcode=ABNF.OPCODE_TEXT):
+    def send(self, data: str, opcode: int = ABNF.OPCODE_TEXT) -> None:
         """
         send message
 
         Parameters
         ----------
         data: str
             Message to send. If you set opcode to OPCODE_TEXT,
@@ -236,58 +240,58 @@
             Operation code of data. Default is OPCODE_TEXT.
         """
 
         if not self.sock or self.sock.send(data, opcode) == 0:
             raise WebSocketConnectionClosedException(
                 "Connection is already closed.")
 
-    def close(self, **kwargs):
+    def close(self, **kwargs) -> None:
         """
         Close websocket connection.
         """
         self.keep_running = False
         if self.sock:
             self.sock.close(**kwargs)
             self.sock = None
 
-    def _start_ping_thread(self):
+    def _start_ping_thread(self) -> None:
         self.last_ping_tm = self.last_pong_tm = 0
         self.stop_ping = threading.Event()
         self.ping_thread = threading.Thread(target=self._send_ping)
         self.ping_thread.daemon = True
         self.ping_thread.start()
 
-    def _stop_ping_thread(self):
+    def _stop_ping_thread(self) -> None:
         if self.stop_ping:
             self.stop_ping.set()
         if self.ping_thread and self.ping_thread.is_alive():
             self.ping_thread.join(3)
         self.last_ping_tm = self.last_pong_tm = 0
 
-    def _send_ping(self):
+    def _send_ping(self) -> None:
         if self.stop_ping.wait(self.ping_interval):
             return
         while not self.stop_ping.wait(self.ping_interval):
             if self.sock:
                 self.last_ping_tm = time.time()
                 try:
                     _logging.debug("Sending ping")
                     self.sock.ping(self.ping_payload)
-                except Exception as ex:
-                    _logging.debug("Failed to send ping: %s", ex)
+                except Exception as e:
+                    _logging.debug("Failed to send ping: {err}".format(err=e))
 
-    def run_forever(self, sockopt=None, sslopt=None,
-                    ping_interval=0, ping_timeout=None,
-                    ping_payload="",
-                    http_proxy_host=None, http_proxy_port=None,
-                    http_no_proxy=None, http_proxy_auth=None,
-                    http_proxy_timeout=None,
-                    skip_utf8_validation=False,
-                    host=None, origin=None, dispatcher=None,
-                    suppress_origin=False, proxy_type=None, reconnect=None):
+    def run_forever(self, sockopt: tuple = None, sslopt: dict = None,
+                    ping_interval: int or float = 0, ping_timeout: int or float = None,
+                    ping_payload: str = "",
+                    http_proxy_host: str = None, http_proxy_port: int or str = None,
+                    http_no_proxy: list = None, http_proxy_auth: tuple = None,
+                    http_proxy_timeout: int or float = None,
+                    skip_utf8_validation: bool = False,
+                    host: str = None, origin: str = None, dispatcher: Dispatcher = None,
+                    suppress_origin: bool = False, proxy_type: str = None, reconnect: int = None) -> bool:
         """
         Run event loop for WebSocket framework.
 
         This loop is an infinite loop and is alive while websocket is available.
 
         Parameters
         ----------
@@ -354,15 +358,15 @@
             raise WebSocketException("socket is already opened")
 
         self.ping_interval = ping_interval
         self.ping_timeout = ping_timeout
         self.ping_payload = ping_payload
         self.keep_running = True
 
-        def teardown(close_frame=None):
+        def teardown(close_frame: ABNF = None) -> None:
             """
             Tears down the connection.
 
             Parameters
             ----------
             close_frame: ABNF frame
                 If close_frame is set, the on_close handler is invoked
@@ -376,15 +380,15 @@
             close_status_code, close_reason = self._get_close_args(
                 close_frame if close_frame else None)
             self.sock = None
 
             # Finally call the callback AFTER all teardown is complete
             self._callback(self.on_close, close_status_code, close_reason)
 
-        def setSock(reconnecting=False):
+        def setSock(reconnecting: bool = False) -> None:
             if reconnecting and self.sock:
                 self.sock.shutdown()
 
             self.sock = WebSocket(
                 self.get_mask_key, sockopt=sockopt, sslopt=sslopt,
                 fire_cont_frame=self.on_cont_message is not None,
                 skip_utf8_validation=skip_utf8_validation,
@@ -408,15 +412,15 @@
 
                 self._callback(self.on_open)
 
                 dispatcher.read(self.sock.sock, read, check)
             except (WebSocketConnectionClosedException, ConnectionRefusedError, KeyboardInterrupt, SystemExit, Exception) as e:
                 handleDisconnect(e, reconnecting)
 
-        def read():
+        def read() -> bool:
             if not self.keep_running:
                 return teardown()
 
             try:
                 op_code, frame = self.sock.recv_data_frame(True)
             except (WebSocketConnectionClosedException, KeyboardInterrupt) as e:
                 if custom_dispatcher:
@@ -441,67 +445,67 @@
                 if op_code == ABNF.OPCODE_TEXT and not skip_utf8_validation:
                     data = data.decode("utf-8")
                 self._callback(self.on_data, data, frame.opcode, True)
                 self._callback(self.on_message, data)
 
             return True
 
-        def check():
+        def check() -> bool:
             if (self.ping_timeout):
                 has_timeout_expired = time.time() - self.last_ping_tm > self.ping_timeout
                 has_pong_not_arrived_after_last_ping = self.last_pong_tm - self.last_ping_tm < 0
                 has_pong_arrived_too_late = self.last_pong_tm - self.last_ping_tm > self.ping_timeout
 
                 if (self.last_ping_tm and
                         has_timeout_expired and
                         (has_pong_not_arrived_after_last_ping or has_pong_arrived_too_late)):
                     raise WebSocketTimeoutException("ping/pong timed out")
             return True
 
-        def handleDisconnect(e, reconnecting=False):
+        def handleDisconnect(e: Exception, reconnecting: bool = False) -> bool:
             self.has_errored = True
             self._stop_ping_thread()
             if not reconnecting:
                 self._callback(self.on_error, e)
 
             if isinstance(e, (KeyboardInterrupt, SystemExit)):
                 teardown()
                 # Propagate further
                 raise
 
             if reconnect:
-                _logging.info("%s - reconnect" % e)
+                _logging.info("{err} - reconnect".format(err=e))
                 if custom_dispatcher:
-                    _logging.debug("Calling custom dispatcher reconnect [%s frames in stack]" % len(inspect.stack()))
+                    _logging.debug("Calling custom dispatcher reconnect [{frame_count} frames in stack]".format(frame_count=len(inspect.stack())))
                     dispatcher.reconnect(reconnect, setSock)
             else:
-                _logging.error("%s - goodbye" % e)
+                _logging.error("{err} - goodbye".format(err=e))
                 teardown()
 
         custom_dispatcher = bool(dispatcher)
         dispatcher = self.create_dispatcher(ping_timeout, dispatcher, parse_url(self.url)[3])
 
         setSock()
         if not custom_dispatcher and reconnect:
             while self.keep_running:
-                _logging.debug("Calling dispatcher reconnect [%s frames in stack]" % len(inspect.stack()))
+                _logging.debug("Calling dispatcher reconnect [{frame_count} frames in stack]".format(frame_count=len(inspect.stack())))
                 dispatcher.reconnect(reconnect, setSock)
 
         return self.has_errored
 
-    def create_dispatcher(self, ping_timeout, dispatcher=None, is_ssl=False):
+    def create_dispatcher(self, ping_timeout: int, dispatcher: Dispatcher = None, is_ssl: bool = False) -> DispatcherBase:
         if dispatcher:  # If custom dispatcher is set, use WrappedDispatcher
             return WrappedDispatcher(self, ping_timeout, dispatcher)
         timeout = ping_timeout or 10
         if is_ssl:
             return SSLDispatcher(self, timeout)
 
         return Dispatcher(self, timeout)
 
-    def _get_close_args(self, close_frame):
+    def _get_close_args(self, close_frame: ABNF) -> list:
         """
         _get_close_args extracts the close code and reason from the close body
         if it exists (RFC6455 says WebSocket Connection Close Code is optional)
         """
         # Need to catch the case where close_frame is None
         # Otherwise the following if statement causes an error
         if not self.on_close or not close_frame:
@@ -512,16 +516,16 @@
             close_status_code = 256 * close_frame.data[0] + close_frame.data[1]
             reason = close_frame.data[2:].decode('utf-8')
             return [close_status_code, reason]
         else:
             # Most likely reached this because len(close_frame_data.data) < 2
             return [None, None]
 
-    def _callback(self, callback, *args):
+    def _callback(self, callback: Callable, *args: tuple) -> None:
         if callback:
             try:
                 callback(self, *args)
 
             except Exception as e:
-                _logging.error("error from callback {}: {}".format(callback, e))
+                _logging.error("error from callback {callback}: {err}".format(callback=callback, err=e))
                 if self.on_error:
                     self.on_error(self, e)
```

### Comparing `websocket-client-1.5.1/websocket/_cookiejar.py` & `websocket-client-1.5.2/websocket/_cookiejar.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,42 +17,42 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
 class SimpleCookieJar:
-    def __init__(self):
+    def __init__(self) -> None:
         self.jar = dict()
 
-    def add(self, set_cookie):
+    def add(self, set_cookie: str) -> None:
         if set_cookie:
             simpleCookie = http.cookies.SimpleCookie(set_cookie)
 
             for k, v in simpleCookie.items():
                 domain = v.get("domain")
                 if domain:
                     if not domain.startswith("."):
                         domain = "." + domain
                     cookie = self.jar.get(domain) if self.jar.get(domain) else http.cookies.SimpleCookie()
                     cookie.update(simpleCookie)
                     self.jar[domain.lower()] = cookie
 
-    def set(self, set_cookie):
+    def set(self, set_cookie: str) -> None:
         if set_cookie:
             simpleCookie = http.cookies.SimpleCookie(set_cookie)
 
             for k, v in simpleCookie.items():
                 domain = v.get("domain")
                 if domain:
                     if not domain.startswith("."):
                         domain = "." + domain
                     self.jar[domain.lower()] = simpleCookie
 
-    def get(self, host):
+    def get(self, host: str) -> str:
         if not host:
             return ""
 
         cookies = []
         for domain, simpleCookie in self.jar.items():
             host = host.lower()
             if host.endswith(domain) or host == domain[1:]:
```

### Comparing `websocket-client-1.5.1/websocket/_core.py` & `websocket-client-1.5.2/websocket/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,15 +407,15 @@
             if (isEnabledForTrace()):
                 trace("++Rcv raw: " + repr(frame.format()))
                 trace("++Rcv decoded: " + frame.__str__())
             if not frame:
                 # handle error:
                 # 'NoneType' object has no attribute 'opcode'
                 raise WebSocketProtocolException(
-                    "Not a valid frame %s" % frame)
+                    "Not a valid frame {frame}".format(frame=frame))
             elif frame.opcode in (ABNF.OPCODE_TEXT, ABNF.OPCODE_BINARY, ABNF.OPCODE_CONT):
                 self.cont_frame.validate(frame)
                 self.cont_frame.add(frame)
 
                 if self.cont_frame.is_fire(frame):
                     return self.cont_frame.extract(frame)
```

### Comparing `websocket-client-1.5.1/websocket/_exceptions.py` & `websocket-client-1.5.2/websocket/_exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,19 +62,19 @@
 
 
 class WebSocketBadStatusException(WebSocketException):
     """
     WebSocketBadStatusException will be raised when we get bad handshake status code.
     """
 
-    def __init__(self, message, status_code, status_message=None, resp_headers=None):
-        msg = message % (status_code, status_message)
-        super().__init__(msg)
+    def __init__(self, message, status_code, status_message=None, resp_headers=None, resp_body=None):
+        super().__init__(message)
         self.status_code = status_code
         self.resp_headers = resp_headers
+        self.resp_body = resp_body
 
 
 class WebSocketAddressException(WebSocketException):
     """
     If the websocket address info cannot be found, this exception will be raised.
     """
     pass
```

### Comparing `websocket-client-1.5.1/websocket/_handshake.py` & `websocket-client-1.5.2/websocket/_handshake.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,56 +70,56 @@
         return '[' + hostname + ']'
 
     return hostname
 
 
 def _get_handshake_headers(resource, url, host, port, options):
     headers = [
-        "GET %s HTTP/1.1" % resource,
+        "GET {resource} HTTP/1.1".format(resource=resource),
         "Upgrade: websocket"
     ]
     if port == 80 or port == 443:
         hostport = _pack_hostname(host)
     else:
-        hostport = "%s:%d" % (_pack_hostname(host), port)
+        hostport = "{h}:{p}".format(h=_pack_hostname(host), p=port)
     if options.get("host"):
-        headers.append("Host: %s" % options["host"])
+        headers.append("Host: {h}".format(h=options["host"]))
     else:
-        headers.append("Host: %s" % hostport)
+        headers.append("Host: {hp}".format(hp=hostport))
 
     # scheme indicates whether http or https is used in Origin
     # The same approach is used in parse_url of _url.py to set default port
     scheme, url = url.split(":", 1)
     if not options.get("suppress_origin"):
         if "origin" in options and options["origin"] is not None:
-            headers.append("Origin: %s" % options["origin"])
+            headers.append("Origin: {origin}".format(origin=options["origin"]))
         elif scheme == "wss":
-            headers.append("Origin: https://%s" % hostport)
+            headers.append("Origin: https://{hp}".format(hp=hostport))
         else:
-            headers.append("Origin: http://%s" % hostport)
+            headers.append("Origin: http://{hp}".format(hp=hostport))
 
     key = _create_sec_websocket_key()
 
     # Append Sec-WebSocket-Key & Sec-WebSocket-Version if not manually specified
     if not options.get('header') or 'Sec-WebSocket-Key' not in options['header']:
-        headers.append("Sec-WebSocket-Key: %s" % key)
+        headers.append("Sec-WebSocket-Key: {key}".format(key=key))
     else:
         key = options['header']['Sec-WebSocket-Key']
 
     if not options.get('header') or 'Sec-WebSocket-Version' not in options['header']:
-        headers.append("Sec-WebSocket-Version: %s" % VERSION)
+        headers.append("Sec-WebSocket-Version: {version}".format(version=VERSION))
 
     if not options.get('connection'):
         headers.append('Connection: Upgrade')
     else:
         headers.append(options['connection'])
 
     subprotocols = options.get("subprotocols")
     if subprotocols:
-        headers.append("Sec-WebSocket-Protocol: %s" % ",".join(subprotocols))
+        headers.append("Sec-WebSocket-Protocol: {protocols}".format(protocols=",".join(subprotocols)))
 
     header = options.get("header")
     if header:
         if isinstance(header, dict):
             header = [
                 ": ".join([k, v])
                 for k, v in header.items()
@@ -129,26 +129,27 @@
 
     server_cookie = CookieJar.get(host)
     client_cookie = options.get("cookie", None)
 
     cookie = "; ".join(filter(None, [server_cookie, client_cookie]))
 
     if cookie:
-        headers.append("Cookie: %s" % cookie)
+        headers.append("Cookie: {cookie}".format(cookie=cookie))
 
     headers.append("")
     headers.append("")
 
     return headers, key
 
 
 def _get_resp_headers(sock, success_statuses=SUCCESS_STATUSES):
     status, resp_headers, status_message = read_headers(sock)
     if status not in success_statuses:
-        raise WebSocketBadStatusException("Handshake status %d %s", status, status_message, resp_headers)
+        response_body = sock.recv(int(resp_headers['content-length']))  # read the body of the HTTP error message response and include it in the exception
+        raise WebSocketBadStatusException("Handshake status {status} {message} -+-+- {headers} -+-+- {body}".format(status=status, message=status_message, headers=resp_headers, body=response_body), status, status_message, resp_headers, response_body)
     return status, resp_headers
 
 
 _HEADERS_TO_CHECK = {
     "upgrade": "websocket",
     "connection": "upgrade",
 }
```

### Comparing `websocket-client-1.5.1/websocket/_http.py` & `websocket-client-1.5.2/websocket/_http.py`

 * *Files 3% similar despite different names*

```diff
@@ -271,37 +271,37 @@
     sock = _wrap_sni_socket(sock, sslopt, hostname, check_hostname)
 
     return sock
 
 
 def _tunnel(sock, host, port, auth):
     debug("Connecting proxy...")
-    connect_header = "CONNECT %s:%d HTTP/1.1\r\n" % (host, port)
-    connect_header += "Host: %s:%d\r\n" % (host, port)
+    connect_header = "CONNECT {h}:{p} HTTP/1.1\r\n".format(h=host, p=port)
+    connect_header += "Host: {h}:{p}\r\n".format(h=host, p=port)
 
     # TODO: support digest auth.
     if auth and auth[0]:
         auth_str = auth[0]
         if auth[1]:
             auth_str += ":" + auth[1]
         encoded_str = base64encode(auth_str.encode()).strip().decode().replace('\n', '')
-        connect_header += "Proxy-Authorization: Basic %s\r\n" % encoded_str
+        connect_header += "Proxy-Authorization: Basic {str}\r\n".format(str=encoded_str)
     connect_header += "\r\n"
     dump("request header", connect_header)
 
     send(sock, connect_header)
 
     try:
         status, resp_headers, status_message = read_headers(sock)
     except Exception as e:
         raise WebSocketProxyException(str(e))
 
     if status != 200:
         raise WebSocketProxyException(
-            "failed CONNECT via proxy status: %r" % status)
+            "failed CONNECT via proxy status: {status}".format(status=status))
 
     return sock
 
 
 def read_headers(sock):
     status = None
     status_message = None
```

### Comparing `websocket-client-1.5.1/websocket/_logging.py` & `websocket-client-1.5.2/websocket/_logging.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,26 +20,28 @@
 """
 
 _logger = logging.getLogger('websocket')
 try:
     from logging import NullHandler
 except ImportError:
     class NullHandler(logging.Handler):
-        def emit(self, record):
+        def emit(self, record) -> None:
             pass
 
 _logger.addHandler(NullHandler())
 
 _traceEnabled = False
 
 __all__ = ["enableTrace", "dump", "error", "warning", "debug", "trace",
            "isEnabledForError", "isEnabledForDebug", "isEnabledForTrace"]
 
 
-def enableTrace(traceable, handler=logging.StreamHandler(), level="DEBUG"):
+def enableTrace(traceable: bool,
+                handler: logging.StreamHandler = logging.StreamHandler(),
+                level: str = "DEBUG") -> None:
     """
     Turn on/off the traceability.
 
     Parameters
     ----------
     traceable: bool
         If set to True, traceability is enabled.
@@ -47,45 +49,45 @@
     global _traceEnabled
     _traceEnabled = traceable
     if traceable:
         _logger.addHandler(handler)
         _logger.setLevel(getattr(logging, level))
 
 
-def dump(title, message):
+def dump(title: str, message: str) -> None:
     if _traceEnabled:
         _logger.debug("--- " + title + " ---")
         _logger.debug(message)
         _logger.debug("-----------------------")
 
 
-def error(msg):
+def error(msg: str) -> None:
     _logger.error(msg)
 
 
-def warning(msg):
+def warning(msg: str) -> None:
     _logger.warning(msg)
 
 
-def debug(msg):
+def debug(msg: str) -> None:
     _logger.debug(msg)
 
 
-def info(msg):
+def info(msg: str) -> None:
     _logger.info(msg)
 
 
-def trace(msg):
+def trace(msg: str) -> None:
     if _traceEnabled:
         _logger.debug(msg)
 
 
-def isEnabledForError():
+def isEnabledForError() -> bool:
     return _logger.isEnabledFor(logging.ERROR)
 
 
-def isEnabledForDebug():
+def isEnabledForDebug() -> bool:
     return _logger.isEnabledFor(logging.DEBUG)
 
 
-def isEnabledForTrace():
+def isEnabledForTrace() -> bool:
     return _traceEnabled
```

### Comparing `websocket-client-1.5.1/websocket/_socket.py` & `websocket-client-1.5.2/websocket/_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,50 +39,50 @@
 
 __all__ = ["DEFAULT_SOCKET_OPTION", "sock_opt", "setdefaulttimeout", "getdefaulttimeout",
            "recv", "recv_line", "send"]
 
 
 class sock_opt:
 
-    def __init__(self, sockopt, sslopt):
+    def __init__(self, sockopt: list, sslopt: dict) -> None:
         if sockopt is None:
             sockopt = []
         if sslopt is None:
             sslopt = {}
         self.sockopt = sockopt
         self.sslopt = sslopt
         self.timeout = None
 
 
-def setdefaulttimeout(timeout):
+def setdefaulttimeout(timeout: int or float) -> None:
     """
     Set the global timeout setting to connect.
 
     Parameters
     ----------
     timeout: int or float
         default socket timeout time (in seconds)
     """
     global _default_timeout
     _default_timeout = timeout
 
 
-def getdefaulttimeout():
+def getdefaulttimeout() -> int or float:
     """
     Get default timeout
 
     Returns
     ----------
     _default_timeout: int or float
         Return the global timeout setting (in seconds) to connect.
     """
     return _default_timeout
 
 
-def recv(sock, bufsize):
+def recv(sock: socket, bufsize: int) -> bytes:
     if not sock:
         raise WebSocketConnectionClosedException("socket is already closed.")
 
     def _recv():
         try:
             return sock.recv(bufsize)
         except SSLWantReadError:
@@ -121,25 +121,25 @@
     if not bytes_:
         raise WebSocketConnectionClosedException(
             "Connection to remote host was lost.")
 
     return bytes_
 
 
-def recv_line(sock):
+def recv_line(sock: socket) -> bytes:
     line = []
     while True:
         c = recv(sock, 1)
         line.append(c)
         if c == b'\n':
             break
     return b''.join(line)
 
 
-def send(sock, data):
+def send(sock: socket, data: bytes) -> int:
     if isinstance(data, str):
         data = data.encode('utf-8')
 
     if not sock:
         raise WebSocketConnectionClosedException("socket is already closed.")
 
     def _send():
```

### Comparing `websocket-client-1.5.1/websocket/_ssl_compat.py` & `websocket-client-1.5.2/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.1/websocket/_url.py` & `websocket-client-1.5.2/websocket/_url.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 __all__ = ["parse_url", "get_proxy_info"]
 
 
-def parse_url(url):
+def parse_url(url: str) -> tuple:
     """
     parse url and the result is tuple of
     (hostname, port, resource path and the flag of secure mode)
 
     Parameters
     ----------
     url: str
@@ -71,41 +71,41 @@
 
     return hostname, port, resource, is_secure
 
 
 DEFAULT_NO_PROXY_HOST = ["localhost", "127.0.0.1"]
 
 
-def _is_ip_address(addr):
+def _is_ip_address(addr: str) -> bool:
     try:
         socket.inet_aton(addr)
     except socket.error:
         return False
     else:
         return True
 
 
-def _is_subnet_address(hostname):
+def _is_subnet_address(hostname: str) -> bool:
     try:
         addr, netmask = hostname.split("/")
         return _is_ip_address(addr) and 0 <= int(netmask) < 32
     except ValueError:
         return False
 
 
-def _is_address_in_network(ip, net):
+def _is_address_in_network(ip: str, net: str) -> bool:
     ipaddr = struct.unpack('!I', socket.inet_aton(ip))[0]
     netaddr, netmask = net.split('/')
     netaddr = struct.unpack('!I', socket.inet_aton(netaddr))[0]
 
     netmask = (0xFFFFFFFF << (32 - int(netmask))) & 0xFFFFFFFF
     return ipaddr & netmask == netaddr
 
 
-def _is_no_proxy_host(hostname, no_proxy):
+def _is_no_proxy_host(hostname: str, no_proxy: list) -> bool:
     if not no_proxy:
         v = os.environ.get("no_proxy", os.environ.get("NO_PROXY", "")).replace(" ", "")
         if v:
             no_proxy = v.split(",")
     if not no_proxy:
         no_proxy = DEFAULT_NO_PROXY_HOST
 
@@ -118,16 +118,16 @@
     for domain in [domain for domain in no_proxy if domain.startswith('.')]:
         if hostname.endswith(domain):
             return True
     return False
 
 
 def get_proxy_info(
-        hostname, is_secure, proxy_host=None, proxy_port=0, proxy_auth=None,
-        no_proxy=None, proxy_type='http'):
+        hostname: str, is_secure: bool, proxy_host: str = None, proxy_port: int = 0, proxy_auth: tuple = None,
+        no_proxy: list = None, proxy_type: str = 'http') -> tuple:
     """
     Try to retrieve proxy host and port from environment
     if not provided in options.
     Result is (proxy_host, proxy_port, proxy_auth).
     proxy_auth is tuple of username and password
     of proxy authentication information.
```

### Comparing `websocket-client-1.5.1/websocket/_utils.py` & `websocket-client-1.5.2/websocket/_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 limitations under the License.
 """
 __all__ = ["NoLock", "validate_utf8", "extract_err_message", "extract_error_code"]
 
 
 class NoLock:
 
-    def __enter__(self):
+    def __enter__(self) -> None:
         pass
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(self, exc_type, exc_value, traceback) -> None:
         pass
 
 
 try:
     # If wsaccel is available we use compiled routines to validate UTF-8
     # strings.
     from wsaccel.utf8validator import Utf8Validator
 
-    def _validate_utf8(utfbytes):
+    def _validate_utf8(utfbytes: bytes) -> bool:
         return Utf8Validator().validate(utfbytes)[0]
 
 except ImportError:
     # UTF-8 validator
     # python implementation of http://bjoern.hoehrmann.de/utf-8/decoder/dfa/
 
     _UTF8_ACCEPT = 0
@@ -59,46 +59,46 @@
         # of a state of the automaton and a character class to a state.
         0,12,24,36,60,96,84,12,12,12,48,72, 12,12,12,12,12,12,12,12,12,12,12,12,
         12, 0,12,12,12,12,12, 0,12, 0,12,12, 12,24,12,12,12,12,12,24,12,24,12,12,
         12,12,12,12,12,12,12,24,12,12,12,12, 12,24,12,12,12,12,12,12,12,24,12,12,
         12,12,12,12,12,12,12,36,12,36,12,12, 12,36,12,12,12,12,12,36,12,36,12,12,
         12,36,12,12,12,12,12,12,12,12,12,12, ]
 
-    def _decode(state, codep, ch):
+    def _decode(state, codep, ch) -> tuple:
         tp = _UTF8D[ch]
 
         codep = (ch & 0x3f) | (codep << 6) if (
             state != _UTF8_ACCEPT) else (0xff >> tp) & ch
         state = _UTF8D[256 + state + tp]
 
         return state, codep
 
-    def _validate_utf8(utfbytes):
+    def _validate_utf8(utfbytes: bytes) -> bool:
         state = _UTF8_ACCEPT
         codep = 0
         for i in utfbytes:
             state, codep = _decode(state, codep, i)
             if state == _UTF8_REJECT:
                 return False
 
         return True
 
 
-def validate_utf8(utfbytes):
+def validate_utf8(utfbytes: str) -> bool:
     """
     validate utf8 byte string.
     utfbytes: utf byte string to check.
     return value: if valid utf8 string, return true. Otherwise, return false.
     """
     return _validate_utf8(utfbytes)
 
 
-def extract_err_message(exception):
+def extract_err_message(exception: Exception) -> str or None:
     if exception.args:
         return exception.args[0]
     else:
         return None
 
 
-def extract_error_code(exception):
+def extract_error_code(exception: Exception) -> int or None:
     if exception.args and len(exception.args) > 1:
         return exception.args[0] if isinstance(exception.args[0], int) else None
```

### Comparing `websocket-client-1.5.1/websocket/_wsdump.py` & `websocket-client-1.5.2/websocket/_wsdump.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,39 +33,39 @@
 
 try:
     import readline
 except ImportError:
     pass
 
 
-def get_encoding():
+def get_encoding() -> str:
     encoding = getattr(sys.stdin, "encoding", "")
     if not encoding:
         return "utf-8"
     else:
         return encoding.lower()
 
 
 OPCODE_DATA = (websocket.ABNF.OPCODE_TEXT, websocket.ABNF.OPCODE_BINARY)
 ENCODING = get_encoding()
 
 
 class VAction(argparse.Action):
 
-    def __call__(self, parser, args, values, option_string=None):
+    def __call__(self, parser: argparse.Namespace, args: tuple, values: str, option_string: str = None) -> None:
         if values is None:
             values = "1"
         try:
             values = int(values)
         except ValueError:
             values = values.count("v") + 1
         setattr(args, self.dest, values)
 
 
-def parse_args():
+def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(description="WebSocket Simple Dump Tool")
     parser.add_argument("url", metavar="ws_url",
                         help="websocket url. ex. ws://echo.websocket.events/")
     parser.add_argument("-p", "--proxy",
                         help="proxy url. ex. http://127.0.0.1:8080")
     parser.add_argument("-v", "--verbose", default=0, nargs='?', action=VAction,
                         dest="verbose",
@@ -89,50 +89,50 @@
                         help="Set custom headers. Use ',' as separator")
 
     return parser.parse_args()
 
 
 class RawInput:
 
-    def raw_input(self, prompt):
+    def raw_input(self, prompt: str = "") -> str:
         line = input(prompt)
 
         if ENCODING and ENCODING != "utf-8" and not isinstance(line, str):
             line = line.decode(ENCODING).encode("utf-8")
         elif isinstance(line, str):
             line = line.encode("utf-8")
 
         return line
 
 
 class InteractiveConsole(RawInput, code.InteractiveConsole):
 
-    def write(self, data):
+    def write(self, data: str) -> None:
         sys.stdout.write("\033[2K\033[E")
         # sys.stdout.write("\n")
         sys.stdout.write("\033[34m< " + data + "\033[39m")
         sys.stdout.write("\n> ")
         sys.stdout.flush()
 
-    def read(self):
+    def read(self) -> str:
         return self.raw_input("> ")
 
 
 class NonInteractive(RawInput):
 
-    def write(self, data):
+    def write(self, data: str) -> None:
         sys.stdout.write(data)
         sys.stdout.write("\n")
         sys.stdout.flush()
 
-    def read(self):
+    def read(self) -> str:
         return self.raw_input("")
 
 
-def main():
+def main() -> None:
     start_time = time.time()
     args = parse_args()
     if args.verbose > 1:
         websocket.enableTrace(True)
     options = {}
     if args.proxy:
         p = urlparse(args.proxy)
@@ -150,33 +150,33 @@
     ws = websocket.create_connection(args.url, sslopt=opts, **options)
     if args.raw:
         console = NonInteractive()
     else:
         console = InteractiveConsole()
         print("Press Ctrl+C to quit")
 
-    def recv():
+    def recv() -> tuple(int, str):
         try:
             frame = ws.recv_frame()
         except websocket.WebSocketException:
             return websocket.ABNF.OPCODE_CLOSE, None
         if not frame:
-            raise websocket.WebSocketException("Not a valid frame %s" % frame)
+            raise websocket.WebSocketException("Not a valid frame {frame}".format(frame=frame))
         elif frame.opcode in OPCODE_DATA:
             return frame.opcode, frame.data
         elif frame.opcode == websocket.ABNF.OPCODE_CLOSE:
             ws.send_close()
             return frame.opcode, None
         elif frame.opcode == websocket.ABNF.OPCODE_PING:
             ws.pong(frame.data)
             return frame.opcode, frame.data
 
         return frame.opcode, frame.data
 
-    def recv_ws():
+    def recv_ws() -> None:
         while True:
             opcode, data = recv()
             msg = None
             if opcode == websocket.ABNF.OPCODE_TEXT and isinstance(data, bytes):
                 data = str(data, "utf-8")
             if isinstance(data, bytes) and len(data) > 2 and data[:2] == b'\037\213':  # gzip magick
                 try:
@@ -189,15 +189,15 @@
                 except:
                     pass
 
             if isinstance(data, bytes):
                 data = repr(data)
 
             if args.verbose:
-                msg = "%s: %s" % (websocket.ABNF.OPCODE_MAP.get(opcode), data)
+                msg = "{opcode}: {data}".format(opcode=websocket.ABNF.OPCODE_MAP.get(opcode), data=data)
             else:
                 msg = data
 
             if msg is not None:
                 if args.timings:
                     console.write(str(time.time() - start_time) + ": " + msg)
                 else:
```

### Comparing `websocket-client-1.5.1/websocket/tests/test_abnf.py` & `websocket-client-1.5.2/websocket/tests/test_abnf.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.1/websocket/tests/test_app.py` & `websocket-client-1.5.2/websocket/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.1/websocket/tests/test_cookiejar.py` & `websocket-client-1.5.2/websocket/tests/test_cookiejar.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.1/websocket/tests/test_http.py` & `websocket-client-1.5.2/websocket/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.1/websocket/tests/test_url.py` & `websocket-client-1.5.2/websocket/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.1/websocket/tests/test_websocket.py` & `websocket-client-1.5.2/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.5.1/websocket_client.egg-info/PKG-INFO` & `websocket-client-1.5.2/websocket_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-client
-Version: 1.5.1
+Version: 1.5.2
 Summary: WebSocket client for Python with low level API options
 Home-page: https://github.com/websocket-client/websocket-client.git
 Download-URL: https://github.com/websocket-client/websocket-client/releases
 Author: liris
 Author-email: liris.pp@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://websocket-client.readthedocs.io/
```

### Comparing `websocket-client-1.5.1/websocket_client.egg-info/SOURCES.txt` & `websocket-client-1.5.2/websocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

