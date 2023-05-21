# Comparing `tmp/qtc-0.0.4.tar.gz` & `tmp/qtc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtc-0.0.4.tar", last modified: Tue May 16 20:02:20 2023, max compression
+gzip compressed data, was "qtc-0.0.5.tar", last modified: Sun May 21 15:48:44 2023, max compression
```

## Comparing `qtc-0.0.4.tar` & `qtc-0.0.5.tar`

### file list

```diff
@@ -1,85 +1,90 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.721361 qtc-0.0.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-04-28 00:35:58.000000 qtc-0.0.4/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-16 20:02:20.717361 qtc-0.0.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-04-28 00:35:58.000000 qtc-0.0.4/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/app_configs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:20.000000 qtc-0.0.4/qtc/app_configs/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/app_configs/bq/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:25.000000 qtc-0.0.4/qtc/app_configs/bq/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-04-29 15:40:25.000000 qtc-0.0.4/qtc/app_configs/bq/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4648 2023-04-29 15:41:30.000000 qtc-0.0.4/qtc/app_configs/bq/params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/app_configs/bq_sim/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:22.000000 qtc-0.0.4/qtc/app_configs/bq_sim/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5745 2023-04-29 15:40:22.000000 qtc-0.0.4/qtc/app_configs/bq_sim/params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/calendar/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/calendar/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10278 2023-05-16 19:59:16.000000 qtc-0.0.4/qtc/calendar/calendar.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7479 2023-05-16 19:58:25.000000 qtc-0.0.4/qtc/calendar/cn_stock_calendar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/consts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/consts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-04-29 15:42:12.000000 qtc-0.0.4/qtc/consts/enums.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 03:32:47.000000 qtc-0.0.4/qtc/data/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/data/dal/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 03:33:01.000000 qtc-0.0.4/qtc/data/dal/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1822 2023-05-16 04:08:20.000000 qtc-0.0.4/qtc/data/dal/calendar.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2023-04-30 15:11:38.000000 qtc-0.0.4/qtc/env_config.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5371 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/env_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/qtc/ext/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-04-28 01:41:03.000000 qtc-0.0.4/qtc/ext/configurable.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1145 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/enum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1992 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/logging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/multiprocessing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1037 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/unittest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/qtc/file/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/file/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9319 2023-04-28 01:57:29.000000 qtc-0.0.4/qtc/file/file_cache.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16376 2023-04-28 01:57:29.000000 qtc-0.0.4/qtc/file/file_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30307 2023-04-28 01:57:29.000000 qtc-0.0.4/qtc/file/file_serialization.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/qtc/toolbox/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/toolbox/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-13 06:34:37.000000 qtc-0.0.4/qtc/toolbox/calcs.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/qtc/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2023-04-30 15:30:33.000000 qtc-0.0.4/qtc/utils/cipher_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3931 2023-04-30 15:30:33.000000 qtc-0.0.4/qtc/utils/dash_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27238 2023-04-30 15:30:33.000000 qtc-0.0.4/qtc/utils/datetime_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31119 2023-05-16 03:51:59.000000 qtc-0.0.4/qtc/utils/db_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7567 2023-04-28 02:56:22.000000 qtc-0.0.4/qtc/utils/email_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4540 2023-04-28 01:49:03.000000 qtc-0.0.4/qtc/utils/endpoint_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6612 2023-04-28 03:01:16.000000 qtc-0.0.4/qtc/utils/file_system_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7840 2023-04-28 01:53:01.000000 qtc-0.0.4/qtc/utils/html_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6663 2023-04-28 01:57:29.000000 qtc-0.0.4/qtc/utils/misc_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11079 2023-04-28 01:57:29.000000 qtc-0.0.4/qtc/utils/notebook_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-05-16 20:02:15.000000 qtc-0.0.4/qtc/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-16 20:02:20.000000 qtc-0.0.4/qtc.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1605 2023-05-16 20:02:20.000000 qtc-0.0.4/qtc.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-16 20:02:20.000000 qtc-0.0.4/qtc.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-29 14:49:44.000000 qtc-0.0.4/qtc.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2023-05-16 20:02:20.000000 qtc-0.0.4/qtc.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-05-16 20:02:20.000000 qtc-0.0.4/qtc.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-16 20:02:20.721361 qtc-0.0.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      724 2023-05-13 06:37:41.000000 qtc-0.0.4/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/tests/ext/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/ext/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1003 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/ext/test_enum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/ext/test_inspect.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/tests/file/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/file/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/file/test_file_cache.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3244 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/file/test_file_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5806 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/file/test_file_serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      431 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/test_env_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/tests/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      558 2023-04-28 02:46:02.000000 qtc-0.0.4/tests/utils/test_cipher_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3939 2023-04-28 02:45:02.000000 qtc-0.0.4/tests/utils/test_datetime_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2604 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/utils/test_db_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1855 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/utils/test_misc_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.187531 qtc-0.0.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-04-28 00:35:58.000000 qtc-0.0.5/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-21 15:48:44.187531 qtc-0.0.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-04-28 00:35:58.000000 qtc-0.0.5/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.151531 qtc-0.0.5/qtc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.155531 qtc-0.0.5/qtc/app_configs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:20.000000 qtc-0.0.5/qtc/app_configs/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.155531 qtc-0.0.5/qtc/app_configs/bq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:25.000000 qtc-0.0.5/qtc/app_configs/bq/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-04-29 15:40:25.000000 qtc-0.0.5/qtc/app_configs/bq/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4648 2023-04-29 15:41:30.000000 qtc-0.0.5/qtc/app_configs/bq/params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.155531 qtc-0.0.5/qtc/app_configs/bq_sim/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:22.000000 qtc-0.0.5/qtc/app_configs/bq_sim/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5745 2023-04-29 15:40:22.000000 qtc-0.0.5/qtc/app_configs/bq_sim/params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.159530 qtc-0.0.5/qtc/calendar/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/calendar/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10276 2023-05-21 01:58:15.000000 qtc-0.0.5/qtc/calendar/calendar.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7419 2023-05-21 01:58:15.000000 qtc-0.0.5/qtc/calendar/cn_stock_calendar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.159530 qtc-0.0.5/qtc/consts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/consts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-04-29 15:42:12.000000 qtc-0.0.5/qtc/consts/enums.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.159530 qtc-0.0.5/qtc/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 03:32:47.000000 qtc-0.0.5/qtc/data/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.163530 qtc-0.0.5/qtc/data/dal/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 03:33:01.000000 qtc-0.0.5/qtc/data/dal/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1883 2023-05-21 01:58:15.000000 qtc-0.0.5/qtc/data/dal/calendar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.163530 qtc-0.0.5/qtc/data/dal/common/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 03:33:01.000000 qtc-0.0.5/qtc/data/dal/common/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1216 2023-05-19 15:41:09.000000 qtc-0.0.5/qtc/data/dal/common/sql_compiler.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1532 2023-05-19 18:30:41.000000 qtc-0.0.5/qtc/data/dal/sec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1363 2023-05-19 18:42:48.000000 qtc-0.0.5/qtc/data/sec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-05-21 01:53:14.000000 qtc-0.0.5/qtc/env_config.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5371 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/env_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.167530 qtc-0.0.5/qtc/ext/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/ext/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-04-28 01:41:03.000000 qtc-0.0.5/qtc/ext/configurable.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1145 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/ext/enum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1992 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/ext/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/ext/logging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/ext/multiprocessing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1037 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/ext/unittest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.167530 qtc-0.0.5/qtc/file/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/file/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9319 2023-04-28 01:57:29.000000 qtc-0.0.5/qtc/file/file_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16376 2023-04-28 01:57:29.000000 qtc-0.0.5/qtc/file/file_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30307 2023-04-28 01:57:29.000000 qtc-0.0.5/qtc/file/file_serialization.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.171531 qtc-0.0.5/qtc/toolbox/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/toolbox/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7484 2023-05-21 01:53:02.000000 qtc-0.0.5/qtc/toolbox/calcs.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.179530 qtc-0.0.5/qtc/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/qtc/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2620 2023-05-21 01:58:15.000000 qtc-0.0.5/qtc/utils/cipher_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3931 2023-04-30 15:30:33.000000 qtc-0.0.5/qtc/utils/dash_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27238 2023-04-30 15:30:33.000000 qtc-0.0.5/qtc/utils/datetime_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31458 2023-05-21 03:22:18.000000 qtc-0.0.5/qtc/utils/db_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7567 2023-04-28 02:56:22.000000 qtc-0.0.5/qtc/utils/email_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4540 2023-04-28 01:49:03.000000 qtc-0.0.5/qtc/utils/endpoint_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6612 2023-04-28 03:01:16.000000 qtc-0.0.5/qtc/utils/file_system_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7840 2023-04-28 01:53:01.000000 qtc-0.0.5/qtc/utils/html_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6663 2023-04-28 01:57:29.000000 qtc-0.0.5/qtc/utils/misc_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11079 2023-04-28 01:57:29.000000 qtc-0.0.5/qtc/utils/notebook_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-05-19 05:56:36.000000 qtc-0.0.5/qtc/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.155531 qtc-0.0.5/qtc.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-21 15:48:44.000000 qtc-0.0.5/qtc.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1709 2023-05-21 15:48:44.000000 qtc-0.0.5/qtc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-21 15:48:44.000000 qtc-0.0.5/qtc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-29 14:49:44.000000 qtc-0.0.5/qtc.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2023-05-21 15:48:44.000000 qtc-0.0.5/qtc.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-05-21 15:48:44.000000 qtc-0.0.5/qtc.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-21 15:48:44.187531 qtc-0.0.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      724 2023-05-13 06:37:41.000000 qtc-0.0.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.179530 qtc-0.0.5/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.179530 qtc-0.0.5/tests/ext/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/ext/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1003 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/ext/test_enum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/ext/test_inspect.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.183530 qtc-0.0.5/tests/file/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/file/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/file/test_file_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3244 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/file/test_file_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5806 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/file/test_file_serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      431 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/test_env_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-21 15:48:44.187531 qtc-0.0.5/tests/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      558 2023-04-28 02:46:02.000000 qtc-0.0.5/tests/utils/test_cipher_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3939 2023-04-28 02:45:02.000000 qtc-0.0.5/tests/utils/test_datetime_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2604 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/utils/test_db_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1855 2023-04-28 00:35:58.000000 qtc-0.0.5/tests/utils/test_misc_utils.py
```

### Comparing `qtc-0.0.4/qtc/app_configs/bq/params.py` & `qtc-0.0.5/qtc/app_configs/bq/params.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/app_configs/bq_sim/params.py` & `qtc-0.0.5/qtc/app_configs/bq_sim/params.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/calendar/calendar.py` & `qtc-0.0.5/qtc/calendar/calendar.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -191,8 +191,8 @@
         start_dateid, end_dateid = \
             Calendar.infer_start_dateid_end_dateid(trading_dateids=trading_dateids,
                                                    start_date=start_date, end_date=end_date,
                                                    date_range_mode=date_range_mode)
         dateids = list(Calendar.get_trading_dateids(trading_dateids=trading_dateids,
                                                     start_date=start_dateid, end_date=end_dateid))
 
