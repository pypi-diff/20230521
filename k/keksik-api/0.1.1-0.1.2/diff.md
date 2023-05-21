# Comparing `tmp/keksik_api-0.1.1.tar.gz` & `tmp/keksik_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keksik_api-0.1.1.tar", max compression
+gzip compressed data, was "keksik_api-0.1.2.tar", max compression
```

## Comparing `keksik_api-0.1.1.tar` & `keksik_api-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1070 2023-05-20 12:43:03.823356 keksik_api-0.1.1/LICENSE
--rw-r--r--   0        0        0     1513 2023-05-20 14:27:31.868826 keksik_api-0.1.1/README.md
--rw-r--r--   0        0        0      260 2023-05-20 14:31:15.277096 keksik_api-0.1.1/keksik_api/__init__.py
--rw-r--r--   0        0        0     2339 2023-05-20 12:26:06.514655 keksik_api-0.1.1/keksik_api/api.py
--rw-r--r--   0        0        0      186 2023-05-20 10:59:09.616140 keksik_api-0.1.1/keksik_api/base.py
--rw-r--r--   0        0        0       98 2023-05-20 14:23:04.945309 keksik_api-0.1.1/keksik_api/callback/__init__.py
--rw-r--r--   0        0        0      193 2023-05-20 13:25:46.835790 keksik_api-0.1.1/keksik_api/callback/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3352 2023-05-20 13:35:39.149843 keksik_api-0.1.1/keksik_api/callback/__pycache__/callback.cpython-311.pyc
--rw-r--r--   0        0        0     1917 2023-05-20 14:17:48.922674 keksik_api-0.1.1/keksik_api/callback/__pycache__/handler.cpython-311.pyc
--rw-r--r--   0        0        0     3472 2023-05-20 14:17:48.918674 keksik_api-0.1.1/keksik_api/callback/__pycache__/router.cpython-311.pyc
--rw-r--r--   0        0        0     1508 2023-05-20 14:17:48.922674 keksik_api-0.1.1/keksik_api/callback/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     2367 2023-05-21 13:09:06.282102 keksik_api-0.1.1/keksik_api/callback/callback.py
--rw-r--r--   0        0        0      878 2023-05-21 13:09:06.566093 keksik_api-0.1.1/keksik_api/callback/handler.py
--rw-r--r--   0        0        0     1786 2023-05-21 13:09:06.422098 keksik_api-0.1.1/keksik_api/callback/router.py
--rw-r--r--   0        0        0      423 2023-05-21 13:09:06.686089 keksik_api-0.1.1/keksik_api/callback/rules.py
--rw-r--r--   0        0        0     1037 2023-05-20 10:39:54.109459 keksik_api-0.1.1/keksik_api/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-20 10:42:38.274538 keksik_api-0.1.1/keksik_api/methods/__init__.py
--rw-r--r--   0        0        0      192 2023-05-20 13:25:46.831790 keksik_api-0.1.1/keksik_api/methods/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      714 2023-05-20 13:25:46.831790 keksik_api-0.1.1/keksik_api/methods/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     6399 2023-05-20 13:25:46.831790 keksik_api-0.1.1/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc
--rw-r--r--   0        0        0     8800 2023-05-20 13:25:46.835790 keksik_api-0.1.1/keksik_api/methods/__pycache__/donates.cpython-311.pyc
--rw-r--r--   0        0        0      159 2023-05-20 10:59:09.576141 keksik_api-0.1.1/keksik_api/methods/base.py
--rw-r--r--   0        0        0     4850 2023-05-20 12:24:21.123997 keksik_api-0.1.1/keksik_api/methods/campaigns.py
--rw-r--r--   0        0        0     7099 2023-05-20 12:24:21.019999 keksik_api-0.1.1/keksik_api/methods/donates.py
--rw-r--r--   0        0        0     3204 2023-05-20 14:31:15.209097 keksik_api-0.1.1/keksik_api/methods/payments.py
--rw-r--r--   0        0        0      114 2023-05-20 14:17:48.110688 keksik_api-0.1.1/keksik_api/schemas/__init__.py
--rw-r--r--   0        0        0      339 2023-05-20 14:17:48.638678 keksik_api-0.1.1/keksik_api/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1216 2023-05-20 13:25:46.503795 keksik_api-0.1.1/keksik_api/schemas/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     3353 2023-05-20 13:25:46.543794 keksik_api-0.1.1/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc
--rw-r--r--   0        0        0     2786 2023-05-20 13:25:46.551794 keksik_api-0.1.1/keksik_api/schemas/__pycache__/donates.cpython-311.pyc
--rw-r--r--   0        0        0     1847 2023-05-20 14:17:48.666678 keksik_api-0.1.1/keksik_api/schemas/__pycache__/events.cpython-311.pyc
--rw-r--r--   0        0        0     2757 2023-05-20 13:25:46.555794 keksik_api-0.1.1/keksik_api/schemas/__pycache__/payments.cpython-311.pyc
--rw-r--r--   0        0        0      456 2023-05-20 14:28:50.491512 keksik_api-0.1.1/keksik_api/schemas/base.py
--rw-r--r--   0        0        0     1331 2023-05-20 12:27:12.277779 keksik_api-0.1.1/keksik_api/schemas/campaigns.py
--rw-r--r--   0        0        0     1051 2023-05-20 11:59:33.646543 keksik_api-0.1.1/keksik_api/schemas/donates.py
--rw-r--r--   0        0        0      630 2023-05-20 14:17:48.058688 keksik_api-0.1.1/keksik_api/schemas/events.py
--rw-r--r--   0        0        0      947 2023-05-20 12:51:48.242846 keksik_api-0.1.1/keksik_api/schemas/payments.py
--rw-r--r--   0        0        0      413 2023-05-21 13:09:09.417995 keksik_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2126 1970-01-01 00:00:00.000000 keksik_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-20 12:43:03.823356 keksik_api-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1513 2023-05-20 14:27:31.868826 keksik_api-0.1.2/README.md
+-rw-r--r--   0        0        0      260 2023-05-20 14:31:15.277096 keksik_api-0.1.2/keksik_api/__init__.py
+-rw-r--r--   0        0        0     2339 2023-05-20 12:26:06.514655 keksik_api-0.1.2/keksik_api/api.py
+-rw-r--r--   0        0        0      186 2023-05-20 10:59:09.616140 keksik_api-0.1.2/keksik_api/base.py
+-rw-r--r--   0        0        0       98 2023-05-20 14:23:04.945309 keksik_api-0.1.2/keksik_api/callback/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-21 14:34:07.095423 keksik_api-0.1.2/keksik_api/callback/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4473 2023-05-21 14:34:59.498604 keksik_api-0.1.2/keksik_api/callback/__pycache__/callback.cpython-311.pyc
+-rw-r--r--   0        0        0     2169 2023-05-21 14:34:59.574603 keksik_api-0.1.2/keksik_api/callback/__pycache__/handler.cpython-311.pyc
+-rw-r--r--   0        0        0     4411 2023-05-21 14:34:59.570603 keksik_api-0.1.2/keksik_api/callback/__pycache__/router.cpython-311.pyc
+-rw-r--r--   0        0        0     1508 2023-05-21 14:34:59.574603 keksik_api-0.1.2/keksik_api/callback/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     2410 2023-05-21 14:34:59.142609 keksik_api-0.1.2/keksik_api/callback/callback.py
+-rw-r--r--   0        0        0      878 2023-05-21 13:09:06.566093 keksik_api-0.1.2/keksik_api/callback/handler.py
+-rw-r--r--   0        0        0     1786 2023-05-21 13:09:06.422098 keksik_api-0.1.2/keksik_api/callback/router.py
+-rw-r--r--   0        0        0      423 2023-05-21 13:09:06.686089 keksik_api-0.1.2/keksik_api/callback/rules.py
+-rw-r--r--   0        0        0     1037 2023-05-20 10:39:54.109459 keksik_api-0.1.2/keksik_api/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-20 10:42:38.274538 keksik_api-0.1.2/keksik_api/methods/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-20 13:25:46.831790 keksik_api-0.1.2/keksik_api/methods/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      714 2023-05-20 13:25:46.831790 keksik_api-0.1.2/keksik_api/methods/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     6399 2023-05-20 13:25:46.831790 keksik_api-0.1.2/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc
+-rw-r--r--   0        0        0     8800 2023-05-20 13:25:46.835790 keksik_api-0.1.2/keksik_api/methods/__pycache__/donates.cpython-311.pyc
+-rw-r--r--   0        0        0      159 2023-05-20 10:59:09.576141 keksik_api-0.1.2/keksik_api/methods/base.py
+-rw-r--r--   0        0        0     4850 2023-05-20 12:24:21.123997 keksik_api-0.1.2/keksik_api/methods/campaigns.py
+-rw-r--r--   0        0        0     7099 2023-05-20 12:24:21.019999 keksik_api-0.1.2/keksik_api/methods/donates.py
+-rw-r--r--   0        0        0     3204 2023-05-20 14:31:15.209097 keksik_api-0.1.2/keksik_api/methods/payments.py
+-rw-r--r--   0        0        0      114 2023-05-20 14:17:48.110688 keksik_api-0.1.2/keksik_api/schemas/__init__.py
+-rw-r--r--   0        0        0      339 2023-05-20 14:17:48.638678 keksik_api-0.1.2/keksik_api/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1483 2023-05-21 14:34:07.035424 keksik_api-0.1.2/keksik_api/schemas/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     3353 2023-05-20 13:25:46.543794 keksik_api-0.1.2/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc
+-rw-r--r--   0        0        0     2786 2023-05-20 13:25:46.551794 keksik_api-0.1.2/keksik_api/schemas/__pycache__/donates.cpython-311.pyc
+-rw-r--r--   0        0        0     1847 2023-05-20 14:17:48.666678 keksik_api-0.1.2/keksik_api/schemas/__pycache__/events.cpython-311.pyc
+-rw-r--r--   0        0        0     2757 2023-05-20 13:25:46.555794 keksik_api-0.1.2/keksik_api/schemas/__pycache__/payments.cpython-311.pyc
+-rw-r--r--   0        0        0      456 2023-05-20 14:28:50.491512 keksik_api-0.1.2/keksik_api/schemas/base.py
+-rw-r--r--   0        0        0     1331 2023-05-20 12:27:12.277779 keksik_api-0.1.2/keksik_api/schemas/campaigns.py
+-rw-r--r--   0        0        0     1051 2023-05-20 11:59:33.646543 keksik_api-0.1.2/keksik_api/schemas/donates.py
+-rw-r--r--   0        0        0      630 2023-05-20 14:17:48.058688 keksik_api-0.1.2/keksik_api/schemas/events.py
+-rw-r--r--   0        0        0      947 2023-05-20 12:51:48.242846 keksik_api-0.1.2/keksik_api/schemas/payments.py
+-rw-r--r--   0        0        0      413 2023-05-21 14:35:55.685728 keksik_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2126 1970-01-01 00:00:00.000000 keksik_api-0.1.2/PKG-INFO
```

### Comparing `keksik_api-0.1.1/LICENSE` & `keksik_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/README.md` & `keksik_api-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/api.py` & `keksik_api-0.1.2/keksik_api/api.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/callback/__pycache__/handler.cpython-311.pyc` & `keksik_api-0.1.2/keksik_api/callback/__pycache__/handler.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x8bd66864 (Sat May 20 14:17:47 2023 UTC)
-files sz: 788
+moddate:  0xf2176a64 (Sun May 21 13:09:06 2023 UTC)
+files sz: 878
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -30,17 +30,17 @@
                 28 IMPORT_FROM              4 (Rule)
                 30 STORE_NAME               4 (Rule)
                 32 POP_TOP
    
      6          34 LOAD_CONST               4 (('Handler',))
                 36 STORE_NAME               5 (__all__)
    
