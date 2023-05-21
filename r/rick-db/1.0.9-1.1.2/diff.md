# Comparing `tmp/rick-db-1.0.9.tar.gz` & `tmp/rick-db-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rick-db-1.0.9.tar", last modified: Sun Feb 26 12:24:55 2023, max compression
+gzip compressed data, was "rick-db-1.1.2.tar", last modified: Sun May 21 18:30:57 2023, max compression
```

## Comparing `rick-db-1.0.9.tar` & `rick-db-1.1.2.tar`

### file list

```diff
@@ -1,52 +1,108 @@
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    15820 2023-02-26 12:24:55.722464 rick-db-1.0.9/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    15044 2021-03-03 01:01:58.000000 rick-db-1.0.9/README.md
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/rick_db/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       86 2023-02-26 12:24:19.000000 rick-db-1.0.9/rick_db/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      919 2021-02-27 00:36:01.000000 rick-db-1.0.9/rick_db/cache.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/rick_db/conn/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       60 2021-02-11 21:00:00.000000 rick-db-1.0.9/rick_db/conn/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4460 2021-02-27 01:52:02.000000 rick-db-1.0.9/rick_db/conn/connection.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/rick_db/conn/pg/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       99 2021-03-02 23:37:39.000000 rick-db-1.0.9/rick_db/conn/pg/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      144 2021-03-15 05:08:53.000000 rick-db-1.0.9/rick_db/conn/pg/json.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2570 2021-02-21 13:24:35.000000 rick-db-1.0.9/rick_db/conn/pg/postgres.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/rick_db/conn/sqlite/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       38 2021-02-11 21:57:00.000000 rick-db-1.0.9/rick_db/conn/sqlite/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1007 2021-02-28 12:06:06.000000 rick-db-1.0.9/rick_db/conn/sqlite/sqlite.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5802 2021-03-02 23:36:35.000000 rick-db-1.0.9/rick_db/mapper.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/rick_db/profiler/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       87 2021-03-03 00:27:18.000000 rick-db-1.0.9/rick_db/profiler/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1008 2021-02-11 21:00:00.000000 rick-db-1.0.9/rick_db/profiler/profilers.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       92 2023-02-26 12:23:07.000000 rick-db-1.0.9/rick_db/version.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/rick_db.egg-info/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    15820 2023-02-26 12:24:55.000000 rick-db-1.0.9/rick_db.egg-info/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      970 2023-02-26 12:24:55.000000 rick-db-1.0.9/rick_db.egg-info/SOURCES.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2023-02-26 12:24:55.000000 rick-db-1.0.9/rick_db.egg-info/dependency_links.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2021-03-02 15:32:55.000000 rick-db-1.0.9/rick_db.egg-info/not-zip-safe
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       16 2023-02-26 12:24:55.000000 rick-db-1.0.9/rick_db.egg-info/requires.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       14 2023-02-26 12:24:55.000000 rick-db-1.0.9/rick_db.egg-info/top_level.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       38 2023-02-26 12:24:55.726464 rick-db-1.0.9/setup.cfg
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1423 2021-03-03 00:56:13.000000 rick-db-1.0.9/setup.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/tests/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-02-27 13:23:35.000000 rick-db-1.0.9/tests/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      282 2021-03-02 17:46:40.000000 rick-db-1.0.9/tests/config.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/tests/conn/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-02-11 21:00:00.000000 rick-db-1.0.9/tests/conn/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/tests/conn/pg/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-02-11 21:00:00.000000 rick-db-1.0.9/tests/conn/pg/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5908 2021-02-24 09:47:36.000000 rick-db-1.0.9/tests/conn/pg/test_postgres.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/tests/conn/sqlite/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-02-11 21:48:07.000000 rick-db-1.0.9/tests/conn/sqlite/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5223 2021-03-03 00:30:01.000000 rick-db-1.0.9/tests/conn/sqlite/test_sqlite3.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1037 2021-03-03 00:21:38.000000 rick-db-1.0.9/tests/pgsql_test_repository.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    10982 2021-03-03 00:27:57.000000 rick-db-1.0.9/tests/repository.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-02-26 12:24:55.722464 rick-db-1.0.9/tests/sql/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2021-02-27 13:23:50.000000 rick-db-1.0.9/tests/sql/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3616 2021-02-27 13:23:50.000000 rick-db-1.0.9/tests/sql/test_delete.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3880 2021-02-27 13:23:50.000000 rick-db-1.0.9/tests/sql/test_dialects.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2340 2021-02-27 13:23:50.000000 rick-db-1.0.9/tests/sql/test_insert.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    24040 2021-03-03 00:28:55.000000 rick-db-1.0.9/tests/sql/test_select.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4624 2021-03-03 00:29:19.000000 rick-db-1.0.9/tests/sql/test_update.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      988 2021-03-03 00:21:38.000000 rick-db-1.0.9/tests/sqlite_test_repository.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4520 2021-03-03 00:28:07.000000 rick-db-1.0.9/tests/test_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.715435 rick-db-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 18:30:36.000000 rick-db-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-21 18:30:57.715435 rick-db-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-21 18:30:36.000000 rick-db-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/cli/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/conn/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/conn/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/pg/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db/conn/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/conn/sqlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/dbgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/rick_db/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/profiler/profilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/rick_db/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47079 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/sql/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/rick_db/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/rick_db/util/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/pg/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/pg/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/pg/pginfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/pg/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/rick_db/util/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/sqlite/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/util/sqlite/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-21 18:30:36.000000 rick-db-1.1.2/rick_db/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.707435 rick-db-1.1.2/rick_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 18:30:57.000000 rick-db-1.1.2/rick_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:30:57.715435 rick-db-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-21 18:30:36.000000 rick-db-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/tests/conn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/conn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/tests/conn/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/conn/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/conn/pg/test_postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.711435 rick-db-1.1.2/tests/conn/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/conn/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/conn/sqlite/test_sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/dbgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.715435 rick-db-1.1.2/tests/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/test_dialects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36045 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/sql/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/test_pgsql_dbgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/test_pgsql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/test_sqlite_dbgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/test_sqlite_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.715435 rick-db-1.1.2/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.715435 rick-db-1.1.2/tests/util/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/pg/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/pg/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/pg/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/pg/test_pginfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:57.715435 rick-db-1.1.2/tests/util/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/sqlite/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-21 18:30:36.000000 rick-db-1.1.2/tests/util/sqlite/test_migrations.py
```

### Comparing `rick-db-1.0.9/rick_db/cache.py` & `rick-db-1.1.2/rick_db/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import collections
 import threading
 from typing import Union
 
 
 class CacheInterface:
-
     def get(self, key):
         pass
 
     def set(self, key, value):
         pass
 
     def has(self, key):
@@ -18,15 +17,14 @@
         pass
 
     def purge(self):
         pass
 
 
 class StrCache(collections.UserDict, CacheInterface):
-
     def get(self, key: str) -> Union[str, None]:
         with threading.Lock():
             if key in self.data.keys():
                 return self.data[key]
             return None
 
     def set(self, key: str, value: str):
```

### Comparing `rick-db-1.0.9/rick_db/conn/connection.py` & `rick-db-1.1.2/rick_db/conn/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from rick_db.profiler import Profiler, NullProfiler
 from timeit import default_timer
 
-from rick_db.sql import SqlDialect
+from rick_db.sql.dialect import SqlDialect
 
 
 class ConnectionError(Exception):
     pass
 
 
 class Cursor:
-
     def __init__(self, conn, profiler, cursor, in_transaction=False):
         super().__init__()
         self._conn = conn
         self._profiler = profiler
         self._cursor = cursor
         self._in_transaction = in_transaction
 
