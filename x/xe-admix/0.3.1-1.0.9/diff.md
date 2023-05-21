# Comparing `tmp/xe-admix-0.3.1.tar.gz` & `tmp/xe-admix-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xe-admix-0.3.1.tar", last modified: Thu Apr 15 19:32:26 2021, max compression
+gzip compressed data, was "xe-admix-1.0.9.tar", last modified: Sun May 21 18:04:49 2023, max compression
```

## Comparing `xe-admix-0.3.1.tar` & `xe-admix-1.0.9.tar`

### file list

```diff
@@ -1,77 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:26.000000 xe-admix-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-04-15 19:32:20.000000 xe-admix-0.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2021-04-15 19:32:20.000000 xe-admix-0.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3207 2021-04-15 19:32:20.000000 xe-admix-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2021-04-15 19:32:26.000000 xe-admix-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-04-15 19:32:26.000000 xe-admix-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2021-04-15 19:32:20.000000 xe-admix-0.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-04-15 19:32:20.000000 xe-admix-0.3.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-04-15 19:32:20.000000 xe-admix-0.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:26.000000 xe-admix-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-04-15 19:32:20.000000 xe-admix-0.3.1/tests/test_admix.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-04-15 19:32:20.000000 xe-admix-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:26.000000 xe-admix-0.3.1/admix/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:26.000000 xe-admix-0.3.1/admix/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     5649 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/check_transfers.py
--rw-r--r--   0 runner    (1001) docker     (121)    19875 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/download_with_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/example_task.py
--rw-r--r--   0 runner    (1001) docker     (121)    11802 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/fix_upload.py
--rw-r--r--   0 runner    (1001) docker     (121)    12228 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/upload_from_lngs_single_thread.py
--rw-r--r--   0 runner    (1001) docker     (121)    15139 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/clean_eb.py
--rw-r--r--   0 runner    (1001) docker     (121)    17175 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     5579 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/clear_transfers_with_mongdb.py
--rw-r--r--   0 runner    (1001) docker     (121)    12418 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/purge_with_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (121)     9755 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/monitor_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     6698 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/move_data_to_rse.py
--rw-r--r--   0 runner    (1001) docker     (121)    12761 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/upload_from_lngs.py
--rw-r--r--   0 runner    (1001) docker     (121)    25659 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/upload_with_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (121)     9995 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/update_runDB.py
--rw-r--r--   0 runner    (1001) docker     (121)    10974 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/init_transfers_with_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:26.000000 xe-admix-0.3.1/admix/helper/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/helper/decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)    11414 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/helper/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/helper/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15707 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/fix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:26.000000 xe-admix-0.3.1/admix/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/utils/list_file_replicas.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12886 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/showrun.py
--rw-r--r--   0 runner    (1001) docker     (121)     7852 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/admix.py
--rw-r--r--   0 runner    (1001) docker     (121)     8897 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/download.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:26.000000 xe-admix-0.3.1/admix/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)    22542 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/interfaces/rucio_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3708 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/interfaces/templater.py
--rw-r--r--   0 runner    (1001) docker     (121)     3425 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/interfaces/rucio_dataformat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3039 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/interfaces/destination.py
--rw-r--r--   0 runner    (1001) docker     (121)    27268 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/interfaces/uploadclient.py
--rw-r--r--   0 runner    (1001) docker     (121)     4876 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/interfaces/rucio_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2455 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/interfaces/keyword.py
--rw-r--r--   0 runner    (1001) docker     (121)    18699 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/interfaces/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    39136 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/interfaces/rucio_summoner.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2021-04-15 19:32:20.000000 xe-admix-0.3.1/admix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2021-04-15 19:32:20.000000 xe-admix-0.3.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:26.000000 xe-admix-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6457 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6758 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)    28723 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/history.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     8661 2021-04-15 19:32:20.000000 xe-admix-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      287 2021-04-15 19:32:20.000000 xe-admix-0.3.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 19:32:26.000000 xe-admix-0.3.1/xe_admix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-04-15 19:32:25.000000 xe-admix-0.3.1/xe_admix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2021-04-15 19:32:25.000000 xe-admix-0.3.1/xe_admix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2021-04-15 19:32:26.000000 xe-admix-0.3.1/xe_admix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-04-15 19:32:25.000000 xe-admix-0.3.1/xe_admix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-15 19:32:25.000000 xe-admix-0.3.1/xe_admix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-04-15 19:32:25.000000 xe-admix-0.3.1/xe_admix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-15 19:32:25.000000 xe-admix-0.3.1/xe_admix.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-21 18:04:44.000000 xe-admix-1.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-21 18:04:44.000000 xe-admix-1.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-21 18:04:44.000000 xe-admix-1.0.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-21 18:04:44.000000 xe-admix-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-21 18:04:44.000000 xe-admix-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-21 18:04:49.279588 xe-admix-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-21 18:04:44.000000 xe-admix-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/admix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/daemons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/fix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/helper/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/helper/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/interfaces/rucio_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36718 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/interfaces/rucio_summoner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/rucio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/showrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-21 18:04:44.000000 xe-admix-1.0.9/bin/admix-download
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8661 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28723 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 18:04:44.000000 xe-admix-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:04:49.279588 xe-admix-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-21 18:04:44.000000 xe-admix-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-21 18:04:44.000000 xe-admix-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-21 18:04:44.000000 xe-admix-1.0.9/tests/test_admix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/xe_admix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xe-admix-0.3.1/setup.py` & `xe-admix-1.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,55 +11,29 @@
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 # Get requirements from requirements.txt, stripping the version tags
 with open('requirements.txt') as f:
     requirements = [r.split('/')[-1] if r.startswith('git+') else r for r in f.read().splitlines()]
 
-setup_requirements = [
-    # TODO(XeBoris): put setup requirements (distutils extensions, etc.) here
-]
-
-test_requirements = [
-    # TODO: put package test requirements here
-]
 
 setup(
     name='xe-admix',
-    version='0.3.1',
+    version='1.0.9',
     description="advanced Data Management In Xenon (aDMIX)",
     long_description=readme + '\n\n' + history,
     url='https://github.com/XENON1T/admix',
-    packages=find_packages(include=['admix',
-                                    'admix.interfaces',
-                                    'admix.tasks',
-                                    'admix.helper',
-                                    'admix.utils'
-                                    ]),
-    package_data={'admix.helper': ['defunc_'],
-                  'admix': ['config/*.*', 'config/rucio_cli/*.*']},
-    include_package_data=True,
     install_requires=requirements,
-    entry_points={
-        'console_scripts': [
-            'admix-version=admix.admix:version',
-            'admix=admix.admix:your_admix',
-            'admix-download=admix.download:main',
-            'admix-showrun=admix.showrun:main',
-            'admix-fix=admix.fix:main',
-            'admix-showcontexts=admix.showcontexts:main'
-        ]
-    },
+    scripts=['bin/admix-download'],
+    packages=find_packages(),
     license="BSD license",
     zip_safe=False,
     keywords='admix',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.6'
     ],
     test_suite='tests',
-    tests_require=test_requirements,
-    setup_requires=setup_requirements,
 )
```

### Comparing `xe-admix-0.3.1/CONTRIBUTING.rst` & `xe-admix-1.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-0.3.1/PKG-INFO` & `xe-admix-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xe-admix
-Version: 0.3.1
+Version: 1.0.9
 Summary: advanced Data Management In Xenon (aDMIX)
 Home-page: https://github.com/XENON1T/admix
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: BSD license
 Description: =====
         aDMIX
```

### Comparing `xe-admix-0.3.1/README.rst` & `xe-admix-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-0.3.1/admix/tasks/download_with_mongodb.py` & `xe-admix-1.0.9/admix/interfaces/rucio_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,386 +1,561 @@
-# -*- coding: utf-8 -*-
-import json
-import os
-from admix.helper import helper
-
-from admix.interfaces.database import ConnectMongoDB
-from admix.helper.decorator import Collector
+"""
+.. module:: rucio_api
+   :platform: Unix
+   :synopsis: An extensive wrapper for the Rucio API in aDMIX
 
-#get Rucio imports done:
-from admix.interfaces.rucio_dataformat import ConfigRucioDataFormat
-from admix.interfaces.rucio_summoner import RucioSummoner
-from admix.interfaces.destination import Destination
-from admix.interfaces.keyword import Keyword
-from admix.interfaces.templater import Templater
+.. moduleauthor:: Boris Bauermeister <Boris.Bauermeister@gmail.com>
 
-@Collector
-class DownloadMongoDB():
-
-    def __init__(self):
-        pass
-
-    def init(self):
-        helper.global_dictionary['logger'].Info(f'Init task {self.__class__.__name__}')
+"""
+#from __future__ import with_statement
+import os
 
-        self.db = ConnectMongoDB()
-        self.db.Connect()
+from admix import logger
+import os
 