-    11          38 PUSH_NULL
+     9          38 PUSH_NULL
                 40 LOAD_BUILD_CLASS
-                42 LOAD_CONST               5 (<code object Handler, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py", line 11>)
+                42 LOAD_CONST               5 (<code object Handler, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py", line 9>)
                 44 MAKE_FUNCTION            0
                 46 LOAD_CONST               6 ('Handler')
                 48 PRECALL                  2
                 52 CALL                     2
                 62 STORE_NAME               6 (Handler)
                 64 LOAD_CONST               1 (None)
                 66 RETURN_VALUE
@@ -63,31 +63,31 @@
             0319000000000000000000660219000000000000000000650664023c0000
             00640165036a040000000000000000650519000000000000000000640265
             036a07000000000000000065086a090000000000000000670165036a0a00
             0000000000000065036a0b000000000000000065036a0b00000000000000
             0065036a0b00000000000000006603190000000000000000006602190000
             000000000000006604640384045a0c640465086a09000000000000000064
             05650d6604640684045a0e640465086a0900000000000000006602640784
-            045a0f64085300
-          11           0 RESUME                   0
+            045a0f640884005a1064095300
+           9           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Handler')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          12          12 LOAD_NAME                3 (typing)
+          10          12 LOAD_NAME                3 (typing)
                       14 LOAD_ATTR                4 (List)
                       24 LOAD_NAME                5 (Rule)
                       26 BINARY_SUBSCR
                       36 LOAD_NAME                6 (__annotations__)
                       38 LOAD_CONST               1 ('rules')
                       40 STORE_SUBSCR
          
-          13          44 LOAD_NAME                3 (typing)
+          11          44 LOAD_NAME                3 (typing)
                       46 LOAD_ATTR                7 (Callable)
                       56 LOAD_NAME                8 (schemas)
                       58 LOAD_ATTR                9 (Event)
                       68 BUILD_LIST               1
                       70 LOAD_NAME                3 (typing)
                       72 LOAD_ATTR               10 (Coroutine)
                       82 LOAD_NAME                3 (typing)
@@ -100,24 +100,24 @@
                      120 BINARY_SUBSCR
                      130 BUILD_TUPLE              2
                      132 BINARY_SUBSCR
                      142 LOAD_NAME                6 (__annotations__)
                      144 LOAD_CONST               2 ('handler')
                      146 STORE_SUBSCR
          
-          15         150 LOAD_CONST               1 ('rules')
+          13         150 LOAD_CONST               1 ('rules')
          
-          17         152 LOAD_NAME                3 (typing)
+          15         152 LOAD_NAME                3 (typing)
                      154 LOAD_ATTR                4 (List)
                      164 LOAD_NAME                5 (Rule)
                      166 BINARY_SUBSCR
          
-          15         176 LOAD_CONST               2 ('handler')
+          13         176 LOAD_CONST               2 ('handler')
          
-          18         178 LOAD_NAME                3 (typing)
+          16         178 LOAD_NAME                3 (typing)
                      180 LOAD_ATTR                7 (Callable)
                      190 LOAD_NAME                8 (schemas)
                      192 LOAD_ATTR                9 (Event)
                      202 BUILD_LIST               1
                      204 LOAD_NAME                3 (typing)
                      206 LOAD_ATTR               10 (Coroutine)
                      216 LOAD_NAME                3 (typing)
@@ -127,140 +127,144 @@
                      240 LOAD_NAME                3 (typing)
                      242 LOAD_ATTR               11 (Any)
                      252 BUILD_TUPLE              3
                      254 BINARY_SUBSCR
                      264 BUILD_TUPLE              2
                      266 BINARY_SUBSCR
          
-          15         276 BUILD_TUPLE              4
-                     278 LOAD_CONST               3 (<code object __init__, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py", line 15>)
+          13         276 BUILD_TUPLE              4
+                     278 LOAD_CONST               3 (<code object __init__, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py", line 13>)
                      280 MAKE_FUNCTION            4 (annotations)
                      282 STORE_NAME              12 (__init__)
          
-          23         284 LOAD_CONST               4 ('event')
+          21         284 LOAD_CONST               4 ('event')
                      286 LOAD_NAME                8 (schemas)
                      288 LOAD_ATTR                9 (Event)
                      298 LOAD_CONST               5 ('return')
                      300 LOAD_NAME               13 (bool)
                      302 BUILD_TUPLE              4
-                     304 LOAD_CONST               6 (<code object check, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py", line 23>)
+                     304 LOAD_CONST               6 (<code object check, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py", line 21>)
                      306 MAKE_FUNCTION            4 (annotations)
                      308 STORE_NAME              14 (check)
          
-          29         310 LOAD_CONST               4 ('event')
+          27         310 LOAD_CONST               4 ('event')
                      312 LOAD_NAME                8 (schemas)
                      314 LOAD_ATTR                9 (Event)
                      324 BUILD_TUPLE              2
-                     326 LOAD_CONST               7 (<code object handle, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py", line 29>)
+                     326 LOAD_CONST               7 (<code object handle, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py", line 27>)
                      328 MAKE_FUNCTION            4 (annotations)
                      330 STORE_NAME              15 (handle)
-                     332 LOAD_CONST               8 (None)
-                     334 RETURN_VALUE
+         
+          30         332 LOAD_CONST               8 (<code object __repr__, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py", line 30>)
+                     334 MAKE_FUNCTION            0
+                     336 STORE_NAME              16 (__repr__)
+                     338 LOAD_CONST               9 (None)
+                     340 RETURN_VALUE
          consts
             'Handler'
             'rules'
             'handler'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   0064005300
-                15           0 RESUME                   0
+                13           0 RESUME                   0
                
-                20           2 LOAD_FAST                1 (rules)
+                18           2 LOAD_FAST                1 (rules)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (rules)
                
-                21          16 LOAD_FAST                2 (handler)
+                19          16 LOAD_FAST                2 (handler)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (handler)
                             30 LOAD_CONST               0 (None)
                             32 RETURN_VALUE
                consts
                   None
                names      ('rules', 'handler')
                varnames   ('self', 'rules', 'handler')
                freevars   ()
                cellvars   ()
                filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py'
                name       '__init__'
-               firstlineno 15
+               firstlineno 13
                lnotab 0x02050e01
             'event'
             'return'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 4
                flags     : 131
                code
                   0x4b00010097007c006a00000000000000000044005d207d027c02a00100
                   000000000000000000000000000000000000007c01a6010000ab01000000
                   0000000000830064007b0356009703860473030100640153008c21640253
                   00
-                23           0 RETURN_GENERATOR
+                21           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                24           6 LOAD_FAST                0 (self)
+                22           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (rules)
                             18 GET_ITER
                        >>   20 FOR_ITER                32 (to 86)
                             22 STORE_FAST               2 (rule)
                
-                25          24 LOAD_FAST                2 (rule)
+                23          24 LOAD_FAST                2 (rule)
                             26 LOAD_METHOD              1 (check)
                             48 LOAD_FAST                1 (event)
                             50 PRECALL                  1
                             54 CALL                     1
                             64 GET_AWAITABLE            0
                             66 LOAD_CONST               0 (None)
                        >>   68 SEND                     3 (to 76)
                             70 YIELD_VALUE
                             72 RESUME                   3
                             74 JUMP_BACKWARD_NO_INTERRUPT     4 (to 68)
                        >>   76 POP_JUMP_FORWARD_IF_TRUE     3 (to 84)
                
-                26          78 POP_TOP
+                24          78 POP_TOP
                             80 LOAD_CONST               1 (False)
                             82 RETURN_VALUE
                
-                25     >>   84 JUMP_BACKWARD           33 (to 20)
+                23     >>   84 JUMP_BACKWARD           33 (to 20)
                
-                27     >>   86 LOAD_CONST               2 (True)
+                25     >>   86 LOAD_CONST               2 (True)
                             88 RETURN_VALUE
                consts
                   None
                   False
                   True
                names      ('rules', 'check')
                varnames   ('self', 'event', 'rule')
                freevars   ()
                cellvars   ()
                filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py'
                name       'check'
-               firstlineno 23
+               firstlineno 21
                lnotab 0x06011201360106ff0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c00a00000000000000000000000000000000000000000
                   007c01a6010000ab010000000000000000830064007b0356009703860453
                   00
-                29           0 RETURN_GENERATOR
+                27           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                30           6 LOAD_FAST                0 (self)
+                28           6 LOAD_FAST                0 (self)
                              8 LOAD_METHOD              0 (handler)
                             30 LOAD_FAST                1 (event)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 GET_AWAITABLE            0
                             48 LOAD_CONST               0 (None)
                        >>   50 SEND                     3 (to 58)
@@ -272,27 +276,62 @@
                   None
                names      ('handler',)
                varnames   ('self', 'event')
                freevars   ()
                cellvars   ()
                filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py'
                name       'handle'
-               firstlineno 29
+               firstlineno 27
                lnotab 0x0601
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 5
+               flags     : 3
+               code
+                  0x970064017c006a0000000000000000006a0100000000000000009b0064
+                  027c006a0200000000000000009b0064039d055300
+                30           0 RESUME                   0
+               
+                31           2 LOAD_CONST               1 ('Handler(')
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (handler)
+                            16 LOAD_ATTR                1 (__name__)
+                            26 FORMAT_VALUE             0
+                            28 LOAD_CONST               2 (', rules=')
+                            30 LOAD_FAST                0 (self)
+                            32 LOAD_ATTR                2 (rules)
+                            42 FORMAT_VALUE             0
+                            44 LOAD_CONST               3 (')')
+                            46 BUILD_STRING             5
+                            48 RETURN_VALUE
+               consts
+                  None
+                  'Handler('
+                  ', rules='
+                  ')'
+               names      ('handler', '__name__', 'rules')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py'
+               name       '__repr__'
+               firstlineno 30
+               lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'typing', 'List', 'Rule', '__annotations__', 'Callable', 'schemas', 'Event', 'Coroutine', 'Any', '__init__', 'bool', 'check', 'handle')
+         names      ('__name__', '__module__', '__qualname__', 'typing', 'List', 'Rule', '__annotations__', 'Callable', 'schemas', 'Event', 'Coroutine', 'Any', '__init__', 'bool', 'check', 'handle', '__repr__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py'
          name       'Handler'
-         firstlineno 11
-         lnotab 0x0c0120016a02020218fe020362fd08081a06
+         firstlineno 9
+         lnotab 0x0c0120016a02020218fe020362fd08081a061603
       'Handler'
    names      ('typing', 'keksik_api', 'schemas', 'keksik_api.callback.rules', 'Rule', '__all__', 'Handler')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/callback/handler.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108020c010c020405
+   lnotab 0x00ff020108020c010c020403
```

### Comparing `keksik_api-0.1.1/keksik_api/callback/__pycache__/rules.cpython-311.pyc` & `keksik_api-0.1.2/keksik_api/callback/__pycache__/rules.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8cd66864 (Sat May 20 14:17:48 2023 UTC)
+moddate:  0xf2176a64 (Sun May 21 13:09:06 2023 UTC)
 files sz: 423
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `keksik_api-0.1.1/keksik_api/callback/callback.py` & `keksik_api-0.1.2/keksik_api/callback/callback.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import hashlib
 import logging
 import typing
 
-from keksik_api import KeksikAPI, schemas
+from keksik_api.api import KeksikAPI
+from keksik_api.schemas.events import EventType, Event, DonateEvent, PaymentStatusEvent
 from keksik_api.callback.router import Router
 
 __all__ = ('Callback',)
 
 logger = logging.getLogger('keksik_api.callback')
 
 
@@ -54,16 +55,16 @@
             return {"status": "error", "msg": "Invalid hash"}
         if event.get('type') == 'confirmation':
             if event.get('group') != str(self.api.group_id):
                 return {"status": "error", "msg": "Invalid group id"}
             return {"status": "ok", "code": self._confirmation_code}
 
         type_to_dataclass = {
-            schemas.EventType.NEW_DONATE.value: schemas.DonateEvent,
-            schemas.EventType.PAYMENT_STATUS.value: schemas.PaymentStatusEvent,
+            EventType.NEW_DONATE.value: DonateEvent,
+            EventType.PAYMENT_STATUS.value: PaymentStatusEvent,
         }
         if event.get('type') not in type_to_dataclass:
-            dataclass = schemas.Event
+            dataclass = Event
         else:
             dataclass = type_to_dataclass[event['type']]
         await self.router.route(dataclass.parse_obj({**event, "api": self.api}))
         return {"status": "ok"}
```

### Comparing `keksik_api-0.1.1/keksik_api/callback/handler.py` & `keksik_api-0.1.2/keksik_api/callback/handler.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/callback/router.py` & `keksik_api-0.1.2/keksik_api/callback/router.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/exceptions.py` & `keksik_api-0.1.2/keksik_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/methods/__pycache__/base.cpython-311.pyc` & `keksik_api-0.1.2/keksik_api/methods/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc` & `keksik_api-0.1.2/keksik_api/methods/__pycache__/campaigns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/methods/__pycache__/donates.cpython-311.pyc` & `keksik_api-0.1.2/keksik_api/methods/__pycache__/donates.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/methods/campaigns.py` & `keksik_api-0.1.2/keksik_api/methods/campaigns.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/methods/donates.py` & `keksik_api-0.1.2/keksik_api/methods/donates.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/methods/payments.py` & `keksik_api-0.1.2/keksik_api/methods/payments.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/schemas/__pycache__/base.cpython-311.pyc` & `keksik_api-0.1.2/keksik_api/schemas/__pycache__/base.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xfda76864 (Sat May 20 10:59:09 2023 UTC)
-files sz: 402
+moddate:  0x22d96864 (Sat May 20 14:28:50 2023 UTC)
+files sz: 456
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -40,17 +40,17 @@
                 42 LOAD_CONST               5 ('BaseModel')
                 44 LOAD_NAME                1 (pydantic)
                 46 LOAD_ATTR                5 (BaseModel)
                 56 PRECALL                  3
                 60 CALL                     3
                 70 STORE_NAME               5 (BaseModel)
    
-    14          72 PUSH_NULL
+    16          72 PUSH_NULL
                 74 LOAD_BUILD_CLASS
-                76 LOAD_CONST               6 (<code object BaseResponse, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/base.py", line 14>)
+                76 LOAD_CONST               6 (<code object BaseResponse, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/base.py", line 16>)
                 78 MAKE_FUNCTION            0
                 80 LOAD_CONST               7 ('BaseResponse')
                 82 LOAD_NAME                5 (BaseModel)
                 84 PRECALL                  3
                 88 CALL                     3
                 98 STORE_NAME               6 (BaseResponse)
                100 LOAD_CONST               1 (None)
@@ -59,68 +59,109 @@
       0
       None
       ('KeksikErrorCode',)
       ('BaseModel', 'BaseResponse')
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 1
+         stacksize : 5
          flags     : 0
-         code 0x970065005a0164005a0264015300
+         code
+            0x970065005a0164005a020200470064018400640265036a040000000000
+            000000a6030000ab0300000000000000005a0564035300
           10           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BaseModel')
                        8 STORE_NAME               2 (__qualname__)
          
-          11          10 LOAD_CONST               1 (None)
-                      12 RETURN_VALUE
+          12          10 PUSH_NULL
+                      12 LOAD_BUILD_CLASS
+                      14 LOAD_CONST               1 (<code object Config, file "/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/base.py", line 12>)
+                      16 MAKE_FUNCTION            0
+                      18 LOAD_CONST               2 ('Config')
+                      20 LOAD_NAME                3 (pydantic)
+                      22 LOAD_ATTR                4 (BaseConfig)
+                      32 PRECALL                  3
+                      36 CALL                     3
+                      46 STORE_NAME               5 (Config)
+                      48 LOAD_CONST               3 (None)
+                      50 RETURN_VALUE
          consts
             'BaseModel'
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 1
+               flags     : 0
+               code 0x970065005a0164005a0264015a0364025300
+                12           0 RESUME                   0
+                             2 LOAD_NAME                0 (__name__)
+                             4 STORE_NAME               1 (__module__)
+                             6 LOAD_CONST               0 ('BaseModel.Config')
+                             8 STORE_NAME               2 (__qualname__)
+               
+                13          10 LOAD_CONST               1 (True)
+                            12 STORE_NAME               3 (frozen)
+                            14 LOAD_CONST               2 (None)
+                            16 RETURN_VALUE
+               consts
+                  'BaseModel.Config'
+                  True
+                  None
+               names      ('__name__', '__module__', '__qualname__', 'frozen')
+               varnames   ()
+               freevars   ()
+               cellvars   ()
+               filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/base.py'
+               name       'Config'
+               firstlineno 12
+               lnotab 0x0a01
+            'Config'
             None
-         names      ('__name__', '__module__', '__qualname__')
+         names      ('__name__', '__module__', '__qualname__', 'pydantic', 'BaseConfig', 'Config')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/base.py'
          name       'BaseModel'
          firstlineno 10
-         lnotab 0x0a01
+         lnotab 0x0a02
       'BaseModel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a02550064015a0365046a05000000000000000064
             0119000000000000000000650664023c000000020065076a080000000000
             00000064036404ac05a6020000ab0200000000000000005a0965046a0a00
             00000000000000650b19000000000000000000650664063c000000020065
             076a08000000000000000064036407ac05a6020000ab0200000000000000
             005a0c65046a0a0000000000000000650d19000000000000000000650664
             083c00000064035300
-          14           0 RESUME                   0
+          16           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BaseResponse')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          15          12 LOAD_CONST               1 (True)
+          17          12 LOAD_CONST               1 (True)
                       14 STORE_NAME               3 (success)
                       16 LOAD_NAME                4 (typing)
                       18 LOAD_ATTR                5 (Literal)
                       28 LOAD_CONST               1 (True)
                       30 BINARY_SUBSCR
                       40 LOAD_NAME                6 (__annotations__)
                       42 LOAD_CONST               2 ('success')
                       44 STORE_SUBSCR
          
-          16          48 PUSH_NULL
+          18          48 PUSH_NULL
                       50 LOAD_NAME                7 (pydantic)
                       52 LOAD_ATTR                8 (Field)
                       62 LOAD_CONST               3 (None)
                       64 LOAD_CONST               4 ('error')
                       66 KW_NAMES                 5
                       68 PRECALL                  2
                       72 CALL                     2
@@ -129,15 +170,15 @@
                       86 LOAD_ATTR               10 (Optional)
                       96 LOAD_NAME               11 (KeksikErrorCode)
                       98 BINARY_SUBSCR
                      108 LOAD_NAME                6 (__annotations__)
                      110 LOAD_CONST               6 ('error_code')
                      112 STORE_SUBSCR
          
-          17         116 PUSH_NULL
+          19         116 PUSH_NULL
                      118 LOAD_NAME                7 (pydantic)
                      120 LOAD_ATTR                8 (Field)
                      130 LOAD_CONST               3 (None)
                      132 LOAD_CONST               7 ('msg')
                      134 KW_NAMES                 5
                      136 PRECALL                  2
                      140 CALL                     2
@@ -163,18 +204,18 @@
             'message'
          names      ('__name__', '__module__', '__qualname__', 'success', 'typing', 'Literal', '__annotations__', 'pydantic', 'Field', 'error_code', 'Optional', 'KeksikErrorCode', 'message', 'str')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/base.py'
          name       'BaseResponse'
-         firstlineno 14
+         firstlineno 16
          lnotab 0x0c0124014401
       'BaseResponse'
    names      ('typing', 'pydantic', 'keksik_api.exceptions', 'KeksikErrorCode', '__all__', 'BaseModel', 'BaseResponse')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/media/lordralinc/data_disk1/new_projects/keksik_api/keksik_api/schemas/base.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080208020c0204032604
+   lnotab 0x00ff0201080208020c0204032606
```

### Comparing `keksik_api-0.1.1/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc` & `keksik_api-0.1.2/keksik_api/schemas/__pycache__/campaigns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/schemas/__pycache__/donates.cpython-311.pyc` & `keksik_api-0.1.2/keksik_api/schemas/__pycache__/donates.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/schemas/__pycache__/events.cpython-311.pyc` & `keksik_api-0.1.2/keksik_api/schemas/__pycache__/events.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/schemas/__pycache__/payments.cpython-311.pyc` & `keksik_api-0.1.2/keksik_api/schemas/__pycache__/payments.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/schemas/campaigns.py` & `keksik_api-0.1.2/keksik_api/schemas/campaigns.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/schemas/donates.py` & `keksik_api-0.1.2/keksik_api/schemas/donates.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/schemas/events.py` & `keksik_api-0.1.2/keksik_api/schemas/events.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/keksik_api/schemas/payments.py` & `keksik_api-0.1.2/keksik_api/schemas/payments.py`

 * *Files identical despite different names*

### Comparing `keksik_api-0.1.1/PKG-INFO` & `keksik_api-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keksik-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Обвертка над API keksik.io
 License: MIT
 Author: lordralinc
 Author-email: lordralinc@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