@@ -130,15 +129,17 @@
         Retrieve connection SQL Dialect
         :return: SqlDialect
         """
         return self._dialect
 
     def begin(self):
         if self.autocommit:
-            raise ConnectionError("begin(): autocommit enabled, transactions are implicit")
+            raise ConnectionError(
+                "begin(): autocommit enabled, transactions are implicit"
+            )
         if not self._in_transaction:
             self._in_transaction = True
         else:
             raise ConnectionError("begin(): transaction already opened")
 
     def commit(self):
         self._conn.commit()
@@ -147,24 +148,35 @@
 
     def rollback(self):
         self._conn.rollback()
         if self._in_transaction:
             self._in_transaction = False
 
     def cursor(self) -> Cursor:
-        return Cursor(self._conn, self._profiler, self._conn.cursor(), self._in_transaction)
+        return Cursor(
+            self._conn, self._profiler, self._conn.cursor(), self._in_transaction
+        )
 
     def backend(self):
         return self._conn
 
     def transaction_status(self) -> bool:
         return self._in_transaction
 
+    def quote_identifier(self, value: str) -> str:
+        raise RuntimeError("virtual method, overriding required")
+
     def close(self):
         if self._conn is not None:
             if self._in_transaction:
                 self.rollback()
             self._conn.close()
             self._conn = None
 
+    def migration_manager(self):
+        raise RuntimeError("migration_manager(): not supported on the current backend")
+
+    def metadata(self):
+        raise RuntimeError("metadata(): not supported on the current backend")
+
     def __del__(self):
         self.close()
```

### Comparing `rick-db-1.0.9/rick_db/conn/pg/postgres.py` & `rick-db-1.1.2/rick_db/conn/pg/postgres.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,41 @@
 import psycopg2
 import psycopg2.extras
+from psycopg2.extensions import quote_ident
 from psycopg2.pool import SimpleConnectionPool, ThreadedConnectionPool
 from rick_db.conn import Connection
 from rick_db.profiler import Profiler, NullProfiler
-from rick_db.sql.dialects import PgSqlDialect
+from rick_db.sql.dialect import PgSqlDialect
+from rick_db.util import Metadata, MigrationManager
+from rick_db.util.pg import PgMetadata, PgMigrationManager
 
 
 class PgConnection(Connection):
-
     def __init__(self, **kwargs):
+        self._conn = None
         self._in_transaction = False
-        kwargs['cursor_factory'] = psycopg2.extras.DictCursor
+        kwargs["cursor_factory"] = psycopg2.extras.DictCursor
         conn = psycopg2.connect(**kwargs)
-        conn.set_session(isolation_level=self.isolation_level, autocommit=self.autocommit)
+        conn.set_session(
+            isolation_level=self.isolation_level, autocommit=self.autocommit
+        )
         super().__init__(conn)
         self._dialect = PgSqlDialect()
 
+    def quote_identifier(self, value: str) -> str:
+        return quote_ident(value, self._conn)
 
-class PgPooledConnection(Connection):
+    def migration_manager(self) -> MigrationManager:
+        return PgMigrationManager(self)
+
+    def metadata(self) -> Metadata:
+        return PgMetadata(self)
 
+
+class PgPooledConnection(Connection):
     def __init__(self, pool_manager, db_connection):
         super().__init__(db_connection)
         self._pool = pool_manager
         self._dialect = PgSqlDialect()
 
     def close(self):
         if self._conn is not None:
@@ -38,19 +51,19 @@
     default_max_conn = 25
     isolation_level = None
     autocommit = False
 
     def __init__(self, **kwargs):
         minconn = self.default_min_conn
         maxconn = self.default_max_conn
-        kwargs['cursor_factory'] = psycopg2.extras.DictCursor
-        if 'minconn' in kwargs:
-            minconn = kwargs.pop('minconn')
-        if 'maxconn' in kwargs:
-            maxconn = kwargs.pop('maxconn')
+        kwargs["cursor_factory"] = psycopg2.extras.DictCursor
+        if "minconn" in kwargs:
+            minconn = kwargs.pop("minconn")
+        if "maxconn" in kwargs:
+            maxconn = kwargs.pop("maxconn")
 
         self._profiler = NullProfiler()
         self._pool = self._buildPool(minconn, maxconn, kwargs)
 
     def _buildPool(self, min_conn, max_conn, conf):
         return SimpleConnectionPool(min_conn, max_conn, **conf)
 
@@ -60,15 +73,17 @@
 
     @profiler.setter
     def profiler(self, profiler: Profiler):
         self._profiler = profiler
 
     def getconn(self):
         conn = self._pool.getconn()
-        conn.set_session(isolation_level=self.isolation_level, autocommit=self.autocommit)
+        conn.set_session(
+            isolation_level=self.isolation_level, autocommit=self.autocommit
+        )
         conn = PgPooledConnection(self, conn)
         conn.profiler = self._profiler
         return conn
 
     def putconn(self, conn):
         self._pool.putconn(conn)
 
@@ -78,10 +93,9 @@
             self._pool = None
 
     def __del__(self):
         self.close()
 
 
 class PgThreadedConnectionPool(PgConnectionPool):
-
     def _buildPool(self, min_conn, max_conn, conf):
         return ThreadedConnectionPool(minconn=min_conn, maxconn=max_conn, **conf)
```

### Comparing `rick-db-1.0.9/rick_db/mapper.py` & `rick-db-1.1.2/rick_db/mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from functools import lru_cache
 import inspect
 
 # Record class attribute names
-ATTR_RECORD_MAGIC = '__PatchedRecordClass__'
-ATTR_FIELDS = '_fieldmap'
-ATTR_TABLE = '_tablename'
-ATTR_SCHEMA = '_schema'
-ATTR_PRIMARY_KEY = '_pk'
-ATTR_ROW = '_row'
+ATTR_RECORD_MAGIC = "__PatchedRecordClass__"
+ATTR_FIELDS = "_fieldmap"
+ATTR_TABLE = "_tablename"
+ATTR_SCHEMA = "_schema"
+ATTR_PRIMARY_KEY = "_pk"
+ATTR_ROW = "_row"
 
 
 class RecordError(Exception):
     pass
 
 
 class Record:
-
     def load(self, **kwargs):
         pass
 
     def fromrecord(self, record):
         pass
 
     def has_pk(self):
@@ -88,14 +87,21 @@
     def has_pk(self):
         """
         Returns true if a pk is defined
         :return:
         """
         return self._pk is not None
 
+    def dbfields(self):
+        """
+        Return the db field list from the fieldmap
+        :return: list
+        """
+        return list(self._fieldmap.values())
+
     def pk(self):
         """
         Return the current pk value, if defined
         If not defined, RecordError is raised
         If defined but value is not set, raises AttributeError
         :return:
         """
@@ -155,14 +161,19 @@
         attribute = object.__getattribute__(self, attr)
         return attribute
 
     def __setattr__(self, key, value):
         fm = object.__getattribute__(self, ATTR_FIELDS)
         if key in fm:
             data = object.__getattribute__(self, ATTR_ROW)
+            if type(data) is not dict:
+                # unwrap dict from dict-like record objects, such as psycopg2 results
+                # this is only necessary when setting values, as original object is often read-only
+                data = dict(data)
+                object.__setattr__(self, ATTR_ROW, data)
             field = fm[key]
             data[field] = value
         else:
             self.__dict__[key] = value
 
 
 @lru_cache(maxsize=None)
@@ -177,19 +188,22 @@
 
 def fieldmapper(cls=None, pk=None, tablename=None, schema=None, clsonly=False):
     def wrap(cls):
         fieldmap = {}
         if clsonly:
             # build fieldmap for current class attributes only
             fieldmap = dict(
-                (field, value) for field, value in cls.__dict__.items() if field[0] != '_' and not callable(value))
+                (field, value)
+                for field, value in cls.__dict__.items()
+                if field[0] != "_" and not callable(value)
+            )
         else:
             # build fieldmap for all available class attributes
             for item in dir(cls):
-                if item[0] != '_':
+                if item[0] != "_":
                     value = getattr(cls, item)
                     if not callable(value):
                         fieldmap[item] = value
 
         # replace class variables
         setattr(cls, ATTR_RECORD_MAGIC, True)
         setattr(cls, ATTR_FIELDS, fieldmap)
@@ -203,7 +217,21 @@
         for name, method in _base_record_method_map().items():
             setattr(cls, name, method)
         return cls
 
     if cls is None:
         return wrap
     return wrap(cls)
+
+
+def patch_record(obj=None, tablename=None, pk=None, schema=None):
+    """
+    Set/update internal attributes for Record obj
+    :param obj: Record object to update
+    :param tablename: table name
+    :param pk: primary key name
+    :param schema: schema name
+    :return:
+    """
+    setattr(obj, ATTR_TABLE, tablename)
+    setattr(obj, ATTR_PRIMARY_KEY, pk)
+    setattr(obj, ATTR_SCHEMA, schema)
```

### Comparing `rick-db-1.0.9/rick_db/profiler/profilers.py` & `rick-db-1.1.2/rick_db/profiler/profilers.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,25 +7,23 @@
     timestamp: float
     query: str
     parameters: dict
     elapsed: float
 
 
 class EventCollection(list):
-
     def filter_duration(self, duration: float) -> list:
         result = []
         for e in self:
             if e.duration >= duration:
                 result.append(e)
         return result
 
 
 class Profiler:
-
     def add_event(self, query: str, parameters: dict, duration: float):
         pass
 
     def clear(self):
         pass
 
     def get_events(self) -> EventCollection:
@@ -33,15 +31,14 @@
 
 
 class NullProfiler(Profiler):
     pass
 
 
 class DefaultProfiler(Profiler):
-
     def __init__(self):
         self._events = EventCollection()
 
     def add_event(self, query: str, parameters: dict, duration: float):
         self._events.append(Event(time.time(), query, parameters, duration))
 
     def clear(self):
```

### Comparing `rick-db-1.0.9/rick_db.egg-info/SOURCES.txt` & `rick-db-1.1.2/rick_db.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,85 @@
+LICENSE
 README.md
-setup.cfg
 setup.py
 rick_db/__init__.py
 rick_db/cache.py
+rick_db/dbgrid.py
 rick_db/mapper.py
+rick_db/repository.py
 rick_db/version.py
 rick_db.egg-info/PKG-INFO
 rick_db.egg-info/SOURCES.txt
 rick_db.egg-info/dependency_links.txt
+rick_db.egg-info/entry_points.txt
 rick_db.egg-info/not-zip-safe
 rick_db.egg-info/requires.txt
 rick_db.egg-info/top_level.txt
+rick_db/cli/__init__.py
+rick_db/cli/command.py
+rick_db/cli/config.py
+rick_db/cli/manage.py
+rick_db/cli/commands/__init__.py
+rick_db/cli/commands/check.py
+rick_db/cli/commands/dto.py
+rick_db/cli/commands/flatten.py
+rick_db/cli/commands/help.py
+rick_db/cli/commands/init.py
+rick_db/cli/commands/list.py
+rick_db/cli/commands/migrate.py
 rick_db/conn/__init__.py
 rick_db/conn/connection.py
 rick_db/conn/pg/__init__.py
-rick_db/conn/pg/json.py
 rick_db/conn/pg/postgres.py
 rick_db/conn/sqlite/__init__.py
 rick_db/conn/sqlite/sqlite.py
 rick_db/profiler/__init__.py
 rick_db/profiler/profilers.py
+rick_db/sql/__init__.py
+rick_db/sql/common.py
+rick_db/sql/delete.py
+rick_db/sql/dialect.py
+rick_db/sql/insert.py
+rick_db/sql/select.py
+rick_db/sql/update.py
+rick_db/util/__init__.py
+rick_db/util/console.py
+rick_db/util/metadata.py
+rick_db/util/migrations.py
+rick_db/util/pg/__init__.py
+rick_db/util/pg/metadata.py
+rick_db/util/pg/migrations.py
+rick_db/util/pg/pginfo.py
+rick_db/util/pg/records.py
+rick_db/util/sqlite/__init__.py
+rick_db/util/sqlite/metadata.py
+rick_db/util/sqlite/migrations.py
 tests/__init__.py
 tests/config.py
-tests/pgsql_test_repository.py
+tests/dbgrid.py
 tests/repository.py
-tests/sqlite_test_repository.py
+tests/test_pgsql_dbgrid.py
+tests/test_pgsql_repository.py
 tests/test_record.py
+tests/test_sqlite_dbgrid.py
+tests/test_sqlite_repository.py
 tests/conn/__init__.py
 tests/conn/pg/__init__.py
 tests/conn/pg/test_postgres.py
 tests/conn/sqlite/__init__.py
 tests/conn/sqlite/test_sqlite3.py
 tests/sql/__init__.py
 tests/sql/test_delete.py
 tests/sql/test_dialects.py
 tests/sql/test_insert.py
 tests/sql/test_select.py
-tests/sql/test_update.py
+tests/sql/test_update.py
+tests/util/__init__.py
+tests/util/migrations.py
+tests/util/pg/__init__.py
+tests/util/pg/common.py
+tests/util/pg/test_metadata.py
+tests/util/pg/test_migrations.py
+tests/util/pg/test_pginfo.py
+tests/util/sqlite/__init__.py
+tests/util/sqlite/test_metadata.py
+tests/util/sqlite/test_migrations.py
```

### Comparing `rick-db-1.0.9/setup.py` & `rick-db-1.1.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,45 +3,56 @@
 import os
 
 try:
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 
-version = __import__('rick_db').get_version()
+# parse/exec version straight from file
+# to avoid __init__.py and bootrsapping of unmet dependencies
+version = {}
+with open("rick_db/version.py") as fp:
+    exec(fp.read(), version)
 
 # read the contents of README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     description = f.read()
 
 setup(
-    name='rick-db',
-    version=version,
+    name="rick-db",
+    version=version["__version__"],
     author="Joao Pinheiro",
     author_email="",
-    url="https://github.com/oddbit-project/rick_db",
-    description='SQL database layer',
-    license='MIT',
+    url="https://git.oddbit.org/OddBit/rick_db",
+    description="SQL database layer",
+    license="MIT",
     long_description=description,
     long_description_content_type="text/markdown",
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: SQL',
-        'Topic :: Database',
-        'Topic :: Software Development :: Libraries :: Application Frameworks',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: SQL",
+        "Topic :: Database",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     packages=find_packages(),
     include_package_data=False,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     extras_require={},
     install_requires=[
-        "psycopg2>=2.8.6",
+        "psycopg2>=2.9.2",
     ],
     zip_safe=False,
+    entry_points={
+        "console_scripts": [
+            "rickdb=rick_db.cli.manage:main",
+        ],
+    },
 )
```

### Comparing `rick-db-1.0.9/tests/conn/pg/test_postgres.py` & `rick-db-1.1.2/tests/conn/pg/test_postgres.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 import pytest
 
 from rick_db.conn.pg import PgConnection, PgThreadedConnectionPool, PgConnectionPool
 from rick_db.sql import PgSqlDialect
-from tests.config import postgres_db
+from tests.config import postgres_db, connectSimple
 from rick_db import fieldmapper
 from rick_db.profiler import NullProfiler
 
 
 @fieldmapper
 class Animal:
-    legs = 'legs'
-    name = 'name'
-
-
-def connectSimple() -> PgConnection:
-    return PgConnection(**postgres_db)
+    legs = "legs"
+    name = "name"
 
 
 def connectPool() -> PgConnectionPool:
     cfg_pool = postgres_db.copy()
-    cfg_pool['minconn'] = 4
+    cfg_pool["minconn"] = 4
     return PgConnectionPool(**postgres_db)
 
 
 def connectThreadedPool() -> PgThreadedConnectionPool:
     cfg_pool = postgres_db.copy()
-    cfg_pool['minconn'] = 4
+    cfg_pool["minconn"] = 4
     return PgThreadedConnectionPool(**postgres_db)
 
 
 class TestPGConnection:
     createTable = "create table if not exists animals(legs int, name varchar);"
     dropTable = "drop table if exists animals"
     insertTable = "insert into animals(legs, name) values(%s, %s)"
     selectByLeg = "select * from animals where legs = %s"
 
-    rows = [(1, 'pirate'), (2, 'canary'), (3, 'maimed dog'), (4, 'cat'), (5, 'pirate ant')]
+    rows = [
+        (1, "pirate"),
+        (2, "canary"),
+        (3, "maimed dog"),
+        (4, "cat"),
+        (5, "pirate ant"),
+    ]
 
     def setup_method(self, test_method):
         conn = connectSimple()
         with conn.cursor() as qry:
             qry.exec(self.createTable)
             for r in self.rows:
                 qry.exec(self.insertTable, r)
@@ -58,36 +60,36 @@
 
     def test_transaction_commit(self, conn):
         conn.begin()
         assert conn.transaction_status() is True
         assert conn.autocommit is False
         with conn.cursor() as c:
             assert c._in_transaction is True
-            c.exec(self.insertTable, (7, 'squid'))
+            c.exec(self.insertTable, (7, "squid"))
 
         # still in transaction, now lets rollback
         assert conn.transaction_status() is True
         conn.commit()
         assert conn.transaction_status() is False
 
         # transaction commit, animal should be found
         with conn.cursor() as c:
             animal = c.fetchone(self.selectByLeg, [7])
             assert len(animal) == 2
-            assert animal['legs'] == 7
-            assert animal['name'] == 'squid'
+            assert animal["legs"] == 7
+            assert animal["name"] == "squid"
 
     def test_transaction_rollback(self, conn):
         # transaction control
         conn.begin()
         assert conn.transaction_status() is True
         assert conn.autocommit is False
         with conn.cursor() as c:
             assert c._in_transaction is True
-            c.exec(self.insertTable, (8, 'octopus'))
+            c.exec(self.insertTable, (8, "octopus"))
 
         # still in transaction, now lets rollback
         assert conn.transaction_status() is True
         conn.rollback()
         assert conn.transaction_status() is False
 
         # transaction rollback, no animal should be found
@@ -98,19 +100,19 @@
     def test_transaction_rollback_multi(self, conn):
         # test rollback of multiple cursors
         conn.begin()
         assert conn.transaction_status() is True
         assert conn.autocommit is False
         with conn.cursor() as c:
             assert c._in_transaction is True
-            c.exec(self.insertTable, (8, 'octopus'))
+            c.exec(self.insertTable, (8, "octopus"))
 
         with conn.cursor() as c:
             assert c._in_transaction is True
-            c.exec(self.insertTable, (7, 'squid'))
+            c.exec(self.insertTable, (7, "squid"))
 
         # still in transaction, now lets rollback
         assert conn.transaction_status() is True
         conn.rollback()
         assert conn.transaction_status() is False
 
         # transaction rollback, no animal should be found
@@ -130,22 +132,22 @@
         # non-existing record with class
         animal = c.fetchone(self.selectByLeg, [16], cls=Animal)
         assert animal is None
 
         # simple record
         animal = c.fetchone(self.selectByLeg, [4])
         assert len(animal) == 2
-        assert animal['legs'] == 4
-        assert animal['name'] == 'cat'
+        assert animal["legs"] == 4
+        assert animal["name"] == "cat"
 
         # simple record as Class
         animal = c.fetchone(self.selectByLeg, [4], Animal)
         assert len(animal.asdict()) == 2
         assert animal.legs == 4
-        assert animal.name == 'cat'
+        assert animal.name == "cat"
 
     def test_fetchall(self, conn):
         c = conn.cursor()
 
         # non-existing record
         animal = c.fetchall(self.selectByLeg, [16])
         assert type(animal) is list
@@ -156,35 +158,33 @@
         assert type(animal) is list
         assert len(animal) == 0
 
         # simple record
         animal = c.fetchall(self.selectByLeg, [4])
         assert type(animal) is list
         assert len(animal) == 1
-        assert animal[0]['legs'] == 4
-        assert animal[0]['name'] == 'cat'
+        assert animal[0]["legs"] == 4
+        assert animal[0]["name"] == "cat"
 
         # simple record as Class
         animal = c.fetchall(self.selectByLeg, [4], cls=Animal)
         assert type(animal) is list
         assert len(animal) == 1
         animal = animal.pop()
         assert len(animal.asdict()) == 2
         assert animal.legs == 4
-        assert animal.name == 'cat'
+        assert animal.name == "cat"
 
     def test_sqldialect(self, conn):
         assert isinstance(conn.dialect(), PgSqlDialect)
 
 
 class TestPGConnectionPool(TestPGConnection):
-
     @pytest.fixture()
     def conn(self):
         return connectPool().getconn()
 
 
 class TestPGThreadedConnectionPool(TestPGConnection):
-
     @pytest.fixture()
     def conn(self):
         return connectThreadedPool().getconn()
```

### Comparing `rick-db-1.0.9/tests/conn/sqlite/test_sqlite3.py` & `rick-db-1.1.2/tests/conn/sqlite/test_sqlite3.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,36 @@
 
 import pytest
 from rick_db.conn.sqlite import Sqlite3Connection
 from rick_db import fieldmapper
 from rick_db.profiler import NullProfiler
 from rick_db.sql import Sqlite3SqlDialect
 
-dbfile = '/tmp/rick_db_sqlite_test.db'
+dbfile = "/tmp/rick_db_sqlite_test.db"
 
 
 @fieldmapper
 class Animal:
-    legs = 'legs'
-    name = 'name'
+    legs = "legs"
+    name = "name"
 
 
 class TestSqlite3Connection:
     createTable = "create table if not exists animals(legs int, name varchar);"
     truncateTable = "delete from animals"
     insertTable = "insert into animals(legs, name) values(?, ?)"
     selectByLeg = "select * from animals where legs = ?"
 
-    rows = [(1, 'pirate'), (2, 'canary'), (3, 'maimed dog'), (4, 'cat'), (5, 'pirate ant')]
+    rows = [
+        (1, "pirate"),
+        (2, "canary"),
+        (3, "maimed dog"),
+        (4, "cat"),
+        (5, "pirate ant"),
+    ]
 
     def setup_method(self, test_method):
         self.conn = Sqlite3Connection(dbfile)
         with self.conn.cursor() as c:
             c.exec(self.createTable)
             c.exec(self.truncateTable)
             for r in self.rows:
@@ -44,36 +50,36 @@
 
     def test_transaction_commit(self, conn):
         conn.begin()
         assert conn.transaction_status() is True
         assert conn.autocommit is False
         with conn.cursor() as c:
             assert c._in_transaction is True
-            c.exec(self.insertTable, (7, 'squid'))
+            c.exec(self.insertTable, (7, "squid"))
 
         # still in transaction, now lets rollback
         assert conn.transaction_status() is True
         conn.commit()
         assert conn.transaction_status() is False
 
         # transaction commit, animal should be found
         with conn.cursor() as c:
             animal = c.fetchone(self.selectByLeg, [7])
             assert len(animal) == 2
-            assert animal['legs'] == 7
-            assert animal['name'] == 'squid'
+            assert animal["legs"] == 7
+            assert animal["name"] == "squid"
 
     def test_transaction_rollback(self, conn):
         # transaction control
         conn.begin()
         assert conn.transaction_status() is True
         assert conn.autocommit is False
         with conn.cursor() as c:
             assert c._in_transaction is True
-            c.exec(self.insertTable, (8, 'octopus'))
+            c.exec(self.insertTable, (8, "octopus"))
 
         # still in transaction, now lets rollback
         assert conn.transaction_status() is True
         conn.rollback()
         assert conn.transaction_status() is False
 
         # transaction rollback, no animal should be found
@@ -84,19 +90,19 @@
     def test_transaction_rollback_multi(self, conn):
         # test rollback of multiple cursors
         conn.begin()
         assert conn.transaction_status() is True
         assert conn.autocommit is False
         with conn.cursor() as c:
             assert c._in_transaction is True
-            c.exec(self.insertTable, (8, 'octopus'))
+            c.exec(self.insertTable, (8, "octopus"))
 
         with conn.cursor() as c:
             assert c._in_transaction is True
-            c.exec(self.insertTable, (7, 'squid'))
+            c.exec(self.insertTable, (7, "squid"))
 
         # still in transaction, now lets rollback
         assert conn.transaction_status() is True
         conn.rollback()
         assert conn.transaction_status() is False
 
         # transaction rollback, no animal should be found
@@ -116,22 +122,22 @@
         # non-existing record with class
         animal = c.fetchone(self.selectByLeg, [16], cls=Animal)
         assert animal is None
 
         # simple record
         animal = c.fetchone(self.selectByLeg, [4])
         assert len(animal) == 2
-        assert animal['legs'] == 4
-        assert animal['name'] == 'cat'
+        assert animal["legs"] == 4
+        assert animal["name"] == "cat"
 
         # simple record as Class
         animal = c.fetchone(self.selectByLeg, [4], Animal)
         assert len(animal.asdict()) == 2
         assert animal.legs == 4
-        assert animal.name == 'cat'
+        assert animal.name == "cat"
 
     def test_fetchall(self, conn):
         c = conn.cursor()
 
         # non-existing record
         animal = c.fetchall(self.selectByLeg, [16])
         assert type(animal) is list
@@ -142,21 +148,21 @@
         assert type(animal) is list
         assert len(animal) == 0
 
         # simple record
         animal = c.fetchall(self.selectByLeg, [4])
         assert type(animal) is list
         assert len(animal) == 1
-        assert animal[0]['legs'] == 4
-        assert animal[0]['name'] == 'cat'
+        assert animal[0]["legs"] == 4
+        assert animal[0]["name"] == "cat"
 
         # simple record as Class
         animal = c.fetchall(self.selectByLeg, [4], cls=Animal)
         assert type(animal) is list
         assert len(animal) == 1
         animal = animal.pop()
         assert len(animal.asdict()) == 2
         assert animal.legs == 4
-        assert animal.name == 'cat'
+        assert animal.name == "cat"
 
     def test_sqldialect(self, conn):
         assert isinstance(conn.dialect(), Sqlite3SqlDialect)
```

### Comparing `rick-db-1.0.9/tests/pgsql_test_repository.py` & `rick-db-1.1.2/tests/test_pgsql_repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-import os
-
 import pytest
 
 from rick_db.conn.pg import PgConnection
 from tests.config import postgres_db
-from tests.repository import RepositoryTest
-
-dbfile = '/tmp/rick_db_sqlite_test.db'
+from tests.repository import RepositoryTest, rows_users
 
 
 class TestPgRepository(RepositoryTest):
     createTable = """
         create table if not exists users(
         id_user serial primary key,
         name text default '',
@@ -22,16 +18,16 @@
     insertTable = "insert into users(name, email, login, active) values(%s,%s,%s,%s)"
     dropTable = "drop table users"
 
     def setup_method(self, test_method):
         self.conn = PgConnection(**postgres_db)
         with self.conn.cursor() as qry:
             qry.exec(self.createTable)
-            for r in self.rows:
-                qry.exec(self.insertTable, r)
+            for r in rows_users:
+                qry.exec(self.insertTable, list(r.values()))
 
     def teardown_method(self, test_method):
         with self.conn.cursor() as c:
             c.exec(self.dropTable)
 
     @pytest.fixture()
     def conn(self):
```

### Comparing `rick-db-1.0.9/tests/repository.py` & `rick-db-1.1.2/tests/repository.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,106 @@
 import pytest
 from rick_db import fieldmapper, Repository, RepositoryError
+from rick_db.conn.pg import PgConnection
+from rick_db.conn.sqlite import Sqlite3Connection
 
 
-@fieldmapper(tablename='users', pk='id_user')
+@fieldmapper(tablename="users", pk="id_user")
 class User:
-    id = 'id_user'
-    name = 'name'
-    email = 'email'
-    login = 'login'
-    active = 'active'
+    id = "id_user"
+    name = "name"
+    email = "email"
+    login = "login"
+    active = "active"
 
 
 @fieldmapper
 class UserName:
-    name = 'name'
+    name = "name"
 
 
 rows_users = [
     {
-        'name': 'aragorn',
-        'email': 'aragorn@lotr',
-        'login': 'aragorn',
-        'active': True,
+        "name": "aragorn",
+        "email": "aragorn@lotr",
+        "login": "aragorn",
+        "active": True,
     },
     {
-        'name': 'bilbo',
-        'email': 'bilbo@lotr',
-        'login': 'bilbo',
-        'active': True,
+        "name": "bilbo",
+        "email": "bilbo@lotr",
+        "login": "bilbo",
+        "active": True,
     },
     {
-        'name': 'samwise',
-        'email': 'samwise@lotr',
-        'login': 'samwise',
-        'active': True,
+        "name": "samwise",
+        "email": "samwise@lotr",
+        "login": "samwise",
+        "active": True,
     },
     {
-        'name': 'gandalf',
-        'email': 'gandalf@lotr',
-        'login': 'gandalf',
-        'active': True,
+        "name": "gandalf",
+        "email": "gandalf@lotr",
+        "login": "gandalf",
+        "active": True,
     },
     {
-        'name': 'gollum',
-        'email': 'gollum@lotr',
-        'login': 'gollum',
-        'active': True,
+        "name": "gollum",
+        "email": "gollum@lotr",
+        "login": "gollum",
+        "active": True,
     },
-
 ]
 
 
 class RepositoryTest:
-
     def test_create_repository(self, conn):
         repo = Repository(conn, User)
-        assert repo._pk == 'id_user'
-        assert repo._tablename == 'users'
+        assert repo._pk == "id_user"
+        assert repo._tablename == "users"
 
     def test_fetchall(self, conn):
         repo = Repository(conn, User)
         users = repo.fetch_all()
         assert type(users) is list
         assert len(users) == len(rows_users)
         for r in users:
             assert isinstance(r, User)
             assert r.id is not None and type(r.id) is int
             assert r.name is not None and type(r.name) is str and len(r.name) > 0
             assert r.email is not None and type(r.email) is str and len(r.email) > 0
-            assert r.active is not None and type(r.active) is int  # bools are mapped as ints
+            assert r.active is not None
+            if isinstance(conn, PgConnection):
+                assert type(r.active) is bool
+            elif isinstance(conn, Sqlite3Connection):
+                assert type(r.active) is int
+
+    def test_fetchall_ordered(self, conn):
+        repo = Repository(conn, User)
+        users = repo.fetch_all_ordered(User.email)
+        assert type(users) is list
+        assert len(users) == len(rows_users)
+        expected_list = []
+        for e in rows_users:
+            expected_list.append(e["email"])
+        expected_list.sort()
+
+        i = 0
+        for r in users:
+            assert isinstance(r, User)
+            assert r.id is not None and type(r.id) is int
+            assert r.name is not None and type(r.name) is str and len(r.name) > 0
+            assert r.email is not None and type(r.email) is str and len(r.email) > 0
+            assert r.email == expected_list[i]
+            i = i + 1
+            assert r.active is not None
+            if isinstance(conn, PgConnection):
+                assert type(r.active) is bool
+            elif isinstance(conn, Sqlite3Connection):
+                assert type(r.active) is int
 
     def test_fetch_pk(self, conn):
         repo = Repository(conn, User)
         users = repo.fetch_all()
         assert len(users) == len(rows_users)
         for u in users:
             record = repo.fetch_pk(u.id)
@@ -83,57 +111,57 @@
         assert record is None
 
     def test_fetch_one(self, conn):
         repo = Repository(conn, User)
         users = repo.fetch_all()
         assert len(users) == len(rows_users)
         for u in users:
-            record = repo.fetch_one(repo.select().where(User.id, '=', u.id))
+            record = repo.fetch_one(repo.select().where(User.id, "=", u.id))
             assert record is not None
             assert record.asdict() == u.asdict()
 
         # if not found, returns None
-        record = repo.fetch_one(repo.select().where(User.id, '=', -1))
+        record = repo.fetch_one(repo.select().where(User.id, "=", -1))
         assert record is None
 
     def test_fetch(self, conn):
         repo = Repository(conn, User)
         users = repo.fetch_all()
         assert len(users) == len(rows_users)
         ids = []
         names = []
         for u in users:
             ids.append(u.id)
             names.append(u.name)
 
-        users = repo.fetch(repo.select().where(User.id, '>', -1))
+        users = repo.fetch(repo.select().where(User.id, ">", -1))
         assert users is not None
         assert len(users) == len(ids)
         for u in users:
             assert u.id in ids
 
         # test empty result query
-        users = repo.fetch(repo.select().where(User.id, '=', -1))
+        users = repo.fetch(repo.select().where(User.id, "=", -1))
         assert type(users) is list
         assert len(users) == 0
 
         # test different record class
-        users = repo.fetch(repo.select().where(User.id, '>', -1), cls=UserName)
+        users = repo.fetch(repo.select().where(User.id, ">", -1), cls=UserName)
         assert users is not None
         assert len(users) == len(ids)
         for u in users:
             assert isinstance(u, UserName)
             assert u.name in names
 
     def test_fetch_raw(self, conn):
         repo = Repository(conn, User)
-        users = repo.fetch_raw(repo.select().where(User.id, '>', 0))
+        users = repo.fetch_raw(repo.select().where(User.id, ">", 0))
         assert len(users) == len(rows_users)
         for u in users:
-            assert len(u['name']) > 0
+            assert len(u["name"]) > 0
 
     def test_fetch_by_field(self, conn):
         repo = Repository(conn, User)
         users = repo.fetch_all()
         assert len(users) == len(rows_users)
         for u in users:
             # fetch all columns
@@ -142,115 +170,121 @@
             assert records.pop().asdict() == u.asdict()
 
             # fetch single column
             records = repo.fetch_by_field(User.id, u.id, cols=[User.name])
             assert len(records) == 1
             record = records.pop().asdict()
             assert len(record) == 1
-            assert record['name'] == u.name
+            assert record["name"] == u.name
 
         # fetch non-existing record
         records = repo.fetch_by_field(User.id, -1)
         assert len(records) == 0
 
     def test_fetch_where(self, conn):
         repo = Repository(conn, User)
         # fetch with one condition
-        records = repo.fetch_where([(User.name, '=', 'gandalf')])
+        records = repo.fetch_where([(User.name, "=", "gandalf")])
         assert len(records) == 1
         record = records.pop()
-        assert record.name == 'gandalf'
+        assert record.name == "gandalf"
 
         # fetch with 2 conditions
-        records = repo.fetch_where([(User.name, '=', 'gandalf'), (User.id, 'is not null', None)])
+        records = repo.fetch_where(
+            [(User.name, "=", "gandalf"), (User.id, "is not null", None)]
+        )
         assert len(records) == 1
         record = records.pop()
-        assert record.name == 'gandalf'
+        assert record.name == "gandalf"
 
         # fetch only some columns
-        records = repo.fetch_where([(User.name, '=', 'gandalf')], cols=[User.id, User.name])
+        records = repo.fetch_where(
+            [(User.name, "=", "gandalf")], cols=[User.id, User.name]
+        )
         record = records.pop()
-        assert record.name == 'gandalf'
+        assert record.name == "gandalf"
         assert record.id > 0
         assert len(record.asdict()) == 2
 
         # fetch non-existing record
-        records = repo.fetch_where([(User.name, 'like', '%john%')])
+        records = repo.fetch_where([(User.name, "like", "%john%")])
         assert len(records) == 0
 
         # incomplete
         with pytest.raises(RepositoryError):
-            repo.fetch_where([(User.name, 'like')])
+            repo.fetch_where([(User.name, "like")])
 
         # wrong type
         with pytest.raises(RepositoryError):
-            repo.fetch_where([({}, 'like')])
+            repo.fetch_where([({}, "like")])
 
         # empty where_list
         with pytest.raises(RepositoryError):
             repo.fetch_where([])
 
     def test_insert(self, conn):
         repo = Repository(conn, User)
         result = repo.insert(User(name="John", email="john.connor@skynet"))
         assert result is None
 
         # try to read inserted record
-        records = repo.fetch_by_field(User.name, 'John')
+        records = repo.fetch_by_field(User.name, "John")
         assert len(records) == 1
         record = records.pop()
-        assert record.name == 'John'
-        assert record.email == 'john.connor@skynet'
+        assert record.name == "John"
+        assert record.email == "john.connor@skynet"
         assert record.login is None
 
         # note: sqlite does not support returning multiple columns
         # it will always return a record with the inserted primary key
-        result = repo.insert(User(name="Sarah", email="sarah.connor@skynet"), cols=[User.id])
+        result = repo.insert(
+            User(name="Sarah", email="sarah.connor@skynet"), cols=[User.id]
+        )
         assert isinstance(result, User)
         assert result.id > 0
         record = repo.fetch_pk(result.id)
         assert record.name == "Sarah"
 
     def test_insert_pk(self, conn):
         repo = Repository(conn, User)
         result = repo.insert_pk(User(name="Sarah", email="sarah.connor@skynet"))
-        assert isinstance(result, User)
-        assert result.id > 0
-        record = repo.fetch_pk(result.id)
+        assert isinstance(result, int)
+        assert result > 0
+        record = repo.fetch_pk(result)
         assert record.name == "Sarah"
 
     def test_delete_pk(self, conn):
         repo = Repository(conn, User)
         result = repo.insert_pk(User(name="Sarah", email="sarah.connor@skynet"))
-        assert isinstance(result, User)
-        assert result.id > 0
-        record = repo.fetch_pk(result.id)
+        assert isinstance(result, int)
+        assert result > 0
+        record = repo.fetch_pk(result)
         assert record.name == "Sarah"
 
-        repo.delete_pk(result.id)
-        record = repo.fetch_pk(result.id)
+        repo.delete_pk(result)
+        record = repo.fetch_pk(result)
         assert record is None
 
     def test_delete_where(self, conn):
         repo = Repository(conn, User)
         result = repo.insert_pk(User(name="Sarah", email="sarah.connor@skynet"))
-        assert isinstance(result, User)
-        assert result.id > 0
-        record = repo.fetch_pk(result.id)
+        assert isinstance(result, int)
+        assert result > 0
+        record = repo.fetch_pk(result)
         assert record.name == "Sarah"
 
         # failed delete, as where doesn't match
-        repo.delete_where([(User.id, '=', result.id), (User.name, '=', 'John')])
-        record = repo.fetch_pk(result.id)
+        repo.delete_where([(User.id, "=", result), (User.name, "=", "John")])
+        record = repo.fetch_pk(result)
         assert record is not None
-        assert record.id == result.id
+        assert record.id == result
 
         # proper delete
-        repo.delete_where([(User.id, '=', result.id), (User.name, '=', 'Sarah')])
-        record = repo.fetch_pk(result.id)
+        repo.delete_where([(User.id, "=", result), (User.name, "=", "Sarah")])
+        record = repo.fetch_pk(result)
         assert record is None
 
     def test_map_result_id(self, conn):
         repo = Repository(conn, User)
         users = repo.map_result_id(repo.fetch_all())
         assert len(users) == len(rows_users)
         for id, record in users.items():
@@ -277,58 +311,80 @@
             else:
                 # existing name with another id is True
                 assert repo.exists(User.name, first, r.id) is True
 
     def test_update(self, conn):
         repo = Repository(conn, User)
 
-        record = User(name='John', email='john.connor@skynet')
+        record = User(name="John", email="john.connor@skynet")
         record = repo.insert(record, cols=[User.id])
         assert isinstance(record, User) is True
         id = record.id
 
         # read inserted record
         record = repo.fetch_pk(id)
         # simple update - pk is in the record
-        record.name = 'Sarah'
+        record.name = "Sarah"
         repo.update(record)
         record = repo.fetch_pk(id)
-        assert record.name == 'Sarah'
-        assert record.email == 'john.connor@skynet'
+        assert record.name == "Sarah"
+        assert record.email == "john.connor@skynet"
 
         # try to update without pk
         with pytest.raises(RepositoryError):
-            repo.update(User(name='John'))
+            repo.update(User(name="John"))
         # correct update procedure
-        repo.update(User(name='John'), pk_value=id)
+        repo.update(User(name="John"), pk_value=id)
         record = repo.fetch_pk(id)
-        assert record.name == 'John'
-        assert record.email == 'john.connor@skynet'
+        assert record.name == "John"
+        assert record.email == "john.connor@skynet"
 
     def test_update_where(self, conn):
         repo = Repository(conn, User)
         users = repo.fetch_all()
         u = users.pop()  # lets just use the last entry
 
         # test exception on empty where clauses
         with pytest.raises(RepositoryError):
-            repo.update_where(User(name='Pocoyo'), [])
+            repo.update_where(User(name="Pocoyo"), [])
         with pytest.raises(RepositoryError):
-            repo.update_where(User(name='Pocoyo'), [()])
+            repo.update_where(User(name="Pocoyo"), [()])
 
-        repo.update_where(User(name='Pocoyo'), [(User.login, '=', u.login)])
+        repo.update_where(User(name="Pocoyo"), [(User.login, "=", u.login)])
         record = repo.fetch_pk(u.id)
-        assert record.name == 'Pocoyo'
+        assert record.name == "Pocoyo"
         assert record.login == u.login
 
     def test_count(self, conn):
         repo = Repository(conn, User)
         users = repo.fetch_all()
         assert len(users) == repo.count()
 
     def test_count_where(self, conn):
         repo = Repository(conn, User)
         users = repo.fetch_all()
-        assert len(users) == repo.count_where([(User.id, '>', 0)])
+        assert len(users) == repo.count_where([(User.id, ">", 0)])
+
+        assert repo.count_where([(User.name, "bilbo")]) == 1
+        assert repo.count_where([(User.name, "John")]) == 0
+
+    def test_list(self, conn):
+        repo = Repository(conn, User)
+        users = repo.fetch_all()
 
-        assert repo.count_where([(User.name, 'bilbo')]) == 1
-        assert repo.count_where([(User.name, 'John')]) == 0
+        qry = repo.select().order(User.id)
+        total, rows = repo.list(qry, 1)
+        assert total == len(users)
+        assert len(rows) == 1
+        assert rows[0].name == "aragorn"
+
+        total, rows = repo.list(qry, 1, 1)
+        assert total == len(users)
+        assert len(rows) == 1
+        assert rows[0].name == "bilbo"
+
+        qry = repo.select().order(User.id)
+        total, rows = repo.list(qry, 2, 2)
+        assert total == len(users)
+        assert len(rows) == 2
+        assert rows[0].name == "samwise"
+        assert rows[1].name == "gandalf"
```

### Comparing `rick-db-1.0.9/tests/sql/test_delete.py` & `rick-db-1.1.2/tests/sql/test_delete.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,111 @@
 import pytest
 from rick_db import fieldmapper
 from rick_db.sql import Delete, Select, Literal
 
-TABLE_NAME = 'test_table'
+TABLE_NAME = "test_table"
 
 
-@fieldmapper(tablename='test_table')
+@fieldmapper(tablename="test_table")
 class SomeTable:
-    field = 'field'
-    other = 'other_field'
+    field = "field"
+    other = "other_field"
 
 
-@fieldmapper(tablename='other_table', schema='public')
+@fieldmapper(tablename="other_table", schema="public")
 class SchemaTestTable:
-    field = 'field'
-    other = 'other_field'
+    field = "field"
+    other = "other_field"
 
 
-sample_query = Select().from_('test', ['id']).where('field', '=', 'abcd')
+sample_query = Select().from_("test", ["id"]).where("field", "=", "abcd")
 
 delete_cases = [
-    ['table1', None, None, 'DELETE FROM "table1"'],
-    ['table1', None, 'public', 'DELETE FROM "public"."table1"'],
-    ['table1', [('id', '=', '5')], None, 'DELETE FROM "table1" WHERE "id" = ?'],
-    ['table1', [('id', '=', '5')], 'public', 'DELETE FROM "public"."table1" WHERE "id" = ?'],
-    ['table1', [('id', 'in', sample_query)], None,
-     'DELETE FROM "table1" WHERE "id" in (SELECT "id" FROM "test" WHERE ("field" = ?))'],
-    ['table1', [('id', 'is null', None), (Literal('LENGTH(name)'), '>', 3)], None,
-     'DELETE FROM "table1" WHERE "id" is null AND LENGTH(name) > ?'],
-
-    [SomeTable, [('id', '=', '5')], None, 'DELETE FROM "test_table" WHERE "id" = ?'],
-    [SomeTable, [('id', '=', '5')], 'public', 'DELETE FROM "test_table" WHERE "id" = ?'],
-    [SchemaTestTable, [('id', '=', '5')], None, 'DELETE FROM "public"."other_table" WHERE "id" = ?'],
-    [SchemaTestTable, [('id', '=', '5')], 'public', 'DELETE FROM "public"."other_table" WHERE "id" = ?'],
-
+    ["table1", None, None, 'DELETE FROM "table1"'],
+    ["table1", None, "public", 'DELETE FROM "public"."table1"'],
+    ["table1", [("id", "=", "5")], None, 'DELETE FROM "table1" WHERE "id" = ?'],
+    [
+        "table1",
+        [("id", "=", "5")],
+        "public",
+        'DELETE FROM "public"."table1" WHERE "id" = ?',
+    ],
+    [
+        "table1",
+        [("id", "in", sample_query)],
+        None,
+        'DELETE FROM "table1" WHERE "id" in (SELECT "id" FROM "test" WHERE ("field" = ?))',
+    ],
+    [
+        "table1",
+        [("id", "is null", None), (Literal("LENGTH(name)"), ">", 3)],
+        None,
+        'DELETE FROM "table1" WHERE "id" is null AND LENGTH(name) > ?',
+    ],
+    [SomeTable, [("id", "=", "5")], None, 'DELETE FROM "test_table" WHERE "id" = ?'],
+    [
+        SomeTable,
+        [("id", "=", "5")],
+        "public",
+        'DELETE FROM "test_table" WHERE "id" = ?',
+    ],
+    [
+        SchemaTestTable,
+        [("id", "=", "5")],
+        None,
+        'DELETE FROM "public"."other_table" WHERE "id" = ?',
+    ],
+    [
+        SchemaTestTable,
+        [("id", "=", "5")],
+        "public",
+        'DELETE FROM "public"."other_table" WHERE "id" = ?',
+    ],
 ]
 delete_cases_or = [
-    ['table1', [('id', 'in', sample_query)], None,
-     'DELETE FROM "table1" WHERE "id" in (SELECT "id" FROM "test" WHERE ("field" = ?))'],
-    ['table1', [('id', 'is null', None), (Literal('LENGTH(name)'), '>', 3)], None,
-     'DELETE FROM "table1" WHERE "id" is null OR LENGTH(name) > ?'],
-    [SomeTable, [('id', 'in', sample_query)], None,
-     'DELETE FROM "test_table" WHERE "id" in (SELECT "id" FROM "test" WHERE ("field" = ?))'],
-    [SomeTable, [('id', 'is null', None), (Literal('LENGTH(name)'), '>', 3)], None,
-     'DELETE FROM "test_table" WHERE "id" is null OR LENGTH(name) > ?'],
-    [SchemaTestTable, [('id', 'is null', None), (Literal('LENGTH(name)'), '>', 3)], None,
-     'DELETE FROM "public"."other_table" WHERE "id" is null OR LENGTH(name) > ?'],
+    [
+        "table1",
+        [("id", "in", sample_query)],
+        None,
+        'DELETE FROM "table1" WHERE "id" in (SELECT "id" FROM "test" WHERE ("field" = ?))',
+    ],
+    [
+        "table1",
+        [("id", "is null", None), (Literal("LENGTH(name)"), ">", 3)],
+        None,
+        'DELETE FROM "table1" WHERE "id" is null OR LENGTH(name) > ?',
+    ],
+    [
+        SomeTable,
+        [("id", "in", sample_query)],
+        None,
+        'DELETE FROM "test_table" WHERE "id" in (SELECT "id" FROM "test" WHERE ("field" = ?))',
+    ],
+    [
+        SomeTable,
+        [("id", "is null", None), (Literal("LENGTH(name)"), ">", 3)],
+        None,
+        'DELETE FROM "test_table" WHERE "id" is null OR LENGTH(name) > ?',
+    ],
+    [
+        SchemaTestTable,
+        [("id", "is null", None), (Literal("LENGTH(name)"), ">", 3)],
+        None,
+        'DELETE FROM "public"."other_table" WHERE "id" is null OR LENGTH(name) > ?',
+    ],
 ]
 
 delete_cases_and_or = [
-    ['table1', [('id', 'in', sample_query)], [('field', '>', 3)], None,
-     'DELETE FROM "table1" WHERE "id" in (SELECT "id" FROM "test" WHERE ("field" = ?)) OR "field" > ?'],
-
+    [
+        "table1",
+        [("id", "in", sample_query)],
+        [("field", ">", 3)],
+        None,
+        'DELETE FROM "table1" WHERE "id" in (SELECT "id" FROM "test" WHERE ("field" = ?)) OR "field" > ?',
+    ],
 ]
 
 
 @pytest.mark.parametrize("table, where_list, schema, result", delete_cases)
 def test_delete(table, where_list, schema, result):
     qry = Delete().from_(table, schema)
     if where_list:
@@ -74,15 +124,17 @@
         field, operator, value = item
         qry.orwhere(field, operator, value)
 
     sql, _ = qry.assemble()
     assert sql == result
 
 
-@pytest.mark.parametrize("table, and_where_list, or_where_list, schema, result", delete_cases_and_or)
+@pytest.mark.parametrize(
+    "table, and_where_list, or_where_list, schema, result", delete_cases_and_or
+)
 def test_delete_and_or(table, and_where_list, or_where_list, schema, result):
     qry = Delete().from_(table, schema)
     for item in and_where_list:
         field, operator, value = item
         qry.where(field, operator, value)
     for item in or_where_list:
         field, operator, value = item
```

### Comparing `rick-db-1.0.9/tests/sql/test_dialects.py` & `rick-db-1.1.2/tests/sql/test_dialects.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from rick_db.sql import PgSqlDialect, SqlDialect
 from rick_db.sql.common import Literal
 
-TABLE_NAME = 'test_table'
+TABLE_NAME = "test_table"
 
 # SqlDialect -----------------------------------------------------------------------------------------------------------
 sql_dialect_table = [
     ["name", None, None, '"name"'],
     ["name", "alias", None, '"name" AS "alias"'],
     ["name", "alias", "schema", '"schema"."name" AS "alias"'],
     ["name", None, "schema", '"schema"."name"'],
@@ -15,31 +15,60 @@
 
 
 @pytest.mark.parametrize("table_name, alias, schema, result", sql_dialect_table)
 def test_sqldialect_table(table_name, alias, schema, result):
     assert PgSqlDialect().table(table_name, alias, schema) == result
 
 
+sql_dialect_database = [
+    ["name", None, '"name"'],
+    ["name", "alias", '"name" AS "alias"'],
+]
+
+
+@pytest.mark.parametrize("db_name, alias, result", sql_dialect_database)
+def test_sqldialect_database(db_name, alias, result):
+    assert PgSqlDialect().database(db_name, alias) == result
+
+
 sql_dialect_field = [
     # simple fields
     ["field", None, None, None, '"field"'],
     ["field", "alias", None, None, '"field" AS "alias"'],
     ["field", "alias", "table", None, '"table"."field" AS "alias"'],
     ["field", "alias", "table", "schema", '"schema"."table"."field" AS "alias"'],
     # field literals
-    [Literal("TOP(field)"), None, None, None, 'TOP(field)'],
+    [Literal("TOP(field)"), None, None, None, "TOP(field)"],
     [Literal("TOP(field)"), "alias", None, None, 'TOP(field) AS "alias"'],
-    [Literal("TOP(field)"), "alias", "table", "schema", 'TOP(field) AS "alias"'],  # table and schema are ignored
+    [
+        Literal("TOP(field)"),
+        "alias",
+        "table",
+        "schema",
+        'TOP(field) AS "alias"',
+    ],  # table and schema are ignored
     # field alias and casting
     ["field", ["text"], None, None, 'CAST("field" AS text)'],
     ["field", ["text"], "table", None, 'CAST("table"."field" AS text)'],
     ["field", ["text"], "table", "schema", 'CAST("schema"."table"."field" AS text)'],
     ["field", ["text", "alias"], None, None, 'CAST("field" AS text) AS "alias"'],
-    ["field", ["text", "alias"], "table", None, 'CAST("table"."field" AS text) AS "alias"'],
-    ["field", ["text", "alias"], "table", "schema", 'CAST("schema"."table"."field" AS text) AS "alias"'],
+    [
+        "field",
+        ["text", "alias"],
+        "table",
+        None,
+        'CAST("table"."field" AS text) AS "alias"',
+    ],
+    [
+        "field",
+        ["text", "alias"],
+        "table",
+        "schema",
+        'CAST("schema"."table"."field" AS text) AS "alias"',
+    ],
 ]
 
 
 @pytest.mark.parametrize("field, field_alias, table, schema, result", sql_dialect_field)
 def test_sqlitedialect_field(field, field_alias, table, schema, result):
     assert SqlDialect().field(field, field_alias, table, schema) == result
 
@@ -61,23 +90,35 @@
 pg_dialect_field = [
     # simple fields
     ["field", None, None, None, '"field"'],
     ["field", "alias", None, None, '"field" AS "alias"'],
     ["field", "alias", "table", None, '"table"."field" AS "alias"'],
     ["field", "alias", "table", "schema", '"schema"."table"."field" AS "alias"'],
     # field literals
-    [Literal("TOP(field)"), None, None, None, 'TOP(field)'],
+    [Literal("TOP(field)"), None, None, None, "TOP(field)"],
     [Literal("TOP(field)"), "alias", None, None, 'TOP(field) AS "alias"'],
-    [Literal("TOP(field)"), "alias", "table", "schema", 'TOP(field) AS "alias"'],  # table and schema are ignored
+    [
+        Literal("TOP(field)"),
+        "alias",
+        "table",
+        "schema",
+        'TOP(field) AS "alias"',
+    ],  # table and schema are ignored
     # field alias and casting
     ["field", ["text"], None, None, '"field"::text'],
     ["field", ["text"], "table", None, '"table"."field"::text'],
     ["field", ["text"], "table", "schema", '"schema"."table"."field"::text'],
     ["field", ["text", "alias"], None, None, '"field"::text AS "alias"'],
     ["field", ["text", "alias"], "table", None, '"table"."field"::text AS "alias"'],
-    ["field", ["text", "alias"], "table", "schema", '"schema"."table"."field"::text AS "alias"'],
+    [
+        "field",
+        ["text", "alias"],
+        "table",
+        "schema",
+        '"schema"."table"."field"::text AS "alias"',
+    ],
 ]
 
 
 @pytest.mark.parametrize("field, field_alias, table, schema, result", pg_dialect_field)
 def test_pgsqldialect_field(field, field_alias, table, schema, result):
     assert PgSqlDialect().field(field, field_alias, table, schema) == result
```

### Comparing `rick-db-1.0.9/tests/sqlite_test_repository.py` & `rick-db-1.1.2/tests/test_sqlite_repository.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import os
 
 import pytest
 from rick_db.conn.sqlite import Sqlite3Connection
 from tests.repository import RepositoryTest, rows_users
 
-dbfile = '/tmp/rick_db_sqlite_test.db'
-
 
 class TestSqlite3Repository(RepositoryTest):
     createTable = """
         create table if not exists users(
         id_user integer primary key autoincrement,
         name text default '',
         email text default '',
         login text default null,
         active boolean default true
         );
         """
     insertTable = "insert into users(name, email, login, active) values(?,?,?,?)"
 
     def setup_method(self, test_method):
-        self.conn = Sqlite3Connection(dbfile)
+        self.conn = Sqlite3Connection(":memory:")
         with self.conn.cursor() as c:
             c.exec(self.createTable)
             for r in rows_users:
                 c.exec(self.insertTable, list(r.values()))
 
     def teardown_method(self, test_method):
         self.conn.close()
-        os.unlink(dbfile)
 
     @pytest.fixture()
     def conn(self):
         return self.conn
```

### Comparing `rick-db-1.0.9/tests/test_record.py` & `rick-db-1.1.2/tests/test_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import pytest
 
-from rick_db.mapper import Record, fieldmapper, ATTR_FIELDS, ATTR_TABLE, ATTR_SCHEMA, ATTR_PRIMARY_KEY, \
-    ATTR_RECORD_MAGIC, ATTR_ROW
+from rick_db.mapper import (
+    Record,
+    fieldmapper,
+    ATTR_FIELDS,
+    ATTR_TABLE,
+    ATTR_SCHEMA,
+    ATTR_PRIMARY_KEY,
+    ATTR_RECORD_MAGIC,
+    ATTR_ROW,
+)
+
+FIELD_USER_ID = "id_user"
+FIELD_USER_NAME = "username"
+
+FIELD_ADDRESS_ID = "id_address"
+FIELD_ADDRESS_USER_ID = "fk_user"
+FIELD_ADDRESS_STREET = "street"
+FIELD_ADDRESS_CITY = "city"
 
-FIELD_USER_ID = 'id_user'
-FIELD_USER_NAME = 'username'
 
-FIELD_ADDRESS_ID = 'id_address'
-FIELD_ADDRESS_USER_ID = 'fk_user'
-FIELD_ADDRESS_STREET = 'street'
-FIELD_ADDRESS_CITY = 'city'
-
-
-@fieldmapper(pk='id_user')
+@fieldmapper(pk="id_user")
 class User(Record):
     id = FIELD_USER_ID
     name = FIELD_USER_NAME
 
 
-@fieldmapper(tablename='addresses')
+@fieldmapper(tablename="addresses")
 class Address(Record):
     id = FIELD_ADDRESS_ID
     user = FIELD_ADDRESS_USER_ID
     street = FIELD_ADDRESS_STREET
     city = FIELD_ADDRESS_CITY
 
 
@@ -40,65 +48,70 @@
     row = getattr(User, ATTR_ROW, None)
     assert type(row) is dict
     assert len(row) == 0
     fm = getattr(User, ATTR_FIELDS, None)
     assert type(fm) is dict
     assert len(fm) == 2
     for k in fm.keys():
-        assert k in ['id', 'name']
+        assert k in ["id", "name"]
     for v in fm.values():
         assert v in [FIELD_USER_ID, FIELD_USER_NAME]
     assert User.id == FIELD_USER_ID
     assert User.name == FIELD_USER_NAME
 
 
 def test_fieldmapper_address():
     # check address class
     assert getattr(Address, ATTR_RECORD_MAGIC, None) is True
     for attr in [ATTR_SCHEMA, ATTR_PRIMARY_KEY]:
         assert getattr(Address, attr, True) is None
-    assert getattr(Address, ATTR_TABLE, None) == 'addresses'
+    assert getattr(Address, ATTR_TABLE, None) == "addresses"
     row = getattr(Address, ATTR_ROW, None)
     assert type(row) is dict
     assert len(row) == 0
     fm = getattr(Address, ATTR_FIELDS, None)
     assert type(fm) is dict
     assert len(fm) == 4
     for k in fm.keys():
-        assert k in ['id', 'user', 'street', 'city']
+        assert k in ["id", "user", "street", "city"]
     for v in fm.values():
-        assert v in [FIELD_ADDRESS_ID, FIELD_ADDRESS_USER_ID, FIELD_ADDRESS_STREET, FIELD_ADDRESS_CITY]
+        assert v in [
+            FIELD_ADDRESS_ID,
+            FIELD_ADDRESS_USER_ID,
+            FIELD_ADDRESS_STREET,
+            FIELD_ADDRESS_CITY,
+        ]
     assert Address.id == FIELD_ADDRESS_ID
     assert Address.user == FIELD_ADDRESS_USER_ID
     assert Address.street == FIELD_ADDRESS_STREET
     assert Address.city == FIELD_ADDRESS_CITY
 
 
 def check_user(u: User, id, name):
     # pk
     assert u.has_pk() is True
     # read attributes
     if id is None:
         assert u.id is None
         d = {
-            'name': name,
+            "name": name,
         }
         r = {
-            'username': name,
+            "username": name,
         }
     else:
         assert u.id == id
         assert u.pk() == id
         d = {
-            'id': id,
-            'name': name,
+            "id": id,
+            "name": name,
         }
         r = {
-            'id_user': id,
-            'username': name,
+            "id_user": id,
+            "username": name,
         }
     assert u.name == name
 
     assert u.fields() == list(d.keys())
     assert u.values() == list(d.values())
     for field, value in u.items():
         assert field in d.keys()
@@ -132,15 +145,17 @@
     new_user = User().load(**user.asdict())
     check_user(new_user, 9, "john doe")
 
     record = user.asrecord()
     new_user = User().fromrecord(record)
     check_user(new_user, 9, "john doe")
 
-    record = record.copy()  # duplicate record, because fromrecord() uses referencing, not a separate copy
+    record = (
+        record.copy()
+    )  # duplicate record, because fromrecord() uses referencing, not a separate copy
     record["unmapped_field"] = "something"
     new_user = User().fromrecord(record)
     check_user(new_user, 9, "john doe")
 
     # ensure dicts are not shared
     user = User().load(name="john connor")
     user2 = User()
@@ -153,9 +168,9 @@
     ua = UserAddress(name="john connor", city="california")
     assert ua._tablename == "view_user"
     assert ua._pk is None
     assert ua.name == "john connor"
     assert ua.street is None
     assert ua.city == "california"
     for field in ua.fields():
-        assert field in ['id', 'name', 'user', 'street', 'city']
+        assert field in ["id", "name", "user", "street", "city"]
     assert len(ua.asdict()) == 2
```

