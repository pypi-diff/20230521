# Comparing `tmp/keksik_api-0.1.4.tar.gz` & `tmp/keksik_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keksik_api-0.1.4.tar", max compression
+gzip compressed data, was "keksik_api-0.1.5.tar", max compression
```

## Comparing `keksik_api-0.1.4.tar` & `keksik_api-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1070 2023-05-20 12:43:03.823356 keksik_api-0.1.4/LICENSE
--rw-r--r--   0        0        0     1513 2023-05-20 14:27:31.868826 keksik_api-0.1.4/README.md
--rw-r--r--   0        0        0      260 2023-05-20 14:31:15.277096 keksik_api-0.1.4/keksik_api/__init__.py
--rw-r--r--   0        0        0     2530 2023-05-21 15:07:17.585925 keksik_api-0.1.4/keksik_api/api.py
--rw-r--r--   0        0        0      186 2023-05-20 10:59:09.616140 keksik_api-0.1.4/keksik_api/base.py
--rw-r--r--   0        0        0       98 2023-05-20 14:23:04.945309 keksik_api-0.1.4/keksik_api/callback/__init__.py
--rw-r--r--   0        0        0      381 2023-05-21 14:34:07.095423 keksik_api-0.1.4/keksik_api/callback/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4473 2023-05-21 14:34:59.498604 keksik_api-0.1.4/keksik_api/callback/__pycache__/callback.cpython-311.pyc
--rw-r--r--   0        0        0     2169 2023-05-21 14:34:59.574603 keksik_api-0.1.4/keksik_api/callback/__pycache__/handler.cpython-311.pyc
--rw-r--r--   0        0        0     4411 2023-05-21 14:34:59.570603 keksik_api-0.1.4/keksik_api/callback/__pycache__/router.cpython-311.pyc
--rw-r--r--   0        0        0     1508 2023-05-21 14:34:59.574603 keksik_api-0.1.4/keksik_api/callback/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     2590 2023-05-21 15:25:41.723995 keksik_api-0.1.4/keksik_api/callback/callback.py
--rw-r--r--   0        0        0      878 2023-05-21 13:09:06.566093 keksik_api-0.1.4/keksik_api/callback/handler.py
--rw-r--r--   0        0        0     1786 2023-05-21 13:09:06.422098 keksik_api-0.1.4/keksik_api/callback/router.py
--rw-r--r--   0        0        0      423 2023-05-21 13:09:06.686089 keksik_api-0.1.4/keksik_api/callback/rules.py
--rw-r--r--   0        0        0     1037 2023-05-20 10:39:54.109459 keksik_api-0.1.4/keksik_api/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-20 10:42:38.274538 keksik_api-0.1.4/keksik_api/methods/__init__.py
--rw-r--r--   0        0        0      192 2023-05-20 13:25:46.831790 keksik_api-0.1.4/keksik_api/methods/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      714 2023-05-20 13:25:46.831790 keksik_api-0.1.4/keksik_api/methods/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     6399 2023-05-20 13:25:46.831790 keksik_api-0.1.4/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc
--rw-r--r--   0        0        0     8800 2023-05-20 13:25:46.835790 keksik_api-0.1.4/keksik_api/methods/__pycache__/donates.cpython-311.pyc
--rw-r--r--   0        0        0     4282 2023-05-21 15:07:18.501937 keksik_api-0.1.4/keksik_api/methods/__pycache__/payments.cpython-311.pyc
--rw-r--r--   0        0        0      159 2023-05-20 10:59:09.576141 keksik_api-0.1.4/keksik_api/methods/base.py
--rw-r--r--   0        0        0     4850 2023-05-20 12:24:21.123997 keksik_api-0.1.4/keksik_api/methods/campaigns.py
--rw-r--r--   0        0        0     7099 2023-05-20 12:24:21.019999 keksik_api-0.1.4/keksik_api/methods/donates.py
--rw-r--r--   0        0        0     3204 2023-05-20 14:31:15.209097 keksik_api-0.1.4/keksik_api/methods/payments.py
--rw-r--r--   0        0        0      114 2023-05-20 14:17:48.110688 keksik_api-0.1.4/keksik_api/schemas/__init__.py
--rw-r--r--   0        0        0      339 2023-05-20 14:17:48.638678 keksik_api-0.1.4/keksik_api/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1483 2023-05-21 14:34:07.035424 keksik_api-0.1.4/keksik_api/schemas/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     3353 2023-05-20 13:25:46.543794 keksik_api-0.1.4/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc
--rw-r--r--   0        0        0     2786 2023-05-20 13:25:46.551794 keksik_api-0.1.4/keksik_api/schemas/__pycache__/donates.cpython-311.pyc
--rw-r--r--   0        0        0     1847 2023-05-20 14:17:48.666678 keksik_api-0.1.4/keksik_api/schemas/__pycache__/events.cpython-311.pyc
--rw-r--r--   0        0        0     2757 2023-05-20 13:25:46.555794 keksik_api-0.1.4/keksik_api/schemas/__pycache__/payments.cpython-311.pyc
--rw-r--r--   0        0        0      456 2023-05-20 14:28:50.491512 keksik_api-0.1.4/keksik_api/schemas/base.py
--rw-r--r--   0        0        0     1331 2023-05-20 12:27:12.277779 keksik_api-0.1.4/keksik_api/schemas/campaigns.py
--rw-r--r--   0        0        0     1051 2023-05-20 11:59:33.646543 keksik_api-0.1.4/keksik_api/schemas/donates.py
--rw-r--r--   0        0        0      630 2023-05-20 14:17:48.058688 keksik_api-0.1.4/keksik_api/schemas/events.py
--rw-r--r--   0        0        0      947 2023-05-20 12:51:48.242846 keksik_api-0.1.4/keksik_api/schemas/payments.py
--rw-r--r--   0        0        0      522 2023-05-21 15:26:46.490834 keksik_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2126 1970-01-01 00:00:00.000000 keksik_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-20 12:43:03.823356 keksik_api-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1513 2023-05-20 14:27:31.868826 keksik_api-0.1.5/README.md
+-rw-r--r--   0        0        0      260 2023-05-20 14:31:15.277096 keksik_api-0.1.5/keksik_api/__init__.py
+-rw-r--r--   0        0        0     2529 2023-05-21 15:30:13.196552 keksik_api-0.1.5/keksik_api/api.py
+-rw-r--r--   0        0        0      186 2023-05-20 10:59:09.616140 keksik_api-0.1.5/keksik_api/base.py
+-rw-r--r--   0        0        0       98 2023-05-20 14:23:04.945309 keksik_api-0.1.5/keksik_api/callback/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-21 14:34:07.095423 keksik_api-0.1.5/keksik_api/callback/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4915 2023-05-21 15:31:36.352640 keksik_api-0.1.5/keksik_api/callback/__pycache__/callback.cpython-311.pyc
+-rw-r--r--   0        0        0     2169 2023-05-21 14:34:59.574603 keksik_api-0.1.5/keksik_api/callback/__pycache__/handler.cpython-311.pyc
+-rw-r--r--   0        0        0     4411 2023-05-21 14:34:59.570603 keksik_api-0.1.5/keksik_api/callback/__pycache__/router.cpython-311.pyc
+-rw-r--r--   0        0        0     1508 2023-05-21 14:34:59.574603 keksik_api-0.1.5/keksik_api/callback/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     2590 2023-05-21 15:25:41.723995 keksik_api-0.1.5/keksik_api/callback/callback.py
+-rw-r--r--   0        0        0      878 2023-05-21 13:09:06.566093 keksik_api-0.1.5/keksik_api/callback/handler.py
+-rw-r--r--   0        0        0     1786 2023-05-21 13:09:06.422098 keksik_api-0.1.5/keksik_api/callback/router.py
+-rw-r--r--   0        0        0      423 2023-05-21 13:09:06.686089 keksik_api-0.1.5/keksik_api/callback/rules.py
+-rw-r--r--   0        0        0     1037 2023-05-20 10:39:54.109459 keksik_api-0.1.5/keksik_api/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-20 10:42:38.274538 keksik_api-0.1.5/keksik_api/methods/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-20 13:25:46.831790 keksik_api-0.1.5/keksik_api/methods/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      714 2023-05-20 13:25:46.831790 keksik_api-0.1.5/keksik_api/methods/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     6399 2023-05-20 13:25:46.831790 keksik_api-0.1.5/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc
+-rw-r--r--   0        0        0     8800 2023-05-20 13:25:46.835790 keksik_api-0.1.5/keksik_api/methods/__pycache__/donates.cpython-311.pyc
+-rw-r--r--   0        0        0     4282 2023-05-21 15:07:18.501937 keksik_api-0.1.5/keksik_api/methods/__pycache__/payments.cpython-311.pyc
+-rw-r--r--   0        0        0      159 2023-05-20 10:59:09.576141 keksik_api-0.1.5/keksik_api/methods/base.py
+-rw-r--r--   0        0        0     4850 2023-05-20 12:24:21.123997 keksik_api-0.1.5/keksik_api/methods/campaigns.py
+-rw-r--r--   0        0        0     7099 2023-05-20 12:24:21.019999 keksik_api-0.1.5/keksik_api/methods/donates.py
+-rw-r--r--   0        0        0     3204 2023-05-20 14:31:15.209097 keksik_api-0.1.5/keksik_api/methods/payments.py
+-rw-r--r--   0        0        0      114 2023-05-21 15:30:54.162557 keksik_api-0.1.5/keksik_api/schemas/__init__.py
+-rw-r--r--   0        0        0      339 2023-05-21 15:30:56.546674 keksik_api-0.1.5/keksik_api/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1483 2023-05-21 14:34:07.035424 keksik_api-0.1.5/keksik_api/schemas/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     3353 2023-05-20 13:25:46.543794 keksik_api-0.1.5/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc
+-rw-r--r--   0        0        0     2786 2023-05-20 13:25:46.551794 keksik_api-0.1.5/keksik_api/schemas/__pycache__/donates.cpython-311.pyc
+-rw-r--r--   0        0        0     2093 2023-05-21 15:31:36.344640 keksik_api-0.1.5/keksik_api/schemas/__pycache__/events.cpython-311.pyc
+-rw-r--r--   0        0        0     2757 2023-05-20 13:25:46.555794 keksik_api-0.1.5/keksik_api/schemas/__pycache__/payments.cpython-311.pyc
+-rw-r--r--   0        0        0      456 2023-05-20 14:28:50.491512 keksik_api-0.1.5/keksik_api/schemas/base.py
+-rw-r--r--   0        0        0     1331 2023-05-20 12:27:12.277779 keksik_api-0.1.5/keksik_api/schemas/campaigns.py
+-rw-r--r--   0        0        0     1051 2023-05-20 11:59:33.646543 keksik_api-0.1.5/keksik_api/schemas/donates.py
+-rw-r--r--   0        0        0      703 2023-05-21 15:31:26.900172 keksik_api-0.1.5/keksik_api/schemas/events.py
+-rw-r--r--   0        0        0      947 2023-05-20 12:51:48.242846 keksik_api-0.1.5/keksik_api/schemas/payments.py
+-rw-r--r--   0        0        0      522 2023-05-21 15:31:58.653748 keksik_api-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2126 1970-01-01 00:00:00.000000 keksik_api-0.1.5/PKG-INFO
```

### Comparing `keksik_api-0.1.4/LICENSE` & `keksik_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/README.md` & `keksik_api-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/api.py` & `keksik_api-0.1.5/keksik_api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 
 import aiohttp
 
 from keksik_api.base import ABCAPI
 from keksik_api.exceptions import KeksikAPIException
 from keksik_api.methods.campaigns import CampaignsCategory
 from keksik_api.methods.donates import DonatesCategory
