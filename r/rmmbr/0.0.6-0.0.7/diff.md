# Comparing `tmp/rmmbr-0.0.6.tar.gz` & `tmp/rmmbr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmmbr-0.0.6.tar", last modified: Sat May 13 10:06:32 2023, max compression
+gzip compressed data, was "rmmbr-0.0.7.tar", last modified: Sun May 21 21:03:59 2023, max compression
```

## Comparing `rmmbr-0.0.6.tar` & `rmmbr-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 10:06:32.616151 rmmbr-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-13 10:06:32.616151 rmmbr-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 10:06:32.616151 rmmbr-0.0.6/rmmbr/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-13 10:06:18.000000 rmmbr-0.0.6/rmmbr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-13 10:06:18.000000 rmmbr-0.0.6/rmmbr/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-13 10:06:18.000000 rmmbr-0.0.6/rmmbr/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-13 10:06:18.000000 rmmbr-0.0.6/rmmbr/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-13 10:06:18.000000 rmmbr-0.0.6/rmmbr/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 10:06:32.616151 rmmbr-0.0.6/rmmbr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-13 10:06:32.000000 rmmbr-0.0.6/rmmbr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-13 10:06:32.000000 rmmbr-0.0.6/rmmbr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 10:06:32.000000 rmmbr-0.0.6/rmmbr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-13 10:06:32.000000 rmmbr-0.0.6/rmmbr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-13 10:06:32.000000 rmmbr-0.0.6/rmmbr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-13 10:06:32.000000 rmmbr-0.0.6/rmmbr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 10:06:32.616151 rmmbr-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-13 10:06:18.000000 rmmbr-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:03:59.344741 rmmbr-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-21 21:03:59.344741 rmmbr-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:03:59.344741 rmmbr-0.0.7/rmmbr/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-21 21:03:48.000000 rmmbr-0.0.7/rmmbr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-21 21:03:48.000000 rmmbr-0.0.7/rmmbr/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-21 21:03:48.000000 rmmbr-0.0.7/rmmbr/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-21 21:03:48.000000 rmmbr-0.0.7/rmmbr/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-21 21:03:48.000000 rmmbr-0.0.7/rmmbr/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:03:59.344741 rmmbr-0.0.7/rmmbr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:03:59.344741 rmmbr-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-21 21:03:48.000000 rmmbr-0.0.7/setup.py
```

### Comparing `rmmbr-0.0.6/PKG-INFO` & `rmmbr-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,120 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # rmmbr
 
 ![rmmbr](https://media.tenor.com/NcnMXggTODAAAAAC/yeah-i-member-memberberries.gif)
 
-`rmmbr` is the simplest way to cache your async functions, locally or in the cloud.
+`rmmbr` is the simplest way to persistently cache async functions, locally or in the
+cloud with end to end encryption (e2ee).
 
 ## Usage
 
-```sh
-npm i rmmbr
-```
+`rmmbr` provides three APIs, in python and javascript.
 
-```js
-import { cloudCache, localCache } from "rmmbr";
+1. cloud caching - persist the cache across devices
+1. local file caching - persist on one device in a text file under a `.rmmbr` directory
+1. In memory caching - no persistence, if you are feeling nostalgic 😉
 
-const cacher = localCache({ id: "name of cache for my function" });
+The cloud cache is free up to a quota. To use it, install the CLI tool:
 
-let nCalled = 0;
-const f = (x: number) => {
-  nCalled++;
-  return Promise.resolve(x);
-};
-const fCached = cacher(f);
-await fCached(3);
-await fCached(3);
-// nCalled is 1 here
+```sh
+source <(curl -s https://raw.githubusercontent.com/uriva/rmmbr/main/cli/install.sh)
 ```
 
-The local cache stores data in a text file under a `.rmmbr` directory.
+To produce a service token:
 
-There is also a `memCache`, if you are feeling nostalgic 😉 and just want to store stuff in memory.
-
-## Cross device caching
+```sh
+rmmbr login
+rmmbr api-token
+```
 
-To persist the cache across devices, we offer a use cloud service, which is free to use up to a quota.
+For sensitive data, you can e2e encrypt it by adding an encryption key parameter.
 
-To use it, you can install the CLI tool:
+To produce an encryption key:
 
-`source <(curl -s https://raw.githubusercontent.com/uriva/rmmbr/main/cli/install.sh)`
+```sh
+rmmbr secret
+```
 
-Then
+### Python
 
 ```sh
-rmmbr login
-rmmbr api-token
+pip install rmmbr
 ```
 
-Use your token with the API as follows:
+```python
+from rmmbr import cloud_cache
 
-```js
-const cacher = cloudCache({
-  token: "service-token",
-  cacheId: "some name for the cache",
-  url: "https://uriva-rmmbr.deno.dev",
-  ttl: 60 * 60 * 24, // Values will expire after one day, omission of this field implies max.
-});
+cacher = cloud_cache(
+    "https://rmmbr.net",
+    "your-service-token",
+    "some name for the cache",
+    60 * 60 * 24, # TTL is one day.
+    "Cqq33cbHu9AEUaP_wS3LCDQN7wy40XKWzALoPHbU5S8=",
+)
+
+n_called = 0
+
+@cacher
+async def f(x: int):
+  nonlocal n_called
+  n_called += 1
+  return x
+
+await f(3)
+await f(3)
+# nCalled is 1 here
 ```
 
-### End to end encryption
+### Javascript / Typescript
 
-If your data is sensitive, you can e2e encrypt it by adding an `encryptionKey` parameter.
+```sh
+npm i rmmbr
+```
 
-To produce an encryption key:
+```js
+import { cloudCache, localCache } from "rmmbr";
 
-```sh
-rmmbr secret
+const cacher = localCache({ id: "name of cache for my function" });
+
+let nCalled = 0;
+const f = (x: number) => {
+  nCalled++;
+  return Promise.resolve(x);
+};
+const fCached = cacher(f);
+await fCached(3);
+await fCached(3);
+// nCalled is 1 here
 ```
 
-Then use it like so:
+Cloud cache example:
 
 ```js
 const cacher = cloudCache({
   token: "service-token",
   cacheId: "some name for the cache",
-  url: "https://uriva-rmmbr.deno.dev",
-  encryptionKey: "eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee",
+  url: "https://rmmbr.net",
+  ttl: 60 * 60 * 24, // Values will expire after one day. Omission implies max (one week).
+  encryptionKey: "your-encryption-key", // This can be omitted if you don't need e2ee.
 });
 ```
 
-## Python
+## Pricing
 
-```sh
-pip install rmmbr
-```
+| Tier        | Requests  | Total data stored | Max entry size | # Entries |
+| ----------- | --------- | ----------------- | -------------- | --------- |
+| Free        | 10,000    | 10 MB             | 1 KB           | 1000      |
+| \$100/month | 1,000,000 | 1 GB              | 100 KB         | Unlimited |
+
+## Regions
 
-The python api mimicks the js one, with exported decorators named `mem_cache`, `local_cache` and `cloud_cache`.
+We currently deploy a backend in us-east region. Please post an issue if you have a need to configure this.
```

### Comparing `rmmbr-0.0.6/rmmbr/crypto.py` & `rmmbr-0.0.7/rmmbr/crypto.py`

 * *Files identical despite different names*

### Comparing `rmmbr-0.0.6/rmmbr/main.py` & `rmmbr-0.0.7/rmmbr/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from functools import partial
 import json
 import os
 from hashlib import sha256
 from typing import Callable, Optional
 
 import aiofiles
@@ -48,26 +49,35 @@
         return default_f()
 
 
 def _deserialize(s):
     return dict(json.loads(s))
 
 
+_cache_background_writes = set()
+
 def _abstract_cache_params(key, f, read, write):
     async def func(*args, **kwargs):
         key_result = key(*args, **kwargs)
         value = await read(key_result)
         if value is not None:
             return value
         y = await f(*args, **kwargs)
-        await write(key_result, y)
+        bg_write = asyncio.create_task(write(key_result, y))
+        # Avoid premature garbage collection, see notes:
+        # https://docs.python.org/3/library/asyncio-task.html#asyncio.create_task
+        _cache_background_writes.add(bg_write)
+        bg_write.add_done_callback(_cache_background_writes.discard)
+
         return y
 
     return func
 
+def wait_all_writes():
+    return asyncio.gather(*_cache_background_writes, return_exceptions=True)
 
 def mem_cache(f):
     cache = {}
 
     async def func(*args, **kwargs):
         key_result = _key_arguments(*args, **kwargs)
         if key_result in cache:
```

### Comparing `rmmbr-0.0.6/rmmbr/main_test.py` & `rmmbr-0.0.7/rmmbr/main_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import asyncio
 import pathlib
 
 import dotenv
 import redis.asyncio as redis
 
-from rmmbr import cloud_cache, local_cache, mem_cache
+from rmmbr import cloud_cache, local_cache, mem_cache, wait_all_writes
 
 
 def _cache_test_helper(instance_implies_new_cache: bool, expires_after_2_seconds: bool):
     async def inner(cacher):
         n_called = 0
 
         async def f(x):
             nonlocal n_called
             n_called += 1
             return await asyncio.sleep(0, x)
 
         f_cached = cacher(f)
         await f_cached(3)
-        results = await asyncio.gather(*map(f_cached, [3, 3, 2, 1]))
+        results = []
+        for n in [3, 3, 2, 1]:
+            await wait_all_writes()
+            results.append(await f_cached(n))
         assert results == [3, 3, 2, 1]
         await cacher(f)(3)
+        await wait_all_writes()
         assert n_called == (4 if instance_implies_new_cache else 3)
         n_called = 0
         await asyncio.sleep(2)
         await f_cached(3)
+        await wait_all_writes()
         assert n_called == (1 if expires_after_2_seconds else 0)
 
     return inner
 
 
 def _rmdir(directory):
     directory = pathlib.Path(directory)
```

### Comparing `rmmbr-0.0.6/rmmbr.egg-info/PKG-INFO` & `rmmbr-0.0.7/rmmbr.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,120 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # rmmbr
 
 ![rmmbr](https://media.tenor.com/NcnMXggTODAAAAAC/yeah-i-member-memberberries.gif)
 
-`rmmbr` is the simplest way to cache your async functions, locally or in the cloud.
+`rmmbr` is the simplest way to persistently cache async functions, locally or in the
+cloud with end to end encryption (e2ee).
 
 ## Usage
 
-```sh
-npm i rmmbr
-```
+`rmmbr` provides three APIs, in python and javascript.
 
-```js
-import { cloudCache, localCache } from "rmmbr";
+1. cloud caching - persist the cache across devices
+1. local file caching - persist on one device in a text file under a `.rmmbr` directory
+1. In memory caching - no persistence, if you are feeling nostalgic 😉
 
-const cacher = localCache({ id: "name of cache for my function" });
+The cloud cache is free up to a quota. To use it, install the CLI tool:
 
-let nCalled = 0;
-const f = (x: number) => {
-  nCalled++;
-  return Promise.resolve(x);
-};
-const fCached = cacher(f);
-await fCached(3);
-await fCached(3);
-// nCalled is 1 here
+```sh
+source <(curl -s https://raw.githubusercontent.com/uriva/rmmbr/main/cli/install.sh)
 ```
 
-The local cache stores data in a text file under a `.rmmbr` directory.
+To produce a service token:
 
-There is also a `memCache`, if you are feeling nostalgic 😉 and just want to store stuff in memory.
-
-## Cross device caching
+```sh
+rmmbr login
+rmmbr api-token
+```
 
-To persist the cache across devices, we offer a use cloud service, which is free to use up to a quota.
+For sensitive data, you can e2e encrypt it by adding an encryption key parameter.
 
-To use it, you can install the CLI tool:
+To produce an encryption key:
 
-`source <(curl -s https://raw.githubusercontent.com/uriva/rmmbr/main/cli/install.sh)`
+```sh
+rmmbr secret
+```
 
-Then
+### Python
 
 ```sh
-rmmbr login
-rmmbr api-token
+pip install rmmbr
 ```
 
-Use your token with the API as follows:
+```python
+from rmmbr import cloud_cache
 
-```js
-const cacher = cloudCache({
-  token: "service-token",
-  cacheId: "some name for the cache",
-  url: "https://uriva-rmmbr.deno.dev",
-  ttl: 60 * 60 * 24, // Values will expire after one day, omission of this field implies max.
-});
+cacher = cloud_cache(
+    "https://rmmbr.net",
+    "your-service-token",
+    "some name for the cache",
+    60 * 60 * 24, # TTL is one day.
+    "Cqq33cbHu9AEUaP_wS3LCDQN7wy40XKWzALoPHbU5S8=",
+)
+
+n_called = 0
+
+@cacher
+async def f(x: int):
+  nonlocal n_called
+  n_called += 1
+  return x
+
+await f(3)
+await f(3)
+# nCalled is 1 here
 ```
 
-### End to end encryption
+### Javascript / Typescript
 
-If your data is sensitive, you can e2e encrypt it by adding an `encryptionKey` parameter.
+```sh
+npm i rmmbr
+```
 
-To produce an encryption key:
+```js
+import { cloudCache, localCache } from "rmmbr";
 
-```sh
-rmmbr secret
+const cacher = localCache({ id: "name of cache for my function" });
+
+let nCalled = 0;
+const f = (x: number) => {
+  nCalled++;
+  return Promise.resolve(x);
+};
+const fCached = cacher(f);
+await fCached(3);
+await fCached(3);
+// nCalled is 1 here
 ```
 
-Then use it like so:
+Cloud cache example:
 
 ```js
 const cacher = cloudCache({
   token: "service-token",
   cacheId: "some name for the cache",
-  url: "https://uriva-rmmbr.deno.dev",
-  encryptionKey: "eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee",
+  url: "https://rmmbr.net",
+  ttl: 60 * 60 * 24, // Values will expire after one day. Omission implies max (one week).
+  encryptionKey: "your-encryption-key", // This can be omitted if you don't need e2ee.
 });
 ```
 
-## Python
+## Pricing
 
-```sh
-pip install rmmbr
-```
+| Tier        | Requests  | Total data stored | Max entry size | # Entries |
+| ----------- | --------- | ----------------- | -------------- | --------- |
+| Free        | 10,000    | 10 MB             | 1 KB           | 1000      |
+| \$100/month | 1,000,000 | 1 GB              | 100 KB         | Unlimited |
+
+## Regions
 
-The python api mimicks the js one, with exported decorators named `mem_cache`, `local_cache` and `cloud_cache`.
+We currently deploy a backend in us-east region. Please post an issue if you have a need to configure this.
```

### Comparing `rmmbr-0.0.6/setup.py` & `rmmbr-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 _repo_dir = os.environ.get("GITHUB_WORKSPACE")
 assert _repo_dir
 setup(
     name="rmmbr",
-    version="0.0.6",
+    version="0.0.7",
     description="Simple persistent caching.",
     long_description=(pathlib.Path(_repo_dir) / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/uriva/rmmbr",
     packages=find_packages(),
     install_requires=[
         "redis>=3.5.3",
```

