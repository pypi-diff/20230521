# Comparing `tmp/duckduckgo_search-3.0.2.tar.gz` & `tmp/duckduckgo_search-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.0.2.tar", last modified: Wed May 17 21:50:09 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.1.0.tar", last modified: Sun May 21 12:52:01 2023, max compression
```

## Comparing `duckduckgo_search-3.0.2.tar` & `duckduckgo_search-3.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:50:09.893731 duckduckgo_search-3.0.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-17 21:50:09.893731 duckduckgo_search-3.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13485 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:50:09.889731 duckduckgo_search-3.0.2/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    23675 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:50:09.893731 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 21:50:09.000000 duckduckgo_search-3.0.2/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:50:09.893731 duckduckgo_search-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:50:09.893731 duckduckgo_search-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-17 21:49:51.000000 duckduckgo_search-3.0.2/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:52:01.104055 duckduckgo_search-3.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-21 12:51:34.000000 duckduckgo_search-3.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-05-21 12:52:01.104055 duckduckgo_search-3.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13413 2023-05-21 12:51:34.000000 duckduckgo_search-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:52:01.100055 duckduckgo_search-3.1.0/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-21 12:51:34.000000 duckduckgo_search-3.1.0/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-21 12:51:34.000000 duckduckgo_search-3.1.0/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-21 12:51:34.000000 duckduckgo_search-3.1.0/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-21 12:51:34.000000 duckduckgo_search-3.1.0/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-05-21 12:51:34.000000 duckduckgo_search-3.1.0/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-21 12:51:34.000000 duckduckgo_search-3.1.0/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:52:01.100055 duckduckgo_search-3.1.0/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-05-21 12:52:01.000000 duckduckgo_search-3.1.0/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-21 12:52:01.000000 duckduckgo_search-3.1.0/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:52:01.000000 duckduckgo_search-3.1.0/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-21 12:52:01.000000 duckduckgo_search-3.1.0/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-21 12:52:01.000000 duckduckgo_search-3.1.0/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 12:52:01.000000 duckduckgo_search-3.1.0/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-21 12:51:34.000000 duckduckgo_search-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 12:52:01.104055 duckduckgo_search-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:52:01.104055 duckduckgo_search-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-21 12:51:34.000000 duckduckgo_search-3.1.0/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.0.2/LICENSE.md` & `duckduckgo_search-3.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.0.2/PKG-INFO` & `duckduckgo_search-3.1.0/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: duckduckgo_search
-Version: 3.0.2
+Name: duckduckgo-search
+Version: 3.1.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -198,15 +198,15 @@
 ## 1. text() - text search by by duckduckgo.com
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m, y. Defaults to None.
@@ -225,15 +225,15 @@
 keywords = 'Bella Ciao'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
 
 # Searching for pdf files
 keywords = 'russia filetype:pdf'
-ddgs_text_gen = ddg(keywords, region='wt-wt', safesearch='Off', timelimit='y')
+ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
@@ -274,15 +274,15 @@
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     size: Optional[str] = None,
     color: Optional[str] = None,
     type_image: Optional[str] = None,
     layout: Optional[str] = None,
     license_image: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo images search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: Day, Week, Month, Year. Defaults to None.
