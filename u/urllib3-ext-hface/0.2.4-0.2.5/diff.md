# Comparing `tmp/urllib3_ext_hface-0.2.4.tar.gz` & `tmp/urllib3_ext_hface-0.2.5.tar.gz`

## Comparing `urllib3_ext_hface-0.2.4.tar` & `urllib3_ext_hface-0.2.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/CHANGELOG.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/dev-requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/changelog.rst
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/cli.rst
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/common.rst
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/conf.py
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/connections.rst
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/facade.rst
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/index.rst
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/install.rst
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/intro.rst
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/license.rst
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/protocols.rst
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/_static/custom.css
--rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/docs/_static/hface.png
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_configuration.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_error_codes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_typing.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/py.typed
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/events/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/events/_events.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/_factories.py
--rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/_protocols.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_factories.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_helpers.py
--rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_protocol.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/_factories.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/_protocol.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_factories.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_protocol.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_quic.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/tests/helpers.py
--rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/tests/test_http1.py
--rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/tests/test_http2.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/tests/test_integration.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/AUTHORS
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/NOTICE
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/README.rst
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/CHANGELOG.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/dev-requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/changelog.rst
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/cli.rst
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/common.rst
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/conf.py
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/connections.rst
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/facade.rst
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/index.rst
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/install.rst
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/intro.rst
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/license.rst
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/protocols.rst
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/_static/custom.css
+-rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/docs/_static/hface.png
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/_error_codes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/_typing.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/py.typed
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/events/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/events/_events.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/_factories.py
+-rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http1/_factories.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http1/_helpers.py
+-rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http1/_protocol.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http2/_factories.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http2/_protocol.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http3/_factories.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http3/_protocol.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http3/_quic.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/tests/helpers.py
+-rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/tests/test_http1.py
+-rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/tests/test_http2.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/tests/test_integration.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/AUTHORS
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/NOTICE
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/README.rst
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.5/PKG-INFO
```

### Comparing `urllib3_ext_hface-0.2.4/CHANGELOG.rst` & `urllib3_ext_hface-0.2.5/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v0.2.5 (2023-05-21)
+--------
+
+* Add getter for the ``SessionTicket`` provided by aioquic in ``HTTP3Protocol``.
+
 v0.2.4 (2023-05-20)
 --------
 
 * Enforce `bytes_to_send` and `bytes_received` for all abstract protocols.
 * Implement graceful close for ``HTTP2Protocol`` (GoAway packet).
 
 v0.2.3 (2023-05-14)
```

### Comparing `urllib3_ext_hface-0.2.4/docs/cli.rst` & `urllib3_ext_hface-0.2.5/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/docs/common.rst` & `urllib3_ext_hface-0.2.5/docs/common.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/docs/conf.py` & `urllib3_ext_hface-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/docs/connections.rst` & `urllib3_ext_hface-0.2.5/docs/connections.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/docs/facade.rst` & `urllib3_ext_hface-0.2.5/docs/facade.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/docs/index.rst` & `urllib3_ext_hface-0.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/docs/install.rst` & `urllib3_ext_hface-0.2.5/docs/install.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/docs/intro.rst` & `urllib3_ext_hface-0.2.5/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/docs/protocols.rst` & `urllib3_ext_hface-0.2.5/docs/protocols.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/docs/_static/hface.png` & `urllib3_ext_hface-0.2.5/docs/_static/hface.png`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/__init__.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_configuration.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_error_codes.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/_typing.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/events/__init__.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/events/_events.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/__init__.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/_factories.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/_protocols.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/_protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,19 @@
 
         This property can be used to assign UDP packets to QUIC connections.
 
         :return: a sequence of connection IDs
         """
         raise NotImplementedError
 
+    @property
+    @abstractmethod
+    def session_ticket(self) -> object | None:
+        raise NotImplementedError
+
 
 class HTTPProtocol(metaclass=ABCMeta):
     """
     Sans-IO representation of an HTTP connection
 
     """
```

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/__init__.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_factories.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http1/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_helpers.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http1/_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http1/_protocol.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http1/_protocol.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/__init__.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/_factories.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http2/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http2/_protocol.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http2/_protocol.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/__init__.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_factories.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http3/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_protocol.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http3/_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from typing import Iterable, Sequence
 
 import aioquic.h3.events as h3_events
 import aioquic.quic.events as quic_events
 from aioquic.h3.connection import H3Connection
 from aioquic.quic.configuration import QuicConfiguration
 from aioquic.quic.connection import QuicConnection
+from aioquic.tls import SessionTicket
 
 from ..._typing import AddressType, HeadersType
 from ...events import ConnectionTerminated, DataReceived, Event
 from ...events import HandshakeCompleted as _HandshakeCompleted
 from ...events import HeadersReceived, StreamResetReceived
 from .._protocols import HTTP3Protocol
 
@@ -54,14 +55,18 @@
         # TODO: check concurrent stream limit
         return not self._terminated
 
     def has_expired(self) -> bool:
         # TODO: check that we do not run out of stream IDs.
         return self._terminated
 
+    @property
+    def session_ticket(self) -> SessionTicket | None:
+        return self._quic.tls.session_ticket if self._quic and self._quic.tls else None
+
     def get_available_stream_id(self) -> int:
         return self._quic.get_next_available_stream_id()
 
     def submit_close(self, error_code: int = 0) -> None:
         # QUIC has two different frame types for closing the connection.
         # From RFC 9000 (QUIC: A UDP-Based Multiplexed and Secure Transport):
         #
```

### Comparing `urllib3_ext_hface-0.2.4/src/urllib3_ext_hface/protocols/http3/_quic.py` & `urllib3_ext_hface-0.2.5/src/urllib3_ext_hface/protocols/http3/_quic.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/tests/helpers.py` & `urllib3_ext_hface-0.2.5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/tests/test_http1.py` & `urllib3_ext_hface-0.2.5/tests/test_http1.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/tests/test_http2.py` & `urllib3_ext_hface-0.2.5/tests/test_http2.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/tests/test_integration.py` & `urllib3_ext_hface-0.2.5/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/LICENSE` & `urllib3_ext_hface-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/NOTICE` & `urllib3_ext_hface-0.2.5/NOTICE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/README.rst` & `urllib3_ext_hface-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/pyproject.toml` & `urllib3_ext_hface-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.4/PKG-INFO` & `urllib3_ext_hface-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3-ext-hface
-Version: 0.2.4
+Version: 0.2.5
 Summary: urllib3 extension to support HTTP/1.1, HTTP/2 and HTTP/3 independently of Python httplib
 Project-URL: Changelog, https://github.com/Ousret/urllib3-ext-hface/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/Ousret/urllib3-ext-hface
 Project-URL: Issue tracker, https://github.com/Ousret/urllib3-ext-hface/issues
 Author-email: Miloslav Pojman <mpojman@akamai.com>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
```

