# Comparing `tmp/rick-0.1.2.tar.gz` & `tmp/rick-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rick-0.1.2.tar", last modified: Mon Mar 22 03:33:33 2021, max compression
+gzip compressed data, was "rick-0.6.0.tar", last modified: Sun May 21 19:03:31 2023, max compression
```

## Comparing `rick-0.1.2.tar` & `rick-0.6.0.tar`

### file list

```diff
@@ -1,48 +1,135 @@
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.774568 rick-0.1.2/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      912 2021-03-22 03:33:33.770568 rick-0.1.2/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       62 2021-03-15 05:15:56.000000 rick-0.1.2/README.md
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.766568 rick-0.1.2/rick/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       33 2021-03-09 13:42:50.000000 rick-0.1.2/rick/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.766568 rick-0.1.2/rick/base/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      120 2021-03-22 03:11:34.000000 rick-0.1.2/rick/base/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3606 2021-03-18 17:13:40.000000 rick-0.1.2/rick/base/container.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3570 2021-03-14 16:44:38.000000 rick-0.1.2/rick/base/di.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2716 2021-03-22 03:11:34.000000 rick-0.1.2/rick/base/maploader.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.766568 rick-0.1.2/rick/crypto/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       49 2021-03-09 13:43:16.000000 rick-0.1.2/rick/crypto/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     6013 2021-03-09 13:43:16.000000 rick-0.1.2/rick/crypto/fernet256.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.770568 rick-0.1.2/rick/crypto/hasher/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       36 2021-03-18 14:25:19.000000 rick-0.1.2/rick/crypto/hasher/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2072 2021-03-18 17:12:50.000000 rick-0.1.2/rick/crypto/hasher/bcrypt.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      217 2021-03-18 14:25:19.000000 rick-0.1.2/rick/crypto/hasher/hasher.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.770568 rick-0.1.2/rick/resource/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       45 2021-03-14 17:17:00.000000 rick-0.1.2/rick/resource/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      465 2021-03-14 17:17:00.000000 rick-0.1.2/rick/resource/cache.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.770568 rick-0.1.2/rick/resource/config/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       28 2021-03-14 15:47:25.000000 rick-0.1.2/rick/resource/config/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      378 2021-03-15 05:17:40.000000 rick-0.1.2/rick/resource/config/json.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.770568 rick-0.1.2/rick/resource/redis/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       47 2021-03-10 01:40:08.000000 rick-0.1.2/rick/resource/redis/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3956 2021-03-18 17:13:20.000000 rick-0.1.2/rick/resource/redis/redis.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       86 2021-03-18 14:25:19.000000 rick-0.1.2/rick/version.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.766568 rick-0.1.2/rick.egg-info/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      912 2021-03-22 03:33:33.000000 rick-0.1.2/rick.egg-info/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      826 2021-03-22 03:33:33.000000 rick-0.1.2/rick.egg-info/SOURCES.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2021-03-22 03:33:33.000000 rick-0.1.2/rick.egg-info/dependency_links.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       20 2021-03-22 03:33:33.000000 rick-0.1.2/rick.egg-info/entry_points.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2021-03-15 05:19:31.000000 rick-0.1.2/rick.egg-info/not-zip-safe
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       46 2021-03-22 03:33:33.000000 rick-0.1.2/rick.egg-info/requires.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       11 2021-03-22 03:33:33.000000 rick-0.1.2/rick.egg-info/top_level.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       38 2021-03-22 03:33:33.774568 rick-0.1.2/setup.cfg
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1617 2021-03-18 14:33:08.000000 rick-0.1.2/setup.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.770568 rick-0.1.2/tests/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-10 02:58:48.000000 rick-0.1.2/tests/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.770568 rick-0.1.2/tests/base/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-10 02:58:59.000000 rick-0.1.2/tests/base/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5130 2021-03-10 04:12:40.000000 rick-0.1.2/tests/base/test_container.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3154 2021-03-14 16:44:38.000000 rick-0.1.2/tests/base/test_di.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.770568 rick-0.1.2/tests/crypto/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-18 14:25:50.000000 rick-0.1.2/tests/crypto/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-22 03:33:33.770568 rick-0.1.2/tests/crypto/hasher/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-03-18 14:25:43.000000 rick-0.1.2/tests/crypto/hasher/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1482 2021-03-19 14:15:49.000000 rick-0.1.2/tests/crypto/hasher/test_bcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.392892 rick-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-21 19:03:17.000000 rick-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-21 19:03:31.392892 rick-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-21 19:03:17.000000 rick-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.380892 rick-0.6.0/rick/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-21 19:03:17.000000 rick-0.6.0/rick/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-21 19:03:17.000000 rick-0.6.0/rick/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-21 19:03:17.000000 rick-0.6.0/rick/base/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-21 19:03:17.000000 rick-0.6.0/rick/base/di.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-21 19:03:17.000000 rick-0.6.0/rick/base/maploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-21 19:03:17.000000 rick-0.6.0/rick/base/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-21 19:03:17.000000 rick-0.6.0/rick/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/fernet256.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/crypto/hasher/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/hasher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/hasher/bcrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-21 19:03:17.000000 rick-0.6.0/rick/crypto/hasher/hasher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-21 19:03:17.000000 rick-0.6.0/rick/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-21 19:03:17.000000 rick-0.6.0/rick/event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-21 19:03:17.000000 rick-0.6.0/rick/event/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 19:03:17.000000 rick-0.6.0/rick/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-21 19:03:17.000000 rick-0.6.0/rick/filter/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/form/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 19:03:17.000000 rick-0.6.0/rick/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-21 19:03:17.000000 rick-0.6.0/rick/form/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-21 19:03:17.000000 rick-0.6.0/rick/form/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-05-21 19:03:17.000000 rick-0.6.0/rick/form/requestrecord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-21 19:03:17.000000 rick-0.6.0/rick/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-21 19:03:17.000000 rick-0.6.0/rick/mixin/injectable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 19:03:17.000000 rick-0.6.0/rick/mixin/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 19:03:17.000000 rick-0.6.0/rick/mixin/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/config/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/config/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/console/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/console/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/console/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/file/filereader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/resource/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-21 19:03:17.000000 rick-0.6.0/rick/resource/stream/multipart_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/rick/serializer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.384892 rick-0.6.0/rick/serializer/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:03:17.000000 rick-0.6.0/rick/serializer/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-21 19:03:17.000000 rick-0.6.0/rick/serializer/json/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/rick/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-21 19:03:17.000000 rick-0.6.0/rick/util/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/rick/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/rick/validator/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/rules/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-21 19:03:17.000000 rick-0.6.0/rick/validator/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.380892 rick-0.6.0/rick.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 19:03:31.000000 rick-0.6.0/rick.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-21 19:03:31.392892 rick-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:03:17.000000 rick-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-21 19:03:17.000000 rick-0.6.0/tests/base/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-21 19:03:17.000000 rick-0.6.0/tests/base/test_di.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-21 19:03:17.000000 rick-0.6.0/tests/base/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/crypto/hasher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/crypto/hasher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-21 19:03:17.000000 rick-0.6.0/tests/crypto/hasher/test_bcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-21 19:03:17.000000 rick-0.6.0/tests/event/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-21 19:03:17.000000 rick-0.6.0/tests/filter/test_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/form/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/test_requestrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/test_requestrecord_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-21 19:03:17.000000 rick-0.6.0/tests/form/test_requestrecord_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/resource/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/config/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/config/test_environment_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/resource/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/file/test_filereader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/resource/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-21 19:03:17.000000 rick-0.6.0/tests/resource/stream/test_multipart_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.388892 rick-0.6.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-21 19:03:17.000000 rick-0.6.0/tests/util/test_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:31.392892 rick-0.6.0/tests/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:17.000000 rick-0.6.0/tests/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-21 19:03:17.000000 rick-0.6.0/tests/validator/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-21 19:03:17.000000 rick-0.6.0/tests/validator/test_validator_list.py
```

### Comparing `rick-0.1.2/rick/base/container.py` & `rick-0.6.0/rick/base/container.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import collections
 import copy
 
 
 class ContainerBase:
-
     def __init__(self, data):
         self._data = data
 
     def has(self, key):
         return key in self._data.keys()
 
     def asdict(self):
@@ -53,15 +52,17 @@
 
     def __init__(self, data: dict):
         """
         Constructor
         :param data: dict with data to be made available
         """
         if not isinstance(data, collections.abc.Mapping):
-            raise ValueError("expected dict/Mapping, %s found instead" % str(type(data)))
+            raise ValueError(
+                "expected dict/Mapping, %s found instead" % str(type(data))
+            )
         super(Container, self).__init__(copy.deepcopy(data))
 
     def __getitem__(self, key):
         v = self._data[key]
         if isinstance(v, collections.abc.Mapping):
             return Container(v)
         return v
@@ -77,15 +78,17 @@
     """
 
     def __init__(self, data: dict = None):
         if data is None:
             super(MutableContainer, self).__init__({})
         else:
             if not isinstance(data, collections.abc.MutableMapping):
-                raise ValueError("expected dict/MutableMapping, %s found instead" % str(type(data)))
+                raise ValueError(
+                    "expected dict/MutableMapping, %s found instead" % str(type(data))
+                )
             super(MutableContainer, self).__init__(copy.deepcopy(data))
 
     def __getitem__(self, key):
         v = self._data[key]
         if isinstance(v, collections.abc.MutableMapping):
             return MutableContainer(v)
         return v
@@ -118,15 +121,17 @@
 
     def __init__(self, data: dict):
         """
         Constructor
         :param data: dict with data to be made available
         """
         if not isinstance(data, collections.abc.Mapping):
-            raise ValueError("expected dict/Mapping, %s found instead" % str(type(data)))
+            raise ValueError(
+                "expected dict/Mapping, %s found instead" % str(type(data))
+            )
         super(ShallowContainer, self).__init__(data)
 
     def copy(self):
         return ShallowContainer(self._data)
 
     def __getitem__(self, key):
         v = self._data[key]
```

### Comparing `rick-0.1.2/rick/base/di.py` & `rick-0.6.0/rick/base/di.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import functools
 import types
 from inspect import isclass
 
 
 class Di:
-
     def __init__(self, di=None):
         """
         Initialize internal variables
         """
         self._parent = di
         self._registry = {}  # internal dependency registry
 
     def register(self, name: str):
         """
         Decorator to register classes
         :param name:
         :return: wrapper function for registered item
         """
 
-        def wrap(fn):  # wrapper function to be detected as callable for the registered class
+        def wrap(
+            fn,
+        ):  # wrapper function to be detected as callable for the registered class
             self.add(name, fn)
 
         return wrap
 
     def override(self, name: str):
         """
         Override a dependency definition
         :param name:
         :return: wrapper function for registered item
         """
 
-        def wrap(fn):  # wrapper function to be detected as callable for the registered class
+        def wrap(
+            fn,
+        ):  # wrapper function to be detected as callable for the registered class
             self.add(name, fn, True)
 
         return wrap
 
     def add(self, name: str, item, replace=False):
         """
         Adds a new item to the registry