@@ -332,15 +332,15 @@
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     resolution: Optional[str] = None,
     duration: Optional[str] = None,
     license_videos: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo videos search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -379,15 +379,15 @@
 
 ```python
 def news(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo news search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -427,15 +427,15 @@
         county: Optional[str] = None,
         state: Optional[str] = None,
         country: Optional[str] = None,
         postalcode: Optional[str] = None,
         latitude: Optional[str] = None,
         longitude: Optional[str] = None,
         radius: int = 0,
-    ) -> Generator[dict, None, None]:
+    ) -> Iterator[dict]:
         """DuckDuckGo maps search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query
             place: if set, the other parameters are not used. Defaults to None.
             street: house number/street. Defaults to None.
             city: city of search. Defaults to None.
@@ -506,15 +506,15 @@
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
 ```python
 def suggestions(
     keywords,
     region: str = "wt-wt",
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo suggestions. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
     Yields:
```

### Comparing `duckduckgo_search-3.0.2/README.md` & `duckduckgo_search-3.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 ## 1. text() - text search by by duckduckgo.com
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m, y. Defaults to None.
@@ -200,15 +200,15 @@
 keywords = 'Bella Ciao'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
 
 # Searching for pdf files
 keywords = 'russia filetype:pdf'
-ddgs_text_gen = ddg(keywords, region='wt-wt', safesearch='Off', timelimit='y')
+ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
@@ -249,15 +249,15 @@
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     size: Optional[str] = None,
     color: Optional[str] = None,
     type_image: Optional[str] = None,
     layout: Optional[str] = None,
     license_image: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo images search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: Day, Week, Month, Year. Defaults to None.
@@ -307,15 +307,15 @@
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     resolution: Optional[str] = None,
     duration: Optional[str] = None,
     license_videos: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo videos search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -354,15 +354,15 @@
 
 ```python
 def news(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo news search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -402,15 +402,15 @@
         county: Optional[str] = None,
         state: Optional[str] = None,
         country: Optional[str] = None,
         postalcode: Optional[str] = None,
         latitude: Optional[str] = None,
         longitude: Optional[str] = None,
         radius: int = 0,
-    ) -> Generator[dict, None, None]:
+    ) -> Iterator[dict]:
         """DuckDuckGo maps search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query
             place: if set, the other parameters are not used. Defaults to None.
             street: house number/street. Defaults to None.
             city: city of search. Defaults to None.
@@ -481,15 +481,15 @@
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
 ```python
 def suggestions(
     keywords,
     region: str = "wt-wt",
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo suggestions. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
     Yields:
```

### Comparing `duckduckgo_search-3.0.2/duckduckgo_search/__init__.py` & `duckduckgo_search-3.1.0/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.0.2/duckduckgo_search/cli.py` & `duckduckgo_search-3.1.0/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.0.2/duckduckgo_search/compat.py` & `duckduckgo_search-3.1.0/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.0.2/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.1.0/duckduckgo_search/duckduckgo_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 import re
 from collections import deque
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from html import unescape
 from time import sleep
-from typing import Dict, Generator, Optional
+from typing import Deque, Dict, Iterator, MutableMapping, Optional
 from urllib.parse import unquote
 
 import requests
+from anti_useragent import UserAgent
+from requests.exceptions import HTTPError, JSONDecodeError, Timeout
+from requests.models import Response
 
 logger = logging.getLogger(__name__)
 
-HEADERS = {
-    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0",
-    "Referer": "https://duckduckgo.com/",
-}
-RE_500_in_URL = re.compile(r"[\d]{3}-[0-9]{2}.js")
-RE_STRIP_TAGS = re.compile("<.*?>")
+UA = UserAgent()
+REGEX_500_IN_URL = re.compile(r"[0-9]{3}-[0-9]{2}.js")
+REGEX_STRIP_TAGS = re.compile("<.*?>")
 
 
 @dataclass
 class MapsResult:
     title: Optional[str] = None
     address: Optional[str] = None
     country_code: Optional[str] = None
@@ -36,91 +36,89 @@
     links: Optional[str] = None
     hours: Optional[Dict] = None
 
 
 class DDGS:
     """DuckDuckgo_search class to get search results from duckduckgo.com"""
 
-    def __init__(self, headers=None, proxies=None, timeout=10):
+    def __init__(
+        self,
+        headers: MutableMapping[str, str] = {},
+        proxies: MutableMapping[str, str] = {},
+        timeout: int = 10,
+    ) -> None:
         self._proxies = proxies
         self._session = requests.Session()
-        self._session.headers = headers
+        self._session.headers = headers if headers else UA.random
         self._session.proxies = proxies
         self._timeout = timeout
 
-    def _get_url(self, method, url, **kwargs):
-        for _ in range(3):
+    def _get_url(self, method: str, url: str, **kwargs) -> Optional[Response]:
+        for i in range(3):
             try:
                 resp = self._session.request(
-                    method, url, timeout=self._timeout, proxies=self._proxies, **kwargs
+                    method, url, timeout=self._timeout, **kwargs
                 )
                 if self._is_500_in_url(resp.url):
-                    logger.debug(f"_get_url() 500 in url={resp.url}. Sleep 5 s.")
-                    sleep(5)
+                    raise requests.HTTPError
                 resp.raise_for_status()
                 return resp
-            except requests.HTTPError:
-                sleep(1)
-            except Exception as ex:
-                logger.debug(f"_get_url() url={url} {type(ex).__name__}")
-            sleep(0.25)
+            except (HTTPError, Timeout) as ex:
+                logger.warning(f"_get_url() {url} {type(ex).__name__} {ex}")
+                if i < 2:
+                    sleep(2**i)
+        return None
 
-    def _resp_to_json(self, resp):
-        try:
-            return resp.json()
-        except Exception as ex:
-            logger.debug(f"_resp_to_json() {type(ex).__name__}")
-
-    def _get_vqd(self, keywords):
+    def _get_vqd(self, keywords: str) -> Optional[str]:
+        """Get vqd value for a search query."""
         resp = self._get_url("POST", "https://duckduckgo.com", data={"q": keywords})
         if resp:
-            vqd_bytes = self._parse_vqd(resp.content)
-            if vqd_bytes:
-                return vqd_bytes
-
-    def _parse_vqd(self, html_bytes):
-        """Parse vqd_bytes from raw html"""
-        for d in "\"'":
-            try:
-                vqd_index_start = html_bytes.index(b"vqd=%b" % d.encode()) + 5
-                vqd_index_end = html_bytes.index(b"%b" % d.encode(), vqd_index_start)
-                return html_bytes[vqd_index_start:vqd_index_end]
-            except Exception as ex:
-                logger.debug(f"_parse_vqd() {type(ex).__name__}")
+            for c1, c2 in (
+                (b'vqd="', b'"'),
+                (b"vqd=", b"&"),
+                (b"vqd='", b"'"),
+            ):
+                try:
+                    start = resp.content.index(c1) + len(c1)
+                    end = resp.content.index(c2, start)
+                    return resp.content[start:end].decode()
+                except ValueError:
+                    logger.warning(f"_get_vqd() keywords={keywords} vqd not found")
+        return None
 
-    def _is_500_in_url(self, url):
+    def _is_500_in_url(self, url: str) -> bool:
         """something like '506-00.js' inside the url"""
-        return RE_500_in_URL.search(url)
+        return bool(REGEX_500_IN_URL.search(url))
 
-    def _normalize(self, raw_html):
+    def _normalize(self, raw_html: str) -> str:
         """strip HTML tags"""
         if raw_html:
-            return unescape(re.sub(RE_STRIP_TAGS, "", raw_html))
+            return unescape(re.sub(REGEX_STRIP_TAGS, "", raw_html))
+        return ""
 
     def text(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
-    ) -> Generator[dict, None, None]:
+    ) -> Iterator[dict]:
         """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
 
         Yields:
             dict with search results.
 
         """
-        if not keywords:
-            return None
+        assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
         if not vqd:
             return None
 
         safesearch_base = {"on": 1, "moderate": -1, "off": -2}
         payload = {
@@ -134,49 +132,57 @@
         }
 
         cache = set()
         for _ in range(10):
             resp = self._get_url(
                 "GET", "https://links.duckduckgo.com/d.js", params=payload
             )
-            resp_json = self._resp_to_json(resp)
-            page_data = resp.json().get("results", None) if resp_json else None
-            if page_data:
-                result_exists = False
-                for i, row in enumerate(page_data):
-                    if "n" not in row and row["u"] not in cache:
-                        cache.add(row["u"])
-                        body = self._normalize(row["a"])
-                        if body:
-                            result_exists = True
-                            yield {
-                                "title": self._normalize(row["t"]),
-                                "href": row["u"],
-                                "body": body,
-                            }
-                    elif "n" in row:
-                        payload["s"] = row["n"].split("s=")[-1].split("&")[0]
-                    elif not result_exists:
-                        break
-                else:
-                    continue
+            if resp is None:
+                break
+            try:
+                page_data = resp.json().get("results", None)
+            except (AttributeError, JSONDecodeError):
+                break
+
+            result_exists = False
+            for row in page_data:
+                if "n" in row:
+                    payload["s"] = row["n"].split("s=")[-1].split("&")[0]  # next page
+                href = row.get("u", None)
+                if (
+                    href
+                    and href not in cache
+                    and href != f"http://www.google.com/search?q={keywords}"
+                ):
+                    cache.add(href)
+                    body = self._normalize(row["a"])
+                    if body:
+                        result_exists = True
+                        yield {
+                            "title": self._normalize(row["t"]),
+                            "href": href,
+                            "body": body,
+                        }
+                elif result_exists is False:
+                    break
+            if result_exists is False:
                 break
 
     def images(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         size: Optional[str] = None,
         color: Optional[str] = None,
         type_image: Optional[str] = None,
         layout: Optional[str] = None,
         license_image: Optional[str] = None,
-    ) -> Generator[dict, None, None]:
+    ) -> Iterator[dict]:
         """DuckDuckGo images search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: Day, Week, Month, Year. Defaults to None.
@@ -191,16 +197,15 @@
                 Modify (Free to Modify, Share, and Use), ModifyCommercially (Free to Modify, Share, and
                 Use Commercially). Defaults to None.
 
         Yields:
             dict with image search results.
 
         """
