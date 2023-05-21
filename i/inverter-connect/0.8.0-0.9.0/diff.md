# Comparing `tmp/inverter-connect-0.8.0.tar.gz` & `tmp/inverter-connect-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inverter-connect-0.8.0.tar", last modified: Thu May 18 17:30:46 2023, max compression
+gzip compressed data, was "inverter-connect-0.9.0.tar", last modified: Fri May 19 17:19:07 2023, max compression
```

## Comparing `inverter-connect-0.8.0.tar` & `inverter-connect-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.448533 inverter-connect-0.8.0/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.8.0/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.8.0/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.444533 inverter-connect-0.8.0/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.444533 inverter-connect-0.8.0/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1570 2023-05-09 16:20:44.000000 inverter-connect-0.8.0/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.8.0/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)    18840 2023-05-18 17:30:46.448533 inverter-connect-0.8.0/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)    18426 2023-05-18 16:01:07.000000 inverter-connect-0.8.0/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.8.0/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.8.0/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.444533 inverter-connect-0.8.0/inverter/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.8.0/inverter/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.8.0/inverter/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.444533 inverter-connect-0.8.0/inverter/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.444533 inverter-connect-0.8.0/inverter/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.8.0/inverter/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.8.0/inverter/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)      148 2023-05-18 17:29:07.000000 inverter-connect-0.8.0/inverter/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.8.0/inverter/__main__.py
--rw-rw-r--   0 jens      (1000) users      (100)     5267 2023-05-18 16:22:12.000000 inverter-connect-0.8.0/inverter/api.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.444533 inverter-connect-0.8.0/inverter/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.8.0/inverter/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    18087 2023-05-18 17:20:12.000000 inverter-connect-0.8.0/inverter/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     9380 2023-05-12 07:19:04.000000 inverter-connect-0.8.0/inverter/cli/dev.py
--rw-rw-r--   0 jens      (1000) users      (100)    11042 2023-05-18 17:18:34.000000 inverter-connect-0.8.0/inverter/connection.py
--rw-rw-r--   0 jens      (1000) users      (100)      392 2023-05-12 06:12:26.000000 inverter-connect-0.8.0/inverter/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     1768 2023-05-06 10:26:14.000000 inverter-connect-0.8.0/inverter/daily_reset.py
--rw-rw-r--   0 jens      (1000) users      (100)     4048 2023-05-18 16:36:49.000000 inverter-connect-0.8.0/inverter/data_types.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.444533 inverter-connect-0.8.0/inverter/definitions/
--rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.8.0/inverter/definitions/deye_2mppt.yaml
--rw-rw-r--   0 jens      (1000) users      (100)      379 2023-05-12 07:21:52.000000 inverter-connect-0.8.0/inverter/definitions/deye_2mppt_validations.yaml
--rw-rw-r--   0 jens      (1000) users      (100)     2260 2023-05-06 10:26:15.000000 inverter-connect-0.8.0/inverter/definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      538 2023-05-06 10:11:26.000000 inverter-connect-0.8.0/inverter/exceptions.py
--rw-rw-r--   0 jens      (1000) users      (100)     3336 2023-05-18 06:35:56.000000 inverter-connect-0.8.0/inverter/publish_loop.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.448533 inverter-connect-0.8.0/inverter/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      256 2023-05-08 19:20:13.000000 inverter-connect-0.8.0/inverter/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3020 2023-05-18 06:35:32.000000 inverter-connect-0.8.0/inverter/tests/fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     3293 2023-05-06 10:24:09.000000 inverter-connect-0.8.0/inverter/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)     1729 2023-05-18 03:55:25.000000 inverter-connect-0.8.0/inverter/tests/test_cli.py
--rw-rw-r--   0 jens      (1000) users      (100)      826 2023-05-06 10:26:14.000000 inverter-connect-0.8.0/inverter/tests/test_connect.py
--rw-rw-r--   0 jens      (1000) users      (100)     5888 2023-05-08 19:33:47.000000 inverter-connect-0.8.0/inverter/tests/test_daily_reset.py
--rw-rw-r--   0 jens      (1000) users      (100)     1563 2023-05-08 19:29:30.000000 inverter-connect-0.8.0/inverter/tests/test_definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      340 2023-05-18 14:29:54.000000 inverter-connect-0.8.0/inverter/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.8.0/inverter/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     4794 2023-05-18 14:26:11.000000 inverter-connect-0.8.0/inverter/tests/test_readme.py
--rw-rw-r--   0 jens      (1000) users      (100)     4230 2023-05-18 08:47:32.000000 inverter-connect-0.8.0/inverter/tests/test_user_settings.py
--rw-rw-r--   0 jens      (1000) users      (100)     2114 2023-05-08 19:34:46.000000 inverter-connect-0.8.0/inverter/tests/test_validators.py
--rw-rw-r--   0 jens      (1000) users      (100)     4306 2023-05-18 09:33:28.000000 inverter-connect-0.8.0/inverter/user_settings.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.448533 inverter-connect-0.8.0/inverter/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.8.0/inverter/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3240 2023-05-18 16:02:56.000000 inverter-connect-0.8.0/inverter/utilities/cli.py
--rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.8.0/inverter/utilities/modbus_converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1562 2023-05-06 10:34:37.000000 inverter-connect-0.8.0/inverter/validators.py
--rw-rw-r--   0 jens      (1000) users      (100)      732 2023-05-08 19:17:53.000000 inverter-connect-0.8.0/inverter/verbosity.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 17:30:46.448533 inverter-connect-0.8.0/inverter_connect.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)    18840 2023-05-18 17:30:46.000000 inverter-connect-0.8.0/inverter_connect.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1403 2023-05-18 17:30:46.000000 inverter-connect-0.8.0/inverter_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-18 17:30:46.000000 inverter-connect-0.8.0/inverter_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-18 17:30:46.000000 inverter-connect-0.8.0/inverter_connect.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      304 2023-05-18 17:30:46.000000 inverter-connect-0.8.0/inverter_connect.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-18 17:30:46.000000 inverter-connect-0.8.0/inverter_connect.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4997 2023-05-18 16:12:30.000000 inverter-connect-0.8.0/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    54025 2023-05-18 16:13:03.000000 inverter-connect-0.8.0/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)    22698 2023-05-18 16:12:46.000000 inverter-connect-0.8.0/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-18 17:30:46.448533 inverter-connect-0.8.0/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.493756 inverter-connect-0.9.0/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.9.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.9.0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.489756 inverter-connect-0.9.0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.489756 inverter-connect-0.9.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1570 2023-05-09 16:20:44.000000 inverter-connect-0.9.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.9.0/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)    18743 2023-05-19 17:19:07.493756 inverter-connect-0.9.0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)    18329 2023-05-19 16:46:55.000000 inverter-connect-0.9.0/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.9.0/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.9.0/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.493756 inverter-connect-0.9.0/inverter/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.9.0/inverter/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.9.0/inverter/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.489756 inverter-connect-0.9.0/inverter/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.493756 inverter-connect-0.9.0/inverter/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.9.0/inverter/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.9.0/inverter/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      148 2023-05-19 17:13:39.000000 inverter-connect-0.9.0/inverter/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.9.0/inverter/__main__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5267 2023-05-18 16:22:12.000000 inverter-connect-0.9.0/inverter/api.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.493756 inverter-connect-0.9.0/inverter/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.9.0/inverter/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    17704 2023-05-19 16:41:17.000000 inverter-connect-0.9.0/inverter/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     9380 2023-05-12 07:19:04.000000 inverter-connect-0.9.0/inverter/cli/dev.py
+-rw-rw-r--   0 jens      (1000) users      (100)    11084 2023-05-19 15:48:44.000000 inverter-connect-0.9.0/inverter/connection.py
+-rw-rw-r--   0 jens      (1000) users      (100)      392 2023-05-12 06:12:26.000000 inverter-connect-0.9.0/inverter/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1768 2023-05-06 10:26:14.000000 inverter-connect-0.9.0/inverter/daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4048 2023-05-18 16:36:49.000000 inverter-connect-0.9.0/inverter/data_types.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.493756 inverter-connect-0.9.0/inverter/definitions/
+-rw-rw-r--   0 jens      (1000) users      (100)     3065 2023-05-19 17:13:39.000000 inverter-connect-0.9.0/inverter/definitions/deye_2mppt.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)      379 2023-05-12 07:21:52.000000 inverter-connect-0.9.0/inverter/definitions/deye_2mppt_validations.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)     2260 2023-05-06 10:26:15.000000 inverter-connect-0.9.0/inverter/definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      538 2023-05-06 10:11:26.000000 inverter-connect-0.9.0/inverter/exceptions.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3336 2023-05-18 06:35:56.000000 inverter-connect-0.9.0/inverter/publish_loop.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.493756 inverter-connect-0.9.0/inverter/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      256 2023-05-08 19:20:13.000000 inverter-connect-0.9.0/inverter/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3020 2023-05-18 06:35:32.000000 inverter-connect-0.9.0/inverter/tests/fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3293 2023-05-06 10:24:09.000000 inverter-connect-0.9.0/inverter/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1729 2023-05-18 03:55:25.000000 inverter-connect-0.9.0/inverter/tests/test_cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)      826 2023-05-06 10:26:14.000000 inverter-connect-0.9.0/inverter/tests/test_connect.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5888 2023-05-08 19:33:47.000000 inverter-connect-0.9.0/inverter/tests/test_daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1563 2023-05-08 19:29:30.000000 inverter-connect-0.9.0/inverter/tests/test_definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      340 2023-05-18 14:29:54.000000 inverter-connect-0.9.0/inverter/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.9.0/inverter/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4909 2023-05-19 16:47:46.000000 inverter-connect-0.9.0/inverter/tests/test_readme.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4230 2023-05-18 08:47:32.000000 inverter-connect-0.9.0/inverter/tests/test_user_settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2114 2023-05-08 19:34:46.000000 inverter-connect-0.9.0/inverter/tests/test_validators.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4306 2023-05-18 09:33:28.000000 inverter-connect-0.9.0/inverter/user_settings.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.493756 inverter-connect-0.9.0/inverter/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.9.0/inverter/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4654 2023-05-19 16:10:13.000000 inverter-connect-0.9.0/inverter/utilities/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.9.0/inverter/utilities/modbus_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1562 2023-05-06 10:34:37.000000 inverter-connect-0.9.0/inverter/validators.py
+-rw-rw-r--   0 jens      (1000) users      (100)      732 2023-05-08 19:17:53.000000 inverter-connect-0.9.0/inverter/verbosity.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 17:19:07.493756 inverter-connect-0.9.0/inverter_connect.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)    18743 2023-05-19 17:19:07.000000 inverter-connect-0.9.0/inverter_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1403 2023-05-19 17:19:07.000000 inverter-connect-0.9.0/inverter_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-19 17:19:07.000000 inverter-connect-0.9.0/inverter_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-19 17:19:07.000000 inverter-connect-0.9.0/inverter_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      304 2023-05-19 17:19:07.000000 inverter-connect-0.9.0/inverter_connect.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-19 17:19:07.000000 inverter-connect-0.9.0/inverter_connect.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4997 2023-05-18 16:12:30.000000 inverter-connect-0.9.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    54025 2023-05-18 16:13:03.000000 inverter-connect-0.9.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    22698 2023-05-18 16:12:46.000000 inverter-connect-0.9.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-19 17:19:07.493756 inverter-connect-0.9.0/setup.cfg
```

### Comparing `inverter-connect-0.8.0/.github/workflows/tests.yml` & `inverter-connect-0.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/PKG-INFO` & `inverter-connect-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.8.0
+Version: 0.9.0
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -135,15 +135,15 @@
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
 Usage: ./cli.py print-values [OPTIONS]
 
  Print all known register values from Inverter, e.g.:
- .../inverter-connect$ ./cli.py print-values 192.168.123.456
+ .../inverter-connect$ ./cli.py print-values
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --ip             TEXT                     IP address of your inverter [required]              │
 │ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
 │                                              [required]                                          │
 │ *  --inverter       TEXT                     Prefix of yaml config files in                      │
 │                                              inverter/definitions/                               │
@@ -170,23 +170,22 @@
 
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
 Usage: ./cli.py print-at-commands [OPTIONS] [COMMANDS]...
 
  Print one or more AT command values from Inverter.
  Use all known AT commands, if no one is given, e.g.:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
+ .../inverter-connect$ ./cli.py print-at-commands
  Or specify one or more AT-commands, e.g.:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER .../inverter-connect$
- ./cli.py print-at-commands 192.168.123.456 WEBVER WEBU
+ .../inverter-connect$ ./cli.py print-at-commands WEBVER .../inverter-connect$ ./cli.py
+ print-at-commands WEBVER WEBU
  e.g.: Set NTP server, enable NTP and check the values:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
- NTPSER NTPEN
+ .../inverter-connect$ ./cli.py print-at-commands NTPSER=192.168.1.1 NTPEN=on NTPSER NTPEN
  wait a while and request the current date time:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
+ .../inverter-connect$ ./cli.py print-at-commands NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --ip             TEXT                     IP address of your inverter [required]              │
 │ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
 │                                              [required]                                          │
 │    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
