# Comparing `tmp/yambs-1.3.1.tar.gz` & `tmp/yambs-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.3.1.tar", last modified: Thu May 18 23:49:31 2023, max compression
+gzip compressed data, was "yambs-1.4.0.tar", last modified: Sun May 21 20:47:00 2023, max compression
```

## Comparing `yambs-1.3.1.tar` & `yambs-1.4.0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.103654 yambs-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 23:48:19.000000 yambs-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-18 23:49:31.103654 yambs-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-18 23:48:19.000000 yambs-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-18 23:48:19.000000 yambs-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:49:31.103654 yambs-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-18 23:48:19.000000 yambs-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-18 23:48:19.000000 yambs-1.3.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-18 23:48:19.000000 yambs-1.3.1/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/includes/chips.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/schemas/Toolchain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.103654 yambs-1.3.1/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.103654 yambs-1.3.1/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/ninja.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.103654 yambs-1.3.1/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.698827 yambs-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 20:45:50.000000 yambs-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-21 20:47:00.698827 yambs-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-21 20:45:50.000000 yambs-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-21 20:45:50.000000 yambs-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 20:47:00.698827 yambs-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-21 20:45:50.000000 yambs-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.690827 yambs-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-21 20:45:50.000000 yambs-1.4.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-21 20:45:50.000000 yambs-1.4.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.694827 yambs-1.4.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.694827 yambs-1.4.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.694827 yambs-1.4.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/config/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.694827 yambs-1.4.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.694827 yambs-1.4.0/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/includes/microchip.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.694827 yambs-1.4.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/schemas/Toolchain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.698827 yambs-1.4.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.698827 yambs-1.4.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/generate/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/generate/ninja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.698827 yambs-1.4.0/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-21 20:45:50.000000 yambs-1.4.0/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:47:00.694827 yambs-1.4.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-21 20:47:00.000000 yambs-1.4.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-21 20:47:00.000000 yambs-1.4.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 20:47:00.000000 yambs-1.4.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-21 20:47:00.000000 yambs-1.4.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-21 20:47:00.000000 yambs-1.4.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 20:47:00.000000 yambs-1.4.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.3.1/LICENSE` & `yambs-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/PKG-INFO` & `yambs-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.3.1
+Version: 1.4.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=ef7f414918ad82f1abad57ff15edbd1b
+    hash=8ce3ed1dcaa2a9870cee9cc7a0216adf
     =====================================
 -->
 
-# yambs ([1.3.1](https://pypi.org/project/yambs/))
+# yambs ([1.4.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.3.1/README.md` & `yambs-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=ef7f414918ad82f1abad57ff15edbd1b
+    hash=8ce3ed1dcaa2a9870cee9cc7a0216adf
     =====================================
 -->
 