-        if not keywords:
-            return None
+        assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
         if not vqd:
             return None
 
         safesearch_base = {"on": 1, "moderate": 1, "off": -1}
         timelimit = f"time:{timelimit}" if timelimit else ""
@@ -218,47 +223,53 @@
             "f": f"{timelimit},{size},{color},{type_image},{layout},{license_image}",
             "p": safesearch_base[safesearch.lower()],
         }
 
         cache = set()
         for _ in range(10):
             resp = self._get_url("GET", "https://duckduckgo.com/i.js", params=payload)
-            resp_json = self._resp_to_json(resp)
-            page_data = resp.json().get("results", None) if resp_json else None
-            if page_data:
-                result_exists = False
-                for row in page_data:
-                    if row["image"] not in cache:
-                        cache.add(row["image"])
-                        result_exists = True
-                        yield {
-                            "title": row["title"],
-                            "image": row["image"],
-                            "thumbnail": row["thumbnail"],
-                            "url": row["url"],
-                            "height": row["height"],
-                            "width": row["width"],
-                            "source": row["source"],
-                        }
-                next = resp.json().get("next", None)
-                if next:
-                    payload["s"] = next.split("s=")[-1].split("&")[0]
-                if not result_exists or not next:
-                    break
+            if resp is None:
+                break
+            try:
+                resp_json = resp.json()
+            except (AttributeError, JSONDecodeError):
+                break
+
+            page_data = resp_json.get("results", None)
+            result_exists = False
+            for row in page_data:
+                image_url = row.get("image", None)
+                if image_url and image_url not in cache:
+                    cache.add(image_url)
+                    result_exists = True
+                    yield {
+                        "title": row["title"],
+                        "image": image_url,
+                        "thumbnail": row["thumbnail"],
+                        "url": row["url"],
+                        "height": row["height"],
+                        "width": row["width"],
+                        "source": row["source"],
+                    }
+            next = resp_json.get("next", None)
+            if next:
+                payload["s"] = next.split("s=")[-1].split("&")[0]
+            if next is None or result_exists is False:
+                break
 
     def videos(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         resolution: Optional[str] = None,
         duration: Optional[str] = None,
         license_videos: Optional[str] = None,
-    ) -> Generator[dict, None, None]:
+    ) -> Iterator[dict]:
         """DuckDuckGo videos search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m. Defaults to None.
@@ -266,16 +277,15 @@
             duration: short, medium, long. Defaults to None.
             license_videos: creativeCommon, youtube. Defaults to None.
 
         Yields:
             dict with videos search results
 
         """