@@ -44,20 +47,25 @@
         :param replace:
         :return:
         """
         if self.has(name) and not replace:
             raise RuntimeError("Dependency name '{}' already in use".format(name))
 
         if isclass(item):
-            def cls_wrap(_di):  # if it is a class, we'll create a wrap function to instantiate the object
+
+            def cls_wrap(
+                _di,
+            ):  # if it is a class, we'll create a wrap function to instantiate the object
                 return item(_di)
 
             self._registry[name] = cls_wrap  # store the wrapper class
         else:
-            self._registry[name] = item  # or if it is an object or callable, just store it
+            self._registry[
+                name
+            ] = item  # or if it is an object or callable, just store it
         if replace:  # if replacing existing item, clear lru_cache
             self.get.cache_clear()
 
     @functools.lru_cache(maxsize=None)
     def get(self, name: str):
         """
         Retrieve a dependency from the registry by name
```

### Comparing `rick-0.1.2/rick/base/maploader.py` & `rick-0.6.0/rick/base/maploader.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from threading import Lock
 
 from .di import Di
 
 
 class MapLoader:
-
     def __init__(self, di: Di, map_: dict = None):
         self._di = di
         self._map = {}
         self._loaded = {}
         self._stack = []
         self._lock = Lock()
         if map_:
@@ -24,20 +23,33 @@
         :param path: object path
         :return: none
         """
         with self._lock:
             self._map[name] = path
 
     def remove(self, name):
+        """
+        Remove a cached entry by name
+        :param name:
+        :return:
+        """
         with self._lock:
             if name in self._map.keys():
                 del self._map[name]
             if name in self._loaded.keys():
                 del self._loaded[name]
 
+    def clear_loaded(self):
+        """
+        Remove all cached entries
+        :return:
+        """
+        with self._lock:
+            self._loaded = {}
+
     def append(self, map: dict):
         """
         Add multiple map entries from a dict
         :param map: dict with name:path
         :return: none
         """
         with self._lock:
@@ -69,25 +81,31 @@
         if name not in self._map.keys():
             raise ValueError("get(): name '%s' does not exist in map" % name)
 
         with self._lock:
             self._stack.append(name)
             path = self._map[name]
 
-        module_path, cls_name = path.rsplit('.', 1)
+        module_path, cls_name = path.rsplit(".", 1)
         try:
             module = importlib.import_module(module_path)
             cls = getattr(module, cls_name, None)
             if cls is None:
-                raise RuntimeError("get(): cannot find class '%s' in module '%s'" % (cls_name, module_path))
+                raise RuntimeError(
+                    "get(): cannot find class '%s' in module '%s'"
+                    % (cls_name, module_path)
+                )
 
-        except ModuleNotFoundError as e:
+        except ModuleNotFoundError:
             with self._lock:
                 self._stack.remove(name)
-            raise RuntimeError("get(): mapped module '%s' not found when discovering path %s" % (module_path, path))
+            raise RuntimeError(
+                "get(): mapped module '%s' not found when discovering path %s"
+                % (module_path, path)
+            )
 
         obj = self.build(cls)
         with self._lock:
             self._loaded[name] = obj
             self._stack.remove(name)
         return obj
```

### Comparing `rick-0.1.2/rick/crypto/fernet256.py` & `rick-0.6.0/rick/crypto/fernet256.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,36 +11,35 @@
 import binascii
 import os
 import struct
 import time
 
 from cryptography import utils
 from cryptography.exceptions import InvalidSignature
-from cryptography.hazmat.backends import _get_backend
+from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, padding
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.hmac import HMAC
 
 
 class InvalidToken(Exception):
     pass
 
 
 _MAX_CLOCK_SKEW = 60
 
 
 class Fernet256(object):
     def __init__(self, key, backend=None):
-        backend = _get_backend(backend)
+        if backend is None:
+            backend = default_backend()
 
         key = base64.urlsafe_b64decode(key)
         if len(key) != 64:
-            raise ValueError(
-                "Fernet key must be 64 url-safe base64-encoded bytes."
-            )
+            raise ValueError("Fernet key must be 64 url-safe base64-encoded bytes.")
 
         self._signing_key = key[:32]
         self._encryption_key = key[32:]
         self._backend = backend
 
     @classmethod
     def generate_key(cls):
@@ -54,33 +53,33 @@
         return self._encrypt_from_parts(data, current_time, iv)
 
     def _encrypt_from_parts(self, data, current_time, iv):
         utils._check_bytes("data", data)
 
         padder = padding.PKCS7(algorithms.AES.block_size).padder()
         padded_data = padder.update(data) + padder.finalize()
-        encryptor = Cipher(algorithms.AES(self._encryption_key), modes.CBC(iv), self._backend).encryptor()
+        encryptor = Cipher(
+            algorithms.AES(self._encryption_key), modes.CBC(iv), self._backend
+        ).encryptor()
         ciphertext = encryptor.update(padded_data) + encryptor.finalize()
 
-        basic_parts = (b"\x81" + struct.pack(">Q", current_time) + iv + ciphertext)
+        basic_parts = b"\x81" + struct.pack(">Q", current_time) + iv + ciphertext
 
         h = HMAC(self._signing_key, hashes.SHA256(), backend=self._backend)
         h.update(basic_parts)
         hmac = h.finalize()
         return base64.urlsafe_b64encode(basic_parts + hmac)
 
     def decrypt(self, token, ttl=None):
         timestamp, data = Fernet256._get_unverified_token_data(token)
         return self._decrypt_data(data, timestamp, ttl, int(time.time()))
 
     def decrypt_at_time(self, token, ttl, current_time):
         if ttl is None:
-            raise ValueError(
-                "decrypt_at_time() can only be used with a non-None ttl"
-            )
+            raise ValueError("decrypt_at_time() can only be used with a non-None ttl")
         timestamp, data = Fernet256._get_unverified_token_data(token)
         return self._decrypt_data(data, timestamp, ttl, current_time)
 
     def extract_timestamp(self, token):
         timestamp, data = Fernet256._get_unverified_token_data(token)
         # Verify the token was not tampered with.
         self._verify_signature(data)
@@ -141,17 +140,15 @@
         return unpadded
 
 
 class MultiFernet256(object):
     def __init__(self, fernets):
         fernets = list(fernets)
         if not fernets:
-            raise ValueError(
-                "MultiFernet requires at least one Fernet instance"
-            )
+            raise ValueError("MultiFernet requires at least one Fernet instance")
         self._fernets = fernets
 
     def encrypt(self, msg):
         return self.encrypt_at_time(msg, int(time.time()))
 
     def encrypt_at_time(self, msg, current_time):
         return self._fernets[0].encrypt_at_time(msg, current_time)
```

### Comparing `rick-0.1.2/rick/crypto/hasher/bcrypt.py` & `rick-0.6.0/rick/crypto/hasher/bcrypt.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,58 +2,57 @@
 import hmac
 
 import bcrypt
 from .hasher import HasherInterface
 
 
 class BcryptHasher(HasherInterface):
-
     def __init__(self, rounds=None, prefix=None):
         if rounds is None:
             rounds = 12
         if prefix is None:
-            prefix = '2b'
+            prefix = "2b"
         self._rounds = rounds
         self._prefix = prefix
 
     def hash(self, password: str) -> str:
         """
         Hashes a password using bcrypt with random salt
         :param password: clear password to hash
         :return: hash string
         """
         if len(password) == 0:
             raise ValueError("hash(): empty password")
 
-        password = hashlib.sha256(password.encode('utf-8')).hexdigest().encode('utf-8')
-        salt = bcrypt.gensalt(rounds=self._rounds, prefix=self._prefix.encode('utf-8'))
+        password = hashlib.sha256(password.encode("utf-8")).hexdigest().encode("utf-8")
+        salt = bcrypt.gensalt(rounds=self._rounds, prefix=self._prefix.encode("utf-8"))
 
-        return bcrypt.hashpw(password, salt).decode('utf-8')
+        return bcrypt.hashpw(password, salt).decode("utf-8")
 
     def is_valid(self, password: str, pw_hash: str) -> bool:
         """
         Compares a cleartext password with a password hash
         :param password: clear password
         :param pw_hash: hash to validate
         :return: True if the hash matches the supplied password
         """
-        pw_hash = pw_hash.encode('utf-8')
-        password = hashlib.sha256(password.encode('utf-8')).hexdigest().encode('utf-8')
+        pw_hash = pw_hash.encode("utf-8")
+        password = hashlib.sha256(password.encode("utf-8")).hexdigest().encode("utf-8")
 
         return hmac.compare_digest(bcrypt.hashpw(password, pw_hash), pw_hash)
 
     def need_rehash(self, pw_hash, prefix=None):
         """
         Check if the number of rounds on the supplied hash is enough, or if one should re-hash the password
         :param pw_hash: hash to verify
         :param prefix: optional prefix
         :return: True if hash number of rounds is below current object configuration
         """
         if prefix is None:
             prefix = self._prefix
         if len(pw_hash) < 4:
             raise ValueError("hash(): hash cannot be empty")
-        tokens = pw_hash[1:].split('$', 2)
+        tokens = pw_hash[1:].split("$", 2)
         if len(tokens) < 3 or tokens[0] != prefix or not tokens[1].isdigit():
             raise ValueError("hash(): invalid hash")
 
         return int(tokens[1]) < self._rounds
```

### Comparing `rick-0.1.2/rick/resource/redis/redis.py` & `rick-0.6.0/rick/resource/redis/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 
     def __del__(self):
         self._redis.close()
         self._redis = None
 
 
 class CryptRedisCache(RedisCache):
-
     def __init__(self, key=None, **kwargs):
         """
         :param key_list: base64-encode key (256 bit)
         :param kwargs: list of optional parameters
 
         Available parameters:
             host='localhost'