```

### Comparing `inverter-connect-0.8.0/README.md` & `inverter-connect-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
 Usage: ./cli.py print-values [OPTIONS]
 
  Print all known register values from Inverter, e.g.:
- .../inverter-connect$ ./cli.py print-values 192.168.123.456
+ .../inverter-connect$ ./cli.py print-values
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --ip             TEXT                     IP address of your inverter [required]              │
 │ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
 │                                              [required]                                          │
 │ *  --inverter       TEXT                     Prefix of yaml config files in                      │
 │                                              inverter/definitions/                               │
@@ -158,23 +158,22 @@
 
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
 Usage: ./cli.py print-at-commands [OPTIONS] [COMMANDS]...
 
  Print one or more AT command values from Inverter.
  Use all known AT commands, if no one is given, e.g.:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
+ .../inverter-connect$ ./cli.py print-at-commands
  Or specify one or more AT-commands, e.g.:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER .../inverter-connect$
- ./cli.py print-at-commands 192.168.123.456 WEBVER WEBU
+ .../inverter-connect$ ./cli.py print-at-commands WEBVER .../inverter-connect$ ./cli.py
+ print-at-commands WEBVER WEBU
  e.g.: Set NTP server, enable NTP and check the values:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
- NTPSER NTPEN
+ .../inverter-connect$ ./cli.py print-at-commands NTPSER=192.168.1.1 NTPEN=on NTPSER NTPEN
  wait a while and request the current date time:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