-        #Init the Rucio data format evaluator in three steps:
-        self.rc_reader = ConfigRucioDataFormat()
-        self.rc_reader.Config(helper.get_hostconfig('rucio_template'))
-
-        #This class will evaluate your destinations:
-        self.destination = Destination()
-
-        #Since we deal with an experiment, everything is predefine:
-        self.exp_temp = Templater()
-        self.exp_temp.Config(helper.get_hostconfig()['template'])
-
-        #Init a class to handle keyword strings:
-        self.keyw = Keyword()
-
-        #Init Rucio for later uploads and handling:
-        self.rc = RucioSummoner(helper.get_hostconfig("rucio_backend"))
-        self.rc.SetRucioAccount(helper.get_hostconfig('rucio_account'))
-        #These are important for CLI choice
-        #self.rc.SetConfigPath(helper.get_hostconfig("rucio_cli"))
-        #self.rc.SetProxyTicket(helper.get_hostconfig('rucio_x509'))
-        #self.rc.SetHost(helper.get_hostconfig('host'))
-        #And get to your Rucio:
-        self.rc.ConfigHost()
-
-
-
-    def run(self,*args, **kwargs):
-        self.init()
-
-        #Specifiy the download path:
-        if 'destination' not in helper.global_dictionary:
-            dw_path = "./"
-        else:
-            dw_path = helper.global_dictionary['destination']
-        if 'rse' not in helper.global_dictionary:
-            dw_rse = None
-        else:
-            dw_rse =  helper.global_dictionary['rse']
-
-        print("Dw path:", dw_path)
-        print("Dw from RSE", dw_rse)
-
-        #Decide if you select runs from argsparse or just take everything:
-        if 'run_beg' in helper.global_dictionary:
-            run_beg = helper.global_dictionary['run_beg']
-        else:
-            run_beg = self.db.GetSmallest('number')
-
-        if 'run_end' in helper.global_dictionary:
-            run_end = helper.global_dictionary['run_end']
-        else:
-            run_end = self.db.GetLargest('number')
-
-        #When you found your run numbers, you want to select timestamps from them
-        #This allows to catch everything in between
-        ts_beg = self.db.FindTimeStamp('number', int(run_beg) )
-        ts_end = self.db.FindTimeStamp('number', int(run_end) )
-
-        #ToDo We need to get the timestamp selector from helper.global_dictionary into the game here!
-        #print( helper.global_dictionary['run_start_time'] )
-        #print( helper.global_dictionary['run_end_time'] )
-        #Get your collection of run numbers and run names
-        collection = self.db.GetRunsByTimestamp(ts_beg, ts_end)
-
-        #Run through the overview collection:
-        for i_run in collection:
-            #Extract run number and name from overview collection
-            r_name = i_run['name']
-            r_number = i_run['number']
-            #Pull the full run information (according to projection which is pre-defined) by the run name
-            db_info = self.db.GetRunByName(r_name)[0]
-
-            #REMOVE AND CHECK FOR UPLOAD DETECTORS (-> config files)
-            #ToDo: Make it work with XENONnT later
-            if db_info['detector'] != 'tpc':
-                continue
-
-            for i_data in db_info['data']:
-
-                helper.global_dictionary['logger'].Info('Run number/type: {0}/{1}'.format(r_number, i_data['type']))
-                helper.global_dictionary['logger'].Debug('Run is at host: {0}'.format(i_data['host']))
-                helper.global_dictionary['logger'].Debug('aDMIX runs at host: {0}'.format(helper.get_hostconfig('host')))
-
-                #get the destination from DB:
-                #origin_dest = None
-                #if 'destination' in i_data:
-                #    origin_dest = i_data['destination']
-
-                #print("destination:", origin_dest)
-                #print(i_data)
-                origin_dest = "file:./:None"
-
-                dest = self.destination.EvalDestination(host=helper.get_hostconfig('host'),
-                                                        origin=i_data['host'],
-                                                        destination=origin_dest)
-                print(dest)
-                #if len(dest) == 0:
-                #    helper.global_dictionary['logger'].Info("No destination specified! Skip")
-                #    continue
-
-
-                continue
-                #reactivate if this is specified in the config file
-                #if helper.global_dictionary['plugin_type'] != None and helper.global_dictionary['plugin_type'] != i_date['type']:
-                    #continue
-
-                ptr0 = None
-                rlt0 = None
-                rse0 = None
-                for i_dest in dest:
-                    if i_dest['upload'] == True:
-                        ptr0 = i_dest['protocol']
-                        rlt0 = i_dest['lifetime']
-                        if rlt0 == "None":
-                            rlt0 = None
-                        rse0 = i_dest['rse']
-                helper.global_dictionary['logger'].Debug("Evaluated destination for upload:")
-                helper.global_dictionary['logger'].Debug(f" > Protocol: {ptr0}")
-                helper.global_dictionary['logger'].Debug(f" > Lifetime: {rlt0}")
-                helper.global_dictionary['logger'].Debug(f" > RSE: {rse0}")
-
-                #pre infos:
-                origin_type     = i_data['type'] #This is the plugin name which is gonna be handled (uploaded)
-                origin_location = i_data['location'] #This holds the physical location of the plugin folder
-                origin_host     = i_data['host']
-                origin_status   = i_data['status']
-
-                helper.global_dictionary['logger'].Info("Evaluate origin information:")
-                helper.global_dictionary['logger'].Debug(" (origin means from where data are uploaded)")
-                helper.global_dictionary['logger'].Info(f" > Origin Type: {origin_type}")
-                helper.global_dictionary['logger'].Info(f" > Origin Location: {origin_location}")
-                helper.global_dictionary['logger'].Debug(f" > Origin Host: {origin_host}")
-                helper.global_dictionary['logger'].Debug(f" > Origin Status: {origin_status}")
-
-                #Extract the template information according the pre-defined physical file structure:
-                template_info = self.exp_temp.GetTemplateEval(plugin=origin_type,
-                                                              host=origin_host,
-                                                              string=origin_location)
-
-
-                print("template info:")
-                print(template_info)
-
-                print("rucio plugin info:")
-                print(":", self.rc_reader.GetPlugin(origin_type))
-                print(":", self.rc_reader.GetTypes())
-
-                #Evaluate the Rucio name template according the plugin which is requested:
-                # rucio_template: Holds the unsorted Rucio container/dataset/file structure in levels
-                # rucio_template_sorted: Holds the sorted levels (L0, L1, L2,...)
-                rucio_template = self.rc_reader.GetPlugin(origin_type)
-                rucio_template_sorted = [key for key in sorted(rucio_template.keys())]
-
-
-                #Fill the key word class with information beforehand:
-                self.keyw.ResetTemplate()
-                self.keyw.SetTemplate(template_info)
-                self.keyw.SetTemplate(db_info)
-                self.keyw.SetTemplate({'science_run': helper.get_science_run(db_info['start'])})
-
-                rucio_template = self.keyw.CompleteTemplate(rucio_template)
-
-                print("rucio template after filling:")
-                print("-", rucio_template)
-
-                #collect all files from the directory and do pre checks:
-                if os.path.isdir(origin_location) == False:
-                    helper.global_dictionary['logger'].Warning(f"Folder {origin_location} does not exists, stop here")
-                    continue
-
-                #load files:
-                r_path, r_folder, r_files = helper.read_folder(origin_location)
-
-                #check if files are there:
-                if len(r_files) == 0:
-                    helper.global_dictionary['logger'].Warning("--> There are no files in the folder")
-
-                #check for zero sizes files before hand:
-                file_checks = False
-                for i_file in r_files:
-                    f_size = os.path.getsize( os.path.join(origin_location, i_file) )
-                    #print(i_file, f_size)
-                    if f_size == 0:
-                        helper.global_dictionary['logger'].Warning(f"--> file {i_file} is 0 bytes")
-                        helper.global_dictionary['logger'].Warning(f"--> Exclude directory {origin_location} from upload")
-                        file_checks=True
-                        continue
-                    if '_temp' in i_file:
-                        #avoid to upload temp. incomplete files (ToDo need to checked with Strax!)
-                        helper.global_dictionary['logger'].Warning(f"Identified _temp extension in file name {i_file}")
-                        file_checks=True
-                        continue
-                    if template_info['plugin'] not in i_file or template_info['hash'] not in i_file:
-                        #avoid to upload wrong file names. (ToDo: Maybe we can improve in this test but works for not)
-                        helper.global_dictionary['logger'].Warning(f"Plugin name and hash is not recognized in file name {i_file}")
-                        file_checks=True
-                        continue
-
-                if file_checks == True:
-                    continue
-
-                #Check if rule exists in Rucio:
-                rule_status = self.rc.CheckRule(upload_structure=rucio_template, rse=rse0)
-                #verify the locations with rucio:
-                verify_location = self.rc.VerifyLocations(upload_structure=rucio_template, upload_path=origin_location, checksum_test=False)
-                #check for a database entry:
-                db_dest_status = self.db.StatusDataField(db_info['_id'], type=origin_type, host=ptr0)
-
-                print("Check:")
-                print("Rucio Rules Status", rule_status)
-                print("Rucio verify location", verify_location)
-                print("DB status: ", db_dest_status)
-                print("-----------------------")
-                for tmpl_key, tmpl_val in rucio_template.items():
-                    print("level", tmpl_key, tmpl_val)
-                print("-----------------------")
-
-#                p = self.db.GetDataField(db_info['_id'], type=origin_type, host=ptr0, key='status')
-#                print(p, origin_type)
-#                #self.db.SetDataField(db_info['_id'], type=origin_type, host=ptr0, key='status', value='RSEreupload')
-#                continue
-
-                skip_upload = False
-                if db_dest_status == False:
-                    #Create a new dictionary in the data field for the plugin/host combination
-                    new_data_dict={}
-                    new_data_dict['location'] = "n/a"
-                    new_data_dict['status'] = "transferring"
-                    new_data_dict['host'] = ptr0
-                    new_data_dict['type'] = origin_type
-                    new_data_dict['meta'] = None
-                    if ptr0 == 'rucio-catalogue':
-                        new_data_dict['rse'] = []
-                        new_data_dict['destination'] = []
-
-                    self.db.AddDatafield(db_info['_id'], new_data_dict)
-
-                elif rule_status == 'OK':
-                    #if there is a rucio rule we can skip here
-                    skip_upload = True
-                elif db_dest_status == True and self.db.GetDataField(db_info['_id'], type=origin_type, host=ptr0, key='status') == 'transferring':
-                    skip_upload = True
-                elif db_dest_status == True and self.db.GetDataField(db_info['_id'], type=origin_type, host=ptr0, key='status') == 'transferred':
-                    skip_upload = True
-                elif db_dest_status == True and self.db.GetDataField(db_info['_id'], type=origin_type, host=ptr0, key='status') == 'RSEreupload':
-                    #There is a database status found in RSEreupload state: Reset it and continoue with uploading:
-                    pass
-                    #self.db.SetDataField(db_info['_id'], type=origin_type, host=ptr0, key='status', value='transferring')
-                    #self.db.SetDataField(db_info['_id'], type=origin_type, host=ptr0, key='location', value='n/a')
-                elif db_dest_status == True and len(self.db.GetDataField(db_info['_id'], type=origin_type, host=ptr0, key='rse'))>0:
-                    #if there exists a list of RSEs for the rucio-catalogue entry which contains the upload RSE we skip
-                    list_rse_is = self.db.GetDataField(db_info['_id'], type=origin_type, host=ptr0, key='rse')
-                    for i_rse_is in list_rse_is:
-                        print("-", i_rse_is)
-                        if i_rse_is.split(":")[0]==rse0 and i_rse_is.split(":")[1]=='OK':
-                            skip_upload = True
-
-                print("skip:", skip_upload)
-                print("-- origin_type: ", origin_type)
-                print("-- DB status:", self.db.GetDataField(db_info['_id'], type=origin_type, host=ptr0, key='status'))
-                print("-- DB RSE: ", self.db.GetDataField(db_info['_id'], type=origin_type, host=ptr0, key='rse'))
-
-                if skip_upload==True:
-                    continue
-
-                #if the pre checks are ok we can upload:
-                self.rc.Upload(upload_structure=rucio_template, upload_path=origin_location, rse=rse0, rse_lifetime=rlt0)
-#[File replicas states successfully updated]
-                verify_location = self.rc.VerifyLocations(upload_structure=rucio_template, upload_path=origin_location, checksum_test=False)
-                rucio_rule = self.rc.GetRule(upload_structure=rucio_template, rse=rse0)
-
-                ##update after initial upload:
-                if verify_location == True and rucio_rule['state'] == 'OK':
-                    rse_to_db = ["{rse}:{state}:{lifetime}".format(rse=rse0, state=rucio_rule['state'], lifetime=rucio_rule['expires'])]
-                    self.db.SetDataField(db_info['_id'], type=origin_type, host=ptr0, key='rse', value=rse_to_db)
-                    rc_location = rucio_template[rucio_template_sorted[-1]]['did']
-                    self.db.SetDataField(db_info['_id'], type=origin_type, host=ptr0, key='location', value=rc_location)
-                    self.db.SetDataField(db_info['_id'], type=origin_type, host=ptr0, key='status', value='transferred')
-
-                    #if everything was ok we can dump the metadata.json to the runDB:
-                    meta_data_file = None
-                    for i_file in r_files:
-                        if 'metadata.json' in i_file:
-                            meta_data_file = os.path.join(origin_location, i_file)
-                            break
-                    if os.path.exists(meta_data_file):
-                        md = json.load(open(meta_data_file))
-                    else:
-                        md = {}
-                    self.db.SetDataField(db_info['_id'], type=origin_type, host=ptr0, key='meta', value=md)
-
-
-                    #Clean up: Remove destination field and add some rules:
-                    #remove destination entry:
-                    #1 find out if other destinations are on the list:
-                    for i_dest in dest:
-                        if i_dest['upload'] == False:
-                            ptr1 = i_dest['protocol']
-                            rlt1 = i_dest['lifetime']
-                            rse1 = i_dest['rse']
-
-                            #apply further rucio rules
-                            if ptr1 == 'rucio-catalogue':
-                                rule_list = ["{ptr}:{rse}:{rlt}".format(ptr=ptr1,
-                                                                        rse=rse1,
-                                                                        rlt=rlt1)]
-                                print(rule_list)
-                                self.rc.AddRules(upload_structure=rucio_template, rse_rules=rule_list)
-
-                    #if we have a complete uploaded data set and further rules initiated
-                    #we can reset the destintaion list
-                    rucio_rule_status = []
-                    rucio_rule_rse0 = self.rc.GetRule(upload_structure=rucio_template, rse=rse0)
-                    rucio_rule_status.append("{rse}:{state}:{lifetime}".format(rse=rse0, state=rucio_rule_rse0['state'], lifetime=rucio_rule_rse0['expires']))
-                    for i_dest in dest:
-                        if i_dest['upload'] == False:
-                            ptr1 = i_dest['protocol']
-                            rlt1 = i_dest['lifetime']
-                            rse1 = i_dest['rse']
-
-                            #apply further rucio rules
-                            if ptr1 == 'rucio-catalogue':
-                                rucio_rule_rse1 = self.rc.GetRule(upload_structure=rucio_template, rse=rse1)
-                                rucio_rule_status.append("{rse}:{state}:{lifetime}".format(rse=rse1, state=rucio_rule_rse1['state'], lifetime=rucio_rule_rse1['expires']))
-                    print(rucio_rule_status)
-                    #delete the destination if everything seems ok:
-                    if rucio_rule_rse0['state'] == 'OK' and len(rucio_rule_status) == len(dest):
-                        print("Destination request seems to be fulfilled")
-                        print(rucio_rule_status)
-                        self.db.SetDataField(db_info['_id'], type=origin_type, host=origin_host, key='destination', value=[])
-
-                    #But also update the data field based on the latest rucio information:
-                    self.db.SetDataField(db_info['_id'], type=origin_type, host=ptr0, key='rse', value=rucio_rule_status)
-                    #------Goes to memberfunctions laters
-
-                else:
-                    rse_to_db = ["{rse}:{state}:{lifetime}".format(rse=rse0, state=rucio_rule['state'], lifetime=rucio_rule['expires'])]
-                    self.db.SetDataField(db_info['_id'], type=origin_type, host=ptr0, key='rse', value=rse_to_db)
-                    self.db.SetDataField(db_info['_id'], type=origin_type, host=ptr0, key='status', value='RSEreupload')
-
-                print("TTTTTTJJJJ")
-                print(rucio_rule)
-                print(verify_location)
-                print(db_dest_status)
-                self.db.ShowDataField(db_info['_id'], type=origin_type, host=ptr0)
-
-
-                for i_dest in dest:
-                    if i_dest['upload'] == False:
-                        ptr1 = i_dest['protocol']
-                        rlt1 = i_dest['lifetime']
-                        rse1 = i_dest['rse']
-                        print(ptr1, rlt1, rse1)
+from rucio.client.client import Client
+from rucio.client.uploadclient import UploadClient
+# from admix.interfaces.uploadclient import UploadClient
+from rucio.client.downloadclient import DownloadClient
+from rucio.common.exception import DataIdentifierAlreadyExists
+from rucio.common.exception import AccessDenied
+from rucio.common.exception import Duplicate
+from rucio.common.exception import DuplicateContent
+from rucio.common.exception import DuplicateRule
+
+
+class RucioAPI():
+    """Class RucioAPI()
+
+    This class presents an approach to collect all necessary Rucio calls
+    in one class. That allows easy handling of Rucio calls based on the
+    Rucio API.
+    If there are ever changes in the Rucio API, here is the wrapper to fix it.
+    """
+
+    def __init__(self, enable_print=False):
+        """Function: __init__()
+
+        Constructor of RucioAPI class. Comes with a setting set up the print statements to terminal
+
+        :param enable_print: If True then enable print to terminal
+        """
+        self._print_to_screen = enable_print
+        self._rucio_ping = None
+        self._rucio_account = os.environ.get("RUCIO_ACCOUNT")
+        self.ConfigHost()
 