```

### Comparing `rick-0.1.2/tests/base/test_container.py` & `rick-0.6.0/tests/base/test_container.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-import os
-
 import pytest
 
-from rick.base.container import ContainerBase, Container, ShallowContainer, MutableContainer
+from rick.base.container import (
+    ContainerBase,
+    Container,
+    ShallowContainer,
+    MutableContainer,
+)
 
 containerbase_data = [
     {
         "key1": "value1",
         "key2": "value2",
         "key3": {
             "subkey1": "subvalue1",
-        }
+        },
     }
 ]
 
 
 @pytest.mark.parametrize("data", containerbase_data)
 def test_containerbase(data):
     container = ContainerBase(data)
@@ -49,33 +52,33 @@
         _ = container.values()
 
     # len()
     assert len(container) == len(data)
 
     # __getitem__()
     with pytest.raises(RuntimeError):
-        v = container["key1"]
+        _ = container["key1"]
 
     # contains()
     for k in data.keys():
         assert container.__contains__(k) is True
-    assert container.__contains__('keyX') is False
+    assert container.__contains__("keyX") is False
 
     # test shallow operation
-    data['newkey'] = "newvalue"
-    assert container.has('newkey') is True
+    data["newkey"] = "newvalue"
+    assert container.has("newkey") is True
 
 
 container_data = [
     {
         "key1": "value1",
         "key2": "value2",
         "key3": {
             "subkey1": "subvalue1",
-        }
+        },
     }
 ]
 
 
 @pytest.mark.parametrize("data", container_data)
 def test_container(data):
     container = Container(data)
