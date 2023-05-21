# Comparing `tmp/agentic-0.0.1.tar.gz` & `tmp/Agentic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentic-0.0.1.tar", last modified: Sun Apr 16 16:01:38 2023, max compression
+gzip compressed data, was "Agentic-0.0.2.tar", last modified: Sun May 21 11:21:57 2023, max compression
```

## Comparing `agentic-0.0.1.tar` & `Agentic-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 willempienaar   (501) staff       (20)        0 2023-04-16 16:01:38.568600 agentic-0.0.1/
--rw-r--r--   0 willempienaar   (501) staff       (20)      181 2023-04-16 16:01:38.568471 agentic-0.0.1/PKG-INFO
--rw-r--r--   0 willempienaar   (501) staff       (20)       52 2023-04-16 16:01:38.000000 agentic-0.0.1/README.md
-drwxr-xr-x   0 willempienaar   (501) staff       (20)        0 2023-04-16 16:01:38.568338 agentic-0.0.1/agentic.egg-info/
--rw-r--r--   0 willempienaar   (501) staff       (20)      181 2023-04-16 16:01:38.000000 agentic-0.0.1/agentic.egg-info/PKG-INFO
--rw-r--r--   0 willempienaar   (501) staff       (20)      153 2023-04-16 16:01:38.000000 agentic-0.0.1/agentic.egg-info/SOURCES.txt
--rw-r--r--   0 willempienaar   (501) staff       (20)        1 2023-04-16 16:01:38.000000 agentic-0.0.1/agentic.egg-info/dependency_links.txt
--rw-r--r--   0 willempienaar   (501) staff       (20)        8 2023-04-16 16:01:38.000000 agentic-0.0.1/agentic.egg-info/top_level.txt
--rw-r--r--   0 willempienaar   (501) staff       (20)       26 2023-04-16 16:01:38.000000 agentic-0.0.1/agentic.py
--rw-r--r--   0 willempienaar   (501) staff       (20)       38 2023-04-16 16:01:38.568655 agentic-0.0.1/setup.cfg
--rw-r--r--   0 willempienaar   (501) staff       (20)      227 2023-04-16 16:01:38.000000 agentic-0.0.1/setup.py
+drwxr-xr-x   0 willempienaar   (501) staff       (20)        0 2023-05-21 11:21:57.914514 Agentic-0.0.2/
+drwxr-xr-x   0 willempienaar   (501) staff       (20)        0 2023-05-21 11:21:57.914084 Agentic-0.0.2/Agentic.egg-info/
+-rw-r--r--   0 willempienaar   (501) staff       (20)      441 2023-05-21 11:21:57.000000 Agentic-0.0.2/Agentic.egg-info/PKG-INFO
+-rw-r--r--   0 willempienaar   (501) staff       (20)      162 2023-05-21 11:21:57.000000 Agentic-0.0.2/Agentic.egg-info/SOURCES.txt
+-rw-r--r--   0 willempienaar   (501) staff       (20)        1 2023-05-21 11:21:57.000000 Agentic-0.0.2/Agentic.egg-info/dependency_links.txt
+-rw-r--r--   0 willempienaar   (501) staff       (20)        8 2023-05-21 11:21:57.000000 Agentic-0.0.2/Agentic.egg-info/top_level.txt
+-rw-r--r--   0 willempienaar   (501) staff       (20)      441 2023-05-21 11:21:57.914363 Agentic-0.0.2/PKG-INFO
+-rw-r--r--   0 willempienaar   (501) staff       (20)      252 2023-04-29 20:56:28.000000 Agentic-0.0.2/README.md
+drwxr-xr-x   0 willempienaar   (501) staff       (20)        0 2023-05-21 11:21:57.914203 Agentic-0.0.2/agentic/
+-rw-r--r--   0 willempienaar   (501) staff       (20)       32 2023-05-21 11:21:20.000000 Agentic-0.0.2/agentic/__init__.py
+-rw-r--r--   0 willempienaar   (501) staff       (20)       38 2023-05-21 11:21:57.914553 Agentic-0.0.2/setup.cfg
+-rw-r--r--   0 willempienaar   (501) staff       (20)      596 2023-05-21 11:21:42.000000 Agentic-0.0.2/setup.py
```