-        if not keywords:
-            return None
+        assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
         if not vqd:
             return None
 
         safesearch_base = {"on": 1, "moderate": -1, "off": -2}
         timelimit = f"publishedAfter:{timelimit}" if timelimit else ""
@@ -291,50 +301,55 @@
             "f": f"{timelimit},{resolution},{duration},{license_videos}",
             "p": safesearch_base[safesearch.lower()],
         }
 
         cache = set()
         for _ in range(10):
             resp = self._get_url("GET", "https://duckduckgo.com/v.js", params=payload)
-            resp_json = self._resp_to_json(resp)
-            page_data = resp.json().get("results", None) if resp_json else None
+            if resp is None:
+                break
+            try:
+                resp_json = resp.json()
+            except (AttributeError, JSONDecodeError):
+                break
+
+            page_data = resp_json.get("results", None)
             if page_data:
                 result_exists = False
                 for row in page_data:
                     if row["content"] not in cache:
                         cache.add(row["content"])
                         result_exists = True
                         yield row
-                next = resp.json().get("next", None)
+                next = resp_json.get("next", None)
                 if next:
                     payload["s"] = next.split("s=")[-1].split("&")[0]
                 if not result_exists or not next:
                     break
 
     def news(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
-    ) -> Generator[dict, None, None]:
+    ) -> Iterator[dict]:
         """DuckDuckGo news search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m. Defaults to None.
 
         Yields:
             dict with news search results.
 
         """