@@ -100,34 +103,34 @@
     values = container.values()
     assert len(values) == len(data)
     last_value = values.pop()
     assert isinstance(last_value, Container)
 
     # __getitem__()
     v = container["key1"]
-    assert v == data['key1']
-    assert isinstance(container.__getitem__('key3'), Container)
+    assert v == data["key1"]
+    assert isinstance(container.__getitem__("key3"), Container)
 
     # contains()
     for k in data.keys():
         assert container.__contains__(k) is True
-    assert container.__contains__('keyX') is False
+    assert container.__contains__("keyX") is False
 
     # test non-shallow immutability
     data.clear()
     assert container.get("key1") is not None
 
 
 shallowcontainer_data = [
     {
         "key1": "value1",
         "key2": "value2",
         "key3": {
             "subkey1": "subvalue1",
-        }
+        },
     }
 ]
 
 
 @pytest.mark.parametrize("data", shallowcontainer_data)
 def test_shallow_container(data):
     container = ShallowContainer(data)
@@ -137,74 +140,74 @@
     assert other_c.asdict() == data
     assert container.asdict() == other_c.asdict()
 
     # test class cast
     val_key3 = container.get("key3")
     assert isinstance(val_key3, ShallowContainer)
     assert val_key3.asdict() == data["key3"]
-    assert isinstance(container.__getitem__('key3'), ShallowContainer)
+    assert isinstance(container.__getitem__("key3"), ShallowContainer)
 
     # test shallow operation