+    def __del__(self):
+        """Function: __del__()
 
+        Destructor - No further description
+        """
+        pass
 
-    def __del__(self):
+    # Here comes the backend configuration part:
+    def SetRucioAccount(self, rucio_account=None):
+        """Function: SetRucioAccount
+        :param rucio_account: The Rucio account you would like to work with
+        """
+
+        self._rucio_account = rucio_account
+
+    def SetConfigPath(self, config_path=None):
+        """Function: SetConfigPath
+        This option is only important for legacy command line support and
+        is ignored in RucioAPI setup.
+        :param config_path: Path to CLI configuration file
+        """
         pass
-#        print( 'Download mongoDB stops')
+    def SetProxyTicket(self, proxy_path=None):
+        """Function: SetProxyTicket
+        This option is only important for legacy command line support and
+        is ignored in RucioAPI setup.
+        :param proxy_path: Path to CLI configuration file
+        """
+        pass
+    def SetHost(self, hostname=None):
+        """Function: SetHost
+        This option is only important for legacy command line support and
+        is ignored in RucioAPI setup.
+        :param hostname: Path to CLI configuration file
+        """
+        pass
+    def ConfigHost(self):
+        """Function: ConfigHost
+
+        This member function setup the rucioAPI backend.
+        To ensure full functionality, it needs:
+        * Client()
+        * UploadClient()
+        * DownloadClient()
+
+        :raise Exception if Rucio API is not ready (miss-configured)
+        """
+        try:
+            self._rucio_client = Client()
+            self._rucio_client_upload = UploadClient(logger=logger)
+#            self._rucio_client_upload = UploadClient(tracing=False)
+#            print("Tracing set to False")
+            self._rucio_client_download = DownloadClient()
+            self._rucio_ping = self._rucio_client.ping
+
+        except:
+            print("Can not init the Rucio API")
+            print("-> Check for your Rucio installation")
+            exit(1)
+
+
+    # finished the backend configuration for the Rucio API
+
+    def Whoami(self):
+        """RucioAPI:Whoami
+        Results a dictionary to identify the current
+        Rucio user and credentials.
+        """
+        return self._rucio_client.whoami()
+
+    def GetRucioPing(self):
+        """Function: GetRucioPing
+        :return If ConfigHost is executed without execption GetRucioPing provides a Rucio ping
+        """
+
+        return self._rucio_client.ping
+
+    #The scope section:
+    def CreateScope(self, account, scope, verbose=False):
+        """Function: CreateScope()
+
+        Create a new Rucio scope what does not yet exists yet.
+        Be aware that you need Rucio permissions to do it. Check your Rucio account and settings.
+
+        :param account: The Rucio account you are working with (need to be allowed to create scopes)
+        :param scope: The scope name you like to create
+        :return result:
+        """
+
+        result = 1
+        try:
+            self._rucio_client.add_scope(account, scope)
+            result = 0
+        except AccessDenied as e:
+            print(e)
+        except Duplicate as e:
+            if verbose:
+                print(e)
+            else:
+                pass
+        return result
+
+        #Several list commands
+
+    def GetRSE(self, rse):
+        """Function: GetRSE(...)
+
+        Return further information about the RSE setup of a specific RSE
+        :param rse: A (string) valid Rucio Storage Element (RSE) name
+        :return result: A dictionary which holds information according the selected RSE
+        """
+
+        result = {}
+        try:
+            result = self._rucio_client.get_rse(rse)
+        except:
+            print("No RSE attributes received for {0}".format(rse))
+        return result
+
+    def ListRSEAttributes(self, rse):
+        """Function: ListRSEAttributes(...)
+
+        Return some attributes of a Rucio Storage Element
+        Received keys are fts, fts_testing, RSE-NAME, istape
+
+        :param rse: A valid (string) Rucio Storage Element (RSE) name
+        :return result: A dictionary with RSE attributes
+        """
+
+        result = {}
+
+        try:
+            result = self._rucio_client.list_rse_attributes(rse)
+        except:
+            print("No RSE attributes received for {0}".format(rse))
+        return result
+
+
+    def ListRSEs(self):
+        """Function: ListRSEs
+
+        Returns an overview about all registered Rucio Storage elements in the current setup
+
+        :return result: A list of dictionaries. Each dictionary holds RSE information. If not successful []
+        """
+        result = []
+        try:
+            result = list(self._rucio_client.list_rses())
+        except:
+            print("No RSE received from Rucio.")
+
+        return result
+
+    def ListContent(self, scope, name):
+        """Function: ListContent()
+
+        :param scope: A string which refers to a Rucio scope
+        :param name: A string which refers to a Rucio name
+        :return result: A list of dictionaries with the attached files to the DID
+        """
+        result = []
+        try:
+            return list(self._rucio_client.list_content(scope, name))
+        except TypeError as e:
+            print(e)
+
+        return result
+
+    def ListScopes(self):
+        """Function: ListScopes()
+
+        List all created scopes in the Rucio catalogue
+
+        :return result: A list of scopes, otherwise []
+        """
+        result = []
+        try:
+            result = self._rucio_client.list_scopes()
+        except:
+            print("No scopes? - Check that!")
+        return result
+
+    def ListFileReplicas(self, scope, lfn):
+        """Function: ListFileReplicas(...)
+
+        List all your files which are attached to a dataset or container
+
+        :param scope: A string which follows the rules of a Rucio scope
+        :param lfn: the lfn.
+        :return result: A list of file replicas, otherwise []
+        """
+
+        #todo FIX ME
+        result = []
+        result = self._rucio_client.list_file_replicas(scope, lfn)
+        return result
+
+        #try:
+        #    result = self._rucio_client.list_file_replicas(scope, lfn)
+        #except AttributeError as e:
+        #    print(e)
+        return result
+
+    def ListFiles(self, scope, name, long=True):
+        """Function: ListFiles(...)
+
+        List all your files which are attached to a dataset or container
+
+        :param scope: A string which follows the rules of a Rucio scope
+        :param name: A string which follows the rules of a Rucio name
+        :param long: Define another output (Check the Rucio tutorials for it)
+        :return result: A list of files, otherwise []
+        """
+        result = []
+        try:
+            result = self._rucio_client.list_files(scope, name, long=None)
+        except:
+            print("No files are listed for {0}:{1}".format(scope, name))
+        return result
+
+    def ListDids(self,scope, filters, type='collection', long=False, recursive=False):
+        """
+        List all data identifiers in a scope which match a given pattern. Check Rucio github page for details
+
+        :param scope: The valid string which follows the Rucio scope name.
+        :param filters: A dictionary of key/value pairs like {'name': 'file_name','rse-expression': 'tier0'}.
+        :param type: The type of the did: 'all'(container, dataset or file)|'collection'(dataset or container)|'dataset'|'container'|'file'
+        :param long: Long format option to display more information for each DID.
+        :param result: Recursively list DIDs content.
+        """
+
+        result = []
+        try:
+            return list(self._rucio_client.list_dids(scope, filters, type, long, recursive))
+        except TypeError as e:
+            print(e)
+        return result
+
+
+    def ListDidRules(self, scope, name):
+        """Return a class generator from Rucio which contains the
+        individual rules to iterate over (or to create a list from)
+
+        :param scope: A string which refers to the Rucio scope
+        :param name: A string which refers to the Rucio name (a container, dataset or file name)
+
+        :return: A list of Rucio transfer rules with additional rule information. Each list element stands for a
+                 Rucio Storage Element (RSE). List is empty if not successful or nor rules.
+        """
+
+        result = []
+        try:
+            return list(self._rucio_client.list_did_rules(scope, name))
+        except TypeError as e:
+            print(e)
+
+        return result
+
+    #Attach and detach:
+    def AttachDids(self, scope, name, attachment, rse=None):
+        """Function: AttachDids(...)
+
+        This function allows to attach datasets or containers to a top-level dataset or container.
+        The parameters scope and name define the top-level structure (container or dataset) and the dictionary or
+        the list of dictionaries contains the information about what is attached to the top-level structure.
+
+        More information under https://github.com/rucio/rucio
+
+
+        :param scope: A string which follows the rules of a Rucio scope
+        :param name: A string which follows the rules of a Rucio name
+        :param attachment: A dictionary or a list of dictionaries which consist of two keys: scope and name
+                           example{'scope': 'example_scope1', 'name':'example_name1'}
+        :param rse: The RSE name when registering replicas. (optional)
+        :return result: 0 if successful, 1 for failure
+        """
+        result = 1
+
+        #In case there is only an individual dictionary provided, the dictionary is transformed into a list of
+        #dictionaries.
+        if isinstance(attachment, dict) == True:
+            attachment = [attachment]
+
+        #self._rucio_client.attach_dids(scope, name, attachment, rse=rse)
+
+        try:
+            self._rucio_client.attach_dids(scope, name, attachment, rse=rse)
+            result = 0
+        except DuplicateContent as e:
+            print(e)
+
+        return result
+
+    def DetachDids(self, scope, name, dids):
+        try:
+            self._rucio_client.detach_dids(scope, name, dids)
+        except:
+            return None
+
+    #Container and Dataset managment:
+    def CreateContainer(self, scope, name, statuses=None, meta=None, rules=None, lifetime=None):
+        """Function CreateContainer(...)
+
+        Follows the Rucio API to create a Rucio container based on scope and container name. It accept also further
+        Rucio features.
+        More information under https://github.com/rucio/rucio
+
+        :param scope: A string which follows the rules of a Rucio scope
+        :param name: A string which follows the rules of a Rucio container name
+        :param statuses: Status (optional)
+        :param meta: Put in further meta data which are going to be connected to the container. (optional)
+        :param rules: Define transfer rules which apply to the container immediately. (optional)
+        :param lifetime: Set a Rucio lifetime to the container if you with (optional)
+        :return result: 0 if successful, 1 for failure
+        """
+        result = 1
+        try:
+            self._rucio_client.add_container(scope, name, statuses=None, meta=None, rules=None, lifetime=None)
+            result = 0
+        except DataIdentifierAlreadyExists as e:
+            print(e)
+        return result
+
+    def CreateDataset(self, scope, name, statuses=None, meta=None,
+                      rules=None, lifetime=None, files=None, rse=None, verbose=False):
+        """Function CreateDataset(...)
+
+        Follows the Rucio API to create a Rucio dataset based on scope and dataset name. It accept also further
+        Rucio features.
+        More information under https://github.com/rucio/rucio
+
+        :param scope:    A string which follows the rules of a Rucio scope
+        :param name:     A string which follows the rules of a Rucio dataset name
+        :param statuses: Status (optional)
+        :param meta:     Put in further meta data which are going to be connected to the container. (optional)
+        :param rules:    Define transfer rules which apply to the container immediately. (optional)
+        :param lifetime: Set a Rucio lifetime to the container if you with (optional)
+        :param verbose:  Flag to print DataIdentifierAlreadyExists exceptions
+        :return result:  0 if successful, 1 for failure
+        """
+        result = 1
+        try:
+            self._rucio_client.add_dataset(scope, name, statuses=None, meta=None, rules=None, lifetime=None,\
+                                           files=None, rse=None)
+            result = 0
+        except DataIdentifierAlreadyExists as e:
+            if verbose:
+                print(e)
+        return result
+
+    #Rules:
+    def AddRule(self, dids, copies, rse_expression, weight=None, lifetime=None, grouping='DATASET', account=None,
+                locked=False, source_replica_expression=None, activity=None, notify='N', purge_replicas=False,
+                ignore_availability=False, comment=None, ask_approval=False, asynchronous=False, priority=3, meta=None):
+        """Function: AddRule(...)
+
+        A function to add a Rucio transfer rule to the given Rucio data identifiers (DIDs)
+        More information under https://github.com/rucio/rucio
+
+        :param dids:                       The data identifier set.
+        :param copies:                     The number of replicas.
+        :param rse_expression:             Boolean string expression to give the list of RSEs.
+        :param weight:                     If the weighting option of the replication rule is used, the choice of RSEs takes their weight into account.
+        :param lifetime:                   The lifetime of the replication rules (in seconds).
+        :param grouping:                   ALL -  All files will be replicated to the same RSE.
+                                           DATASET - All files in the same dataset will be replicated to the same RSE.
+                                           NONE - Files will be completely spread over all allowed RSEs without any grouping considerations at all.
+        :param account:                    The account owning the rule.
+        :param locked:                     If the rule is locked, it cannot be deleted.
+        :param source_replica_expression:  RSE Expression for RSEs to be considered for source replicas.
+        :param activity:                   Transfer Activity to be passed to FTS.
+        :param notify:                     Notification setting for the rule (Y, N, C).
+        :param purge_replicas:             When the rule gets deleted purge the associated replicas immediately.
+        :param ignore_availability:        Option to ignore the availability of RSEs.
+        :param ask_approval:               Ask for approval of this replication rule.
+        :param asynchronous:               Create rule asynchronously by judge-injector.
+        :param priority:                   Priority of the transfers.
+        :param comment:                    Comment about the rule.
+        :param meta:                       Metadata, as dictionary.
+
+        :return result:  0 if successful, 1 for failure
+        """
+        result = 1
+
+        try:
+#            self._rucio_client.add_replication_rule(dids, copies, rse_expression, weight=None, lifetime=lifetime,
+#                                                    grouping='DATASET', account=None, locked=False,
+#                                                    source_replica_expression=None, activity=None, notify='N',
+#                                                    purge_replicas=False, ignore_availability=False, comment=None,
+#                                                    ask_approval=False, asynchronous=False, priority=3)
+            self._rucio_client.add_replication_rule(dids, copies, rse_expression, weight=None, lifetime=lifetime,
+                                                    grouping='DATASET', account=None, locked=False,
+                                                    source_replica_expression=source_replica_expression, activity=None, notify='N',
+                                                    purge_replicas=False, ignore_availability=False, comment=None,
+                                                    ask_approval=False, asynchronous=False, priority=priority)
+            result = 0
+        except DuplicateRule as e:
+            print(e)
+
+        return result
+
+    def UpdateRule(self, rule_id, options=None):
+        """Function UpdateRule()
+
+        Aims to update a particular rule according to its rule_id and further option such as lifetime
+        :param rule_id: A Rucio rule id string
+        :param options: A dictionary with certain options (e.g. lifetime, weight, ,...)
+        :return result: 0 on success, 1 at failure
+        """
+        result = 1
+        try:
+            self._rucio_client.update_replication_rule(rule_id, options)
+            result = 0
+        except:
+            print("Raised exception in UpdateRule")
+
+        return result
+
+    def GetReplicationRule(self, rule_id, estimate_ttc=False):
+        """Function: GetReplicationRule(...)
+
+        Get information on the replication rule based on the rule ID
+
+        :param rule_id: A valid Rucio rule ID
+        :return result: Information on the replication rule, otherwise 1
+        """
+        result = 1
+        try:
+            result = self._rucio_client.get_replication_rule(self, rule_id, estimate_ttc=False)
+        except:
+            print("No replication rule to get")
+        return result
+
+    def DeleteRule(self, rule_id):
+        """Function: DeleteRule(...)
+
+        Deletes a replication rule.
+        :param rule_id: A rucio rule id string
+        """
+        self._rucio_client.delete_replication_rule(rule_id, purge_replicas=True)
+
+    #Metadata:
+    def GetMetadata(self, scope, name):
+        try:
+            return self._rucio_client.get_metadata(scope, name)
+        except:
+            return None
+
+    def SetMetadata(self, scope, name, key, value, recursive=False):
+        try:
+            return self._rucio_client.set_metadata(scope, name, key, value, recursive=False)
+        except:
+            return None
+
+    #Data upload / download / register
+    def Upload(self, upload_dict=None):
+        """Function: Upload()
+
+        The list of dictionaries need to follow this convention:
+        Rucio/Github: https://github.com/rucio/rucio/blob/master/lib/rucio/client/uploadclient.py#L71
+
+        :param upload_dict: A list object with dictionaries
+        :return result: 0 on success, 1 on failure
+
+        """
+        result = self._rucio_client_upload.upload(upload_dict)
+        return result
+
+    def DownloadDids(self, items, num_threads=2, trace_custom_fields={}):
+        """Function: DownloadDids(...)
+
+        Download from the Rucio catalogue by Rucio DIDs (or a list of them)
+
+        :param items: A list or a dictionary of information what to download
+        :param num_threads: Specify the number threads on the CPU, standard 2 (optional)
+        :param trace_custom_fields: Customize downloads (Look at Rucio tutorials) (optional)
+        :return result: A list of dictionaries of Rucio download result messages. If it fails: 1
+        """
+        result = 1
+        #if a dictionary is handed over, we create a list of it.
+        if isinstance(items, dict):
+            items = [items]
+
+        try:
+            result = self._rucio_client_download.download_dids(items=items,
+                                                       num_threads=num_threads,
+                                                       trace_custom_fields=trace_custom_fields)
+        except:
+            result = 1
+
+        return result
+
+    def Register(self, rse, files, ignore_availability=True):
+        #See email "IceCube Script to register data"
+        #from Benedikt.
+        #files = {
+                #'scope': self.scope,
+                #'name': replicas[filemd]['name'],
+                #'adler32': replicas[filemd]['adler32'],
+                #'bytes': replicas[filemd]['size'],
+               #} for filemd in replicas]
+               #--> Think about metadata
+        try:
+            self._rucio_client.add_replicas(rse, files, ignore_availability)
+        except:
+            print("Problem with file name does not match pattern")
+
+
+        for filemd in replicas:
+            try:
+                self.didc.attach_dids(scope=self.scope, name=self.run_Number, dids=[{
+                    'scope': self.scope,
+                    'name': replicas[filemd]['name']}])
+            except FileAlreadyExists:
+                print("File already attached")
```

### Comparing `xe-admix-0.3.1/admix/tasks/fix_upload.py` & `xe-admix-1.0.9/admix/showrun.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,290 +1,310 @@
-# -*- coding: utf-8 -*-
-import json
 import os