+from keksik_api.methods.payments import PaymentsCategory
 
 __all__ = ('KeksikAPI',)
 
-from keksik_api.methods.payments import PaymentsCategory
-
 logger = logging.getLogger('keksik_api')
 
 
 class KeksikAPI(ABCAPI):
 
     def __init__(
             self,
```

### Comparing `keksik_api-0.1.4/keksik_api/callback/__pycache__/callback.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/callback/__pycache__/callback.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x132c6a64 (Sun May 21 14:34:59 2023 UTC)
-files sz: 2410
+moddate:  0xf5376a64 (Sun May 21 15:25:41 2023 UTC)
+files sz: 2590
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -133,30 +133,30 @@
                       64 LOAD_CONST               8 ('return')
                       66 LOAD_NAME               10 (bool)
                       68 BUILD_TUPLE              4
                       70 LOAD_CONST               9 (<code object check_hash, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py", line 29>)
                       72 MAKE_FUNCTION            4 (annotations)
                       74 STORE_NAME              11 (check_hash)
          
-          40          76 LOAD_CONST              16 (('',))
+          45          76 LOAD_CONST              16 (('',))
                       78 LOAD_CONST               7 ('params')
                       80 LOAD_NAME                9 (dict)
                       82 LOAD_CONST              11 ('index')
                       84 LOAD_NAME                4 (str)
                       86 BUILD_TUPLE              4
-                      88 LOAD_CONST              12 (<code object get_hash_dict, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py", line 40>)
+                      88 LOAD_CONST              12 (<code object get_hash_dict, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py", line 45>)
                       90 MAKE_FUNCTION            5 (defaults, annotations)
                       92 STORE_NAME              12 (get_hash_dict)
          
-          52          94 LOAD_CONST              13 ('event')
+          57          94 LOAD_CONST              13 ('event')
                       96 LOAD_NAME                9 (dict)
                       98 LOAD_CONST               8 ('return')
                      100 LOAD_NAME                9 (dict)
                      102 BUILD_TUPLE              4
-                     104 LOAD_CONST              14 (<code object route_web_request, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py", line 52>)
+                     104 LOAD_CONST              14 (<code object route_web_request, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py", line 57>)
                      106 MAKE_FUNCTION            4 (annotations)
                      108 STORE_NAME              13 (route_web_request)
                      110 LOAD_CONST               1 (None)
                      112 RETURN_VALUE
          consts
             'Callback'
             None
@@ -225,19 +225,20 @@
                   007c01a0030000000000000000000000000000000000000000a6000000ab
                   000000000000000000a6010000ab010000000000000000a6010000ab0100
                   000000000000007d017409000000000000000000007c01a0050000000000
                   000000000000000000000000000000a6000000ab000000000000000000a6
                   010000ab0100000000000000007d037c03a0060000000000000000000000
                   0000000000000000007c006a070000000000000000a6010000ab01000000
                   000000000001006402a00800000000000000000000000000000000000000
-                  007c03a6010000ab0100000000000000007d047413000000000000000000
-                  006a0a00000000000000007c04a00b000000000000000000000000000000
-                  0000000000a6000000ab000000000000000000a6010000ab010000000000
-                  000000a00c0000000000000000000000000000000000000000a6000000ab
-                  0000000000000000007d057c057c026b02000000005300
+                  00640384007c034400a6000000ab000000000000000000a6010000ab0100
+                  000000000000007d047413000000000000000000006a0a00000000000000
+                  007c04a00b0000000000000000000000000000000000000000a6000000ab
+                  000000000000000000a6010000ab010000000000000000a00c0000000000
+                  000000000000000000000000000000a6000000ab0000000000000000007d
+                  057c057c026b02000000005300
                 29           0 RESUME                   0
                
                 30           2 LOAD_FAST                1 (params)
                              4 LOAD_CONST               1 ('hash')
                              6 BINARY_SUBSCR
                             16 STORE_FAST               2 (hash_value)
                
@@ -279,48 +280,114 @@
                            250 LOAD_ATTR                7 (_secret_key)
                            260 PRECALL                  1
                            264 CALL                     1
                            274 POP_TOP
                
                 36         276 LOAD_CONST               2 (',')
                            278 LOAD_METHOD              8 (join)
-                           300 LOAD_FAST                3 (params_values)
-                           302 PRECALL                  1
-                           306 CALL                     1
-                           316 STORE_FAST               4 (hash_str)
-               
-                37         318 LOAD_GLOBAL             19 (NULL + hashlib)
-                           330 LOAD_ATTR               10 (sha256)
-                           340 LOAD_FAST                4 (hash_str)
-                           342 LOAD_METHOD             11 (encode)
-                           364 PRECALL                  0
-                           368 CALL                     0
-                           378 PRECALL                  1
-                           382 CALL                     1
-                           392 LOAD_METHOD             12 (hexdigest)
-                           414 PRECALL                  0
-                           418 CALL                     0
-                           428 STORE_FAST               5 (sha256)
-               
-                38         430 LOAD_FAST                5 (sha256)
-                           432 LOAD_FAST                2 (hash_value)
-                           434 COMPARE_OP               2 (==)
-                           440 RETURN_VALUE
+                           300 LOAD_CONST               3 (<code object <listcomp>, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py", line 36>)
+                           302 MAKE_FUNCTION            0
+               
+                40         304 LOAD_FAST                3 (params_values)
+               
+                36         306 GET_ITER
+                           308 PRECALL                  0
+                           312 CALL                     0
+                           322 PRECALL                  1
+                           326 CALL                     1
+                           336 STORE_FAST               4 (hash_str)
+               
+                42         338 LOAD_GLOBAL             19 (NULL + hashlib)
+                           350 LOAD_ATTR               10 (sha256)
+                           360 LOAD_FAST                4 (hash_str)
+                           362 LOAD_METHOD             11 (encode)
+                           384 PRECALL                  0
+                           388 CALL                     0
+                           398 PRECALL                  1
+                           402 CALL                     1
+                           412 LOAD_METHOD             12 (hexdigest)
+                           434 PRECALL                  0
+                           438 CALL                     0
+                           448 STORE_FAST               5 (sha256)
+               
+                43         450 LOAD_FAST                5 (sha256)
+                           452 LOAD_FAST                2 (hash_value)
+                           454 COMPARE_OP               2 (==)
+                           460 RETURN_VALUE
                consts
                   None
                   'hash'
                   ','
+                  code
+                     argcount  : 1
+                     nlocals   : 2
+                     stacksize : 6
+                     flags     : 19
+                     code
+                        0x970067007c005d437d017401000000000000000000007c017402000000
+                        00000000000000a6020000ab02000000000000000072067c01720264006e
+                        2764016e257401000000000000000000007c017404000000000000000000
+                        00a6020000ab020000000000000000730f7405000000000000000000007c
+                        01a6010000ab0100000000000000006e017c0191028c445300
+                      36           0 RESUME                   0
+                                   2 BUILD_LIST               0
+                                   4 LOAD_FAST                0 (.0)
+                             >>    6 FOR_ITER                67 (to 142)
+                     
+                      40           8 STORE_FAST               1 (value)
+                     
+                      37          10 LOAD_GLOBAL              1 (NULL + isinstance)
+                                  22 LOAD_FAST                1 (value)
+                                  24 LOAD_GLOBAL              2 (bool)
+                                  36 PRECALL                  2
+                                  40 CALL                     2
+                                  50 POP_JUMP_FORWARD_IF_FALSE     6 (to 64)
+                                  52 LOAD_FAST                1 (value)
+                                  54 POP_JUMP_FORWARD_IF_FALSE     2 (to 60)
+                                  56 LOAD_CONST               0 ('1')
+                                  58 JUMP_FORWARD            39 (to 138)
+                             >>   60 LOAD_CONST               1 ('')
+                                  62 JUMP_FORWARD            37 (to 138)
+                     
+                      38     >>   64 LOAD_GLOBAL              1 (NULL + isinstance)
+                                  76 LOAD_FAST                1 (value)
+                                  78 LOAD_GLOBAL              4 (str)
+                                  90 PRECALL                  2
+                                  94 CALL                     2
+                                 104 POP_JUMP_FORWARD_IF_TRUE    15 (to 136)
+                                 106 LOAD_GLOBAL              5 (NULL + str)
+                                 118 LOAD_FAST                1 (value)
+                                 120 PRECALL                  1
+                                 124 CALL                     1
+                                 134 JUMP_FORWARD             1 (to 138)
+                     
+                      39     >>  136 LOAD_FAST                1 (value)
+                     
+                      36     >>  138 LIST_APPEND              2
+                                 140 JUMP_BACKWARD           68 (to 6)
+                             >>  142 RETURN_VALUE
+                     consts
+                        '1'
+                        ''
+                     names      ('isinstance', 'bool', 'str')
+                     varnames   ('.0', 'value')
+                     freevars   ()
+                     cellvars   ()
+                     filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py'
+                     name       '<listcomp>'
+                     firstlineno 36
+                     lnotab 0x080402fd3601480102fd
                names      ('get_hash_dict', 'dict', 'sorted', 'items', 'list', 'values', 'append', '_secret_key', 'join', 'hashlib', 'sha256', 'encode', 'hexdigest')
                varnames   ('self', 'params', 'hash_value', 'params_values', 'hash_str', 'sha256')
                freevars   ()
                cellvars   ()
                filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py'
                name       'check_hash'
                firstlineno 29
-               lnotab 0x0201100106012a015c01420134012a017001
+               lnotab 0x0201100106012a015c01420134011c0402fc20067001
             ''
             'index'
             code
                argcount  : 3
                nlocals   : 7
                stacksize : 6
                flags     : 3
@@ -329,82 +396,82 @@
                   000000000000000000000000000000a6000000ab00000000000000000044
                   005d515c0200007d047d057403000000000000000000007c057404000000
                   00000000000000a6020000ab020000000000000000722f7c00a003000000
                   00000000000000000000000000000000007c057c027c047a000000a60200
                   00ab0200000000000000007d067c03a00400000000000000000000000000
                   000000000000007c06a6010000ab01000000000000000001008c497c057c
                   037c027c047a0000003c0000008c527c035300
-                40           0 RESUME                   0
+                45           0 RESUME                   0
                
-                41           2 BUILD_MAP                0
+                46           2 BUILD_MAP                0
                              4 STORE_FAST               3 (hash_dict)
                
-                42           6 LOAD_FAST                2 (index)
+                47           6 LOAD_FAST                2 (index)
                              8 POP_JUMP_FORWARD_IF_FALSE     5 (to 20)
                
-                43          10 LOAD_FAST                2 (index)
+                48          10 LOAD_FAST                2 (index)
                             12 LOAD_CONST               1 ('/')
                             14 BINARY_OP               13 (+=)
                             18 STORE_FAST               2 (index)
                
-                44     >>   20 LOAD_FAST                1 (params)
+                49     >>   20 LOAD_FAST                1 (params)
                             22 LOAD_METHOD              0 (items)
                             44 PRECALL                  0
                             48 CALL                     0
                             58 GET_ITER
                        >>   60 FOR_ITER                81 (to 224)
                             62 UNPACK_SEQUENCE          2
                             66 STORE_FAST               4 (key)
                             68 STORE_FAST               5 (val)
                
-                45          70 LOAD_GLOBAL              3 (NULL + isinstance)
+                50          70 LOAD_GLOBAL              3 (NULL + isinstance)
                             82 LOAD_FAST                5 (val)
                             84 LOAD_GLOBAL              4 (dict)
                             96 PRECALL                  2
                            100 CALL                     2
                            110 POP_JUMP_FORWARD_IF_FALSE    47 (to 206)
                
-                46         112 LOAD_FAST                0 (self)
+                51         112 LOAD_FAST                0 (self)
                            114 LOAD_METHOD              3 (get_hash_dict)
                            136 LOAD_FAST                5 (val)
                            138 LOAD_FAST                2 (index)
                            140 LOAD_FAST                4 (key)
                            142 BINARY_OP                0 (+)
                            146 PRECALL                  2
                            150 CALL                     2
                            160 STORE_FAST               6 (new_dict)
                
-                47         162 LOAD_FAST                3 (hash_dict)
+                52         162 LOAD_FAST                3 (hash_dict)
                            164 LOAD_METHOD              4 (update)
                            186 LOAD_FAST                6 (new_dict)
                            188 PRECALL                  1
                            192 CALL                     1
                            202 POP_TOP
                            204 JUMP_BACKWARD           73 (to 60)
                
-                49     >>  206 LOAD_FAST                5 (val)
+                54     >>  206 LOAD_FAST                5 (val)
                            208 LOAD_FAST                3 (hash_dict)
                            210 LOAD_FAST                2 (index)
                            212 LOAD_FAST                4 (key)
                            214 BINARY_OP                0 (+)
                            218 STORE_SUBSCR
                            222 JUMP_BACKWARD           82 (to 60)
                
-                50     >>  224 LOAD_FAST                3 (hash_dict)
+                55     >>  224 LOAD_FAST                3 (hash_dict)
                            226 RETURN_VALUE
                consts
                   None
                   '/'
                names      ('items', 'isinstance', 'dict', 'get_hash_dict', 'update')
                varnames   ('self', 'params', 'index', 'hash_dict', 'key', 'val', 'new_dict')
                freevars   ()
                cellvars   ()
                filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py'
                name       'get_hash_dict'
-               firstlineno 40
+               firstlineno 45
                lnotab 0x0201040104010a0132012a0132012c021201
             'event'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 7
                flags     : 131
@@ -427,114 +494,114 @@
                   00ab0100000000000000007c0276017208741e000000000000000000007d
                   036e0e7c027c01640519000000000000000000190000000000000000007d
                   037c006a100000000000000000a011000000000000000000000000000000
                   00000000007c03a012000000000000000000000000000000000000000069
                   007c01a501640b7c006a0600000000000000006901a501a6010000ab0100
                   00000000000000a6010000ab010000000000000000830064007b03560097
                   0386040100640c640969015300
-                52           0 RETURN_GENERATOR
+                57           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                53           6 LOAD_GLOBAL              0 (logger)
+                58           6 LOAD_GLOBAL              0 (logger)
                             18 LOAD_METHOD              1 (debug)
                             40 LOAD_CONST               1 ('New event: ')
                             42 LOAD_FAST                1 (event)
                             44 FORMAT_VALUE             0
                             46 BUILD_STRING             2
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-                54          64 LOAD_FAST                0 (self)
+                59          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              2 (check_hash)
                             88 LOAD_FAST                1 (event)
                             90 LOAD_METHOD              3 (copy)
                            112 PRECALL                  0
                            116 CALL                     0
                            126 PRECALL                  1
                            130 CALL                     1
                            140 POP_JUMP_FORWARD_IF_TRUE     5 (to 152)
                
-                55         142 LOAD_CONST               2 ('error')
+                60         142 LOAD_CONST               2 ('error')
                            144 LOAD_CONST               3 ('Invalid hash')
                            146 LOAD_CONST               4 (('status', 'msg'))
                            148 BUILD_CONST_KEY_MAP      2
                            150 RETURN_VALUE
                
-                56     >>  152 LOAD_FAST                1 (event)
+                61     >>  152 LOAD_FAST                1 (event)
                            154 LOAD_METHOD              4 (get)
                            176 LOAD_CONST               5 ('type')
                            178 PRECALL                  1
                            182 CALL                     1
                            192 LOAD_CONST               6 ('confirmation')
                            194 COMPARE_OP               2 (==)
                            200 POP_JUMP_FORWARD_IF_FALSE    63 (to 328)
                
-                57         202 LOAD_FAST                1 (event)
+                62         202 LOAD_FAST                1 (event)
                            204 LOAD_METHOD              4 (get)
                            226 LOAD_CONST               7 ('group')
                            228 PRECALL                  1
                            232 CALL                     1
                            242 LOAD_GLOBAL             11 (NULL + str)
                            254 LOAD_FAST                0 (self)
                            256 LOAD_ATTR                6 (api)
                            266 LOAD_ATTR                7 (group_id)
                            276 PRECALL                  1
                            280 CALL                     1
                            290 COMPARE_OP               3 (!=)
                            296 POP_JUMP_FORWARD_IF_FALSE     5 (to 308)
                
-                58         298 LOAD_CONST               2 ('error')
+                63         298 LOAD_CONST               2 ('error')
                            300 LOAD_CONST               8 ('Invalid group id')
                            302 LOAD_CONST               4 (('status', 'msg'))
                            304 BUILD_CONST_KEY_MAP      2
                            306 RETURN_VALUE
                
-                59     >>  308 LOAD_CONST               9 ('ok')
+                64     >>  308 LOAD_CONST               9 ('ok')
                            310 LOAD_FAST                0 (self)
                            312 LOAD_ATTR                8 (_confirmation_code)
                            322 LOAD_CONST              10 (('status', 'code'))
                            324 BUILD_CONST_KEY_MAP      2
                            326 RETURN_VALUE
                
-                62     >>  328 LOAD_GLOBAL             18 (EventType)
+                67     >>  328 LOAD_GLOBAL             18 (EventType)
                            340 LOAD_ATTR               10 (NEW_DONATE)
                            350 LOAD_ATTR               11 (value)
                            360 LOAD_GLOBAL             24 (DonateEvent)
                
-                63         372 LOAD_GLOBAL             18 (EventType)
+                68         372 LOAD_GLOBAL             18 (EventType)
                            384 LOAD_ATTR               13 (PAYMENT_STATUS)
                            394 LOAD_ATTR               11 (value)
                            404 LOAD_GLOBAL             28 (PaymentStatusEvent)
                
-                61         416 BUILD_MAP                2
+                66         416 BUILD_MAP                2
                            418 STORE_FAST               2 (type_to_dataclass)
                
-                65         420 LOAD_FAST                1 (event)
+                70         420 LOAD_FAST                1 (event)
                            422 LOAD_METHOD              4 (get)
                            444 LOAD_CONST               5 ('type')
                            446 PRECALL                  1
                            450 CALL                     1
                            460 LOAD_FAST                2 (type_to_dataclass)
                            462 CONTAINS_OP              1
                            464 POP_JUMP_FORWARD_IF_FALSE     8 (to 482)
                
-                66         466 LOAD_GLOBAL             30 (Event)
+                71         466 LOAD_GLOBAL             30 (Event)
                            478 STORE_FAST               3 (dataclass)
                            480 JUMP_FORWARD            14 (to 510)
                
-                68     >>  482 LOAD_FAST                2 (type_to_dataclass)
+                73     >>  482 LOAD_FAST                2 (type_to_dataclass)
                            484 LOAD_FAST                1 (event)
                            486 LOAD_CONST               5 ('type')
                            488 BINARY_SUBSCR
                            498 BINARY_SUBSCR
                            508 STORE_FAST               3 (dataclass)
                
-                69     >>  510 LOAD_FAST                0 (self)
+                74     >>  510 LOAD_FAST                0 (self)
                            512 LOAD_ATTR               16 (router)
                            522 LOAD_METHOD             17 (route)
                            544 LOAD_FAST                3 (dataclass)
                            546 LOAD_METHOD             18 (parse_obj)
                            568 BUILD_MAP                0
                            570 LOAD_FAST                1 (event)
                            572 DICT_UPDATE              1
@@ -551,15 +618,15 @@
                            622 LOAD_CONST               0 (None)
                        >>  624 SEND                     3 (to 632)
                            626 YIELD_VALUE
                            628 RESUME                   3
                            630 JUMP_BACKWARD_NO_INTERRUPT     4 (to 624)
                        >>  632 POP_TOP
                
-                70         634 LOAD_CONST              12 ('status')
+                75         634 LOAD_CONST              12 ('status')
                            636 LOAD_CONST               9 ('ok')
                            638 BUILD_MAP                1
                            640 RETURN_VALUE
                consts
                   None
                   'New event: '
                   'error'
@@ -575,28 +642,28 @@
                   'status'
                names      ('logger', 'debug', 'check_hash', 'copy', 'get', 'str', 'api', 'group_id', '_confirmation_code', 'EventType', 'NEW_DONATE', 'value', 'DonateEvent', 'PAYMENT_STATUS', 'PaymentStatusEvent', 'Event', 'router', 'route', 'parse_obj')
                varnames   ('self', 'event', 'type_to_dataclass', 'dataclass')
                freevars   ()
                cellvars   ()
                filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py'
                name       'route_web_request'
-               firstlineno 52
+               firstlineno 57
                lnotab
                   0x06013a014e010a01320160010a0114032c012cfe04042e0110021c017c
                   01
             (None,)
             ('',)
          names      ('__name__', '__module__', '__qualname__', 'KeksikAPI', 'str', 'typing', 'Optional', 'Router', '__init__', 'dict', 'bool', 'check_hash', 'get_hash_dict', 'route_web_request')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py'
          name       'Callback'
          firstlineno 14
-         lnotab 0x0a0702fb040202fe020302fd020402fc020518fb080d100b120c
+         lnotab 0x0a0702fb040202fe020302fd020402fc020518fb080d1010120c
       'Callback'
    names      ('hashlib', 'logging', 'typing', 'keksik_api.api', 'KeksikAPI', 'keksik_api.schemas.events', 'EventType', 'Event', 'DonateEvent', 'PaymentStatusEvent', 'keksik_api.callback.router', 'Router', '__all__', 'getLogger', 'logger', 'Callback')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/callback.py'
    name       '<module>'
```

### Comparing `keksik_api-0.1.4/keksik_api/callback/__pycache__/handler.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/callback/__pycache__/handler.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/callback/__pycache__/router.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/callback/__pycache__/router.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/callback/__pycache__/rules.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/callback/__pycache__/rules.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/callback/callback.py` & `keksik_api-0.1.5/keksik_api/callback/callback.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/callback/handler.py` & `keksik_api-0.1.5/keksik_api/callback/handler.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/callback/router.py` & `keksik_api-0.1.5/keksik_api/callback/router.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/exceptions.py` & `keksik_api-0.1.5/keksik_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/methods/__pycache__/base.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/methods/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/methods/__pycache__/donates.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/methods/__pycache__/donates.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/methods/__pycache__/payments.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/methods/__pycache__/payments.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/methods/campaigns.py` & `keksik_api-0.1.5/keksik_api/methods/campaigns.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/methods/donates.py` & `keksik_api-0.1.5/keksik_api/methods/donates.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/methods/payments.py` & `keksik_api-0.1.5/keksik_api/methods/payments.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/schemas/__pycache__/base.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/schemas/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/schemas/__pycache__/donates.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/schemas/__pycache__/donates.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/schemas/__pycache__/events.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/schemas/__pycache__/events.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,139 +1,128 @@
 magic:    0xa70d0d0a
-moddate:  0x8cd66864 (Sat May 20 14:17:48 2023 UTC)
-files sz: 630
+moddate:  0x4e396a64 (Sun May 21 15:31:26 2023 UTC)
+files sz: 703
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a00640064016c015a01640064016c025a02640264
-      036c036d045a040100640264046c056d065a06010065016a070000000000
-      0000007206640064056c086d095a09010064065a0a020047006407840064
-      0865006a0b0000000000000000a6030000ab0300000000000000005a0c02
-      00470064098400640a65026a0d0000000000000000a6030000ab03000000
-      00000000005a0e02004700640b8400640c650ea6030000ab030000000000
-      0000005a0f02004700640d8400640e650ea6030000ab0300000000000000
-      005a1064015300
+      0x9700640064016c005a00640064016c015a01640064026c026d035a0301
+      00640064036c046d055a050100640064046c066d075a07010064055a0802
+      00470064068400640765006a090000000000000000a6030000ab03000000
+      00000000005a0a0200470064088400640965016a0b0000000000000000a6
+      030000ab0300000000000000005a0c02004700640a8400640b650ca60300
+      00ab0300000000000000005a0d02004700640c8400640d650ca6030000ab
+      0300000000000000005a0e64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (enum)
                  8 STORE_NAME               0 (enum)
    
-     2          10 LOAD_CONST               0 (0)
+     3          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (typing)
-                16 STORE_NAME               1 (typing)
+                14 IMPORT_NAME              1 (pydantic)
+                16 STORE_NAME               1 (pydantic)
    
-     4          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               1 (None)
-                22 IMPORT_NAME              2 (pydantic)
-                24 STORE_NAME               2 (pydantic)
-   
-     6          26 LOAD_CONST               2 (1)
-                28 LOAD_CONST               3 (('Donate',))
-                30 IMPORT_NAME              3 (donates)
-                32 IMPORT_FROM              4 (Donate)
-                34 STORE_NAME               4 (Donate)
-                36 POP_TOP
-   
-     7          38 LOAD_CONST               2 (1)
-                40 LOAD_CONST               4 (('Payment',))
-                42 IMPORT_NAME              5 (payments)
-                44 IMPORT_FROM              6 (Payment)
-                46 STORE_NAME               6 (Payment)
-                48 POP_TOP
-   
-     9          50 LOAD_NAME                1 (typing)
-                52 LOAD_ATTR                7 (TYPE_CHECKING)
-                62 POP_JUMP_FORWARD_IF_FALSE     6 (to 76)
-   
-    10          64 LOAD_CONST               0 (0)
-                66 LOAD_CONST               5 (('KeksikAPI',))
-                68 IMPORT_NAME              8 (keksik_api)
-                70 IMPORT_FROM              9 (KeksikAPI)
-                72 STORE_NAME               9 (KeksikAPI)
-                74 POP_TOP
-   
-    12     >>   76 LOAD_CONST               6 (('EventType', 'Event', 'DonateEvent', 'PaymentStatusEvent'))
-                78 STORE_NAME              10 (__all__)
-   
-    20          80 PUSH_NULL
-                82 LOAD_BUILD_CLASS
-                84 LOAD_CONST               7 (<code object EventType, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py", line 20>)
-                86 MAKE_FUNCTION            0
-                88 LOAD_CONST               8 ('EventType')
-                90 LOAD_NAME                0 (enum)
-                92 LOAD_ATTR               11 (Enum)
-               102 PRECALL                  3
-               106 CALL                     3
-               116 STORE_NAME              12 (EventType)
-   
-    26         118 PUSH_NULL
-               120 LOAD_BUILD_CLASS
-               122 LOAD_CONST               9 (<code object Event, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py", line 26>)
-               124 MAKE_FUNCTION            0
-               126 LOAD_CONST              10 ('Event')
-               128 LOAD_NAME                2 (pydantic)
-               130 LOAD_ATTR               13 (BaseModel)
-               140 PRECALL                  3
-               144 CALL                     3
-               154 STORE_NAME              14 (Event)
-   
-    33         156 PUSH_NULL
-               158 LOAD_BUILD_CLASS
-               160 LOAD_CONST              11 (<code object DonateEvent, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py", line 33>)
-               162 MAKE_FUNCTION            0
-               164 LOAD_CONST              12 ('DonateEvent')
-               166 LOAD_NAME               14 (Event)
-               168 PRECALL                  3
-               172 CALL                     3
-               182 STORE_NAME              15 (DonateEvent)
-   
-    37         184 PUSH_NULL
-               186 LOAD_BUILD_CLASS
-               188 LOAD_CONST              13 (<code object PaymentStatusEvent, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py", line 37>)
-               190 MAKE_FUNCTION            0
-               192 LOAD_CONST              14 ('PaymentStatusEvent')
-               194 LOAD_NAME               14 (Event)
-               196 PRECALL                  3
-               200 CALL                     3
-               210 STORE_NAME              16 (PaymentStatusEvent)
-               212 LOAD_CONST               1 (None)
-               214 RETURN_VALUE
+     5          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('KeksikAPI',))
+                22 IMPORT_NAME              2 (keksik_api.api)
+                24 IMPORT_FROM              3 (KeksikAPI)
+                26 STORE_NAME               3 (KeksikAPI)
+                28 POP_TOP
+   
+     6          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('Donate',))
+                34 IMPORT_NAME              4 (keksik_api.schemas.donates)
+                36 IMPORT_FROM              5 (Donate)
+                38 STORE_NAME               5 (Donate)
+                40 POP_TOP
+   
+     7          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               4 (('Payment',))
+                46 IMPORT_NAME              6 (keksik_api.schemas.payments)
+                48 IMPORT_FROM              7 (Payment)
+                50 STORE_NAME               7 (Payment)
+                52 POP_TOP
+   
+     9          54 LOAD_CONST               5 (('EventType', 'Event', 'DonateEvent', 'PaymentStatusEvent'))
+                56 STORE_NAME               8 (__all__)
+   
+    17          58 PUSH_NULL
+                60 LOAD_BUILD_CLASS
+                62 LOAD_CONST               6 (<code object EventType, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py", line 17>)
+                64 MAKE_FUNCTION            0
+                66 LOAD_CONST               7 ('EventType')
+                68 LOAD_NAME                0 (enum)
+                70 LOAD_ATTR                9 (Enum)
+                80 PRECALL                  3
+                84 CALL                     3
+                94 STORE_NAME              10 (EventType)
+   
+    23          96 PUSH_NULL
+                98 LOAD_BUILD_CLASS
+               100 LOAD_CONST               8 (<code object Event, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py", line 23>)
+               102 MAKE_FUNCTION            0
+               104 LOAD_CONST               9 ('Event')
+               106 LOAD_NAME                1 (pydantic)
+               108 LOAD_ATTR               11 (BaseModel)
+               118 PRECALL                  3
+               122 CALL                     3
+               132 STORE_NAME              12 (Event)
+   
+    33         134 PUSH_NULL
+               136 LOAD_BUILD_CLASS
+               138 LOAD_CONST              10 (<code object DonateEvent, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py", line 33>)
+               140 MAKE_FUNCTION            0
+               142 LOAD_CONST              11 ('DonateEvent')
+               144 LOAD_NAME               12 (Event)
+               146 PRECALL                  3
+               150 CALL                     3
+               160 STORE_NAME              13 (DonateEvent)
+   
+    37         162 PUSH_NULL
+               164 LOAD_BUILD_CLASS
+               166 LOAD_CONST              12 (<code object PaymentStatusEvent, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py", line 37>)
+               168 MAKE_FUNCTION            0
+               170 LOAD_CONST              13 ('PaymentStatusEvent')
+               172 LOAD_NAME               12 (Event)
+               174 PRECALL                  3
+               178 CALL                     3
+               188 STORE_NAME              14 (PaymentStatusEvent)
+               190 LOAD_CONST               1 (None)
+               192 RETURN_VALUE
    consts
       0
       None
-      1
+      ('KeksikAPI',)
       ('Donate',)
       ('Payment',)
-      ('KeksikAPI',)
       ('EventType', 'Event', 'DonateEvent', 'PaymentStatusEvent')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025a0464035a0564045300
-          20           0 RESUME                   0
+          17           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('EventType')
                        8 STORE_NAME               2 (__qualname__)
          
-          21          10 LOAD_CONST               1 ('confirmation')
+          18          10 LOAD_CONST               1 ('confirmation')
                       12 STORE_NAME               3 (CONFIRMATION)
          
-          22          14 LOAD_CONST               2 ('new_donate')
+          19          14 LOAD_CONST               2 ('new_donate')
                       16 STORE_NAME               4 (NEW_DONATE)
          
-          23          18 LOAD_CONST               3 ('payment_status')
+          20          18 LOAD_CONST               3 ('payment_status')
                       20 STORE_NAME               5 (PAYMENT_STATUS)
                       22 LOAD_CONST               4 (None)
                       24 RETURN_VALUE
          consts
             'EventType'
             'confirmation'
             'new_donate'
@@ -141,81 +130,121 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'CONFIRMATION', 'NEW_DONATE', 'PAYMENT_STATUS')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py'
          name       'EventType'
-         firstlineno 20
+         firstlineno 17
          lnotab 0x0a0104010401
       'EventType'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 3
+         stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a025500020065036a0400000000000000006401ac
             02a6010000ab0100000000000000005a056506650764033c000000650865
-            0764043c0000006509650764053c0000006406650764073c000000640853
-            00
-          26           0 RESUME                   0
+            0764043c0000006509650764053c000000650a650764063c000000020047
+            0064078400640865036a0b0000000000000000a6030000ab030000000000
+            0000005a0c64095300
+          23           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Event')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          27          12 PUSH_NULL
+          24          12 PUSH_NULL
                       14 LOAD_NAME                3 (pydantic)
                       16 LOAD_ATTR                4 (Field)
                       26 LOAD_CONST               1 ('group')
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_NAME               5 (group_id)
                       46 LOAD_NAME                6 (int)
                       48 LOAD_NAME                7 (__annotations__)
                       50 LOAD_CONST               3 ('group_id')
                       52 STORE_SUBSCR
          
-          28          56 LOAD_NAME                8 (EventType)
+          25          56 LOAD_NAME                8 (EventType)
                       58 LOAD_NAME                7 (__annotations__)
                       60 LOAD_CONST               4 ('type')
                       62 STORE_SUBSCR
          
-          29          66 LOAD_NAME                9 (str)
+          26          66 LOAD_NAME                9 (str)
                       68 LOAD_NAME                7 (__annotations__)
                       70 LOAD_CONST               5 ('hash')
                       72 STORE_SUBSCR
          
-          30          76 LOAD_CONST               6 ('KeksikAPI')
+          27          76 LOAD_NAME               10 (KeksikAPI)
                       78 LOAD_NAME                7 (__annotations__)
-                      80 LOAD_CONST               7 ('api')
+                      80 LOAD_CONST               6 ('api')
                       82 STORE_SUBSCR
-                      86 LOAD_CONST               8 (None)
-                      88 RETURN_VALUE
+         
+          29          86 PUSH_NULL
+                      88 LOAD_BUILD_CLASS
+                      90 LOAD_CONST               7 (<code object Config, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py", line 29>)
+                      92 MAKE_FUNCTION            0
+                      94 LOAD_CONST               8 ('Config')
+                      96 LOAD_NAME                3 (pydantic)
+                      98 LOAD_ATTR               11 (BaseConfig)
+                     108 PRECALL                  3
+                     112 CALL                     3
+                     122 STORE_NAME              12 (Config)
+                     124 LOAD_CONST               9 (None)
+                     126 RETURN_VALUE
          consts
             'Event'
             'group'
             ('alias',)
             'group_id'
             'type'
             'hash'
-            'KeksikAPI'
             'api'
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 1
+               flags     : 0
+               code 0x970065005a0164005a0264015a0364025300
+                29           0 RESUME                   0
+                             2 LOAD_NAME                0 (__name__)
+                             4 STORE_NAME               1 (__module__)
+                             6 LOAD_CONST               0 ('Event.Config')
+                             8 STORE_NAME               2 (__qualname__)
+               
+                30          10 LOAD_CONST               1 (True)
+                            12 STORE_NAME               3 (arbitrary_types_allowed)
+                            14 LOAD_CONST               2 (None)
+                            16 RETURN_VALUE
+               consts
+                  'Event.Config'
+                  True
+                  None
+               names      ('__name__', '__module__', '__qualname__', 'arbitrary_types_allowed')
+               varnames   ()
+               freevars   ()
+               cellvars   ()
+               filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py'
+               name       'Config'
+               firstlineno 29
+               lnotab 0x0a01
+            'Config'
             None
-         names      ('__name__', '__module__', '__qualname__', 'pydantic', 'Field', 'group_id', 'int', '__annotations__', 'EventType', 'str')
+         names      ('__name__', '__module__', '__qualname__', 'pydantic', 'Field', 'group_id', 'int', '__annotations__', 'EventType', 'str', 'KeksikAPI', 'BaseConfig', 'Config')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py'
          name       'Event'
-         firstlineno 26
-         lnotab 0x0c012c010a010a01
+         firstlineno 23
+         lnotab 0x0c012c010a010a010a02
       'Event'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code 0x970065005a0164005a0255006503650464013c00000064025300
@@ -273,15 +302,15 @@
          freevars   ()
          cellvars   ()
          filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py'
          name       'PaymentStatusEvent'
          firstlineno 37
          lnotab 0x0c01
       'PaymentStatusEvent'
-   names      ('enum', 'typing', 'pydantic', 'donates', 'Donate', 'payments', 'Payment', 'TYPE_CHECKING', 'keksik_api', 'KeksikAPI', '__all__', 'Enum', 'EventType', 'BaseModel', 'Event', 'DonateEvent', 'PaymentStatusEvent')
+   names      ('enum', 'pydantic', 'keksik_api.api', 'KeksikAPI', 'keksik_api.schemas.donates', 'Donate', 'keksik_api.schemas.payments', 'Payment', '__all__', 'Enum', 'EventType', 'BaseModel', 'Event', 'DonateEvent', 'PaymentStatusEvent')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/events.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010801080208020c010c020e010c020408260626071c04
+   lnotab 0x00ff0201080208020c010c010c0204082606260a1c04
```

### Comparing `keksik_api-0.1.4/keksik_api/schemas/__pycache__/payments.cpython-311.pyc` & `keksik_api-0.1.5/keksik_api/schemas/__pycache__/payments.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/schemas/campaigns.py` & `keksik_api-0.1.5/keksik_api/schemas/campaigns.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/schemas/donates.py` & `keksik_api-0.1.5/keksik_api/schemas/donates.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/keksik_api/schemas/payments.py` & `keksik_api-0.1.5/keksik_api/schemas/payments.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.4/pyproject.toml` & `keksik_api-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keksik-api"
-version = "0.1.4"
+version = "0.1.5"
 description = "Обвертка над API keksik.io"
 authors = ["lordralinc <lordralinc@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "keksik_api"}]
 
 [tool.poetry.dependencies]
```

### Comparing `keksik_api-0.1.4/PKG-INFO` & `keksik_api-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keksik-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: Обвертка над API keksik.io
 License: MIT
 Author: lordralinc
 Author-email: lordralinc@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