-    data['newkey'] = "newvalue"
-    assert container.get('newkey') == "newvalue"
+    data["newkey"] = "newvalue"
+    assert container.get("newkey") == "newvalue"
 
 
 mutablecontainer_data = [
     {
         "key1": "value1",
         "key2": "value2",
         "key3": {
             "subkey1": "subvalue1",
-        }
+        },
     }
 ]
 
 
 @pytest.mark.parametrize("data", mutablecontainer_data)
 def test_mutable_container(data):
     container = MutableContainer(data)
 
     # copy()
     other_c = container.copy()
     assert other_c.asdict() == data
     assert container.asdict() == other_c.asdict()
 
     # A MutableContainer is *not* shallow
-    data['newkey'] = "newvalue"
-    assert container.get('newkey') is None
+    data["newkey"] = "newvalue"
+    assert container.get("newkey") is None
 
     # test class cast
     val_key3 = container.get("key3")
     assert isinstance(val_key3, MutableContainer)
     assert val_key3.asdict() == data["key3"]
-    assert isinstance(container.__getitem__('key3'), MutableContainer)
+    assert isinstance(container.__getitem__("key3"), MutableContainer)
 
     # clear()
     clone = container.copy()
     container.clear()
-    assert container.get('key1') is None
+    assert container.get("key1") is None
     assert len(container.keys()) == 0
     container = clone
 
     # update()
     # add
     container.update("newkey", "newvalue")
     assert container.get("newkey") == "newvalue"
     # replace
     container.update("newkey", "replacevalue")
     assert container.get("newkey") == "replacevalue"
 
     # __setitem__()
     # add
     container["key9"] = "value9"
-    assert container.has('key9') is True
-    assert container.get('key9') == 'value9'
+    assert container.has("key9") is True
+    assert container.get("key9") == "value9"
     # replace
     container["key9"] = "other_value9"
-    assert container.has('key9') is True
-    assert container.get('key9') == 'other_value9'
+    assert container.has("key9") is True
+    assert container.get("key9") == "other_value9"
 
     # __delitem__()
 
     # remove()
-    container.remove('key9')
-    assert container.has('key9') is False
+    container.remove("key9")
+    assert container.has("key9") is False
```

### Comparing `rick-0.1.2/tests/base/test_di.py` & `rick-0.6.0/tests/base/test_di.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pytest
 
 from rick.base import Di
 
 
 class Dummy:
-
     def __init__(self, di):
         pass
 
 
 class Dummy2:
     def __init__(self, di):
         pass
@@ -37,67 +36,67 @@
         di.add(self.item_mask.format(0), Dummy2, True)
         item = di.get(self.item_mask.format(0))
         assert isinstance(item, Dummy2) is True
 
     def test_get(self):
         di = Di()
         # Test get() internal unrapping
-        di.add('item1', Dummy)
-        di.add('item2', Dummy2)
-        assert isinstance(di.get('item1'), Dummy) is True
-        assert isinstance(di.get('item2'), Dummy2) is True
+        di.add("item1", Dummy)
+        di.add("item2", Dummy2)
+        assert isinstance(di.get("item1"), Dummy) is True
+        assert isinstance(di.get("item2"), Dummy2) is True
         # test exception raise on unknown item
         with pytest.raises(RuntimeError):
-            di.get('non-existing-item')
+            di.get("non-existing-item")
 
         # test get() with custom factory
         def init_dummy(di):
             return Dummy(di)
 
-        di.add('custom_factory', init_dummy)
-        item = di.get('custom_factory')
+        di.add("custom_factory", init_dummy)
+        item = di.get("custom_factory")
         assert isinstance(item, Dummy) is True
 
         # test get() with pre-instantiated object
         obj = Dummy(di)
-        di.add('pre-instantiated', obj)
-        item = di.get('pre-instantiated')
+        di.add("pre-instantiated", obj)
+        item = di.get("pre-instantiated")
         assert isinstance(item, Dummy) is True
         assert item.__hash__() == obj.__hash__()
 
     def test_register_override(self):
         di = Di()
 
         # test register decorator with a simple custom factory
