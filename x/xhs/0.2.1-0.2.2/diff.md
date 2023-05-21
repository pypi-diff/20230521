# Comparing `tmp/xhs-0.2.1.tar.gz` & `tmp/xhs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.2.1.tar", last modified: Sat May 13 03:35:20 2023, max compression
+gzip compressed data, was "xhs-0.2.2.tar", last modified: Sun May 21 02:03:15 2023, max compression
```

## Comparing `xhs-0.2.1.tar` & `xhs-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 03:35:20.098182 xhs-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-13 03:35:06.000000 xhs-0.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-13 03:35:06.000000 xhs-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-13 03:35:06.000000 xhs-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-13 03:35:20.098182 xhs-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-13 03:35:06.000000 xhs-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-13 03:35:06.000000 xhs-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-13 03:35:20.098182 xhs-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-13 03:35:06.000000 xhs-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 03:35:20.094182 xhs-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-13 03:35:06.000000 xhs-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-13 03:35:06.000000 xhs-0.2.1/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-13 03:35:06.000000 xhs-0.2.1/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-13 03:35:06.000000 xhs-0.2.1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 03:35:20.098182 xhs-0.2.1/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-13 03:35:06.000000 xhs-0.2.1/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-13 03:35:06.000000 xhs-0.2.1/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-05-13 03:35:06.000000 xhs-0.2.1/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-13 03:35:06.000000 xhs-0.2.1/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-05-13 03:35:06.000000 xhs-0.2.1/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 03:35:20.098182 xhs-0.2.1/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-13 03:35:20.000000 xhs-0.2.1/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-13 03:35:20.000000 xhs-0.2.1/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 03:35:20.000000 xhs-0.2.1/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 03:35:19.000000 xhs-0.2.1/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-13 03:35:20.000000 xhs-0.2.1/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-13 03:35:20.000000 xhs-0.2.1/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:03:15.621158 xhs-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-21 02:03:04.000000 xhs-0.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-21 02:03:04.000000 xhs-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-21 02:03:04.000000 xhs-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-21 02:03:15.621158 xhs-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-21 02:03:04.000000 xhs-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-21 02:03:04.000000 xhs-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-21 02:03:15.621158 xhs-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-21 02:03:04.000000 xhs-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:03:15.621158 xhs-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-21 02:03:04.000000 xhs-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-21 02:03:04.000000 xhs-0.2.2/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-21 02:03:04.000000 xhs-0.2.2/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 02:03:04.000000 xhs-0.2.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:03:15.621158 xhs-0.2.2/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-21 02:03:04.000000 xhs-0.2.2/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-21 02:03:04.000000 xhs-0.2.2/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-05-21 02:03:04.000000 xhs-0.2.2/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-21 02:03:04.000000 xhs-0.2.2/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-05-21 02:03:04.000000 xhs-0.2.2/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:03:15.621158 xhs-0.2.2/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.2.1/CHANGELOG.md` & `xhs-0.2.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.2.2
+
+### Added
+
+- add a custom sign func to constructor
+
 ## 0.2.1
 
 ### Fixed
 
 - fixed get_note_by_id_from_html with video note parse error
 
 ## 0.2.0