-        if not keywords:
-            return None
+        assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
         if not vqd:
             return None
 
         safesearch_base = {"on": 1, "moderate": -1, "off": -2}
         payload = {
@@ -349,60 +364,70 @@
         }
 
         cache = set()
         for _ in range(10):
             resp = self._get_url(
                 "GET", "https://duckduckgo.com/news.js", params=payload
             )
-            resp_json = self._resp_to_json(resp)
-            page_data = resp.json().get("results", None) if resp_json else None
+            if resp is None:
+                break
+            try:
+                resp_json = resp.json()
+            except (AttributeError, JSONDecodeError):
+                break
+
+            page_data = resp_json.get("results", None)
             if page_data:
                 result_exists = False
                 for row in page_data:
                     if row["url"] not in cache:
                         cache.add(row["url"])
                         result_exists = True
                         yield {
                             "date": datetime.utcfromtimestamp(row["date"]).isoformat(),
                             "title": row["title"],
                             "body": self._normalize(row["excerpt"]),
                             "url": row["url"],
                             "image": row.get("image", None),
                             "source": row["source"],
                         }
-                next = resp.json().get("next", None)
+                next = resp_json.get("next", None)
                 if next:
                     payload["s"] = next.split("s=")[-1].split("&")[0]
                 if not result_exists or not next:
                     break
 
     def answers(
         self,
         keywords: str,
-    ) -> Generator[dict, None, None]:
+    ) -> Iterator[dict]:
         """DuckDuckGo instant answers. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
 
         Yields:
             dict with instant answers results.
 
         """
-        if not keywords:
-            return None
+        assert keywords, "keywords is mandatory"
 
         payload = {
             "q": f"what is {keywords}",
             "format": "json",
         }
 
         resp = self._get_url("GET", "https://api.duckduckgo.com/", params=payload)
-        resp_json = self._resp_to_json(resp)
-        page_data = resp.json() if resp_json else None
+        if resp is None:
+            return None
+        try:
+            page_data = resp.json()
+        except (AttributeError, JSONDecodeError):
+            page_data = None
+
         if page_data:
             answer = page_data.get("AbstractText", None)
             url = page_data.get("AbstractURL", None)
             if answer:
                 yield {
                     "icon": None,
                     "text": answer,
@@ -412,15 +437,21 @@
 
         # related:
         payload = {
             "q": f"{keywords}",
             "format": "json",
         }
         resp = self._get_url("GET", "https://api.duckduckgo.com/", params=payload)
-        page_data = resp.json().get("RelatedTopics", []) if resp else None
+        if resp is None:
+            return None
+        try:
+            page_data = resp.json().get("RelatedTopics", None)
+        except (AttributeError, JSONDecodeError):
+            page_data = None
+
         if page_data:
             for i, row in enumerate(page_data):
                 topic = row.get("Name", None)
                 if not topic:
                     icon = row["Icon"].get("URL", None)
                     yield {
                         "icon": f"https://duckduckgo.com{icon}" if icon else None,
@@ -436,54 +467,57 @@
                             "text": subrow["Text"],
                             "topic": topic,
                             "url": subrow["FirstURL"],
                         }
 
     def suggestions(
         self,
-        keywords,
+        keywords: str,
         region: str = "wt-wt",
-    ) -> Generator[dict, None, None]:
+    ) -> Iterator[dict]:
         """DuckDuckGo suggestions. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
         Yields:
             dict with suggestions results.
         """
 