-# yambs ([1.3.1](https://pypi.org/project/yambs/))
+# yambs ([1.4.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.3.1/pyproject.toml` & `yambs-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.3.1"
+version = "1.4.0"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.3.1/setup.py` & `yambs-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/tests/test_entry.py` & `yambs-1.4.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/yambs/app.py` & `yambs-1.4.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/yambs/commands/all.py` & `yambs-1.4.0/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/yambs/commands/gen.py` & `yambs-1.4.0/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/yambs/commands/uf2conv.py` & `yambs-1.4.0/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/yambs/config/__init__.py` & `yambs-1.4.0/yambs/config/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
 A module implementing a configuration interface for the package.
 """
 
 # built-in
 from pathlib import Path
+from typing import Any, Dict, Iterator, Tuple
 
 # third-party
 from vcorelib.dict import merge
 from vcorelib.dict.codec import BasicDictCodec as _BasicDictCodec
 from vcorelib.io import ARBITER as _ARBITER
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.paths import Pathlike, find_file
 
 # internal
 from yambs import PKG_NAME
+from yambs.config.board import Board
 from yambs.schemas import YambsDictCodec as _YambsDictCodec
 
 
 class Config(_YambsDictCodec, _BasicDictCodec):
     """The top-level configuration object for the package."""
 
+    data: Dict[str, Any]
+
     def init(self, data: _JsonObject) -> None:
         """Initialize this instance."""
 
         self.data = data
         self.root = Path()
 
     def directory(self, name: str, mkdir: bool = True) -> Path:
@@ -34,14 +38,22 @@
             name_root = self.root.joinpath(name_root)
 
         if mkdir:
             name_root.mkdir(parents=True, exist_ok=True)
 
         return name_root
 
+    def boards(self) -> Iterator[Tuple[Board, Dict[str, Any]]]:
+        """Iterate over boards."""
+
+        for board in self.data["boards"]:
+            yield Board.from_dict(
+                board, self.data["architectures"], self.data["chips"]
+            ), board
+
 
 def load(path: Pathlike) -> Config:
     """Load a configuration."""
 
     src_config = find_file(f"{PKG_NAME}.yaml", package=PKG_NAME)
     assert src_config is not None
```

### Comparing `yambs-1.3.1/yambs/data/includes/chips.yaml` & `yambs-1.4.0/yambs/data/includes/microchip.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,25 @@
 ---
 chips:
-  # Memory Map (Reference Manual sect. 7.3, p. 370):
-  #
-  # 24 MHz clock (default), 144 MHz max.
-  #
-  # - BROM (PMU ROM)       0x 0000 0000 (0x      4000,  16 Kb)
-  # - PMU/FLASH (cached)   0x 0800 0000 (0x   20 0000,   2 Mb)
-  # - PMU/FLASH (uncached) 0x 0C00 0000
-  # - PSRAM (code)         0x 1FFE 8000 (0x    1 8000,  96 Kb)
-  # - DSRAM1 (system)      0x 2000 0000 (0x    2 0000, 128 Kb)
-  # - DSRAM2 (comm)        0x 2002 0000 (0x    2 0000, 128 Kb)
-  #
-  # See p. 2825 for a flow diagram for startup modes.
-  xmc4700-2048:
-    architecture: armv7e-m+fp
-    cpu: cortex-m4
-    jlink: XMC4700-2048
-    linker:
-      symbols:
-        __flash: "0x08000000"
-        __flash_size: "0x00200000"
-        __ram: "0x20000000"
-        __ram_size: "0x00020000"
-        __stack_size: "1k"
-
-  # Memory Map (Data Sheet sect. 9.2 p. 53):
-  #
   # 48 MHz clock (default), 120 MHz max.
-  #
-  # - Embedded Flash      0x 0000 0000 (  1 Mb)
-  # - Embedded SRAM       0x 2000 0000 (256 Kb)
-  # - Peripheral Bridge A 0x 4000 0000 ( 16 Kb)
-  # - Peripheral Bridge B 0x 4100 0000 ( 16 Kb)
-  # - Peripheral Bridge C 0x 4200 0000 ( 16 Kb)
-  # - Peripheral Bridge D 0x 4300 0000 ( 16 Kb)
-  # - Backup SRAM         0x 4700 0000 (  8 Kb)
-  # - NVM User Row        0x 0080 4000 (512  b)
-  #
   # See p. 46 for a power domain block diagram.
   atsamd51x20:
     architecture: armv7e-m+fp
     cpu: cortex-m4
-    jlink: ATSAMD51P20A
+    jlink: [ATSAMD51P20A]
+    uf2_family: SAMD51
     linker:
       symbols:
+        # Memory Map (Data Sheet sect. 9.2 p. 53):
+        # - Embedded Flash      0x 0000 0000 (  1 Mb)
+        # - Embedded SRAM       0x 2000 0000 (256 Kb)
+        # - Peripheral Bridge A 0x 4000 0000 ( 16 Kb)
+        # - Peripheral Bridge B 0x 4100 0000 ( 16 Kb)
+        # - Peripheral Bridge C 0x 4200 0000 ( 16 Kb)
+        # - Peripheral Bridge D 0x 4300 0000 ( 16 Kb)
+        # - Backup SRAM         0x 4700 0000 (  8 Kb)
+        # - NVM User Row        0x 0080 4000 (512  b)
         __flash: "0x00000000"
         __flash_size: "0x00100000"
         __ram: "0x20000000"
         __ram_size: "0x00040000"
         __stack_size: "1k"
```

### Comparing `yambs-1.3.1/yambs/data/schemas/Chip.yaml` & `yambs-1.4.0/yambs/data/schemas/Chip.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -5,23 +5,30 @@
 
 properties:
   architecture:
     type: string
   cpu:
     type: string
 
+  uf2_family:
+    type: string
+    default: ""
+
   extra_cflags:
     type: array
     default: []
     items:
       type: string
 
   # The '-device' argument for use with the Segger J-Link.
   jlink:
-    type: string
+    type: array
+    default: []
+    items:
+      type: string
 
   linker:
     type: object
     additionalProperties: false
     required: [symbols]
 
     properties:
```

### Comparing `yambs-1.3.1/yambs/data/schemas/Config.yaml` & `yambs-1.4.0/yambs/data/schemas/Config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -57,10 +57,10 @@
 
   cc:
     type: string
     default: gcc
 
   common_cflags:
     type: array
-    default: [-Wall, -Werror, -g]
+    default: [-Wall, -g]
     items:
       type: string
```

### Comparing `yambs-1.3.1/yambs/data/templates/rules.ninja.j2` & `yambs-1.4.0/yambs/data/templates/rules.ninja.j2`

 * *Files 8% similar despite different names*

```diff
@@ -16,25 +16,23 @@
 tool = ${toolchain_prefix}{{cc}}
 
 rule cc
   depfile = $out.d
   deps = gcc
   command = $tool -MD -MF $out.d $cflags -c $in -o $out
 
-ldflags = -T$include_dir/chips/$chip/chip.ld
-
 rule link
-  command = $tool $cflags $ldflags -Wl,-Map=$out.map $in -o $out
+  command = $tool $cflags $board_ldflags -Wl,-Map=$out.map $in -o $out
 
 rule bin
   command = ${toolchain_prefix}objcopy -O binary $in $out
 
 rule hex
   command = ${toolchain_prefix}objcopy -O ihex $in $out
 
 rule dump
   command = ${toolchain_prefix}objdump -D $in > $out
 
 rule uf2
-  command = mbs uf2conv -o $out $in
+  command = mbs uf2conv $uf2conv_args -o $out $in
 
 build_dir = {{build_root}}/$toolchain/$architecture/$cpu
```

### Comparing `yambs-1.3.1/yambs/data/uf2families.json` & `yambs-1.4.0/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/yambs/entry.py` & `yambs-1.4.0/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/yambs/generate/__init__.py` & `yambs-1.4.0/yambs/generate/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 A module for generating templated outputs.
 """
 
 # third-party
 from datazen.templates import environment
 from jinja2 import FileSystemLoader