+ .../inverter-connect$ ./cli.py print-at-commands NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --ip             TEXT                     IP address of your inverter [required]              │
 │ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
 │                                              [required]                                          │
 │    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
```

### Comparing `inverter-connect-0.8.0/cli.py` & `inverter-connect-0.9.0/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/dev-cli.py` & `inverter-connect-0.9.0/dev-cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/.github/workflows/tests.yml` & `inverter-connect-0.9.0/inverter/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/api.py` & `inverter-connect-0.9.0/inverter/api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/cli/cli_app.py` & `inverter-connect-0.9.0/inverter/cli/cli_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 """
     CLI for usage
 """
-
+import atexit
+import datetime
+import locale
 import logging
 import sys
 import time
 from pathlib import Path
 
 import rich_click
 import rich_click as click
 from bx_py_utils.path import assert_is_file
 from ha_services.mqtt4homeassistant.mqtt import get_connected_client
 from ha_services.systemd.api import ServiceControl
 from ha_services.toml_settings.api import TomlSettings
 from ha_services.toml_settings.exceptions import UserSettingsNotFound
 from rich import get_console, print  # noqa
-from rich.console import Console
+from rich.pretty import pprint
 from rich.table import Table
 from rich.traceback import install as rich_traceback_install
 from rich_click import RichGroup
 
 import inverter
 from inverter import constants
 from inverter.api import Inverter, fetch_inverter_versions, set_current_time
 from inverter.connection import InverterSock
-from inverter.constants import ERROR_STR_NO_DATA, SETTINGS_DIR_NAME, SETTINGS_FILE_NAME
-from inverter.data_types import InverterRegisterVersionInfo, Parameter, ValueType
+from inverter.constants import SETTINGS_DIR_NAME, SETTINGS_FILE_NAME
+from inverter.data_types import InverterRegisterVersionInfo
 from inverter.exceptions import ReadInverterError
 from inverter.publish_loop import publish_forever
 from inverter.user_settings import SystemdServiceInfo, UserSettings, make_config, migrate_old_settings
-from inverter.utilities.cli import convert_address_option, print_inverter_versions, print_register
+from inverter.utilities.cli import (
+    convert_address_option,
+    print_inverter_values,
+    print_inverter_versions,
+    print_register,
+)
 from inverter.verbosity import OPTION_KWARGS_VERBOSE, setup_logging
 
 
 logger = logging.getLogger(__name__)
 
 
 PACKAGE_ROOT = Path(inverter.__file__).parent.parent
