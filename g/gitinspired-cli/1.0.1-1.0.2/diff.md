# Comparing `tmp/gitinspired-cli-1.0.1.tar.gz` & `tmp/gitinspired-cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitinspired-cli-1.0.1.tar", last modified: Thu May 18 16:03:34 2023, max compression
+gzip compressed data, was "gitinspired-cli-1.0.2.tar", last modified: Sun May 21 10:33:28 2023, max compression
```

## Comparing `gitinspired-cli-1.0.1.tar` & `gitinspired-cli-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-18 16:03:34.823591 gitinspired-cli-1.0.1/
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)     1078 2023-05-18 15:12:54.000000 gitinspired-cli-1.0.1/LICENSE
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      162 2023-05-18 16:03:34.823591 gitinspired-cli-1.0.1/PKG-INFO
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      163 2023-05-18 15:56:52.000000 gitinspired-cli-1.0.1/README.md
-drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-18 16:03:34.823591 gitinspired-cli-1.0.1/gitinspired_cli.egg-info/
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      162 2023-05-18 16:03:34.000000 gitinspired-cli-1.0.1/gitinspired_cli.egg-info/PKG-INFO
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      299 2023-05-18 16:03:34.000000 gitinspired-cli-1.0.1/gitinspired_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        1 2023-05-18 16:03:34.000000 gitinspired-cli-1.0.1/gitinspired_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)       56 2023-05-18 16:03:34.000000 gitinspired-cli-1.0.1/gitinspired_cli.egg-info/entry_points.txt
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        9 2023-05-18 16:03:34.000000 gitinspired-cli-1.0.1/gitinspired_cli.egg-info/requires.txt
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        4 2023-05-18 16:03:34.000000 gitinspired-cli-1.0.1/gitinspired_cli.egg-info/top_level.txt
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)       38 2023-05-18 16:03:34.823591 gitinspired-cli-1.0.1/setup.cfg
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      298 2023-05-18 16:01:57.000000 gitinspired-cli-1.0.1/setup.py
-drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-18 16:03:34.823591 gitinspired-cli-1.0.1/src/
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        0 2023-05-18 15:26:18.000000 gitinspired-cli-1.0.1/src/__init__.py
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      318 2023-05-18 15:47:27.000000 gitinspired-cli-1.0.1/src/greetings_cli.py
+drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-21 10:33:28.862757 gitinspired-cli-1.0.2/
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)     1078 2023-05-18 15:12:54.000000 gitinspired-cli-1.0.2/LICENSE
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      162 2023-05-21 10:33:28.862757 gitinspired-cli-1.0.2/PKG-INFO
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      156 2023-05-18 16:04:24.000000 gitinspired-cli-1.0.2/README.md
+drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-21 10:33:28.862757 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      162 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      319 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        1 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)       56 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        9 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/requires.txt
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        4 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/top_level.txt
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)       38 2023-05-21 10:33:28.862757 gitinspired-cli-1.0.2/setup.cfg
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      298 2023-05-21 10:33:18.000000 gitinspired-cli-1.0.2/setup.py
+drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-21 10:33:28.862757 gitinspired-cli-1.0.2/src/
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        0 2023-05-18 15:26:18.000000 gitinspired-cli-1.0.2/src/__init__.py
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      861 2023-05-21 10:30:23.000000 gitinspired-cli-1.0.2/src/file_manager.py
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      779 2023-05-21 10:31:53.000000 gitinspired-cli-1.0.2/src/greetings_cli.py
```

### Comparing `gitinspired-cli-1.0.1/LICENSE` & `gitinspired-cli-1.0.2/LICENSE`

 * *Files identical despite different names*