-        if not keywords:
-            return None
+        assert keywords, "keywords is mandatory"
 
         payload = {
             "q": keywords,
             "kl": region,
         }
         resp = self._get_url("GET", "https://duckduckgo.com/ac", params=payload)
-        resp_json = self._resp_to_json(resp)
-        if resp_json:
-            for r in resp_json:
+        if resp is None:
+            return None
+        try:
+            page_data = resp.json()
+            for r in page_data:
                 yield r
+        except (AttributeError, JSONDecodeError):
+            pass
 
     def maps(
         self,
-        keywords,
+        keywords: str,
         place: Optional[str] = None,
         street: Optional[str] = None,
         city: Optional[str] = None,
         county: Optional[str] = None,
         state: Optional[str] = None,
         country: Optional[str] = None,
         postalcode: Optional[str] = None,
         latitude: Optional[str] = None,
         longitude: Optional[str] = None,
         radius: int = 0,
-    ) -> Generator[dict, None, None]:
+    ) -> Iterator[dict]:
         """DuckDuckGo maps search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query
             place: if set, the other parameters are not used. Defaults to None.
             street: house number/street. Defaults to None.
             city: city of search. Defaults to None.
@@ -496,16 +530,15 @@
                 longitude are set, the other parameters are not used. Defaults to None.
             radius: expand the search square by the distance in kilometers. Defaults to 0.
 
         Yields:
             dict with maps search results
         """
 
-        if not keywords:
-            return None
+        assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
         if not vqd:
             return None
 
         # if longitude and latitude are specified, skip the request about bbox to the nominatim api
         if latitude and longitude:
@@ -514,15 +547,15 @@
             lon_l = Decimal(longitude.replace(",", "."))
             lon_r = Decimal(longitude.replace(",", "."))
             if radius == 0:
                 radius = 1
         # otherwise request about bbox to nominatim api
         else:
             if place:
-                params = {
+                params: Dict[str, Optional[str]] = {
                     "q": place,
                     "polygon_geojson": "0",
                     "format": "jsonv2",
                 }
             else:
                 params = {
                     "street": street,
@@ -536,14 +569,17 @@
                 }
             try:
                 resp = self._get_url(
                     "GET",
                     "https://nominatim.openstreetmap.org/search.php",
                     params=params,
                 )
+                if resp is None:
+                    return None
+
                 coordinates = resp.json()[0]["boundingbox"]
                 lat_t, lon_l = Decimal(coordinates[1]), Decimal(coordinates[2])
                 lat_b, lon_r = Decimal(coordinates[0]), Decimal(coordinates[3])
             except Exception as ex:
                 logger.debug(f"ddg_maps() keywords={keywords} {type(ex).__name__} {ex}")
                 return
 
@@ -551,15 +587,15 @@
         lat_t += Decimal(radius) * Decimal(0.008983)
         lat_b -= Decimal(radius) * Decimal(0.008983)
         lon_l -= Decimal(radius) * Decimal(0.008983)
         lon_r += Decimal(radius) * Decimal(0.008983)
         logging.debug(f"bbox coordinates\n{lat_t} {lon_l}\n{lat_b} {lon_r}")
 
         # сreate a queue of search squares (bboxes)
-        work_bboxes = deque()
+        work_bboxes: Deque = deque()
         work_bboxes.append((lat_t, lon_l, lat_b, lon_r))
 
         # bbox iterate
         cache = set()
         stop_find = False
         while work_bboxes and not stop_find:
             lat_t, lon_l, lat_b, lon_r = work_bboxes.pop()
@@ -574,27 +610,29 @@
                 "bbox_tl": f"{lat_t},{lon_l}",
                 "bbox_br": f"{lat_b},{lon_r}",
                 "strict_bbox": "1",
             }
             resp = self._get_url(
                 "GET", "https://duckduckgo.com/local.js", params=params
             )