+from vcorelib.io import ARBITER
 from vcorelib.paths import resource
 
 # internal
 from yambs import PKG_NAME
 from yambs.config import Config
 from yambs.generate.architectures import generate as generate_architectures
 from yambs.generate.boards import generate as generate_boards
@@ -31,13 +32,17 @@
     # generated into the root directory.
     render_template(jinja, config.root, "build.ninja", config.data)
 
     ninja_root = config.directory("ninja_out")
 
     # Generate all other files.
     for gen in [
-        generate_boards,
         generate_chips,
         generate_toolchains,
         generate_architectures,
     ]:
         gen(jinja, ninja_root, config)
+
+    ARBITER.encode(
+        ninja_root.joinpath("board_apps.json"),
+        generate_boards(jinja, ninja_root, config),
+    )
```

### Comparing `yambs-1.3.1/yambs/generate/architectures.py` & `yambs-1.4.0/yambs/generate/architectures.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from yambs.config import Config
 from yambs.generate.common import render_template
 
 
 def generate(jinja: Environment, ninja_root: Path, config: Config) -> None:
     """Generate architecture-related ninja files."""
 
-    for name, data in config.data["architectures"].items():  # type: ignore
+    for name, data in config.data["architectures"].items():
         architectures_root = ninja_root.joinpath("architectures", name)
         architectures_root.mkdir(parents=True, exist_ok=True)
 
         render_template(
             jinja,
             architectures_root,
             "architecture.ninja",
-            data,  # type: ignore
+            data,
         )