-        return dateids, start_dateid, end_dateid
+        return dateids, start_dateid, end_dateid
```

### Comparing `qtc-0.0.4/qtc/calendar/cn_stock_calendar.py` & `qtc-0.0.5/qtc/calendar/cn_stock_calendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 
 class CNStockCalendar(Calendar):
     @staticmethod
     @lru_cache
     def _load_trading_dateids():
         """
         >>> from qtc.calendar.cn_stock_calendar import CNStockCalendar
-        >>> trading_dateids = CNStockCalendar._load_trading_dateids()
+        >>> trading_dateids =DB  CNStockCalendar._load_trading_dateids()
         >>> trading_dateids[:5]
         [19901219, 19901220, 19901221, 19901224, 19901225]
         """
 
-        cal = dalcal.query_calendar(exchanges='SSE,SZSE',
-                                    database='CN-EQUITY-VENDOR')
-        trading_dateids = sorted(cal['cal_date'].unique())
+        cal = dalcal.query_calendar(exchanges='SSE,SZSE')
+        trading_dateids = sorted(list(set(cal['cal_date'])))
 
         return trading_dateids
 
     @staticmethod
     def _get_trading_dateids(start_dateid=None, end_dateid=None):
         """
         >>> from qtc.calendar.cn_stock_calendar import CNStockCalendar
```

### Comparing `qtc-0.0.4/qtc/consts/enums.py` & `qtc-0.0.5/qtc/consts/enums.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/data/dal/calendar.py` & `qtc-0.0.5/qtc/data/dal/calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from functools import lru_cache
-import pandas as pd
 import qtc.utils.db_utils as dbu
 import qtc.utils.misc_utils as mu
 
 
 @lru_cache
 def query_calendar(exchanges=None,
                    is_open=True,
+                   database='CN-EQUITY-VENDOR',
                    **db_config):
     """
     >>> import qtc.data.dal.calendar as dalcal
     >>> dalcal.query_calendar().head()
       exchange  cal_date  is_open             UpdateDateTime
     0      SSE  20231231    False 2023-05-15 13:25:24.219822
     1      SSE  20231230    False 2023-05-15 13:25:24.219822