@@ -239,15 +246,15 @@
 @click.option('--port', **option_kwargs_port)
 @click.option('--inverter', **option_kwargs_inverter_name)
 @click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
 def print_values(ip, port, inverter, verbosity: int):
     """
     Print all known register values from Inverter, e.g.:
 
-    .../inverter-connect$ ./cli.py print-values 192.168.123.456
+    .../inverter-connect$ ./cli.py print-values
     """
     setup_logging(verbosity=verbosity)
 
     print()
 
     config = make_config(
         user_settings=user_settings,
@@ -260,35 +267,23 @@
     with Inverter(config=config) as inverter:
         try:
             inverter.connect()
         except ReadInverterError as err:
             print(f'[red]{err}')
             sys.exit(1)
 
+        print('Fetch', end='...')
+        values = []
         for value in inverter:
-            print(f'\t* [yellow]{value.name:<31}[/yellow]:', end=' ')
-            if value.value == ERROR_STR_NO_DATA:
-                color = 'red'
-                msg = ERROR_STR_NO_DATA
-            else:
-                color = 'green'
-                msg = f'{value.value} {value.unit}'
-            print(f'[{color}]{msg:<11}[/{color}]', end=' ')
-
-            if value.type == ValueType.READ_OUT:
-                parameter: Parameter = value.result.parameter
-                print(
-                    f'(Register: [cyan]{parameter.start_register:04X}[/cyan], length:'
-                    f' [blue]{parameter.length}[/blue])'
-                )
-            elif value.type == ValueType.COMPUTED:
-                print('(Computed)')
+            print(f'[yellow]{value.name}[/yellow],', end='')
+            values.append(value)
 
-            if verbosity:
-                print()
+    if verbosity > 1:
+        pprint(values)
+    print_inverter_values(values)
 
 
 cli.add_command(print_values)
 
 
 @click.command()
 @click.argument('commands', nargs=-1)
@@ -297,28 +292,28 @@
 @click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
 def print_at_commands(ip, port, commands, verbosity: int):
     """
     Print one or more AT command values from Inverter.
 
     Use all known AT commands, if no one is given, e.g.:
 
-    .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
+    .../inverter-connect$ ./cli.py print-at-commands
 
     Or specify one or more AT-commands, e.g.:
 
-    .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER
-    .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER WEBU
+    .../inverter-connect$ ./cli.py print-at-commands WEBVER
+    .../inverter-connect$ ./cli.py print-at-commands WEBVER WEBU
 
     e.g.: Set NTP server, enable NTP and check the values:
 
-    .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on NTPSER NTPEN
+    .../inverter-connect$ ./cli.py print-at-commands NTPSER=192.168.1.1 NTPEN=on NTPSER NTPEN
 
     wait a while and request the current date time:
 
-    .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
+    .../inverter-connect$ ./cli.py print-at-commands NTPTM
 
     (Note: The prefix "AT+" will be added to every command)
     """
     setup_logging(verbosity=verbosity)
 
     if not commands:
         commands = (
@@ -382,14 +377,17 @@
         results = []
         for command in commands:
             print(f'[yellow]{command}', end='')
             result: str = inv_sock.cleaned_at_command(command)
             results.append(dict(command=command, result=result))
             print(',', end='')
 
+    if verbosity > 1:
+        pprint(results)
+
     console = get_console()
     console.print('\n')
     console.rule()
 
     table = Table(title='AT-command results')
     table.add_column('Counter', justify='right')
     table.add_column('Command', justify='right')
@@ -591,21 +589,29 @@
     except KeyboardInterrupt:
         print('Bye, bye')
 
 
 cli.add_command(publish_loop)
 
 
+def exit_func():
+    console = get_console()
+    console.rule(datetime.datetime.now().strftime('%c'))
+
+
 def main():
     print(f'[bold][green]{inverter.__name__}[/green] v[cyan]{inverter.__version__}')
+    locale.setlocale(locale.LC_ALL, '')
 
-    console = Console()
+    console = get_console()
     rich_traceback_install(
         width=console.size.width,  # full terminal width
         show_locals=True,
         suppress=[click, rich_click],
         max_frames=2,
     )
 
+    atexit.register(exit_func)
+
     # Execute Click CLI:
     cli.name = './cli.py'
     cli()
```

### Comparing `inverter-connect-0.8.0/inverter/cli/dev.py` & `inverter-connect-0.9.0/inverter/cli/dev.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/connection.py` & `inverter-connect-0.9.0/inverter/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,19 +204,19 @@
         data = data.decode()
         data = data.split(',')
         self.inverter_info = InverterInfo(ip=data[0], mac=data[1], serial=int(data[2]))
 
         print(self.inverter_info)
         print()
 
+    @backoff.on_exception(backoff.expo, ReadTimeout, **BACKOFF_DEFAULTS)
     def connect(self) -> None:
-        assert self.sock is None
         logger.info(f'Connect to {self.config.host}:{self.config.port}...')
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
-        self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        # self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.sock.settimeout(self.config.socket_timeout)
 
         self.init_inventer()
 
     def send(self, *, command: bytes):
         if self.config.verbosity > 1:
             print(f'send: {command}', end='...', flush=True)
```

### Comparing `inverter-connect-0.8.0/inverter/daily_reset.py` & `inverter-connect-0.9.0/inverter/daily_reset.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/data_types.py` & `inverter-connect-0.9.0/inverter/data_types.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/definitions/deye_2mppt.yaml` & `inverter-connect-0.9.0/inverter/definitions/deye_2mppt.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -135,7 +135,15 @@
       class: ""
       state_class: ""
       uom: ""
       scale: 1
       rule: 5
       registers: [0x0003,0x0004,0x0005,0x0006,0x0007]
       isstr: true
+
+    - name: "Power factor"
+      class: ""
+      state_class: "measurement"
+      uom: "%"
+      scale: 1
+      rule: 1
+      registers: [0x0028]
```

### Comparing `inverter-connect-0.8.0/inverter/definitions.py` & `inverter-connect-0.9.0/inverter/definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/exceptions.py` & `inverter-connect-0.9.0/inverter/exceptions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/publish_loop.py` & `inverter-connect-0.9.0/inverter/publish_loop.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/tests/fixtures.py` & `inverter-connect-0.9.0/inverter/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/tests/test_api.py` & `inverter-connect-0.9.0/inverter/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/tests/test_cli.py` & `inverter-connect-0.9.0/inverter/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/tests/test_connect.py` & `inverter-connect-0.9.0/inverter/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/tests/test_daily_reset.py` & `inverter-connect-0.9.0/inverter/tests/test_daily_reset.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/tests/test_definitions.py` & `inverter-connect-0.9.0/inverter/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/tests/test_project_setup.py` & `inverter-connect-0.9.0/inverter/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/tests/test_readme.py` & `inverter-connect-0.9.0/inverter/tests/test_readme.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,19 @@
     def test_cli_mock(self):
         assert_no_color_env(width=TERM_WIDTH)
         assert_subprocess_rich_diagnose_no_color(width=TERM_WIDTH)
         assert_rich_no_color(width=TERM_WIDTH)
         assert_rich_click_no_color(width=TERM_WIDTH)
 
     def invoke_cli(self, *args):
-        return self.cli_mock.invoke(cli_bin=PACKAGE_ROOT / 'cli.py', args=args, strip_line_prefix='Usage: ')
+        stdout = self.cli_mock.invoke(cli_bin=PACKAGE_ROOT / 'cli.py', args=args, strip_line_prefix='Usage: ')
+
+        # Remove last line:
+        stdout = '\n'.join(stdout.splitlines()[:-1])
+        return stdout.rstrip()
 
     def invoke_dev_cli(self, *args):
         return self.cli_mock.invoke(cli_bin=PACKAGE_ROOT / 'dev-cli.py', args=args, strip_line_prefix='Usage: ')
 
     def test_main_help(self):
         stdout = self.invoke_cli('--help')
         assert_in(
```

### Comparing `inverter-connect-0.8.0/inverter/tests/test_user_settings.py` & `inverter-connect-0.9.0/inverter/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/tests/test_validators.py` & `inverter-connect-0.9.0/inverter/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/user_settings.py` & `inverter-connect-0.9.0/inverter/user_settings.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/utilities/cli.py` & `inverter-connect-0.9.0/inverter/utilities/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 
 from bx_py_utils.iteration import chunk_iterable
 from rich import get_console, print  # noqa
 from rich.table import Table
 
-from inverter.data_types import InverterRegisterVersionResult, ModbusResponse
+from inverter.constants import ERROR_STR_NO_DATA
+from inverter.data_types import InverterRegisterVersionResult, InverterValue, ModbusResponse, Parameter, ValueType
 from inverter.exceptions import ModbusNoData, ModbusNoHexData
 
 
 def convert_address_option(raw_address: str, debug: bool = True) -> int:
     """
     >>> convert_address_option(raw_address='0x123', debug=True)
     Address: 0x123
@@ -88,7 +89,48 @@
             f'v{result.version}',  # Human readable version
         )
 
     console = get_console()
     console.print('\n')
     console.rule()
     console.print(table)
+
+
+def print_inverter_values(values: list[InverterValue], title='Inverter Values'):
+    table = Table(title=title)
+
+    table.add_column('Counter', justify='right')
+    table.add_column('Name', justify='right')
+    table.add_column('Value', justify='left')
+    table.add_column('Register', justify='center')
+    table.add_column('Length', justify='center')
+    table.add_column('Raw data', justify='right')
+
+    for offset, value in enumerate(values):
+        if value.value == ERROR_STR_NO_DATA:
+            value_str = f'[red]{ERROR_STR_NO_DATA}'
+        else:
+            value_str = f'[green]{value.value:>12} [blue]{value.unit}'
+
+        if value.type == ValueType.READ_OUT:
+            parameter: Parameter = value.result.parameter
+            register_str = f'[cyan]{parameter.start_register:04X}'
+            length_str = f'{parameter.length}'
+            raw_data_str = value.result.response.data_hex
+        else:
+            register_str = '-'
+            length_str = '-'
+            raw_data_str = '(Computed)'
+
+        table.add_row(
+            str(offset + 1),  # Counter
+            f'[blue]{value.name}',
+            value_str,
+            register_str,
+            length_str,
+            raw_data_str,
+        )
+
+    console = get_console()
+    console.print('\n')
+    console.rule()
+    console.print(table)
```

### Comparing `inverter-connect-0.8.0/inverter/utilities/modbus_converter.py` & `inverter-connect-0.9.0/inverter/utilities/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/validators.py` & `inverter-connect-0.9.0/inverter/validators.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter/verbosity.py` & `inverter-connect-0.9.0/inverter/verbosity.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/inverter_connect.egg-info/PKG-INFO` & `inverter-connect-0.9.0/inverter_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.8.0
+Version: 0.9.0
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -135,15 +135,15 @@
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
 Usage: ./cli.py print-values [OPTIONS]
 
  Print all known register values from Inverter, e.g.:
- .../inverter-connect$ ./cli.py print-values 192.168.123.456
+ .../inverter-connect$ ./cli.py print-values
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --ip             TEXT                     IP address of your inverter [required]              │
 │ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
 │                                              [required]                                          │
 │ *  --inverter       TEXT                     Prefix of yaml config files in                      │
 │                                              inverter/definitions/                               │
@@ -170,23 +170,22 @@
 
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
 Usage: ./cli.py print-at-commands [OPTIONS] [COMMANDS]...
 
  Print one or more AT command values from Inverter.
  Use all known AT commands, if no one is given, e.g.:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
+ .../inverter-connect$ ./cli.py print-at-commands
  Or specify one or more AT-commands, e.g.:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER .../inverter-connect$
- ./cli.py print-at-commands 192.168.123.456 WEBVER WEBU
+ .../inverter-connect$ ./cli.py print-at-commands WEBVER .../inverter-connect$ ./cli.py
+ print-at-commands WEBVER WEBU
  e.g.: Set NTP server, enable NTP and check the values:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
- NTPSER NTPEN
+ .../inverter-connect$ ./cli.py print-at-commands NTPSER=192.168.1.1 NTPEN=on NTPSER NTPEN
  wait a while and request the current date time:
- .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
+ .../inverter-connect$ ./cli.py print-at-commands NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --ip             TEXT                     IP address of your inverter [required]              │
 │ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
 │                                              [required]                                          │
 │    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
```

### Comparing `inverter-connect-0.8.0/inverter_connect.egg-info/SOURCES.txt` & `inverter-connect-0.9.0/inverter_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/pyproject.toml` & `inverter-connect-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/requirements.dev.txt` & `inverter-connect-0.9.0/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.8.0/requirements.txt` & `inverter-connect-0.9.0/requirements.txt`

 * *Files identical despite different names*

