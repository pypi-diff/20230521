# Comparing `tmp/glances_api-0.4.1.tar.gz` & `tmp/glances_api-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glances_api-0.4.1.tar", max compression
+gzip compressed data, was "glances_api-0.4.2.tar", max compression
```

## Comparing `glances_api-0.4.1.tar` & `glances_api-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1110 2022-01-16 22:16:50.701895 glances_api-0.4.1/LICENSE
--rw-r--r--   0        0        0      956 2022-01-16 22:16:50.769895 glances_api-0.4.1/README.rst
--rw-r--r--   0        0        0     5818 2022-08-28 21:00:01.105630 glances_api-0.4.1/glances_api/__init__.py
--rw-r--r--   0        0        0      455 2021-11-06 17:15:40.773828 glances_api-0.4.1/glances_api/exceptions.py
--rw-r--r--   0        0        0     1390 2022-08-28 21:22:52.451274 glances_api-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1691 2022-08-28 21:23:18.545339 glances_api-0.4.1/setup.py
--rw-r--r--   0        0        0     1957 2022-08-28 21:23:18.545527 glances_api-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1110 2023-05-21 11:03:42.721345 glances_api-0.4.2/LICENSE
+-rw-r--r--   0        0        0      956 2023-05-21 11:03:42.721345 glances_api-0.4.2/README.rst
+-rw-r--r--   0        0        0     5820 2023-05-21 11:03:42.721345 glances_api-0.4.2/glances_api/__init__.py
+-rw-r--r--   0        0        0      459 2023-05-21 11:03:42.721345 glances_api-0.4.2/glances_api/exceptions.py
+-rw-r--r--   0        0        0     1388 2023-05-21 11:08:13.471569 glances_api-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 glances_api-0.4.2/PKG-INFO
```

### Comparing `glances_api-0.4.1/LICENSE` & `glances_api-0.4.2/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017-2022 Fabian Affolter <fabian@affolter-engineering.ch>
+Copyright (c) 2017-2023 Fabian Affolter <fabian@affolter-engineering.ch>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `glances_api-0.4.1/README.rst` & `glances_api-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `glances_api-0.4.1/glances_api/__init__.py` & `glances_api-0.4.2/glances_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         except (httpx.ConnectError, httpx.TimeoutException):
             raise exceptions.GlancesApiConnectionError(f"Connection to {url} failed")
 
         if response.status_code == httpx.codes.UNAUTHORIZED:
             raise exceptions.GlancesApiAuthorizationError(
                 "Please check your credentials"
             )
-            
+
         if response.status_code != httpx.codes.OK:
             raise exceptions.GlancesApiNoDataAvailable(
                 f"endpoint: '{endpoint}' is not valid"
             )
         try:
             _LOGGER.debug(response.json())
             if endpoint == "all":
@@ -138,16 +138,16 @@
         if "docker" in self.data and (data := self.data["docker"].get("containers")):
             active_containers = [
                 container for container in data if container["Status"] == "running"
             ]
             sensor_data["docker"] = {"docker_active": len(active_containers)}
             cpu_use = 0.0
             for container in active_containers:
-                cpu_use += container["cpu"]["total"]
+                cpu_use += container["cpu"].get("total", 0)
             sensor_data["docker"]["docker_cpu_use"] = round(cpu_use, 1)
             mem_use = 0.0
             for container in active_containers:
-                mem_use += container["memory"]["usage"]
+                mem_use += container["memory"].get("usage", 0)
             sensor_data["docker"]["docker_memory_use"] = round(mem_use / 1024**2, 1)
         if data := self.data.get("raid"):
             sensor_data["raid"] = data
         return sensor_data
```

### Comparing `glances_api-0.4.1/pyproject.toml` & `glances_api-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glances_api"
-version = "0.4.1"
+version = "0.4.2"
 description = "Python API for interacting with Glances"
 authors = ["Fabian Affolter <fabian@affolter-engineering.ch>"]
 homepage = "https://github.com/home-assistant-ecosystem/python-glances-api"
 repository = "https://github.com/home-assistant-ecosystem/python-glances-api/releases"
 readme = "README.rst"
 license = "MIT"
 classifiers = [
@@ -14,19 +14,19 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 httpx = ">=0.23,<1"
 
 [tool.poetry.dev-dependencies]
-black = "^22.6.0"
+black = "^23.3"
 pytest = "^7.1.2"
 pytest-httpx = ">0.15,<1"
 pytest-asyncio = "^0.16.0"
 isort = "^5.10.0"
 mypy = "^0.971"
 
 [tool.mypy]
```

### Comparing `glances_api-0.4.1/PKG-INFO` & `glances_api-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: glances-api
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python API for interacting with Glances
 Home-page: https://github.com/home-assistant-ecosystem/python-glances-api
 License: MIT
 Author: Fabian Affolter
 Author-email: fabian@affolter-engineering.ch
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: httpx (>=0.23,<1)
 Project-URL: Repository, https://github.com/home-assistant-ecosystem/python-glances-api/releases
 Description-Content-Type: text/x-rst
 
 python-glances-api
 ==================
```

