# Comparing `tmp/aioratelimits-0.2.1.tar.gz` & `tmp/aioratelimits-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioratelimits-0.2.1.tar", max compression
+gzip compressed data, was "aioratelimits-0.2.2.tar", max compression
```

## Comparing `aioratelimits-0.2.1.tar` & `aioratelimits-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      868 2022-08-21 06:32:22.351981 aioratelimits-0.2.1/README.md
--rw-r--r--   0        0        0     1190 2022-08-20 17:58:32.002976 aioratelimits-0.2.1/aioratelimits.py
--rw-r--r--   0        0        0      475 2022-08-21 06:40:23.424418 aioratelimits-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1384 2022-08-21 06:40:36.931116 aioratelimits-0.2.1/setup.py
--rw-r--r--   0        0        0     1422 2022-08-21 06:40:36.931393 aioratelimits-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      868 2022-08-21 06:32:22.351981 aioratelimits-0.2.2/README.md
+-rw-r--r--   0        0        0     1223 2023-05-21 17:00:17.396159 aioratelimits-0.2.2/aioratelimits.py
+-rw-r--r--   0        0        0      475 2023-05-21 17:06:24.793694 aioratelimits-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1384 2023-05-21 17:08:41.878096 aioratelimits-0.2.2/setup.py
+-rw-r--r--   0        0        0     1422 2023-05-21 17:08:41.878355 aioratelimits-0.2.2/PKG-INFO
```

### Comparing `aioratelimits-0.2.1/README.md` & `aioratelimits-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aioratelimits-0.2.1/setup.py` & `aioratelimits-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['aioratelimits']
 setup_kwargs = {
     'name': 'aioratelimits',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': '',
     'long_description': "# aioratelimits\n\nClient rate limiter. It enqueues function calls and run them as leaky bucket to\nensure specified rates.\n\n## Implementation\n\nLeaky bucket. We have one queue for requests and `count` number of workers.\nEach worker can handle one request per `delay` seconds\n\n## Install\n\n```\npip install aioratelimits\n```\n\n## Use\n\nThe following code prints not more than 2 lines per second.\n\n```python\nimport asyncio\nfrom aioratelimits import RateLimiter\n\n\nasync def critical_resource(i: int):\n    print('request:', i)\n\n\nasync def main():\n    async with RateLimiter(count=2, delay=1) as limiter:\n        await asyncio.gather(*(\n            limiter.run(critical_resource(i))\n            for i in range(10)\n        ))\n\n\nasyncio.run(main())\n```\n\nArguments to `RateLimiter`:\n- `count` - how many calls can we do in the specified interval\n- `delay` - the interval in seconds \n",
     'author': 'Dmitry Kostromin',
     'author_email': 'kupec-k@ya.ru',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/kupec/aioratelimits',
```

### Comparing `aioratelimits-0.2.1/PKG-INFO` & `aioratelimits-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioratelimits
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Home-page: https://github.com/kupec/aioratelimits
 Keywords: rates,ratelimit,ratelimiter,leaky,bucket
 Author: Dmitry Kostromin
 Author-email: kupec-k@ya.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

