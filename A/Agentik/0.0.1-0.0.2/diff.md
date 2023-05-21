# Comparing `tmp/agentik-0.0.1.tar.gz` & `tmp/Agentik-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentik-0.0.1.tar", last modified: Sun Apr 16 15:59:01 2023, max compression
+gzip compressed data, was "Agentik-0.0.2.tar", last modified: Sun May 21 11:20:12 2023, max compression
```

## Comparing `agentik-0.0.1.tar` & `Agentik-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 willempienaar   (501) staff       (20)        0 2023-04-16 15:59:01.428145 agentik-0.0.1/
--rw-r--r--   0 willempienaar   (501) staff       (20)      181 2023-04-16 15:59:01.428013 agentik-0.0.1/PKG-INFO
--rw-r--r--   0 willempienaar   (501) staff       (20)       52 2023-04-16 15:59:00.000000 agentik-0.0.1/README.md
-drwxr-xr-x   0 willempienaar   (501) staff       (20)        0 2023-04-16 15:59:01.427857 agentik-0.0.1/agentik.egg-info/
--rw-r--r--   0 willempienaar   (501) staff       (20)      181 2023-04-16 15:59:01.000000 agentik-0.0.1/agentik.egg-info/PKG-INFO
--rw-r--r--   0 willempienaar   (501) staff       (20)      153 2023-04-16 15:59:01.000000 agentik-0.0.1/agentik.egg-info/SOURCES.txt
--rw-r--r--   0 willempienaar   (501) staff       (20)        1 2023-04-16 15:59:01.000000 agentik-0.0.1/agentik.egg-info/dependency_links.txt
--rw-r--r--   0 willempienaar   (501) staff       (20)        8 2023-04-16 15:59:01.000000 agentik-0.0.1/agentik.egg-info/top_level.txt
--rw-r--r--   0 willempienaar   (501) staff       (20)       26 2023-04-16 15:59:00.000000 agentik-0.0.1/agentik.py
--rw-r--r--   0 willempienaar   (501) staff       (20)       38 2023-04-16 15:59:01.428183 agentik-0.0.1/setup.cfg
--rw-r--r--   0 willempienaar   (501) staff       (20)      227 2023-04-16 15:59:00.000000 agentik-0.0.1/setup.py
+drwxr-xr-x   0 willempienaar   (501) staff       (20)        0 2023-05-21 11:20:12.478504 Agentik-0.0.2/
+drwxr-xr-x   0 willempienaar   (501) staff       (20)        0 2023-05-21 11:20:12.478098 Agentik-0.0.2/Agentik.egg-info/
+-rw-r--r--   0 willempienaar   (501) staff       (20)      441 2023-05-21 11:20:12.000000 Agentik-0.0.2/Agentik.egg-info/PKG-INFO
+-rw-r--r--   0 willempienaar   (501) staff       (20)      162 2023-05-21 11:20:12.000000 Agentik-0.0.2/Agentik.egg-info/SOURCES.txt
+-rw-r--r--   0 willempienaar   (501) staff       (20)        1 2023-05-21 11:20:12.000000 Agentik-0.0.2/Agentik.egg-info/dependency_links.txt
+-rw-r--r--   0 willempienaar   (501) staff       (20)        8 2023-05-21 11:20:12.000000 Agentik-0.0.2/Agentik.egg-info/top_level.txt
+-rw-r--r--   0 willempienaar   (501) staff       (20)      441 2023-05-21 11:20:12.478366 Agentik-0.0.2/PKG-INFO
+-rw-r--r--   0 willempienaar   (501) staff       (20)       28 2023-05-21 11:19:21.000000 Agentik-0.0.2/README.md
+drwxr-xr-x   0 willempienaar   (501) staff       (20)        0 2023-05-21 11:20:12.478215 Agentik-0.0.2/agentik/
+-rw-r--r--   0 willempienaar   (501) staff       (20)       32 2023-05-21 11:17:57.000000 Agentik-0.0.2/agentik/__init__.py
+-rw-r--r--   0 willempienaar   (501) staff       (20)       38 2023-05-21 11:20:12.478541 Agentik-0.0.2/setup.cfg
+-rw-r--r--   0 willempienaar   (501) staff       (20)      596 2023-05-21 11:19:07.000000 Agentik-0.0.2/setup.py
```