-            resp_json = self._resp_to_json(resp)
-            page_data = resp.json().get("results") if resp_json else None
-            if not page_data:
+            if resp is None:
+                break
+            try:
+                page_data = resp.json().get("results", [])
+            except (AttributeError, JSONDecodeError):
                 break
 
             for res in page_data:
                 result = MapsResult()
                 result.title = res["name"]
                 result.address = res["address"]
-                if result.title + result.address in cache:
+                if f"{result.title} {result.address}" in cache:
                     continue
                 else:
-                    cache.add(result.title + result.address)
+                    cache.add(f"{result.title} {result.address}")
                     result.country_code = res["country_code"]
                     result.url = res["website"]
                     result.phone = res["phone"]
                     result.latitude = res["coordinates"]["latitude"]
                     result.longitude = res["coordinates"]["longitude"]
                     result.source = unquote(res["url"])
                     if res["embed"]:
@@ -627,16 +665,15 @@
             from_: translate from (defaults automatically). Defaults to None.
             to: what language to translate. Defaults to "en".
 
         Returns:
             dict with translated keywords.
         """
 
-        if not keywords:
-            return None
+        assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd("translate")
         if not vqd:
             return None
 
         payload = {
             "vqd": vqd,
@@ -647,11 +684,15 @@
 
         resp = self._get_url(
             "POST",
             "https://duckduckgo.com/translation.js",
             params=payload,
             data=keywords.encode(),
         )
-        resp_json = self._resp_to_json(resp)
-        if resp_json:
-            resp_json["original"] = keywords
-            return resp_json
+        if resp is None:
+            return None
+        try:
+            page_data = resp.json()
+            page_data["original"] = keywords
+        except (AttributeError, JSONDecodeError):
+            page_data = None
+        return page_data
```

### Comparing `duckduckgo_search-3.0.2/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: duckduckgo-search
-Version: 3.0.2
+Name: duckduckgo_search
+Version: 3.1.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -198,15 +198,15 @@
 ## 1. text() - text search by by duckduckgo.com
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m, y. Defaults to None.
@@ -225,15 +225,15 @@
 keywords = 'Bella Ciao'
 ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
 
 # Searching for pdf files
 keywords = 'russia filetype:pdf'
-ddgs_text_gen = ddg(keywords, region='wt-wt', safesearch='Off', timelimit='y')
+ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
 for r in ddgs_text_gen:
 	print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
@@ -274,15 +274,15 @@
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     size: Optional[str] = None,
     color: Optional[str] = None,
     type_image: Optional[str] = None,
     layout: Optional[str] = None,
     license_image: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo images search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: Day, Week, Month, Year. Defaults to None.
@@ -332,15 +332,15 @@
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     resolution: Optional[str] = None,
     duration: Optional[str] = None,
     license_videos: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo videos search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -379,15 +379,15 @@
 
 ```python
 def news(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo news search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -427,15 +427,15 @@
         county: Optional[str] = None,
         state: Optional[str] = None,
         country: Optional[str] = None,
         postalcode: Optional[str] = None,
         latitude: Optional[str] = None,
         longitude: Optional[str] = None,
         radius: int = 0,
-    ) -> Generator[dict, None, None]:
+    ) -> Iterator[dict]:
         """DuckDuckGo maps search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query
             place: if set, the other parameters are not used. Defaults to None.
             street: house number/street. Defaults to None.
             city: city of search. Defaults to None.
@@ -506,15 +506,15 @@
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
 ```python
 def suggestions(
     keywords,
     region: str = "wt-wt",
-) -> Generator[dict, None, None]:
+) -> Iterator[dict]:
     """DuckDuckGo suggestions. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
     Yields:
```

### Comparing `duckduckgo_search-3.0.2/pyproject.toml` & `duckduckgo_search-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "click>=8.1.3",
     "requests>=2.30.0",
+    "anti_useragent==1.0.10",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
 
 [project.scripts]
```

### Comparing `duckduckgo_search-3.0.2/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.1.0/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