@@ -33,15 +33,15 @@
     if is_open is not None:
         sql_and_clauses.append(f'"is_open" IS {str(is_open).upper()}')
 
     sql = f'''
         SELECT * FROM "mktmeta"."Calendar"
         {dbu.compile_sql_where_clause(sql_and_clauses)}
     '''
-    # print(sql)
 
-    conn = dbu.get_os_env_conn(**db_config)
+    conn = dbu.get_os_env_conn(database=database,
+                               **db_config)
     # print(conn)
     calendar = dbu.sql2df(sql=sql, conn=conn,
                           preprocess_cols=False,
                           quotes_on_colnames=True)
     return calendar
```

### Comparing `qtc-0.0.4/qtc/env_config.py` & `qtc-0.0.5/qtc/env_config.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/ext/configurable.py` & `qtc-0.0.5/qtc/ext/configurable.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/ext/enum.py` & `qtc-0.0.5/qtc/ext/enum.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/ext/inspect.py` & `qtc-0.0.5/qtc/ext/inspect.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/ext/logging.py` & `qtc-0.0.5/qtc/ext/logging.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/ext/multiprocessing.py` & `qtc-0.0.5/qtc/ext/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/ext/unittest.py` & `qtc-0.0.5/qtc/ext/unittest.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/file/file_cache.py` & `qtc-0.0.5/qtc/file/file_cache.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/file/file_manager.py` & `qtc-0.0.5/qtc/file/file_manager.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/file/file_serialization.py` & `qtc-0.0.5/qtc/file/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/utils/cipher_utils.py` & `qtc-0.0.5/qtc/utils/cipher_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import getpass
 import itertools
 import qtc.env_config as ecfg
 import qtc.utils.endpoint_utils as epu