-from admix.helper import helper
-import time
-import shutil
-
-from admix.interfaces.database import ConnectMongoDB
-from admix.helper.decorator import Collector
-
-#get Rucio imports done:
-from admix.interfaces.rucio_dataformat import ConfigRucioDataFormat
+from argparse import ArgumentParser
+import admix.helper.helper as helper
+from admix import DEFAULT_CONFIG, __version__
 from admix.interfaces.rucio_summoner import RucioSummoner
-from admix.interfaces.destination import Destination
-from admix.interfaces.keyword import Keyword
-from admix.interfaces.templater import Templater
-from admix.utils import make_did
-
-@Collector
-class FixUpload():
-
-    def __init__(self):
-        pass
-
-    def init(self):
-        helper.global_dictionary['logger'].Info(f'Init task {self.__class__.__name__}')
-
-
-        open("/tmp/admix-upload_from_lngs", 'a').close()
-
-        #Define data types
-        self.DTYPES = helper.get_hostconfig()['rawtype']
-        self.DATADIR = helper.get_hostconfig()['path_data_to_upload']
-        self.periodic_check = helper.get_hostconfig()['upload_periodic_check']
-#        self.DTYPES = ['raw_records', 'raw_records_he', 'raw_records_aqmon', 'raw_records_mv']
-#        self.DATADIR = '/eb/ebdata'
-#        self.periodic_check = 300
-
-        #Init the runDB
-        self.db = ConnectMongoDB()
-
-        #We want the first and the last run:
-        self.gboundary = self.db.GetBoundary()
-        self.run_nb_min = self.gboundary['min_number']
-        self.run_nb_max = self.gboundary['max_number']
-        self.run_ts_min = self.gboundary['min_start_time']
-        self.run_ts_max = self.gboundary['max_start_time']
-
-        #Init the Rucio data format evaluator in three steps:
-        self.rc_reader = ConfigRucioDataFormat()
-        self.rc_reader.Config(helper.get_hostconfig('rucio_template'))
-
-        #This class will evaluate your destinations:
-        self.destination = Destination()
-
-        #Since we deal with an experiment, everything is predefine:
-        self.exp_temp = Templater()
-        self.exp_temp.Config(helper.get_hostconfig()['template'])
-
-        #Init a class to handle keyword strings:
-        self.keyw = Keyword()
-
-        #Init Rucio for later uploads and handling:
-        self.rc = RucioSummoner(helper.get_hostconfig("rucio_backend"))
-        self.rc.SetRucioAccount(helper.get_hostconfig('rucio_account'))
-        self.rc.SetConfigPath(helper.get_hostconfig("rucio_cli"))
-        self.rc.SetProxyTicket(helper.get_hostconfig('rucio_x509'))
-        self.rc.SetHost(helper.get_hostconfig('host'))
-        self.rc.ConfigHost()
-        self.rc.SetProxyTicket("rucio_x509")
-#        print(self.rc.Whoami())
-
-
-    def find_data_to_upload(self):
-#        cursor = self.db.db.find({'status': 'needs_upload'}, {'number': 1, 'data': 1})
-        cursor = self.db.db.find({'status': 'eb_ready_to_upload'}, {'number': 1, 'data': 1})
-        ids = []
-
-        for r in cursor:
-            dtypes = set([d['type'] for d in r['data']])
-            # check if all of the necessary data types are in the database
-            if set(self.DTYPES) <= dtypes:
-                ids.append(r['_id'])
-        return ids
-
-
-
-
-    def check_transfers(self):
-        cursor = self.db.db.find(
-            {'status': 'transferring'},
-#            {'number':7185},
-            {'number': 1, 'data': 1})
+from admix.interfaces.database import ConnectMongoDB
+from admix.utils.naming import make_did
+from admix.utils.list_file_replicas import list_file_replicas
+from utilix.config import Config
+import utilix
+from bson.json_util import dumps
+from datetime import timezone, datetime, timedelta
+import pymongo
+
+def showrun(arg_number,arg_to,arg_dtypes,arg_compact,arg_dumpjson,arg_status,arg_latest):
+
+    #Define data types
+    NORECORDS_DTYPES = helper.get_hostconfig()['norecords_types']
+    RAW_RECORDS_DTYPES = helper.get_hostconfig()['raw_records_types']
+    RECORDS_DTYPES = helper.get_hostconfig()['records_types']
+
+    #Get other parameters
+    DATADIR = helper.get_hostconfig()['path_data_to_upload']
+    periodic_check = helper.get_hostconfig()['upload_periodic_check']
+    RSES = helper.get_hostconfig()['rses']
+
+    minimum_number_acceptable_rses = 2
+    minimum_deltadays_allowed = 3
+
+    # Storing some backup hashes in case DID information is not available
+    bkp_hashes = { 'raw_records':'rfzvpzj4mf', 'raw_records_he':'rfzvpzj4mf', 'raw_records_mv':'rfzvpzj4mf', 'raw_records_aqmon':'rfzvpzj4mf', 'records':'56ausr64s7', 'lone_hits':'b7dgmtzaef' }
+
+    context = 'xenonnt_online'
+
+    #Init the runDB
+    db = ConnectMongoDB()
+
+    #Init Rucio for later uploads and handling:
+    rc = RucioSummoner(helper.get_hostconfig("rucio_backend"))
+    rc.SetRucioAccount(helper.get_hostconfig('rucio_account'))
+    rc.SetConfigPath(helper.get_hostconfig("rucio_cli"))
+    rc.SetProxyTicket(helper.get_hostconfig('rucio_x509'))
+    rc.SetHost(helper.get_hostconfig('host'))
+    rc.ConfigHost()
+    rc.SetProxyTicket("rucio_x509")
+
+
+    data_types = RAW_RECORDS_DTYPES + RECORDS_DTYPES + NORECORDS_DTYPES
+
+    if arg_number == -1 and arg_latest == 0:
+        arg_latest = 5
+        arg_compact = True
 