```

### Comparing `yambs-1.3.1/yambs/generate/boards.py` & `yambs-1.4.0/yambs/generate/boards.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,152 +1,178 @@
 """
 A module for generating board-related files.
 """
 
 # built-in
+from logging import getLogger
 from os import linesep
 from pathlib import Path
 from typing import Any, Dict, Set, TextIO, Tuple
 
 # third-party
 from jinja2 import Environment
 from vcorelib.paths import rel
 
 # internal
 from yambs.config import Config
-from yambs.generate.common import render_template
+from yambs.config.board import Board
+from yambs.generate.common import is_source, render_template
 from yambs.generate.ninja import (
     write_link_line,
     write_phony,
     write_source_line,
 )
 
-
-def is_source(path: Path) -> bool:
-    """Determine if a file is a source file."""
-
-    return path.name.endswith(".c") or path.name.endswith(".cc")
+LOG = getLogger(__name__)
 
 
 def add_dir(
     stream: TextIO,
     paths: Set[Path],
     path: Path,
     comment: str,
     base: Path,
     current_sources: Set[Path],
-    board: str = None,
+    board: Board,
+    board_specific: bool = False,
 ) -> None:
     """Add a directory to set of paths."""
 
-    print(f"{comment}: checking '{path}' for sources.")
+    LOG.debug("%s: checking '%s' for sources.", comment, path)
+
     if path.is_dir():
         stream.write(linesep + f"# {comment}." + linesep)
         for item in path.iterdir():
             if is_source(item):
                 paths.add(
                     write_source_line(
-                        stream, item, base, current_sources, board=board
+                        stream,
+                        item,
+                        base,
+                        current_sources,
+                        board,
+                        board_specific=board_specific,
                     )
                 )
 
 
-def create_paths_dict(
-    root: Path, board: Dict[str, Any], config: Config
-) -> Dict[str, Any]:
+def create_paths_dict(root: Path, board: Board) -> Dict[str, Any]:
     """Create paths based on common pathing conventions."""
 
-    chip = config.data["chips"][board["chip"]]  # type: ignore
+    chip = board.chip
 
     return {
         "Common": root.joinpath("common"),
-        "Chip": root.joinpath("chips", board["chip"]),
-        "Architecture": root.joinpath(chip["architecture"]),  # type: ignore
-        "CPU": root.joinpath(chip["cpu"]),  # type: ignore
-        "Board": root.joinpath("boards", board["name"]),
+        "Chip": root.joinpath("chips", chip.name),
+        "Architecture": root.joinpath(chip.architecture.name),
+        "CPU": root.joinpath(chip.cpu),
+        "Board": root.joinpath("boards", board.name),
     }
 
 
 def write_sources(
     stream: TextIO,
-    board: Dict[str, Any],
-    config: Config,
+    board: Board,
     src_root: Path,
     global_sources: Set[Path],
 ) -> Tuple[Set[Path], Set[Path]]:
     """Write the source-file manifest."""
 
     # Add regular sources.
     all_srcs: Set[Path] = set()
 