-import typing as T
 
 _BASE_SALT = 'QuantTrading'
 
 
 def intersperse(str1: str, str2: str) -> str:
     """Mixes together two strings.  If one string is longer, the shorter sting is cycled.
     >>> import qtc.utils.cipher_utils as cu
```

### Comparing `qtc-0.0.4/qtc/utils/dash_utils.py` & `qtc-0.0.5/qtc/utils/dash_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/utils/datetime_utils.py` & `qtc-0.0.5/qtc/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/utils/db_utils.py` & `qtc-0.0.5/qtc/utils/db_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
 import time
 import getpass
 import traceback
+from functools import lru_cache
 import pandas as pd
 import sqlalchemy
 from urllib.parse import quote
 from typing import Optional, Dict
 from qtc.consts.enums import DBType
 import qtc.env_config as ecfg
 import qtc.utils.misc_utils as mu
@@ -89,41 +90,41 @@
     engine = _get_engine(db_type=DBType.POSTGRES,
                          host=host, port=port, user=user, password=password,
                          database=database)
     conn = engine.connect()
     return conn
 
 
-def _get_conn_mysql(host, port, user, password,
-                    database=None):
-    # engine = _get_engine(db_type=DBType.MYSQL,
-    #                      host=host, port=port, user=user, password=password,
-    #                      database=database)
-    # conn = engine.connect()
-    import pymysql
-    conn = pymysql.connect(host=host, port=int(port), user=user, passwd=password, db=database)
-
-    return conn
+# def _get_conn_mysql(host, port, user, password,
+#                     database=None):
+#     # engine = _get_engine(db_type=DBType.MYSQL,
+#     #                      host=host, port=port, user=user, password=password,
+#     #                      database=database)
+#     # conn = engine.connect()
+#     import pymysql
+#     conn = pymysql.connect(host=host, port=int(port), user=user, passwd=password, db=database)
+#
+#     return conn
 
 
 def _init_conn(host, port=None,
                user=None, password=None,
                database=None,
                db_type=None):
 
     conn = None
     if db_type is None:
         try:
-            conn = _get_conn_mysql(host=host, port=port, user=user, password=password, database=database)
+            conn = _get_conn_postgres(host=host, port=port, user=user, password=password, database=database)
         except:
             try:
                 conn = _get_conn_mssql(host=host, port=port, user=user, password=password, database=database)
             except:
                 try:
-                    conn = _get_conn_postgres(host=host, port=port, user=user, password=password, database=database)
+                    conn = _get_conn_mysql(host=host, port=port, user=user, password=password, database=database)
                 except:
                     try:
                         conn = _get_conn_redshift(host=host, port=port, user=user, password=password, database=database)
                     except:
                         logger.warn(f'Unable to create connection by db_type=[MSSQL|MYSQL|REDSHIFT|POSTGRES] with '
                                     f'host={host}, port={port}, user={user}, password={password}, database={database} !')
                         return None
@@ -133,16 +134,16 @@
         db_type = DBType.retrieve(value=db_type)
 
     if user is None:
         user = getpass.getuser()
 
     if db_type==DBType.MSSQL:
         conn = _get_conn_mssql(host=host, port=port, user=user, password=password, database=database)
-    elif db_type==DBType.MYSQL:
-        conn = _get_conn_mysql(host=host, port=port, user=user, password=password, database=database)
+    # elif db_type==DBType.MYSQL:
+    #     conn = _get_conn_mysql(host=host, port=port, user=user, password=password, database=database)
     elif db_type==DBType.REDSHIFT:
         conn = _get_conn_redshift(host=host, port=port, user=user, password=password, database=database)
     elif db_type==DBType.POSTGRES:
         conn = _get_conn_postgres(host=host, port=port, user=user, password=password, database=database)
     else:
         logger.error(f'db_type={db_type} is not supported in [MSSQL | REDSHIFT | POSTGRES] !')
 
@@ -544,31 +545,36 @@
     if log_df_head:
         logger.info(f"Dataframe with shape {df.shape} returned from\n{sql}\nExamples:\n{df.head()}")
 
     return df
 
 
 def create_upsert_method(db_code=None, schema=None,
-                         meta: sqlalchemy.MetaData = None, extra_update_fields: Optional[Dict[str, str]] = None):
+                         meta: sqlalchemy.MetaData = None, extra_update_fields: Optional[Dict[str, str]] = None,
+                         **db_config):
     """
     Create upsert method that satisfied the pandas's to_sql API.
     """
 
     if meta is None:
-        if db_code is None:
-            raise Exception(f'Please provide either "meta" or "db_code" !')
-
-        host, port, user, password, database, db_type, db_name = _get_db_config(db_code=db_code)
-        if db_type==DBType.POSTGRES:
+        if db_code is not None:
+            host, port, user, password, database, db_type, db_name = _get_db_config(db_code=db_code)
             db_engine = _get_engine(db_type=db_type,
                                     host=host, port=port, user=user, password=password,
                                     database=database)
-            meta = sqlalchemy.MetaData(db_engine)
-            if schema is not None:
-                meta.schema = schema
+        else:
+            db_type = db_config.get('db_type', 'POSTGRES')
+            db_engine = get_os_env_engine(**db_config)
+
+        meta = sqlalchemy.MetaData(db_engine)
+        if schema is not None:
+            meta.schema = schema
+
+        if isinstance(db_type, str):
+            db_type = DBType.retrieve(value=db_type)
 
     def method(table, conn, keys, data_iter):
         # select table that data is being inserted to (from pandas's context)
         sql_table = sqlalchemy.Table(table.name, meta, autoload=True)
 
         # list of dictionaries {col_name: value} of data to insert
         values_to_insert = [dict(zip(keys, data)) for data in data_iter]
@@ -593,26 +599,33 @@
         )
 
         # execute upsert statement
         conn.execute(upsert_stmt)
 
     return method
 
-
-def get_os_env_conn(**db_config):
+@lru_cache
+def get_os_env_engine(**db_config):
     db_type = db_config.get('db_type', 'POSTGRES')
     host = db_config.get('host', os.getenv('DB_HOST', None))
     port = db_config.get('port', os.getenv('DB_PORT', None))
     user = db_config.get('user', os.getenv('DB_USER', None))
     password = db_config.get('password', os.getenv('DB_PASSWORD', None))
     database = db_config.get('database', os.getenv('DB_DATABASE', None))
 
-    conn = _get_engine(
+    engine = _get_engine(
         db_type=db_type,
         host=host,
         port=port,
         user=user,
         password=cu.from_salted(secret_str=password),
         database=database
-    ).connect()
+    )
+
+    return engine
+
+
+def get_os_env_conn(**db_config):
+    engine = get_os_env_engine(**db_config)
+    conn = engine.connect()
 
     return conn
```

### Comparing `qtc-0.0.4/qtc/utils/email_utils.py` & `qtc-0.0.5/qtc/utils/email_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/utils/endpoint_utils.py` & `qtc-0.0.5/qtc/utils/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/utils/file_system_utils.py` & `qtc-0.0.5/qtc/utils/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/utils/html_utils.py` & `qtc-0.0.5/qtc/utils/html_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/utils/misc_utils.py` & `qtc-0.0.5/qtc/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc/utils/notebook_utils.py` & `qtc-0.0.5/qtc/utils/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/qtc.egg-info/SOURCES.txt` & `qtc-0.0.5/qtc.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 qtc/app_configs/bq_sim/params.py
 qtc/calendar/__init__.py
 qtc/calendar/calendar.py
 qtc/calendar/cn_stock_calendar.py
 qtc/consts/__init__.py
 qtc/consts/enums.py
 qtc/data/__init__.py
+qtc/data/sec.py
 qtc/data/dal/__init__.py
 qtc/data/dal/calendar.py
+qtc/data/dal/sec.py
+qtc/data/dal/common/__init__.py
+qtc/data/dal/common/sql_compiler.py
 qtc/ext/__init__.py
 qtc/ext/configurable.py
 qtc/ext/enum.py
 qtc/ext/inspect.py
 qtc/ext/logging.py
 qtc/ext/multiprocessing.py
 qtc/ext/unittest.py
```

### Comparing `qtc-0.0.4/setup.py` & `qtc-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/tests/ext/test_enum.py` & `qtc-0.0.5/tests/ext/test_enum.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/tests/ext/test_inspect.py` & `qtc-0.0.5/tests/ext/test_inspect.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/tests/file/test_file_cache.py` & `qtc-0.0.5/tests/file/test_file_cache.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/tests/file/test_file_manager.py` & `qtc-0.0.5/tests/file/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/tests/file/test_file_serialization.py` & `qtc-0.0.5/tests/file/test_file_serialization.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/tests/utils/test_cipher_utils.py` & `qtc-0.0.5/tests/utils/test_cipher_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/tests/utils/test_datetime_utils.py` & `qtc-0.0.5/tests/utils/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/tests/utils/test_db_utils.py` & `qtc-0.0.5/tests/utils/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.4/tests/utils/test_misc_utils.py` & `qtc-0.0.5/tests/utils/test_misc_utils.py`

 * *Files identical despite different names*

