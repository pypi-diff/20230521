# Comparing `tmp/keksik_api-0.1.3.tar.gz` & `tmp/keksik_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keksik_api-0.1.3.tar", max compression
+gzip compressed data, was "keksik_api-0.1.4.tar", max compression
```

## Comparing `keksik_api-0.1.3.tar` & `keksik_api-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1070 2023-05-20 12:43:03.823356 keksik_api-0.1.3/LICENSE
--rw-r--r--   0        0        0     1513 2023-05-20 14:27:31.868826 keksik_api-0.1.3/README.md
--rw-r--r--   0        0        0      260 2023-05-20 14:31:15.277096 keksik_api-0.1.3/keksik_api/__init__.py
--rw-r--r--   0        0        0     2530 2023-05-21 15:07:17.585925 keksik_api-0.1.3/keksik_api/api.py
--rw-r--r--   0        0        0      186 2023-05-20 10:59:09.616140 keksik_api-0.1.3/keksik_api/base.py
--rw-r--r--   0        0        0       98 2023-05-20 14:23:04.945309 keksik_api-0.1.3/keksik_api/callback/__init__.py
--rw-r--r--   0        0        0      381 2023-05-21 14:34:07.095423 keksik_api-0.1.3/keksik_api/callback/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4473 2023-05-21 14:34:59.498604 keksik_api-0.1.3/keksik_api/callback/__pycache__/callback.cpython-311.pyc
--rw-r--r--   0        0        0     2169 2023-05-21 14:34:59.574603 keksik_api-0.1.3/keksik_api/callback/__pycache__/handler.cpython-311.pyc
--rw-r--r--   0        0        0     4411 2023-05-21 14:34:59.570603 keksik_api-0.1.3/keksik_api/callback/__pycache__/router.cpython-311.pyc
--rw-r--r--   0        0        0     1508 2023-05-21 14:34:59.574603 keksik_api-0.1.3/keksik_api/callback/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     2410 2023-05-21 14:34:59.142609 keksik_api-0.1.3/keksik_api/callback/callback.py
--rw-r--r--   0        0        0      878 2023-05-21 13:09:06.566093 keksik_api-0.1.3/keksik_api/callback/handler.py
--rw-r--r--   0        0        0     1786 2023-05-21 13:09:06.422098 keksik_api-0.1.3/keksik_api/callback/router.py
--rw-r--r--   0        0        0      423 2023-05-21 13:09:06.686089 keksik_api-0.1.3/keksik_api/callback/rules.py
--rw-r--r--   0        0        0     1037 2023-05-20 10:39:54.109459 keksik_api-0.1.3/keksik_api/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-20 10:42:38.274538 keksik_api-0.1.3/keksik_api/methods/__init__.py
--rw-r--r--   0        0        0      192 2023-05-20 13:25:46.831790 keksik_api-0.1.3/keksik_api/methods/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      714 2023-05-20 13:25:46.831790 keksik_api-0.1.3/keksik_api/methods/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     6399 2023-05-20 13:25:46.831790 keksik_api-0.1.3/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc
--rw-r--r--   0        0        0     8800 2023-05-20 13:25:46.835790 keksik_api-0.1.3/keksik_api/methods/__pycache__/donates.cpython-311.pyc
--rw-r--r--   0        0        0     4282 2023-05-21 15:07:18.501937 keksik_api-0.1.3/keksik_api/methods/__pycache__/payments.cpython-311.pyc
--rw-r--r--   0        0        0      159 2023-05-20 10:59:09.576141 keksik_api-0.1.3/keksik_api/methods/base.py
--rw-r--r--   0        0        0     4850 2023-05-20 12:24:21.123997 keksik_api-0.1.3/keksik_api/methods/campaigns.py
--rw-r--r--   0        0        0     7099 2023-05-20 12:24:21.019999 keksik_api-0.1.3/keksik_api/methods/donates.py
--rw-r--r--   0        0        0     3204 2023-05-20 14:31:15.209097 keksik_api-0.1.3/keksik_api/methods/payments.py
--rw-r--r--   0        0        0      114 2023-05-20 14:17:48.110688 keksik_api-0.1.3/keksik_api/schemas/__init__.py
--rw-r--r--   0        0        0      339 2023-05-20 14:17:48.638678 keksik_api-0.1.3/keksik_api/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1483 2023-05-21 14:34:07.035424 keksik_api-0.1.3/keksik_api/schemas/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     3353 2023-05-20 13:25:46.543794 keksik_api-0.1.3/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc
--rw-r--r--   0        0        0     2786 2023-05-20 13:25:46.551794 keksik_api-0.1.3/keksik_api/schemas/__pycache__/donates.cpython-311.pyc
--rw-r--r--   0        0        0     1847 2023-05-20 14:17:48.666678 keksik_api-0.1.3/keksik_api/schemas/__pycache__/events.cpython-311.pyc
--rw-r--r--   0        0        0     2757 2023-05-20 13:25:46.555794 keksik_api-0.1.3/keksik_api/schemas/__pycache__/payments.cpython-311.pyc
--rw-r--r--   0        0        0      456 2023-05-20 14:28:50.491512 keksik_api-0.1.3/keksik_api/schemas/base.py
--rw-r--r--   0        0        0     1331 2023-05-20 12:27:12.277779 keksik_api-0.1.3/keksik_api/schemas/campaigns.py
--rw-r--r--   0        0        0     1051 2023-05-20 11:59:33.646543 keksik_api-0.1.3/keksik_api/schemas/donates.py
--rw-r--r--   0        0        0      630 2023-05-20 14:17:48.058688 keksik_api-0.1.3/keksik_api/schemas/events.py
--rw-r--r--   0        0        0      947 2023-05-20 12:51:48.242846 keksik_api-0.1.3/keksik_api/schemas/payments.py
--rw-r--r--   0        0        0      522 2023-05-21 14:49:35.157138 keksik_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2126 1970-01-01 00:00:00.000000 keksik_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-20 12:43:03.823356 keksik_api-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1513 2023-05-20 14:27:31.868826 keksik_api-0.1.4/README.md
+-rw-r--r--   0        0        0      260 2023-05-20 14:31:15.277096 keksik_api-0.1.4/keksik_api/__init__.py
+-rw-r--r--   0        0        0     2530 2023-05-21 15:07:17.585925 keksik_api-0.1.4/keksik_api/api.py
+-rw-r--r--   0        0        0      186 2023-05-20 10:59:09.616140 keksik_api-0.1.4/keksik_api/base.py
+-rw-r--r--   0        0        0       98 2023-05-20 14:23:04.945309 keksik_api-0.1.4/keksik_api/callback/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-21 14:34:07.095423 keksik_api-0.1.4/keksik_api/callback/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4473 2023-05-21 14:34:59.498604 keksik_api-0.1.4/keksik_api/callback/__pycache__/callback.cpython-311.pyc
+-rw-r--r--   0        0        0     2169 2023-05-21 14:34:59.574603 keksik_api-0.1.4/keksik_api/callback/__pycache__/handler.cpython-311.pyc
+-rw-r--r--   0        0        0     4411 2023-05-21 14:34:59.570603 keksik_api-0.1.4/keksik_api/callback/__pycache__/router.cpython-311.pyc
+-rw-r--r--   0        0        0     1508 2023-05-21 14:34:59.574603 keksik_api-0.1.4/keksik_api/callback/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     2590 2023-05-21 15:25:41.723995 keksik_api-0.1.4/keksik_api/callback/callback.py
+-rw-r--r--   0        0        0      878 2023-05-21 13:09:06.566093 keksik_api-0.1.4/keksik_api/callback/handler.py
+-rw-r--r--   0        0        0     1786 2023-05-21 13:09:06.422098 keksik_api-0.1.4/keksik_api/callback/router.py
+-rw-r--r--   0        0        0      423 2023-05-21 13:09:06.686089 keksik_api-0.1.4/keksik_api/callback/rules.py
+-rw-r--r--   0        0        0     1037 2023-05-20 10:39:54.109459 keksik_api-0.1.4/keksik_api/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-20 10:42:38.274538 keksik_api-0.1.4/keksik_api/methods/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-20 13:25:46.831790 keksik_api-0.1.4/keksik_api/methods/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      714 2023-05-20 13:25:46.831790 keksik_api-0.1.4/keksik_api/methods/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     6399 2023-05-20 13:25:46.831790 keksik_api-0.1.4/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc
+-rw-r--r--   0        0        0     8800 2023-05-20 13:25:46.835790 keksik_api-0.1.4/keksik_api/methods/__pycache__/donates.cpython-311.pyc
+-rw-r--r--   0        0        0     4282 2023-05-21 15:07:18.501937 keksik_api-0.1.4/keksik_api/methods/__pycache__/payments.cpython-311.pyc
+-rw-r--r--   0        0        0      159 2023-05-20 10:59:09.576141 keksik_api-0.1.4/keksik_api/methods/base.py
+-rw-r--r--   0        0        0     4850 2023-05-20 12:24:21.123997 keksik_api-0.1.4/keksik_api/methods/campaigns.py
+-rw-r--r--   0        0        0     7099 2023-05-20 12:24:21.019999 keksik_api-0.1.4/keksik_api/methods/donates.py
+-rw-r--r--   0        0        0     3204 2023-05-20 14:31:15.209097 keksik_api-0.1.4/keksik_api/methods/payments.py
+-rw-r--r--   0        0        0      114 2023-05-20 14:17:48.110688 keksik_api-0.1.4/keksik_api/schemas/__init__.py
+-rw-r--r--   0        0        0      339 2023-05-20 14:17:48.638678 keksik_api-0.1.4/keksik_api/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1483 2023-05-21 14:34:07.035424 keksik_api-0.1.4/keksik_api/schemas/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     3353 2023-05-20 13:25:46.543794 keksik_api-0.1.4/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc
+-rw-r--r--   0        0        0     2786 2023-05-20 13:25:46.551794 keksik_api-0.1.4/keksik_api/schemas/__pycache__/donates.cpython-311.pyc
+-rw-r--r--   0        0        0     1847 2023-05-20 14:17:48.666678 keksik_api-0.1.4/keksik_api/schemas/__pycache__/events.cpython-311.pyc
+-rw-r--r--   0        0        0     2757 2023-05-20 13:25:46.555794 keksik_api-0.1.4/keksik_api/schemas/__pycache__/payments.cpython-311.pyc
+-rw-r--r--   0        0        0      456 2023-05-20 14:28:50.491512 keksik_api-0.1.4/keksik_api/schemas/base.py
+-rw-r--r--   0        0        0     1331 2023-05-20 12:27:12.277779 keksik_api-0.1.4/keksik_api/schemas/campaigns.py
+-rw-r--r--   0        0        0     1051 2023-05-20 11:59:33.646543 keksik_api-0.1.4/keksik_api/schemas/donates.py
+-rw-r--r--   0        0        0      630 2023-05-20 14:17:48.058688 keksik_api-0.1.4/keksik_api/schemas/events.py
+-rw-r--r--   0        0        0      947 2023-05-20 12:51:48.242846 keksik_api-0.1.4/keksik_api/schemas/payments.py
+-rw-r--r--   0        0        0      522 2023-05-21 15:26:46.490834 keksik_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2126 1970-01-01 00:00:00.000000 keksik_api-0.1.4/PKG-INFO
```

### Comparing `keksik_api-0.1.3/LICENSE` & `keksik_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/README.md` & `keksik_api-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/api.py` & `keksik_api-0.1.4/keksik_api/api.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/callback/__pycache__/callback.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/callback/__pycache__/callback.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/callback/__pycache__/handler.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/callback/__pycache__/handler.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/callback/__pycache__/router.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/callback/__pycache__/router.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/callback/__pycache__/rules.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/callback/__pycache__/rules.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/callback/callback.py` & `keksik_api-0.1.4/keksik_api/callback/callback.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,20 @@
     def check_hash(self, params: dict) -> bool:
         hash_value = params['hash']
         del params['hash']
         params = self.get_hash_dict(params)
         params = dict(sorted(params.items()))
         params_values = list(params.values())
         params_values.append(self._secret_key)