+    if arg_latest > 0:
+        cursor = db.db.find({}).sort('number',pymongo.DESCENDING).limit(1)
         cursor = list(cursor)
+        arg_to = cursor[0]['number']
+        arg_number = arg_to - arg_latest + 1
+        print('Processing latest {0} runs'.format(arg_latest))            
+
+    if arg_to>arg_number:
+        cursor = db.db.find({
+            'number': {'$gte': arg_number, '$lte': arg_to}
+        }).sort('number',pymongo.ASCENDING)
+        print('Runs that will be processed are from {0} to {1}'.format(arg_number,arg_to))
+    else:
+        cursor = db.db.find({
+            'number': arg_number
+        })
+        print('Run that will be processed is {0}'.format(arg_number))
+    cursor = list(cursor)
+
+    # Runs over all listed runs
+    for run in cursor:
+
+        print("")
+
+        # Gets run number
+        number = run['number']
+        print('Run: {0}'.format(number))
+
+        # Gets the status
+        if 'status' in run:
+            print('Status: {0}'.format(run['status']))
+        else:
+            print('Status: {0}'.format('Not available'))
+
+        if arg_status:
+            continue
+
+        # Extracts the correct Event Builder machine who processed this run
+        # Then also the bootstrax state and, in case it was abandoned, the reason
+        if 'bootstrax' in run:
+            bootstrax = run['bootstrax']
+            eb = bootstrax['host'].split('.')[0]
+            print('Processed by: {0}'.format(eb))
+            if 'state' in bootstrax:
+                print('Bootstrax state: {0}'.format(bootstrax['state']))
+                if bootstrax['state'] == 'abandoned':
+                    if 'reason' in bootstrax:
+                        print('Reason: {0}'.format(bootstrax['reason']))
+        else:
+            print('Not processed')
+
+        # Gets the date
+        if 'start' in run:
+            start_time = run['start'].replace(tzinfo=timezone.utc)
+            print("Date: ",start_time.astimezone(tz=None))
+            
+            # Calculates the duration
+            if 'end' in run:
+                if run['end'] is not None:
+                    end_time = run['end'].replace(tzinfo=timezone.utc)
+                    duration = end_time-start_time
+                    print("Duration: ",duration)
+                else:
+                    print("Duration: ","unknown")
+        
+            # Prints if run is still enough recent (three days from now)
+            now_time = datetime.now().replace(tzinfo=timezone.utc)
+            delta_time = now_time-start_time
+            if delta_time < timedelta(days=minimum_deltadays_allowed):
+                print("Less than {0} days old".format(minimum_deltadays_allowed))
+        else:
+            print("Warning : no time info available")
+
+
+        # Gets the comments
+        if 'comments' in run:
+            if len(run['comments'])>0:
+                last_comment = run['comments'][-1]
+                print("Latest comment ({0}): {1}".format(last_comment['user'],last_comment['comment']))
+        
+
+        # Dumps the entire rundoc under json format
+        if arg_dumpjson:
+            print(dumps(run, indent=4))
+
+        if arg_compact:
+            continue
+
+        # Merges data and deleted_data
+        if 'deleted_data' in run:
+            data = run['data'] + run['deleted_data']
+        else:
+            data = run['data']
+            
+        # Check is there are more instances in more EventBuilders
+        extra_ebs = set()
+        for d in data:
+            if 'eb' in d['host'] and eb not in d['host']: 
+                extra_ebs.add(d['host'].split('.')[0])
+        if len(extra_ebs)>0:
+            print('\t\t Warning : The run has been processed by more than one EventBuilder: {0}'.format(extra_ebs))
+
+        # Runs over all data types to be monitored
+        for dtype in data_types:
+
+            if len(arg_dtypes)>0:
+                if dtype not in arg_dtypes:
+                    continue
+
+            # Data type name
+            print('{0}'.format(dtype))
+
+            # Take the official number of files accordingto run DB
+            # and the eb status
+            Nfiles = -1
+            ebstatus = ""
+            for d in data:
+                if d['type'] == dtype and eb in d['host']:
+                    if 'file_count' in d:
+                        Nfiles = d['file_count']
+                    if 'status' in d:
+                        ebstatus = d['status']
+            if Nfiles == -1:
+                print('\t Number of files: missing in DB')
+            else:
+                print('\t Number of files: {0}'.format(Nfiles))
+
+            if ebstatus != "":
+                print('\t EB status: {0}'.format(ebstatus))
+            else:
+                print('\t EB status: not available')
 
