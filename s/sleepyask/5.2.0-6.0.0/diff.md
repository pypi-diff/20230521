# Comparing `tmp/sleepyask-5.2.0.tar.gz` & `tmp/sleepyask-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyask-5.2.0.tar", last modified: Sat May 13 02:43:52 2023, max compression
+gzip compressed data, was "C:\Users\nocet\OneDrive\Documents\Projects\one_thing\naggingGPT\dist\.tmp-57ovnsc3\sleepyask-6.0.0.tar", last modified: Sun May 21 07:51:55 2023, max compression
```

## Comparing `sleepyask-5.2.0.tar` & `sleepyask-6.0.0.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:43:52.804676 sleepyask-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-13 02:43:35.000000 sleepyask-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-13 02:43:52.804676 sleepyask-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-13 02:43:35.000000 sleepyask-5.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-13 02:43:35.000000 sleepyask-5.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 02:43:52.804676 sleepyask-5.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:43:52.800676 sleepyask-5.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:43:52.800676 sleepyask-5.2.0/src/sleepyask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:43:52.804676 sleepyask-5.2.0/src/sleepyask/openai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 02:43:35.000000 sleepyask-5.2.0/src/sleepyask/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-13 02:43:35.000000 sleepyask-5.2.0/src/sleepyask/openai/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-13 02:43:35.000000 sleepyask-5.2.0/src/sleepyask/openai/chatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:43:52.800676 sleepyask-5.2.0/src/sleepyask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-13 02:43:52.000000 sleepyask-5.2.0/src/sleepyask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-13 02:43:52.000000 sleepyask-5.2.0/src/sleepyask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 02:43:52.000000 sleepyask-5.2.0/src/sleepyask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-13 02:43:52.000000 sleepyask-5.2.0/src/sleepyask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-13 02:43:52.000000 sleepyask-5.2.0/src/sleepyask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 07:51:55.000000 sleepyask-6.0.0/
+-rw-rw-rw-   0        0        0      378 2023-05-21 07:51:55.000000 sleepyask-6.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-05-21 07:51:25.000000 sleepyask-6.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 07:51:55.000000 sleepyask-6.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/naggpt/
+-rw-rw-rw-   0        0        0        0 2023-05-19 08:52:03.000000 sleepyask-6.0.0/src/naggpt/__init__.py
+-rw-rw-rw-   0        0        0     2515 2023-05-21 07:44:34.000000 sleepyask-6.0.0/src/naggpt/nag.py
+drwxrwxrwx   0        0        0        0 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 07:51:55.000000 sleepyask-6.0.0/src/sleepyask.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sleepyask-5.2.0/pyproject.toml` & `sleepyask-6.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "sleepyask"
-version = "5.2.0"
-authors = [
-  { name="hwelsters", email="redacted@redacted.redacted" },
-]
-description = "A small tool for automating collecting data from ChatGPT"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = []
-dependencies = [
-  'openai >= 0.27.2',
-  'fasteners >= 0.18'
-]
-
-[project.urls]
-"Homepage" = "https://github.com/hwelsters/sleepyask"
-"Bug Tracker" = "https://github.com/hwelsters/sleepyask/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "sleepyask"
+version = "6.0.0"
+authors = [
+  { name="hwelsters", email="redacted@redacted.redacted" },
+]
+description = "A small tool for automating collecting data from ChatGPT"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = []
+dependencies = [
+  'openai-async>=0.0.3'
+]
+
+[project.urls]
+"Homepage" = "https://github.com/hwelsters/sleepyask"
+"Bug Tracker" = "https://github.com/hwelsters/sleepyask/issues"
```