-        hash_str = ','.join(params_values)
+        hash_str = ','.join([
+            ("1" if value else "") if isinstance(value, bool) else
+            str(value) if not isinstance(value, str) else
+            value
+            for value in params_values
+        ])
         sha256 = hashlib.sha256(hash_str.encode()).hexdigest()
         return sha256 == hash_value
 
     def get_hash_dict(self, params: dict, index: str = ''):
         hash_dict = {}
         if index:
             index += '/'
```

### Comparing `keksik_api-0.1.3/keksik_api/callback/handler.py` & `keksik_api-0.1.4/keksik_api/callback/handler.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/callback/router.py` & `keksik_api-0.1.4/keksik_api/callback/router.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/exceptions.py` & `keksik_api-0.1.4/keksik_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/methods/__pycache__/base.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/methods/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/methods/__pycache__/donates.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/methods/__pycache__/donates.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/methods/__pycache__/payments.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/methods/__pycache__/payments.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/methods/campaigns.py` & `keksik_api-0.1.4/keksik_api/methods/campaigns.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/methods/donates.py` & `keksik_api-0.1.4/keksik_api/methods/donates.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/methods/payments.py` & `keksik_api-0.1.4/keksik_api/methods/payments.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/schemas/__pycache__/base.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/schemas/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/schemas/__pycache__/donates.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/schemas/__pycache__/donates.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/schemas/__pycache__/events.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/schemas/__pycache__/events.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/schemas/__pycache__/payments.cpython-311.pyc` & `keksik_api-0.1.4/keksik_api/schemas/__pycache__/payments.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/schemas/campaigns.py` & `keksik_api-0.1.4/keksik_api/schemas/campaigns.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/schemas/donates.py` & `keksik_api-0.1.4/keksik_api/schemas/donates.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/schemas/events.py` & `keksik_api-0.1.4/keksik_api/schemas/events.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/keksik_api/schemas/payments.py` & `keksik_api-0.1.4/keksik_api/schemas/payments.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.3/pyproject.toml` & `keksik_api-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keksik-api"
-version = "0.1.3"
+version = "0.1.4"
 description = "Обвертка над API keksik.io"
 authors = ["lordralinc <lordralinc@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "keksik_api"}]
 
 [tool.poetry.dependencies]
```

### Comparing `keksik_api-0.1.3/PKG-INFO` & `keksik_api-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keksik-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Обвертка над API keksik.io
 License: MIT
 Author: lordralinc
 Author-email: lordralinc@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

