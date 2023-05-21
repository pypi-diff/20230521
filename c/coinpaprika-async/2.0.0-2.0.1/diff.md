# Comparing `tmp/coinpaprika_async-2.0.0.tar.gz` & `tmp/coinpaprika_async-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinpaprika_async-2.0.0.tar", last modified: Mon Jun 13 12:25:03 2022, max compression
+gzip compressed data, was "coinpaprika_async-2.0.1.tar", last modified: Sun May 21 18:02:35 2023, max compression
```

## Comparing `coinpaprika_async-2.0.0.tar` & `coinpaprika_async-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-06-13 12:25:02.984610 coinpaprika_async-2.0.0/
--rw-rw-rw-   0        0        0     1084 2022-06-12 22:11:42.000000 coinpaprika_async-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     1611 2022-06-13 12:25:02.984610 coinpaprika_async-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      948 2022-06-12 22:35:14.000000 coinpaprika_async-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-06-13 12:25:02.895615 coinpaprika_async-2.0.0/coinpaprika_async/
--rw-rw-rw-   0        0        0      239 2022-06-13 00:18:46.000000 coinpaprika_async-2.0.0/coinpaprika_async/__init__.py
--rw-rw-rw-   0        0        0      125 2022-06-13 00:21:31.000000 coinpaprika_async-2.0.0/coinpaprika_async/__version__.py
--rw-rw-rw-   0        0        0      647 2022-06-13 00:41:20.000000 coinpaprika_async-2.0.0/coinpaprika_async/api_exception.py
--rw-rw-rw-   0        0        0     4629 2022-06-13 01:02:25.000000 coinpaprika_async-2.0.0/coinpaprika_async/cp_async_client.py
--rw-rw-rw-   0        0        0      740 2022-06-13 00:58:39.000000 coinpaprika_async-2.0.0/coinpaprika_async/response_object.py
-drwxrwxrwx   0        0        0        0 2022-06-13 12:25:02.983612 coinpaprika_async-2.0.0/coinpaprika_async.egg-info/
--rw-rw-rw-   0        0        0     1611 2022-06-13 12:25:01.000000 coinpaprika_async-2.0.0/coinpaprika_async.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2022-06-13 12:25:02.000000 coinpaprika_async-2.0.0/coinpaprika_async.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-13 12:25:01.000000 coinpaprika_async-2.0.0/coinpaprika_async.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-06-13 12:25:02.000000 coinpaprika_async-2.0.0/coinpaprika_async.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-06-13 12:25:02.000000 coinpaprika_async-2.0.0/coinpaprika_async.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      182 2022-01-18 14:40:37.000000 coinpaprika_async-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      139 2022-06-13 12:25:03.070622 coinpaprika_async-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      755 2022-06-13 00:21:30.000000 coinpaprika_async-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 18:02:35.158793 coinpaprika_async-2.0.1/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 17:45:15.000000 coinpaprika_async-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2075 2023-05-21 18:02:35.159792 coinpaprika_async-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-05-21 17:45:15.000000 coinpaprika_async-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 18:02:35.123797 coinpaprika_async-2.0.1/coinpaprika_async/
+-rw-rw-rw-   0        0        0      228 2023-05-21 17:51:17.000000 coinpaprika_async-2.0.1/coinpaprika_async/__init__.py
+-rw-rw-rw-   0        0        0      125 2023-05-21 17:49:59.000000 coinpaprika_async-2.0.1/coinpaprika_async/_version__.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 17:45:15.000000 coinpaprika_async-2.0.1/coinpaprika_async/api_exception.py
+-rw-rw-rw-   0        0        0     4573 2023-05-21 17:55:39.000000 coinpaprika_async-2.0.1/coinpaprika_async/client.py
+-rw-rw-rw-   0        0        0      740 2023-05-21 17:45:15.000000 coinpaprika_async-2.0.1/coinpaprika_async/response_object.py
+drwxrwxrwx   0        0        0        0 2023-05-21 18:02:35.146794 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/
+-rw-rw-rw-   0        0        0     2075 2023-05-21 18:02:34.000000 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2023-05-21 18:02:35.000000 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 18:02:34.000000 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-21 18:02:34.000000 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-21 18:02:34.000000 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      209 2023-05-21 17:49:30.000000 coinpaprika_async-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      139 2023-05-21 18:02:35.163810 coinpaprika_async-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-05-21 18:02:12.000000 coinpaprika_async-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 18:02:35.156795 coinpaprika_async-2.0.1/tests/
+-rw-rw-rw-   0        0        0     1239 2023-05-21 17:45:15.000000 coinpaprika_async-2.0.1/tests/test_client.py
```

### Comparing `coinpaprika_async-2.0.0/LICENSE` & `coinpaprika_async-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-2.0.0/README.md` & `coinpaprika_async-2.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+<div align="center">
+<h1 style="font-size:50px;">Coinpaprika Async Client</h1>
+  
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-# Coinpaprika API Python Asynchronous Client
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/coinpaprika-async)
+[![Actions Status](https://github.com/DroidZed/coinpaprika-async-client/workflows/Python%20package/badge.svg)](https://github.com/DroidZed/coinpaprika-async-client/actions)
+  
+</div>
 
 ## 1. Usage
 
 This library provides convenient and modern way to use [coinpaprika.com](https://api.coinpaprika.com/) API in Python.
 
 [Coinpaprika](https://coinpaprika.com/) delivers full market data to the world of crypto: coin prices, volumes, market caps, ATHs, return rates and more.
```

### Comparing `coinpaprika_async-2.0.0/coinpaprika_async/api_exception.py` & `coinpaprika_async-2.0.1/coinpaprika_async/api_exception.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-2.0.0/coinpaprika_async/cp_async_client.py` & `coinpaprika_async-2.0.1/coinpaprika_async/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,141 +3,113 @@
 from coinpaprika_async.api_exception import ApiException
 from coinpaprika_async.response_object import ResponseObject
 
 
 class Client:
 
     """
-    An **async** client for interacting with Coinpaprika's API backend.
+    ### An async client for interacting with Coinpaprika's API backend.
+
     """
 
     __API_URL = "https://api.coinpaprika.com/v1"
 
     def __init__(self):
-
         self.__async_client: AsyncClient = AsyncClient(
             headers={"Accept": "application/json", "User-Agent": "coinpaprika_async-async/python"}, timeout=20
         )
 
     # Internal handlers
 
     @staticmethod
     def __handle_response(response: Response) -> ResponseObject:
-
         resp = ResponseObject(status_code=response.status_code)
 
         try:
             resp.data = response.json()
             response.raise_for_status()
-
-        except HTTPError:
-            raise ApiException(response)
-
-        finally:
             return resp
 
-    async def __request(self, path: str, query_params: dict = None) -> ResponseObject:
+        except HTTPError as exc:
+            raise ApiException(response) from exc
 
+    async def __request(self, path: str, query_params: dict = None) -> ResponseObject:
         async with self.__async_client:
             uri = self.__create_api_uri(path)
 
             response: Response = await self.__async_client.get(url=uri, params=query_params)
 
         return self.__handle_response(response)
 
     def __create_api_uri(self, path: str) -> str:
-
         return f"{self.__API_URL}/{path}"
 
     async def __request_api(self, path: str, params: dict = None) -> ResponseObject:
-
         return await self.__request(path, params)
 
     async def __call_api(self, path: str, params: dict = None) -> ResponseObject:
-
         return await self.__request_api(path, params)
 
     # API CALLS
 
     async def global_market(self) -> ResponseObject:
-
         return await self.__call_api("global")
 
     async def coins(self) -> ResponseObject:
-
         return await self.__call_api("coins")
 
     async def coin(self, coin_id: str) -> ResponseObject:
-
         return await self.__call_api(f"coins/{coin_id}")
 
     async def twitter(self, coin_id: str) -> ResponseObject:
-
         return await self.__call_api(f"coins/{coin_id}/twitter")
 
     async def events(self, coin_id: str) -> ResponseObject:
-
         return await self.__call_api(f"coins/{coin_id}/events")
 
     async def exchanges(self, coin_id: str) -> ResponseObject:
-
         return await self.__call_api(f"coins/{coin_id}/exchanges")
 
     async def markets(self, coin_id: str, params: dict) -> ResponseObject:
-
         return await self.__call_api(f"coins/{coin_id}/markets", params)
 
     async def candle(self, coin_id: str, params: dict = None) -> ResponseObject:
-
         return await self.__call_api(f"coins/{coin_id}/ohlcv/latest", params)
 
     async def candles(self, coin_id: str, params: dict = None) -> ResponseObject:
-
         return await self.__call_api(f"coins/{coin_id}/ohlcv/historical", params)
 
     async def today(self, coin_id: str, params: dict = None) -> ResponseObject:
-
         return await self.__call_api(f"coins/{coin_id}/ohlcv/today", params)
 
     async def people(self, person_id: str = None):
-
         return await self.__call_api(f"people/{person_id}")
 
     async def tags(self, params: dict = None) -> ResponseObject:
-
         return await self.__call_api("tags", params)
 
     async def tag(self, tag_id: str, params: dict = None) -> ResponseObject:
-
         return await self.__call_api(f"tags/{tag_id}", params)
 
     async def tickers(self, params: dict = None) -> ResponseObject:
-
         return await self.__call_api("tickers", params)
 
     async def ticker(self, coin_id: str, params: dict = None) -> ResponseObject:
-
         return await self.__call_api(f"tickers/{coin_id}", params)
 
     async def historical(self, coin_id: str, params: dict) -> ResponseObject:
-
         return await self.__call_api(f"tickers/{coin_id}/historical", params)
 
     async def exchange_list(self, params: dict = None) -> ResponseObject:
-
         return await self.__call_api("exchanges", params)
 
     async def exchange(self, exchange_id: str, params: dict) -> ResponseObject:
-
         return await self.__call_api(f"exchanges/{exchange_id}", params)
 
     async def exchange_markets(self, exchange_id: str, params: dict = None) -> ResponseObject:
-
         return await self.__call_api(f"exchanges/{exchange_id}/markets", params)
 
     async def search(self, params: dict = None) -> ResponseObject:
-
         return await self.__call_api("search", params)
 
     async def price_converter(self, params: dict = None) -> ResponseObject:
-
         return await self.__call_api("price-converter", params)
```

### Comparing `coinpaprika_async-2.0.0/coinpaprika_async/response_object.py` & `coinpaprika_async-2.0.1/coinpaprika_async/response_object.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-2.0.0/setup.py` & `coinpaprika_async-2.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from setuptools import setup
 
 setup(
     name="coinpaprika_async",
-    version="2.0.0",
+    version="2.0.1",
     author="DroidZed",
     author_email="droid.zed77@outlook.com",
     description="An asynchronous client for the coinpaprika API.",
     packages=["coinpaprika_async"],
     url="https://github.com/DroidZed/coinpaprika-async-client.git",
     license="MIT",
     install_requires=["httpx"],
     keywords="coinpaprika_async api cryptocurrency async httpx client",
     classifiers=[
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

