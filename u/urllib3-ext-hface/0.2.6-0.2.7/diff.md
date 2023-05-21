# Comparing `tmp/urllib3_ext_hface-0.2.6.tar.gz` & `tmp/urllib3_ext_hface-0.2.7.tar.gz`

## Comparing `urllib3_ext_hface-0.2.6.tar` & `urllib3_ext_hface-0.2.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/CHANGELOG.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/dev-requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/changelog.rst
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/cli.rst
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/common.rst
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/conf.py
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/connections.rst
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/facade.rst
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/index.rst
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/install.rst
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/intro.rst
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/license.rst
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/protocols.rst
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/_static/custom.css
--rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/docs/_static/hface.png
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/_configuration.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/_error_codes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/_typing.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/py.typed
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/events/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/events/_events.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/_factories.py
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/_protocols.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http1/_factories.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http1/_helpers.py
--rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http1/_protocol.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http2/_factories.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http2/_protocol.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http3/_factories.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http3/_protocol.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http3/_quic.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/tests/helpers.py
--rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/tests/test_http1.py
--rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/tests/test_http2.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/tests/test_integration.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/AUTHORS
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/NOTICE
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/README.rst
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/CHANGELOG.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/dev-requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/changelog.rst
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/cli.rst
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/common.rst
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/conf.py
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/connections.rst
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/facade.rst
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/index.rst
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/install.rst
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/intro.rst
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/license.rst
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/protocols.rst
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/_static/custom.css
+-rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/docs/_static/hface.png
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/_error_codes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/_typing.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/py.typed
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/events/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/events/_events.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/_factories.py
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http1/_factories.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http1/_helpers.py
+-rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http1/_protocol.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http2/_factories.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http2/_protocol.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http3/_factories.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http3/_protocol.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http3/_quic.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/tests/helpers.py
+-rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/tests/test_http1.py
+-rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/tests/test_http2.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/tests/test_integration.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/AUTHORS
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/NOTICE
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/README.rst
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.7/PKG-INFO
```

### Comparing `urllib3_ext_hface-0.2.6/CHANGELOG.rst` & `urllib3_ext_hface-0.2.7/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v0.2.7 (2023-05-21)
+--------
+
+* Remove undesired and miscalled ping() method in quic connection.
+
 v0.2.6 (2023-05-21)
 --------
 
 * Fix ``OverUDPProtocol`` not inheriting ``BaseProtocol``.
 
 v0.2.5 (2023-05-21)
 --------
```

### Comparing `urllib3_ext_hface-0.2.6/docs/cli.rst` & `urllib3_ext_hface-0.2.7/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/docs/common.rst` & `urllib3_ext_hface-0.2.7/docs/common.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/docs/conf.py` & `urllib3_ext_hface-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/docs/connections.rst` & `urllib3_ext_hface-0.2.7/docs/connections.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/docs/facade.rst` & `urllib3_ext_hface-0.2.7/docs/facade.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/docs/index.rst` & `urllib3_ext_hface-0.2.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/docs/install.rst` & `urllib3_ext_hface-0.2.7/docs/install.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/docs/intro.rst` & `urllib3_ext_hface-0.2.7/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/docs/protocols.rst` & `urllib3_ext_hface-0.2.7/docs/protocols.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/docs/_static/hface.png` & `urllib3_ext_hface-0.2.7/docs/_static/hface.png`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/__init__.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/_configuration.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/_error_codes.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/_typing.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/events/__init__.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/events/_events.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/__init__.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/_factories.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/_protocols.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http1/__init__.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http1/_factories.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http1/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http1/_helpers.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http1/_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http1/_protocol.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http1/_protocol.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http2/__init__.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http2/_factories.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http2/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http2/_protocol.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http2/_protocol.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http3/__init__.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http3/_factories.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http3/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http3/_protocol.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http3/_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
     def is_available(self) -> bool:
         # TODO: check concurrent stream limit
         return not self._terminated
 
     def has_expired(self) -> bool:
         # TODO: check that we do not run out of stream IDs.
-        self._quic.send_ping()
         return self._terminated
 
     @property
     def session_ticket(self) -> SessionTicket | None:
         return self._quic.tls.session_ticket if self._quic and self._quic.tls else None
 
     def get_available_stream_id(self) -> int:
```

### Comparing `urllib3_ext_hface-0.2.6/src/urllib3_ext_hface/protocols/http3/_quic.py` & `urllib3_ext_hface-0.2.7/src/urllib3_ext_hface/protocols/http3/_quic.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/tests/helpers.py` & `urllib3_ext_hface-0.2.7/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/tests/test_http1.py` & `urllib3_ext_hface-0.2.7/tests/test_http1.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/tests/test_http2.py` & `urllib3_ext_hface-0.2.7/tests/test_http2.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/tests/test_integration.py` & `urllib3_ext_hface-0.2.7/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/LICENSE` & `urllib3_ext_hface-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/NOTICE` & `urllib3_ext_hface-0.2.7/NOTICE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/README.rst` & `urllib3_ext_hface-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/pyproject.toml` & `urllib3_ext_hface-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.6/PKG-INFO` & `urllib3_ext_hface-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3-ext-hface
-Version: 0.2.6
+Version: 0.2.7
 Summary: urllib3 extension to support HTTP/1.1, HTTP/2 and HTTP/3 independently of Python httplib
 Project-URL: Changelog, https://github.com/Ousret/urllib3-ext-hface/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/Ousret/urllib3-ext-hface
 Project-URL: Issue tracker, https://github.com/Ousret/urllib3-ext-hface/issues
 Author-email: Miloslav Pojman <mpojman@akamai.com>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
```