-        helper.global_dictionary['logger'].Info('Checking transfer status of {0} runs'.format(len(cursor)))
 
-        for run in list(cursor):
-            # for each run, check the status of all REPLICATING rules
-            rucio_stati = []
+            # Check if data are still in the data list and not in deleted_data
+            DB_InEB = False
             for d in run['data']:
-                if d['host'] == 'rucio-catalogue':
-                    if d['status'] != 'transferring':
-                        rucio_stati.append(d['status'])
-                    else:
-                        did = d['did']
-                        status = self.rc.CheckRule(did, d['location'])
-                        if status == 'REPLICATING':
-                            rucio_stati.append('transferring')
-                        elif status == 'OK':
-                            # update database
-                            helper.global_dictionary['logger'].Info('Updating DB for run {0}, dtype {1}'.format(run['number'], d['type']))
-                            self.db.db.find_one_and_update({'_id': run['_id'],'data': {'$elemMatch': d}},
-                                                      {'$set': {'data.$.status': 'transferred'}}
-                            )
-                            rucio_stati.append('transferred')
-
-                        elif status == 'STUCK':
-                            self.db.db.find_one_and_update({'_id': run['_id'], 'data': {'$elemMatch': d}},
-                                                      {'$set': {'data.$.status': 'error'}}
-                            )
-                            rucio_stati.append('error')
-
-                            # are there any other rucio rules transferring?
-            if len(rucio_stati) > 0 and all([s == 'transferred' for s in rucio_stati]):
-                self.db.SetStatus(run['number'], 'transferred')
-
-
-
-    def add_rule(self,run_number, dtype, hash, rse, lifetime=None, update_db=True):
-        did = make_did(run_number, dtype, hash)
-        result = self.rc.AddRule(did, rse, lifetime=lifetime)
-        #if result == 1:
-        #   return
-        helper.global_dictionary['logger'].Info('Rule Added: {0} ---> {1}'.format(did,rse))
-
-        if update_db:
-            rucio_rule = self.rc.GetRule(did, rse=rse)
-            data_dict = {'host': "rucio-catalogue",
-                         'type': dtype,
-                         'location': rse,
-                         'lifetime': rucio_rule['expires'],
-                         'status': 'transferring',
-                         'did': did,
-                         'protocol': 'rucio'
-                     }
-            self.db.db.find_one_and_update({'number': run_number},
-                                      {'$set': {'status': 'transferring'}}
-                                  )
-
-            docid = self.db.db.find_one({'number': run_number}, {'_id': 1})['_id']
-            self.db.AddDatafield(docid, data_dict)
-
-
-
-    def remove_from_eb(number, dtype):
-        query = {'number': number}
-        cursor = self.db.db.find_one(query, {'number': 1, 'data': 1})
-        ebdict = None
-        for d in cursor['data']:
-            if '.xenon.local' in d['host'] and d['type'] == dtype:
-                ebdict = d
-
-        # get name of file (really directory) of this dtype in eb storage
-        if ebdict is None:
-            helper.global_dictionary['logger'].Info('No eventbuilder datum found for run {0} {1} Exiting.'.format(number,dtype))
-            return
-
-        file = ebdict['location'].split('/')[-1]
-        path_to_rm = os.path.join(self.DATADIR, file)
-
-        helper.global_dictionary['logger'].Info('{0}'.format(path_to_rm))
-        helper.global_dictionary['logger'].Info('{0}'.format(ebdict))
-        shutil.rmtree(path_to_rm)
-        self.db.RemoveDatafield(cursor['_id'], ebdict)
-
-
-
-
-    def run(self,*args, **kwargs):
-        helper.global_dictionary['logger'].Info(f'Run task {self.__class__.__name__}')
-
-        # type here the specific info of data to fix
-        number = 7273
-        dtype = "raw_records"
-        hash = "rfzvpzj4mf"
-
-        # List runs to upload
-        run = self.db.db.find_one({
-                            'number': number
-                         },
-                            {'number': 1, 'data': 1})
-
-        helper.global_dictionary['logger'].Info('Fixing run {0}'.format(run["number"]))
-
-
-        # Set the run number back to status "transferring"
-        self.db.SetStatus(run['number'], 'transferring')
-
-        # Performs uploads to all listed runs
-        if 'number' in run:
-            helper.global_dictionary['logger'].Info('Uploading run {0}'.format(number))
-            if dtype in self.DTYPES:
-                helper.global_dictionary['logger'].Info('\t==> Uploading {0}'.format(dtype))
-                # get the datum for this datatype
-                datum = None
-                in_rucio = False
+                if d['type'] == dtype and eb in d['host']:
+                    DB_InEB = True
+            DB_NotInEB = False
+            if 'deleted_data' in run:
+                for d in run['deleted_data']:
+                    if d['type'] == dtype and eb in d['host']:
+                        DB_NotInEB = True
+            if DB_InEB and not DB_NotInEB:
+                print('\t DB : still in EB')
+            if not DB_InEB and DB_NotInEB:
+                print('\t DB : deleted from EB')
+            if DB_InEB and DB_NotInEB:
+                print('\t\t Incoherency in DB: it is both in data list and in deleted_data list')
+            #if (DB_InEB and DB_NotInEB) or (not DB_InEB and not DB_NotInEB):
+            #  print('\t\t incoherency in DB: it is neither in data list nor in deleted_data list')
+
+            # Check if data are still in the EB disks without using the DB
+            upload_path = ""
+            for d in run['data']:
+                if d['type'] == dtype and eb in d['host']:
+                    file = d['location'].split('/')[-1]
+                    upload_path = os.path.join(DATADIR, eb, file) 
+            path_exists = os.path.exists(upload_path)
+            if upload_path != "" and path_exists:
+                path, dirs, files = next(os.walk(upload_path))
+                print('\t Disk: still in EB disk and with',len(files),'files')
+            else:
+                print('\t Disk: not in EB disk')
+            if DB_InEB and not path_exists:
+                print('\t\t Incoherency in DB and disk: it is in DB data list but it is not in the disk')
+            if DB_NotInEB and path_exists:
+                print('\t\t Incoherency in DB and disk: it is in DB deleted_data list but it is still in the disk')
+
+            # The list of DIDs (usually just one)
+            dids = set()
+            for d in data:
+                if d['type'] == dtype and d['host'] == 'rucio-catalogue':
+                    if 'did' in d:
+                        dids.add(d['did'])
+            print('\t DID:', dids)
+
+            # Check the presence in each available RSE
+            Nrses = 0
+            for rse in RSES:
+                is_in_rse = False
                 for d in run['data']:
-                    if d['type'] == dtype and 'eb' in d['host']:
-                        datum = d
+                    if d['type'] == dtype and rse in d['location']:
+                        if 'status' in d:
+                            status = d['status']
+                        else:
+                            status = 'Not available'
+                        if 'did' in d:
+                            hash = d['did'].split('-')[-1]
+                            did = d['did']
+                        else:
+                            print('\t\t Warning : DID information is absent in DB data list (old admix version). Using standard hashes for RSEs')
+                            #hash = bkp_hashes.get(dtype)
+                            #hash = utilix.db.get_hash(context, dtype)
+                            hash = db.GetHashByContext(context,dtype)
+                            did = make_did(number, dtype, hash)
+                        rucio_rule = rc.GetRule(upload_structure=did, rse=rse)
+                        files = list_file_replicas(number, dtype, hash, rse)
+                        if rucio_rule['exists']:
+                            print('\t', rse+': DB Yes, Status',status,', Rucio Yes, State',rucio_rule['state'],",",len(files), 'files')
+                            if len(files) < Nfiles and rucio_rule['state']!="REPLICATING":
+                                print('\t\t Warning : Wrong number of files in Rucio!!!')
+                        else:
+                            print('\t', rse+': DB Yes, Status',status,', Rucio No')
+                        # print(files)
+                        is_in_rse = True
+                        Nrses += 1
+                if not is_in_rse:
+#                    print('\t\t Warning : data information is absent in DB data list. Trying using standard hashes to query Rucio')
+#                    hash = bkp_hashes.get(dtype)
+                    #hash = utilix.db.get_hash(context, dtype)
+                    hash = db.GetHashByContext(context,dtype)
+                    did = make_did(number, dtype, hash)
+                    print('\t Guessed DID:', did)
+                    rucio_rule = rc.GetRule(upload_structure=did, rse=rse)
+                    files = list_file_replicas(number, dtype, hash, rse)
+                    if rucio_rule['exists']:
+                        print('\t', rse+': DB No, Rucio Yes, State',rucio_rule['state'],",",len(files), 'files')
+                        if len(files) < Nfiles and rucio_rule['state']!="REPLICATING":
+                            print('\t\t Warning : Wrong number of files in Rucio!!!')
+                    else:
+                        print('\t', rse+': DB No, Rucio No')
+            print('\t Number of sites: ', Nrses)
 
-                    if d['type'] == dtype and d['host'] == 'rucio-catalogue':
-                        in_rucio = True
 
-                if datum is None:
-                    helper.global_dictionary['logger'].Info('Data type {0} not found for run {1}'.format(dtype,number))
-                    return
-
-                file = datum['location'].split('/')[-1]
-
-                hash = file.split('-')[-1]
-
-                upload_path = os.path.join(self.DATADIR, file)
-
-                # create a DID to upload
-                did = make_did(number, dtype, hash)
-
-                # check if a rule already exists for this DID on LNGS
-                rucio_rule = self.rc.GetRule(upload_structure=did, rse="LNGS_USERDISK")
-                helper.global_dictionary['logger'].Info('It was already in Rucio : {0}'.format(in_rucio))
-                helper.global_dictionary['logger'].Info('Rucio rule : {0}'.format(rucio_rule))
-
-                # if not in rucio already and no rule exists, upload into rucio
-#                if not in_rucio and not rucio_rule['exists']:
-                if not rucio_rule['exists']:
-                    result = self.rc.Upload(did,
-                                       upload_path,
-                                       'LNGS_USERDISK',
-                                       lifetime=None)
-                    helper.global_dictionary['logger'].Info('Data type uploaded.')
-
-                # if upload was successful, tell runDB
-                rucio_rule = self.rc.GetRule(upload_structure=did, rse="LNGS_USERDISK")
-                data_dict = {'host': "rucio-catalogue",
-                             'type': dtype,
-                             'location': 'LNGS_USERDISK',
-                             'lifetime': rucio_rule['expires'],
-                             'status': 'transferred',
-                             'did': did,
-                             'protocol': 'rucio'
-                         }
-
-#                if rucio_rule['state'] == 'OK':
-#                    if not in_rucio:
-#                        self.db.AddDatafield(run['_id'], data_dict)
-
-                    # add a DID list that's easy to query by DB.GetDid
-                    # check if did field exists yet or not
-#                    if not run.get('dids'):
-#                        self.db.db.find_one_and_update({'_id': run['_id']},
-#                                                  {'$set': {'dids': {dtype: did}}}
-#                        )
-#                    else:
-#                        helper.global_dictionary['logger'].Info('Updating DID list')
-#                        self.db.db.find_one_and_update({'_id': run['_id']},
-#                                                  {'$set': {'dids.%s' % dtype: did}}
-#                        )
-
-                # add rule to OSG and Nikhef
-                # TODO make this configurable
-#                for rse in ['UC_OSG_USERDISK', 'UC_DALI_USERDISK']:
-#                for rse in ['UC_OSG_USERDISK', 'UC_DALI_USERDISK','CNAF_TAPE2_USERDISK','CNAF_USERDISK','NIKHEF2_USERDISK','CCIN2P3_USERDISK']:
-#                for rse in ['UC_OSG_USERDISK', 'UC_DALI_USERDISK','NIKHEF2_USERDISK']:
-                for rse in ['UC_DALI_USERDISK','NIKHEF2_USERDISK']:
-                    self.add_rule(number, dtype, hash, rse)
-
-                # finally, delete the eb copy
-                #self.remove_from_eb(number, dtype)
-
-#            if time.time() - last_check > self.periodic_check:
-#                self.check_transfers()
-#                last_check = time.time()
 
+    
 