-    for kind, path in create_paths_dict(src_root, board, config).items():
+    for kind, path in create_paths_dict(src_root, board).items():
         add_dir(
             stream,
             all_srcs,
             path,
             f"{kind} sources",
             src_root,
             global_sources,
+            board,
+        )
+
+    # Add any extra sources this board specified.
+    for extra in board.extra_dirs:
+        add_dir(
+            stream,
+            all_srcs,
+            src_root.joinpath("third-party", extra),
+            "extra sources",
+            src_root,
+            global_sources,
+            board,
         )
 
     # Add application sources.
     app_srcs: Set[Path] = set()
     for kind, path in create_paths_dict(
-        src_root.joinpath("apps"), board, config
+        src_root.joinpath("apps"), board
     ).items():
         add_dir(
             stream,
             app_srcs,
             path,
             f"{kind} application sources",
             src_root,
             global_sources,
-            board=board["name"],
+            board,
+            # Avoid having a redundant directory in the path when the source
+            # directory is already the board-specific one.
+            board_specific="boards" not in str(path),
         )
 
     return all_srcs, app_srcs
 
 
-def generate(jinja: Environment, ninja_root: Path, config: Config) -> None:
+def generate(
+    jinja: Environment,
+    ninja_root: Path,
+    config: Config,
+) -> Dict[str, Any]:
     """Generate board-related ninja files."""
 
+    board_apps: Dict[str, Any] = {}
+
     # Render the board manifest and rules file.
     for template in ["all.ninja", "rules.ninja"]:
         render_template(jinja, ninja_root, template, config.data)
 
     src_root = rel(config.directory("src_root"))
 
-    # Render board top-level files.
-    board: Dict[str, Any] = {}
-
     # Keep track of all overall sources, so that no duplicate rules are
     # generated.
     global_sources: Set[Path] = set()
 
-    for board in config.data["boards"]:  # type: ignore
-        board_root = ninja_root.joinpath("boards", board["name"])
+    for board, raw_data in config.boards():
+        board_root = ninja_root.joinpath("boards", board.name)
         board_root.mkdir(parents=True, exist_ok=True)
-        render_template(jinja, board_root, "board.ninja", board)
+        render_template(jinja, board_root, "board.ninja", raw_data)
 
         # Perform source-file discovery.
         with board_root.joinpath("sources.ninja").open("w") as path_fd:
             path_fd.write(f"src_dir = {config.data['src_root']}" + linesep)
 
             all_srcs, app_srcs = write_sources(
-                path_fd, board, config, src_root, global_sources
+                path_fd, board, src_root, global_sources
             )
 