-        @di.register('dep-to-be-overridden')
+        @di.register("dep-to-be-overridden")
         def init_dummy(di):
             return Dummy(di)
 
-        item = di.get('dep-to-be-overridden')
+        item = di.get("dep-to-be-overridden")
         assert isinstance(item, Dummy) is True
 
         # test override decorator
-        @di.override('dep-to-be-overridden')
+        @di.override("dep-to-be-overridden")
         def init_dummy2(di):
             return Dummy2(di)
 
-        item = di.get('dep-to-be-overridden')
+        item = di.get("dep-to-be-overridden")
         assert isinstance(item, Dummy2) is True
 
     def test_scope(self):
         di = Di()
 
         # register global dependencies, one of them to be shadowed by a scoped di
-        di.add('global-item', Dummy)
-        di.add('global-item-will-be-shadowed', Dummy2)
+        di.add("global-item", Dummy)
+        di.add("global-item-will-be-shadowed", Dummy2)
 
         # create a scoped di called local-di
-        local_di = di.scoped('local-di')
+        local_di = di.scoped("local-di")
         # add a local dependency that will shadow global one
-        local_di.add('global-item-will-be-shadowed', Dummy)
+        local_di.add("global-item-will-be-shadowed", Dummy)
 
         # test get() global via local instance
-        assert isinstance(local_di.get('global-item'), Dummy) is True
+        assert isinstance(local_di.get("global-item"), Dummy) is True
         # test get() local dependency shadows global one
-        assert isinstance(local_di.get('global-item-will-be-shadowed'), Dummy) is True
+        assert isinstance(local_di.get("global-item-will-be-shadowed"), Dummy) is True
         # test shadowed global dependency remains unchanged
-        assert isinstance(di.get('global-item-will-be-shadowed'), Dummy2) is True
+        assert isinstance(di.get("global-item-will-be-shadowed"), Dummy2) is True
```

### Comparing `rick-0.1.2/tests/crypto/hasher/test_bcrypt.py` & `rick-0.6.0/tests/crypto/hasher/test_bcrypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import pytest
 from rick.crypto.hasher.bcrypt import BcryptHasher
 
 
 class TestBcryptHasher:
     rounds = 8  # lower round count for testing purposes
     valid_passwords = {
-        '12345678': '$2b$08$Y1nUUzX0ZikQi0hSoGZXlODlQYUnF6SnyZIrFIVUZ2jgnIun/mDOO',
-        'sdktrqjkl4dskl': '$2b$08$5McEp4dvSohJdxnWONX3JOYJ8P6TQK6qosOAz0CSAkOr5T647r5G2',
-        '423FDS$&dYdcWs/dAS5': '$2b$08$WiCcKN2HtPzjH58dNEIcf.o/NoFKCZDJIr0c/Fqy1jKiknpvIuvTC'
-
+        "12345678": "$2b$08$Y1nUUzX0ZikQi0hSoGZXlODlQYUnF6SnyZIrFIVUZ2jgnIun/mDOO",
+        "sdktrqjkl4dskl": "$2b$08$5McEp4dvSohJdxnWONX3JOYJ8P6TQK6qosOAz0CSAkOr5T647r5G2",
+        "423FDS$&dYdcWs/dAS5": "$2b$08$WiCcKN2HtPzjH58dNEIcf.o/NoFKCZDJIr0c/Fqy1jKiknpvIuvTC",
     }
 
-    invalid_passwords = ['', ]
+    invalid_passwords = [
+        "",
+    ]
 
     def test_hash(self):
         bc = BcryptHasher(self.rounds)
         for pw, compat_hash in self.valid_passwords.items():
             pw_hash = bc.hash(pw)
             assert len(pw_hash) > 16
-            tokens = pw_hash[1:].split('$', 2)
+            tokens = pw_hash[1:].split("$", 2)
             assert tokens[0] == bc._prefix
             assert int(tokens[1]) == bc._rounds
             assert bc.is_valid(pw, compat_hash) is True
             assert bc.need_rehash(pw_hash) is False
 
         # test cases where rehash is needed
         bc = BcryptHasher(self.rounds + 1)
```