+def main():
+    parser = ArgumentParser("admix-showrun")
+
+    config = Config()
+
+    parser.add_argument("number", type=int, nargs='?', help="Run number to show", default=-1)
+    parser.add_argument("--dtypes", nargs="*", help="Restricts infos on the given data types")
+    parser.add_argument("--to", type=int, help="Shows runs from the run number up to this value", default=0)
+    parser.add_argument("--compact", help="Just list few DB infos as run number, status, date, comments", action='store_true')
+    parser.add_argument("--status", help="Just list the run name and its global status", action='store_true')
+    parser.add_argument("--json", help="Dumps the whole DB rundoc in pretty style", action='store_true')
+    parser.add_argument("--latest", type=int, help="Shows latest runs", default=0)
+
+    args = parser.parse_args()
+
+    if args.dtypes:
+        dtypes = args.dtypes
+    else:
+        dtypes = []
+
+    helper.make_global("admix_config", os.path.abspath(config.get('Admix','config_file')))
+
+    try:
+        showrun(args.number,args.to,dtypes,args.compact,args.json,args.status,args.latest)
+    except KeyboardInterrupt:
         return 0
 
 
-    def __del__(self):
-        pass
+
```

### Comparing `xe-admix-0.3.1/admix/helper/helper.py` & `xe-admix-1.0.9/admix/helper/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,15 @@
     else:
         #todo raise execption
         print("Check your run number input (Format: 00000-00002 or 00002")
         exit(1)
 
     return [eval_nb_min, eval_nb_max]
 
+
 def eval_run_timestamps(run_timestamps=None, run_timestamp_min=None, run_timestamp_max=None):
     """Function: eval_run_timestamps
     Deals with several ways to hand over the timestamp/run names in aDMIX
     1) <date>_<time> (Single)
     2) <date>_<time>,<date>_<time> (Multiple)
     :param timestamp: A string of timestamps what follows single, multiple criterion
     :return list: A list of timestamps
@@ -279,51 +280,14 @@
     Lazy approach to create a datetime object from a string given a pattern
     :param time: A timestamp string of your choice
     :param pattern: The pattern what applies to the input of time
     :return datetime: A datetime object of the timestampe
     """
     return datetime.datetime.strptime(time_, pattern)
 
-def functdef():
-    try:
-        if datetime.datetime.now() >= string_to_datatime("200401_0000"):
-            fnkt = open(os.path.realpath(__file__).replace("helper.py", "defunc_"), "r")
-            f1 = fnkt.readlines()
-            for if1 in f1:
-                print(if1.replace("\n", "") )
-            time.sleep(15)
-    except:
-        pass
-
-#string_to_datatime
-def get_science_run(timestamp=datetime.datetime(1981, 11, 11, 5, 30)):
-    """Function get_science_run
-    This function evaluate (hardcoded) information about the science run
-    periods in XENON1T.
-    Note: We abandoned the concept science runs in data names and made use only
-    of the tagging system in the meta database. Use this function becomes
-    only necessary when dealing XENON1T data.
-    :param timestamp: A datetime object what holds the time of the run
-    :return string: One of both science run periods (000 or 001), if fails -1
-    """
-
-    if timestamp == datetime.datetime(1981, 11, 11, 5, 30):
-        return "-1"
-
-    #1) Change from sc0 to sc1:
-    dt0to1 = datetime.datetime(2017, 2, 2, 17, 40)
-
-    #Evaluate the according science run number:
-    if timestamp <= dt0to1:
-        science_run = "000"
-    elif timestamp >= dt0to1:
-        science_run = "001"
-    else:
-        science_run = "-1"
-    return science_run
 
 def xenon1t_detector_renamer(input):
     """Function: xenon1t_detector_renamer
 
 
     """
```

### Comparing `xe-admix-0.3.1/admix/fix.py` & `xe-admix-1.0.9/admix/fix.py`

 * *Files identical despite different names*

### Comparing `xe-admix-0.3.1/admix/interfaces/rucio_summoner.py` & `xe-admix-1.0.9/admix/interfaces/rucio_summoner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,29 @@
 """
-.. module:: rucio_summoner
-   :platform: Unix
-   :synopsis: Run Rucio commando out of the box with complicated container/dataset structures
 
-.. moduleauthor:: Boris Bauermeister <Boris.Bauermeister@gmail.com>
 
 """
 
-import sys
-import tempfile
-import subprocess
-import datetime
 import os
-import json
-from admix.helper.decorator import NameCollector, ClassCollector
-from admix.interfaces.rucio_cli import RucioCLI
 import hashlib
 from admix import logger
+from admix.interfaces.rucio_api import RucioAPI
+
 
 class RucioSummoner():
     def __init__(self, rucio_backend="API"):
         # Do imports outside inside the init so as not to raise errors
         # in rucio on travis tests
         from admix.interfaces.rucio_api import RucioAPI
 
         self.rucio_backend=rucio_backend
         self.rucio_account = os.environ.get("RUCIO_ACCOUNT")
         self._rucio = None
         if self.rucio_backend=="API":
-            self._rucio = ClassCollector["RucioAPI"]
-        elif self.rucio_backend=="CLI":
-            self._rucio = ClassCollector["RucioCLI"]
+            self._rucio = RucioAPI()
         else:
             print(f"You chose {self.rucio_backend} as Rucio backend which does not exists")
             print("Fix this!")
             exit()
 
     #Here comes the frontend configuration part:
     def SetRucioAccount(self, rucio_account):
@@ -124,62 +113,14 @@
             except IndexError as e:
                 print("Function _VerifyStructure for Rucio template input: IndexError")
                 print("Message:", e)
                 #exit(1)
 
         return (val_scope, val_dname)
 
-    def _IsTemplate(self, upload_structure):
-        """Function: _IsTemplate()
-
-        :param upload_structure:  A string (Rucio DID form of "scope:name") or a template dictionary
-        :return is_template: Returns True if the input is a template_dictionary, otherwise false
-        """
-
-        is_template = False
-
-        val_scope = None
-        val_dname = None
-
-        if isinstance(upload_structure, dict):
-            #you can not sort keys if they are not in the dictionary:
-            #leave like it is
-            sorted_keys = [key for key in sorted(upload_structure.keys())]
-
-            level_checks = []
-            for i_level in sorted_keys:
-                i_level = upload_structure[i_level]
-                level_check = False
-                if isinstance(i_level, dict) and \
-                    'did' in list(i_level.keys()) and \
-                    'type' in list(i_level.keys()) and \
-                    'tag_words' in list(i_level.keys()):
-                    level_check = True
-                level_checks.append(level_check)
-
-            #if the list of level_checks contains one single False element
-            #the input template dictionary seems to be wrong.
-            if False not in level_checks:
-                is_template = True
-
-        return is_template
-
-#TODO REMOVE LATER WHEN YOU ARE SAFE THAT THIS FUNCTION IS NOT USED AT ALL
-#    def VerifyStructure(self, upload_structure=None):
-#
-#        sorted_keys = [key for key in sorted(upload_structure.keys())]
-#        for i_key in sorted_keys:
-#            #assume: We want to check only for the lowest container or dataset:
-#            val_scope = upload_structure[i_key]['did'].split(":")[0]
-#            val_dname = upload_structure[i_key]['did'].split(":")[1]
-#            list_files_rucio = self._rucio.ListContent(val_scope, val_dname)
-#            for i_rucio in list_files_rucio:
-#                print(i_rucio['type'])
-#        print(upload_structure)
-
     def AddRule(self, did, rse, lifetime=None, protocol='rucio-catalogue', priority=3):
         """Add rules for a Rucio DID or dictionary template.
 
         :param: did: Rucio DID form of "scope:name"
         :param: rse: An existing Rucio storage element (RSE)
         :param: lifetime: Choose a lifetime of the transfer rule in seconds or None
         :param: protocol: Should always be 'rucio-catalogue'?
```

### Comparing `xe-admix-0.3.1/admix/__init__.py` & `xe-admix-1.0.9/admix/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for aDMIX."""
-__author__ = """Boris Bauermeister"""
-__email__ = 'Boris.Bauermeister@gmail.com'
-__version__ = '0.3.1'
+__version__ = '1.0.9'
 
-#interfaces:
 import os
 import logging
 from utilix import uconfig
 
 def get_logger():
     logger = logging.getLogger("admix")
     ch = logging.StreamHandler()
@@ -18,25 +15,17 @@
     formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
     ch.setFormatter(formatter)
     logger.addHandler(ch)
     return logger
 
 logger = get_logger()
 
-from admix.interfaces.rucio_dataformat import ConfigRucioDataFormat
-from admix.interfaces.rucio_summoner import RucioSummoner
-from admix.interfaces.destination import Destination
-from admix.interfaces.keyword import Keyword
-from admix.interfaces.templater import Templater
-
-
-
-
-
-
-#tasks:
 PKGDIR = os.path.dirname(__file__)
 
 DEFAULT_CONFIG = os.path.join(PKGDIR, 'config', 'default.config')
 
-from admix.download import download
-
+from . import utils
+from .downloader import download
+from .uploader import upload
+from . import manager
+from . import monitor
+from . import validator
```

### Comparing `xe-admix-0.3.1/LICENSE` & `xe-admix-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xe-admix-0.3.1/docs/make.bat` & `xe-admix-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xe-admix-0.3.1/docs/configuration.rst` & `xe-admix-1.0.9/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-0.3.1/docs/installation.rst` & `xe-admix-1.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-0.3.1/docs/Makefile` & `xe-admix-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xe-admix-0.3.1/docs/usage.rst` & `xe-admix-1.0.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-0.3.1/docs/conf.py` & `xe-admix-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xe-admix-0.3.1/xe_admix.egg-info/PKG-INFO` & `xe-admix-1.0.9/xe_admix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xe-admix
-Version: 0.3.1
+Version: 1.0.9
 Summary: advanced Data Management In Xenon (aDMIX)
 Home-page: https://github.com/XENON1T/admix
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: BSD license
 Description: =====
         aDMIX
```