-        print(
-            (
-                f"({board['name']}) Found {len(all_srcs)} "
-                f"sources and {len(app_srcs)} applications."
-            )
+        LOG.info(
+            "(%s) Found %d sources and %d applications.",
+            board.name,
+            len(all_srcs),
+            len(app_srcs),
         )
 
+        # Keep track of each board's applications.
+        board_apps[board.name] = list(str(x) for x in app_srcs)
+
         # Write the application manifest.
         with board_root.joinpath("apps.ninja").open("w") as path_fd:
             for app_src in app_srcs:
                 write_link_line(path_fd, app_src, all_srcs, src_root)
 
             # Write the phony target.
             path_fd.write("# A target to build all applications." + linesep)
-            write_phony(path_fd, app_srcs, src_root, board["name"])
+            write_phony(path_fd, app_srcs, src_root, board.name)
+
+    return board_apps
```

### Comparing `yambs-1.3.1/yambs/generate/chips.py` & `yambs-1.4.0/yambs/generate/chips.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 from yambs.config import Config
 from yambs.generate.common import render_template
 
 
 def generate(jinja: Environment, ninja_root: Path, config: Config) -> None:
     """Generate chip-related ninja files."""
 
-    for name, data in config.data["chips"].items():  # type: ignore
+    for name, data in config.data["chips"].items():
         chips_root = ninja_root.joinpath("chips", name)
         chips_root.mkdir(parents=True, exist_ok=True)
 
         # Render chip files and linker scripts.
         render_template(
             jinja,
             chips_root,
             "chip.ninja",
-            data,  # type: ignore
+            data,
         )
         render_template(
             jinja,
             chips_root,
             "chip.ld",
-            data["linker"],  # type: ignore
+            data["linker"],
         )
```

### Comparing `yambs-1.3.1/yambs/generate/ninja.py` & `yambs-1.4.0/yambs/generate/ninja.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,31 +3,37 @@
 """
 
 # built-in
 from os import linesep
 from pathlib import Path
 from typing import Set, TextIO
 
+# internal
+from yambs.config.board import Board
+
 
 def write_source_line(
     stream: TextIO,
     source: Path,
     base: Path,
     current_sources: Set[Path],
-    board: str = None,
+    board: Board,
+    board_specific: bool = False,
 ) -> Path:
     """Write a ninja configuration line for a source file."""
 
     dest = source
-    if board is not None:
-        dest = source.parent.joinpath(board, source.name)
+    if board_specific:
+        dest = source.parent.joinpath(board.name, source.name)
+
+    build_loc = board.build.joinpath(dest)
 
     # Don't generate any duplicate compilation rules.
-    if dest not in current_sources:
-        current_sources.add(dest)
+    if build_loc not in current_sources:
+        current_sources.add(build_loc)
 
         stream.write(
             (
                 f"build $build_dir/"
                 f"{dest.relative_to(base).with_suffix('.o')}: "
                 f"cc $src_dir/{source.relative_to(base)}"
             )
```

### Comparing `yambs-1.3.1/yambs/generate/toolchains.py` & `yambs-1.4.0/yambs/generate/toolchains.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from yambs.config import Config
 from yambs.generate.common import render_template
 
 
 def generate(jinja: Environment, ninja_root: Path, config: Config) -> None:
     """Generate toolchain-related ninja files."""
 
-    for name, data in config.data["toolchains"].items():  # type: ignore
+    for name, data in config.data["toolchains"].items():
         toolchains_root = ninja_root.joinpath("toolchains", name)
         toolchains_root.mkdir(parents=True, exist_ok=True)
 
         render_template(
             jinja,
             toolchains_root,
             "toolchain.ninja",
-            data,  # type: ignore
+            data,
         )
```

### Comparing `yambs-1.3.1/yambs/schemas.py` & `yambs-1.4.0/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/yambs/uf2/__init__.py` & `yambs-1.4.0/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.1/yambs.egg-info/PKG-INFO` & `yambs-1.4.0/yambs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.3.1
+Version: 1.4.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=ef7f414918ad82f1abad57ff15edbd1b
+    hash=8ce3ed1dcaa2a9870cee9cc7a0216adf
     =====================================
 -->
 
-# yambs ([1.3.1](https://pypi.org/project/yambs/))
+# yambs ([1.4.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.3.1/yambs.egg-info/SOURCES.txt` & `yambs-1.4.0/yambs.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,20 @@
 yambs.egg-info/requires.txt
 yambs.egg-info/top_level.txt
 yambs/commands/__init__.py
 yambs/commands/all.py
 yambs/commands/gen.py
 yambs/commands/uf2conv.py
 yambs/config/__init__.py
+yambs/config/board.py
 yambs/data/uf2families.json
 yambs/data/yambs.yaml
 yambs/data/includes/chips.yaml
+yambs/data/includes/infineon.yaml
+yambs/data/includes/microchip.yaml
 yambs/data/schemas/Architecture.yaml
 yambs/data/schemas/Board.yaml
 yambs/data/schemas/Chip.yaml
 yambs/data/schemas/Config.yaml
 yambs/data/schemas/Toolchain.yaml
 yambs/data/templates/all.ninja.j2
 yambs/data/templates/architecture.ninja.j2
```

