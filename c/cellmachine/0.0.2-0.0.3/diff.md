# Comparing `tmp/cellmachine-0.0.2.tar.gz` & `tmp/cellmachine-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmachine-0.0.2.tar", last modified: Tue Jun 21 14:45:19 2022, max compression
+gzip compressed data, was "cellmachine-0.0.3.tar", max compression
```

## Comparing `cellmachine-0.0.2.tar` & `cellmachine-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,5 @@
-drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 14:45:19.859187 cellmachine-0.0.2/
--rw-r--r--   0 189741     (502) staff       (20)    35149 2022-06-21 01:57:50.000000 cellmachine-0.0.2/LICENSE
--rw-r--r--   0 189741     (502) staff       (20)     6179 2022-06-21 14:45:19.859042 cellmachine-0.0.2/PKG-INFO
--rw-r--r--   0 189741     (502) staff       (20)     5615 2022-06-21 14:43:54.000000 cellmachine-0.0.2/README.md
--rw-r--r--   0 189741     (502) staff       (20)      636 2022-06-21 14:44:20.000000 cellmachine-0.0.2/pyproject.toml
--rw-r--r--   0 189741     (502) staff       (20)       38 2022-06-21 14:45:19.859223 cellmachine-0.0.2/setup.cfg
-drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 14:45:19.857244 cellmachine-0.0.2/src/
-drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 14:45:19.858196 cellmachine-0.0.2/src/cellmachine/
--rw-r--r--   0 189741     (502) staff       (20)     3880 2022-06-21 14:43:56.000000 cellmachine-0.0.2/src/cellmachine/__init__.py
-drwxr-xr-x   0 189741     (502) staff       (20)        0 2022-06-21 14:45:19.858853 cellmachine-0.0.2/src/cellmachine.egg-info/
--rw-r--r--   0 189741     (502) staff       (20)     6179 2022-06-21 14:45:19.000000 cellmachine-0.0.2/src/cellmachine.egg-info/PKG-INFO
--rw-r--r--   0 189741     (502) staff       (20)      216 2022-06-21 14:45:19.000000 cellmachine-0.0.2/src/cellmachine.egg-info/SOURCES.txt
--rw-r--r--   0 189741     (502) staff       (20)        1 2022-06-21 14:45:19.000000 cellmachine-0.0.2/src/cellmachine.egg-info/dependency_links.txt
--rw-r--r--   0 189741     (502) staff       (20)       12 2022-06-21 14:45:19.000000 cellmachine-0.0.2/src/cellmachine.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2023-05-21 11:46:07.141865 cellmachine-0.0.3/LICENSE
+-rw-r--r--   0        0        0       60 2023-05-21 11:46:07.141865 cellmachine-0.0.3/README.md
+-rw-r--r--   0        0        0      341 2023-05-21 11:46:07.141865 cellmachine-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-05-21 11:46:07.141865 cellmachine-0.0.3/src/cellmachine/__init__.py
+-rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 cellmachine-0.0.3/PKG-INFO
```

### Comparing `cellmachine-0.0.2/LICENSE` & `cellmachine-0.0.3/LICENSE`

 * *Files identical despite different names*