```

### Comparing `xhs-0.2.1/LICENSE` & `xhs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.2.1/PKG-INFO` & `xhs-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.2.1
+Version: 0.2.2
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
@@ -36,35 +36,43 @@
 [![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
 [![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
 
 </div>
 
 > **Warning**
 >
-> I sincerely apologize for informing you that the sign is not functioning properly, indicating that certain APIs are experiencing issues. To address the anti-aliasing of the sign, I will devote time to further learning. 👋
->
-> This is in expriemental, so the api is not stable, every update should be cautious
+> The primary purpose of this repository is to practice my Python skills. It is important to note that web crawling may be considered illegal, and therefore, it is crucial to refrain from exerting any pressure or engaging in unauthorized activities on websites.
 
 **xhs** is a crawling tool designed to extract data from [xiaohongshu website](https://www.xiaohongshu.com/explore)
 
 ## Usage
 
 xhs is available on PyPI:
 
 ```console
 $ python -m pip install xhs
 ```
 
 basic usage:
 
 ```python
+import requests
 from xhs import FeedType, XhsClient
 
 cookie = "please get cookie in website"
-xhs_client = XhsClient(cookie)
+def sign(uri, data=None, a1=""):
+    """You can implement this sign function on your own."""
+    res = requests.post("http://127.0.0.1:5000/xhs/sign", json={
+        "uri": uri,
+        "data": data,
+        "a1": a1
+    })
+    return res.json()
+
+xhs_client = XhsClient(cookie, sign=sign)
 
 # get note info
 note_info = xhs_client.get_note_by_id("63db8819000000001a01ead1")
 
 # get user info
 user_info = xhs_client.get_user_info("5ff0e6410000000001008400")
 
@@ -86,15 +94,15 @@
 notes = xhs_client.get_user_all_notes("5c2766b500000000050283f1")
 
 # more functions in development
 ```
 
 Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
 
-use signature function:
+~~use signature function~~( it's useless ):
 
 ```python
 # sign get request
 >>> from xhs import help
 >>> help.sign("/api/sns/web/v1/user/otherinfo?target_user_id=5ff0e6410000000001008400")
 {'x-s': 'sYMlOB5W0YdvZBVvOBw6slZJZjM+ZgaUOlFisBwJslc3', 'x-t': '1683368960336', 'x-s-common': '2UQAPsHC+aIjqArjwjHjNsQhPsHCH0rjNsQhPaHCH0P1PjhIHjIj2eHjwjQgynEDJ74AHjIj2ePjwjQhyoPTqBPT49pjHjIj2ecjwjHUN0P1PaHVHdWMH0ijHjIj2eGjwjHl+0W
 APAGhw/GIPAP9HjIj2eqjwjQAnLMV/FHMpAm88o8ycS89/FQ7+d+VnDkyyDF3nf4YpLRVzfSAcd4tq9l0PUHVHdWhH0ijHjIj2eDjwjFAPAPU+eHMweDANsQhP/Zjw0bR'}
@@ -109,11 +117,7 @@
 >>> help.get_a1_and_web_id()
 ('187f09d3bc6wUrNpFbQ9Yc431AenpvlBJh2QIQahI50000261040', '12b49a1fd517aa8df85380e9961b6800')
 
 # get search_id parameter
 >>> help.get_search_id()
 '2BHU39J8HCTIW665YHFCW'
 ```
-
-## Donate
-
-[![](https://afdian.net/static/img/logo/logo.png)](https://afdian.net/a/reajason)
```

### Comparing `xhs-0.2.1/README.md` & `xhs-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,35 +11,43 @@
 [![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
 [![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
 
 </div>
 
 > **Warning**
 >
-> I sincerely apologize for informing you that the sign is not functioning properly, indicating that certain APIs are experiencing issues. To address the anti-aliasing of the sign, I will devote time to further learning. 👋
->
-> This is in expriemental, so the api is not stable, every update should be cautious
+> The primary purpose of this repository is to practice my Python skills. It is important to note that web crawling may be considered illegal, and therefore, it is crucial to refrain from exerting any pressure or engaging in unauthorized activities on websites.
 
 **xhs** is a crawling tool designed to extract data from [xiaohongshu website](https://www.xiaohongshu.com/explore)
 
 ## Usage
 
 xhs is available on PyPI:
 
 ```console
 $ python -m pip install xhs
 ```
 
 basic usage:
 
 ```python
+import requests
 from xhs import FeedType, XhsClient
 
 cookie = "please get cookie in website"
-xhs_client = XhsClient(cookie)
+def sign(uri, data=None, a1=""):
+    """You can implement this sign function on your own."""
+    res = requests.post("http://127.0.0.1:5000/xhs/sign", json={
+        "uri": uri,
+        "data": data,
+        "a1": a1
+    })
+    return res.json()
+
+xhs_client = XhsClient(cookie, sign=sign)
 
 # get note info
 note_info = xhs_client.get_note_by_id("63db8819000000001a01ead1")
 
 # get user info
 user_info = xhs_client.get_user_info("5ff0e6410000000001008400")
 
@@ -61,15 +69,15 @@
 notes = xhs_client.get_user_all_notes("5c2766b500000000050283f1")
 
 # more functions in development
 ```
 
 Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
 
-use signature function:
+~~use signature function~~( it's useless ):
 
 ```python
 # sign get request
 >>> from xhs import help
 >>> help.sign("/api/sns/web/v1/user/otherinfo?target_user_id=5ff0e6410000000001008400")
 {'x-s': 'sYMlOB5W0YdvZBVvOBw6slZJZjM+ZgaUOlFisBwJslc3', 'x-t': '1683368960336', 'x-s-common': '2UQAPsHC+aIjqArjwjHjNsQhPsHCH0rjNsQhPaHCH0P1PjhIHjIj2eHjwjQgynEDJ74AHjIj2ePjwjQhyoPTqBPT49pjHjIj2ecjwjHUN0P1PaHVHdWMH0ijHjIj2eGjwjHl+0W
 APAGhw/GIPAP9HjIj2eqjwjQAnLMV/FHMpAm88o8ycS89/FQ7+d+VnDkyyDF3nf4YpLRVzfSAcd4tq9l0PUHVHdWhH0ijHjIj2eDjwjFAPAPU+eHMweDANsQhP/Zjw0bR'}
@@ -84,11 +92,7 @@
 >>> help.get_a1_and_web_id()
 ('187f09d3bc6wUrNpFbQ9Yc431AenpvlBJh2QIQahI50000261040', '12b49a1fd517aa8df85380e9961b6800')
 
 # get search_id parameter
 >>> help.get_search_id()
 '2BHU39J8HCTIW665YHFCW'
 ```
-
-## Donate
-
-[![](https://afdian.net/static/img/logo/logo.png)](https://afdian.net/a/reajason)
```

### Comparing `xhs-0.2.1/setup.py` & `xhs-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.1/tests/__init__.py` & `xhs-0.2.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.1/tests/test_help.py` & `xhs-0.2.2/tests/test_help.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,16 @@
                      "target_user_id=5ff0e6410000000001008400")
     print(sign)
 
 
 def test_sign_get(header):
     uri = ("/api/sns/web/v1/user/otherinfo?"
            "target_user_id=5ff0e6410000000001008400")
-    sign = help.sign(uri=uri)
+    cookie_dict = help.cookie_str_to_cookie_dict(header["cookie"])
+    sign = help.sign(uri=uri, a1=cookie_dict.get("a1"))
 
     url = f"https://edith.xiaohongshu.com{uri}"
 
     headers = {
       'x-s': sign["x-s"],
       'x-t': sign["x-t"],
       'cookie': header['cookie'],
@@ -44,15 +45,16 @@
     print(json_data)
     assert json_data["code"] == 0
 
 
 def test_sign_post(header):
     uri = "/api/sns/web/v1/feed"
     data = {"source_note_id": "63db8819000000001a01ead1"}
-    sign = help.sign(uri=uri, data=data)
+    cookie_dict = help.cookie_str_to_cookie_dict(header["cookie"])
+    sign = help.sign(uri=uri, data=data, a1=cookie_dict.get("a1"))
 
     url = f"https://edith.xiaohongshu.com{uri}"
 
     payload = json.dumps(data, separators=(',', ':'))
     headers = {
       'x-s': sign["x-s"],
       'x-t': sign["x-t"],
```

### Comparing `xhs-0.2.1/tests/test_xhs.py` & `xhs-0.2.2/tests/test_xhs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,49 @@
 import pytest
+import requests
 
-from xhs import FeedType, IPBlockError, XhsClient
+from xhs import DataFetchError, FeedType, IPBlockError, XhsClient
 
 from . import test_cookie
 from .utils import beauty_print
 
 
 @pytest.fixture
 def xhs_client():
-    return XhsClient(cookie=test_cookie)
+    def sign(uri, data=None, a1=""):
+        res = requests.post("http://35.78.99.223:5000/xhs/sign", json={
+            "uri": uri,
+            "data": data,
+            "a1": a1
+        })
+        return res.json()
+    return XhsClient(cookie=test_cookie, sign=sign)
 
 
-def test_xhs_client_init():
-    xhs_client = XhsClient()
-    assert xhs_client
+# def test_xhs_client_init():
+#     xhs_client = XhsClient()
+#     assert xhs_client
 
 
-def test_cookie_setter_getter():
-    xhs_client = XhsClient()
-    cd = xhs_client.cookie_dict
-    beauty_print(cd)
-    assert "web_session" in cd
+# def test_cookie_setter_getter():
+#     xhs_client = XhsClient()
+#     cd = xhs_client.cookie_dict
+#     beauty_print(cd)
+#     assert "web_session" in cd
+
+
+def test_external_sign_func():
+
+    def sign(url, data=None, a1=""):
+        """signature url and data in here"""
+        return {}
+
+    with pytest.raises(DataFetchError):
+        xhs_client = XhsClient(sign=sign)
+        xhs_client.get_qrcode()
 
 
 def test_get_note_by_id(xhs_client: XhsClient):
     note_id = "6413cf6b00000000270115b5"
     data = xhs_client.get_note_by_id(note_id)
     beauty_print(data)
     assert data["note_id"] == note_id
@@ -184,11 +203,11 @@
 def test_ip_block_error(xhs_client: XhsClient):
     with pytest.raises(IPBlockError):
         note_id = "6413cf6b00000000270115b5"
         for _ in range(150):
             xhs_client.get_note_by_id(note_id)
 
 
-def test_activate(xhs_client: XhsClient):
-    info = xhs_client.activate()
-    beauty_print(info)
-    assert info["session"]
+# def test_activate(xhs_client: XhsClient):
+#     info = xhs_client.activate()
+#     beauty_print(info)
+#     assert info["session"]
```

### Comparing `xhs-0.2.1/xhs/core.py` & `xhs-0.2.2/xhs/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,19 +87,21 @@
 
 
 class XhsClient:
     def __init__(self,
                  cookie=None,
                  user_agent=None,
                  timeout=10,
-                 proxies=None):
+                 proxies=None,
+                 sign=None):
         """constructor"""
         self.proxies = proxies
         self.__session: requests.Session = requests.session()
         self.timeout = timeout
+        self.sign = sign
         self._host = "https://edith.xiaohongshu.com"
         self.home = "https://www.xiaohongshu.com"
         user_agent = user_agent or ("Mozilla/5.0 "
                                     "(Windows NT 10.0; Win64; x64) "
                                     "AppleWebKit/537.36 "
                                     "(KHTML, like Gecko) "
                                     "Chrome/111.0.0.0 Safari/537.36")
@@ -136,18 +138,21 @@
         return self.__session.headers.get("user-agent")
 
     @user_agent.setter
     def user_agent(self, user_agent: str):
         self.__session.headers.update({"user-agent": user_agent})
 
     def _pre_headers(self, url: str, data=None):
-        signs = sign(url, data)
-        self.__session.headers.update({"x-s": signs["x-s"]})
-        self.__session.headers.update({"x-t": signs["x-t"]})
-        self.__session.headers.update({"x-s-common": signs["x-s-common"]})
+        if self.sign:
+            self.__session.headers.update(self.sign(url, data, a1=self.cookie_dict.get("a1")))
+        else:
+            signs = sign(url, data, a1=self.cookie_dict.get("a1"))
+            self.__session.headers.update({"x-s": signs["x-s"]})
+            self.__session.headers.update({"x-t": signs["x-t"]})
+            self.__session.headers.update({"x-s-common": signs["x-s-common"]})
 
     def request(self, method, url, **kwargs):
         response = self.__session.request(
                         method, url, timeout=self.timeout,
                         proxies=self.proxies, **kwargs)
         data = response.json()
         if data["success"]:
```

### Comparing `xhs-0.2.1/xhs/help.py` & `xhs-0.2.2/xhs/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     return f"{random.choice(video_cdns)}/{origin_video_key}"
 
 
 def get_video_urls_from_note(note) -> list:
     if not note.get("video"):
         return []
     origin_video_key = note['video']['consumer']['origin_video_key']
-    return [f"{cdn}/{origin_video_key}?imageView2/format/{format}" for cdn in video_cdns]
+    return [f"{cdn}/{origin_video_key}" for cdn in video_cdns]
 
 
 def download_file(url: str, filename: str):
     with requests.get(url, stream=True) as r:
         r.raise_for_status()
         with open(filename, 'wb') as f:
             for chunk in r.iter_content(chunk_size=8192):
```

### Comparing `xhs-0.2.1/xhs.egg-info/PKG-INFO` & `xhs-0.2.2/xhs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.2.1
+Version: 0.2.2
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
@@ -36,35 +36,43 @@
 [![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
 [![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
 
 </div>
 
 > **Warning**
 >
-> I sincerely apologize for informing you that the sign is not functioning properly, indicating that certain APIs are experiencing issues. To address the anti-aliasing of the sign, I will devote time to further learning. 👋
->
-> This is in expriemental, so the api is not stable, every update should be cautious
+> The primary purpose of this repository is to practice my Python skills. It is important to note that web crawling may be considered illegal, and therefore, it is crucial to refrain from exerting any pressure or engaging in unauthorized activities on websites.
 
 **xhs** is a crawling tool designed to extract data from [xiaohongshu website](https://www.xiaohongshu.com/explore)
 
 ## Usage
 
 xhs is available on PyPI:
 
 ```console
 $ python -m pip install xhs
 ```
 
 basic usage:
 
 ```python
+import requests
 from xhs import FeedType, XhsClient
 
 cookie = "please get cookie in website"
-xhs_client = XhsClient(cookie)
+def sign(uri, data=None, a1=""):
+    """You can implement this sign function on your own."""
+    res = requests.post("http://127.0.0.1:5000/xhs/sign", json={
+        "uri": uri,
+        "data": data,
+        "a1": a1
+    })
+    return res.json()
+
+xhs_client = XhsClient(cookie, sign=sign)
 
 # get note info
 note_info = xhs_client.get_note_by_id("63db8819000000001a01ead1")
 
 # get user info
 user_info = xhs_client.get_user_info("5ff0e6410000000001008400")
 
@@ -86,15 +94,15 @@
 notes = xhs_client.get_user_all_notes("5c2766b500000000050283f1")
 
 # more functions in development
 ```
 
 Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
 
-use signature function:
+~~use signature function~~( it's useless ):
 
 ```python
 # sign get request
 >>> from xhs import help
 >>> help.sign("/api/sns/web/v1/user/otherinfo?target_user_id=5ff0e6410000000001008400")
 {'x-s': 'sYMlOB5W0YdvZBVvOBw6slZJZjM+ZgaUOlFisBwJslc3', 'x-t': '1683368960336', 'x-s-common': '2UQAPsHC+aIjqArjwjHjNsQhPsHCH0rjNsQhPaHCH0P1PjhIHjIj2eHjwjQgynEDJ74AHjIj2ePjwjQhyoPTqBPT49pjHjIj2ecjwjHUN0P1PaHVHdWMH0ijHjIj2eGjwjHl+0W
 APAGhw/GIPAP9HjIj2eqjwjQAnLMV/FHMpAm88o8ycS89/FQ7+d+VnDkyyDF3nf4YpLRVzfSAcd4tq9l0PUHVHdWhH0ijHjIj2eDjwjFAPAPU+eHMweDANsQhP/Zjw0bR'}
@@ -109,11 +117,7 @@
 >>> help.get_a1_and_web_id()
 ('187f09d3bc6wUrNpFbQ9Yc431AenpvlBJh2QIQahI50000261040', '12b49a1fd517aa8df85380e9961b6800')
 
 # get search_id parameter
 >>> help.get_search_id()
 '2BHU39J8HCTIW665YHFCW'
 ```
-
-## Donate
-
-[![](https://afdian.net/static/img/logo/logo.png)](https://afdian.net/a/reajason)
```

