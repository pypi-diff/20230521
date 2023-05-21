# Comparing `tmp/talondoc-0.5.1.tar.gz` & `tmp/talondoc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talondoc-0.5.1.tar", last modified: Thu May 18 12:54:39 2023, max compression
+gzip compressed data, was "talondoc-0.6.0.tar", last modified: Sun May 21 20:48:56 2023, max compression
```

## Comparing `talondoc-0.5.1.tar` & `talondoc-0.6.0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-18 12:54:26.000000 talondoc-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-18 12:54:39.178819 talondoc-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-18 12:54:26.000000 talondoc-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-18 12:54:26.000000 talondoc-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:54:39.178819 talondoc-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 12:54:26.000000 talondoc-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.170819 talondoc-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/_autogen/
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/_autogen/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/conf.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/index.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/index.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/python_file.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/python_file.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/talon_file.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/talon_file.rst.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/_cache_builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_cache_builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_util/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_util/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/analysis/live/
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/analysis/live/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_captures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    36057 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/talon_actions_dict-0.3.1-437-g8fea.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/analysis/registry/
--rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/analysis/registry/data/
--rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/registry/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/registry/data/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/registry/data/serialise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/analysis/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/analysis/static/python/
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/static/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/static/python/shims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/static/talon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/description/
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/description/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/description/describer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/sphinx/_util/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/_util/addnodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/_util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/sphinx/directives/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/capture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/sphinx/directives/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/command/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/command/hlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/command/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.210946 talondoc-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-21 20:48:42.000000 talondoc-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-21 20:48:56.210946 talondoc-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-21 20:48:42.000000 talondoc-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-21 20:48:42.000000 talondoc-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 20:48:56.210946 talondoc-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 20:48:42.000000 talondoc-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.198946 talondoc-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/_autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/_autogen/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/conf.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/index.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/index.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/python_file.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/python_file.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/talon_file.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_autogen/resources/talon_file.rst.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/_cache_builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_cache_builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/_cache_builtin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    38478 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_cache_builtin/resources/talon.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_util/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_util/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc/analysis/live/
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/analysis/live/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_captures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/live/resources/get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/analysis/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/analysis/registry/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/registry/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/registry/data/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/registry/data/serialise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/analysis/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/analysis/static/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/static/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21613 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/static/python/shims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/analysis/static/talon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/description/
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/description/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/description/describer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/sphinx/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/_util/addnodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/_util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.206946 talondoc-0.6.0/src/talondoc/sphinx/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/capture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.210946 talondoc-0.6.0/src/talondoc/sphinx/directives/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/command/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/command/hlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/command/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/directives/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-21 20:48:42.000000 talondoc-0.6.0/src/talondoc/sphinx/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:48:56.202946 talondoc-0.6.0/src/talondoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 20:48:56.000000 talondoc-0.6.0/src/talondoc.egg-info/top_level.txt
```

### Comparing `talondoc-0.5.1/PKG-INFO` & `talondoc-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talondoc
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Sphinx extension for Talon user directories.
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 Keywords: talon,sphinx
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `talondoc-0.5.1/README.md` & `talondoc-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `talondoc-0.5.1/pyproject.toml` & `talondoc-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talondoc"
-version = "0.5.1"
+version = "0.6.0"
 description = "A Sphinx extension for Talon user directories."
 license = { file = 'LICENSE' }
 authors = [{ name = "Wen Kokke", email = "wenkokke@users.noreply.github.com" }]
 readme = "README.md"
 keywords = ["talon", "sphinx"]
 classifiers = [
   "License :: OSI Approved :: MIT License",
@@ -25,15 +25,16 @@
   "editdistance >=0.6,<0.7",
   "Jinja2 >=3,<4",
   "Sphinx >=5,<8",
   "talonfmt >=1.7.4,<2",
   "tree_sitter_talon >=3!1.0,<3!2",
   "colorlog >=6.7,<7",
   "packaging >=23.1,<24",
-  'pywin32;platform_system=="Windows"',
+  'pywin32; platform_system=="Windows"',
+  "singledispatchmethod >=1.0,<2; python_version <'3.8'",
 ]
 
 [project.optional-dependencies]
 mypy = [
   "types_click",
   "types_docutils",
   "types_editdistance",
@@ -53,15 +54,15 @@
   "sphinx_tabs >=3.4,<5"
 ]
 
 [project.scripts]
 talondoc = "talondoc:talondoc"
 
 [tool.bumpver]
-current_version = "0.5.1"
+current_version = "0.6.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
@@ -74,55 +75,34 @@
 
 [tool.isort]
 profile = "black"
 line_length = 88
 
 [tool.mypy]
 python_version = 3.9
-check_untyped_defs = true
-strict_optional = true
+strict = true
 ignore_missing_imports = true
-warn_redundant_casts = true
-warn_unused_ignores = false
-warn_no_return = true
-warn_return_any = true
-warn_unreachable = true
 implicit_reexport = false
-strict_concatenate = true
-strict_equality = true
-# disallow_untyped_calls = true
-# disallow_untyped_defs = true
-# disallow_incomplete_defs = true
-disallow_untyped_decorators = true
+warn_unused_ignores = false
 
 [tool.pytest.ini_options]
 enable_assertion_pass_hook = true
 filterwarnings = ["ignore::DeprecationWarning:.*:"]
 minversion = "6.0"
 testpaths = ["tests"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py39-md, py39-rst, py310-md, py310-rst, py311-md, py311-rst
+envlist = py39, py39-md, py310, py310-md, py311, py311-md
 isolated_build = true
 
-[md]
-description = Tests TalonDoc with Markdown
-setenv =
-  TALONDOC_FORMAT = md
-
-[rst]
-description = Tests TalonDoc with reStructuredText
-setenv =
-  TALONDOC_FORMAT = md
-
 [testenv]
 allowlist_externals = cp, mkdir, sh, rm
 extras =
   test
 setenv =
   TALONDOC_STRICT = 1
 commands_pre =
@@ -139,24 +119,18 @@
   rm -f '{env_tmp_dir}/build.sh'
   rm -rf '{env_tmp_dir}/knausj_talon'
   rm -f '{env_tmp_dir}/docs/conf.py'
   rm -f '{env_tmp_dir}/docs/index.md'
   rm -rf '{env_tmp_dir}/docs/_static'
 
 [testenv:py39-md]
-setenv = {[md]setenv}
+setenv =
+  TALONDOC_FORMAT = md
 
 [testenv:py310-md]
-setenv = {[md]setenv}
+setenv =
+  TALONDOC_FORMAT = md
 
 [testenv:py311-md]
-setenv = {[md]setenv}
-
-[testenv:py39-rst]
-setenv = {[rst]setenv}
-
-[testenv:py310-rst]
-setenv = {[rst]setenv}
-
-[testenv:py311-rst]
-setenv = {[rst]setenv}
+setenv =
+  TALONDOC_FORMAT = md
 """
```

### Comparing `talondoc-0.5.1/src/talondoc/__init__.py` & `talondoc-0.6.0/src/talondoc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     version=__version__,
 )
 @click.option(
     "--log-level",
     type=click.Choice(["ERROR", "WARNING", "INFO", "DEBUG"], case_sensitive=False),
     default="INFO",
 )
-def talondoc(*, log_level: Literal["ERROR", "WARNING", "INFO", "DEBUG"]):
+def talondoc(*, log_level: Literal["ERROR", "WARNING", "INFO", "DEBUG"]) -> None:
     logging.basicConfig(
         level={
             "ERROR": logging.ERROR,
             "WARNING": logging.WARNING,
             "INFO": logging.INFO,
             "DEBUG": logging.DEBUG,
         }.get(log_level.upper(), logging.INFO),
@@ -121,15 +121,15 @@
     project: Optional[str],
     author: Optional[str],
     release: Optional[str],
     generate_conf: bool,
     generate_index: bool,
     continue_on_error: bool,
     format: Literal["rst", "md"],
-):
+) -> None:
     autogen(
         package_dir,
         output_dir=output_dir,
         sphinx_root=sphinx_root,
         template_dir=template_dir,
         package_name=package_name,
         include=tuple(include),
@@ -148,13 +148,13 @@
 @talondoc.command(name="cache_builtin")
 @click.argument(
     "output_dir",
     type=click.Path(),
 )
 def _cache_builtin(
     output_dir: str,
-):
+) -> None:
     cache_builtin(output_dir=output_dir)
 
 
 if __name__ == "__main__":
     talondoc()
```

### Comparing `talondoc-0.5.1/src/talondoc/_autogen/__init__.py` & `talondoc-0.6.0/src/talondoc/_autogen/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import os
 import subprocess
+from collections.abc import Sequence
 from pathlib import Path
 from typing import Optional, Union
 
 import jinja2
 import jinja2.sandbox
 from typing_extensions import Literal
 
@@ -37,25 +38,25 @@
 def autogen(
     package_dir: Union[str, Path],
     *,
     package_name: Optional[str] = None,
     sphinx_root: Union[None, str, Path] = None,
     output_dir: Union[None, str, Path] = None,
     template_dir: Union[None, str, Path] = None,
-    include: tuple[str, ...] = (),
-    exclude: tuple[str, ...] = (),
-    trigger: tuple[str, ...] = (),
+    include: Sequence[str] = (),
+    exclude: Sequence[str] = (),
+    trigger: Sequence[str] = (),
     project: Optional[str] = None,
     author: Optional[str] = None,
     release: Optional[str] = None,
     generate_conf: bool = True,
     generate_index: bool = True,
     continue_on_error: bool = True,
     format: Literal["md", "rst"] = "rst",
-):
+) -> None:
     # Set defaults for arguments
     if isinstance(package_dir, str):
         package_dir = Path(package_dir)
     package_name = _default_package_name(package_name, package_dir)
     if isinstance(sphinx_root, str):
         sphinx_root = Path(sphinx_root)
     if isinstance(output_dir, str):
@@ -93,15 +94,15 @@
         include=include,
         exclude=exclude,
         trigger=trigger,
         show_progress=True,
         continue_on_error=continue_on_error,
     )
     assert package_name in registry.packages
-    package = registry.get(data.Package, package_name)
+    package: data.Package = registry.get(data.Package, package_name)
 
     # Make package path relative to output_dir:
     package_path = Path(os.path.relpath(package.location.path, start=sphinx_root))
 
     ctx = {
         "project": project,
         "author": author,
@@ -123,24 +124,30 @@
     total: int = len(package.files)
     if generate_conf:
         total += 1
     if generate_index:
         total += 1
     bar = ProgressBar(total=total)
     for file_name in package.files:
-        file = registry.get(data.File, file_name, referenced_by=package)
+        file: data.File = registry.get(data.File, file_name, referenced_by=package)
         # Create path/to/talon/file.{md,rst}:
         if file.location.path.suffix == ".talon":
             bar.step(f" {str(file.location.path)}")
             output_relpath = file.location.path.with_suffix(f".{format}")
             toc.append(output_relpath)
             output_path = output_dir / output_relpath
             output_path.parent.mkdir(parents=True, exist_ok=True)
+            command_names: set[str] = set()
+            for context_name in file.contexts:
+                context = registry.get(data.Context, context_name)
+                command_names.update(context.commands)
             output_path.write_text(
-                template_talon_file.render(file_name=file_name, **ctx)
+                template_talon_file.render(
+                    file_name=file_name, command_names=command_names, **ctx
+                )
             )
 
         # Create path/to/python/file/api.{md,rst}:
         elif file.location.path.suffix == ".py":
             bar.step(f" {str(file.location.path)}")
             output_relpath = file.location.path.with_suffix("") / f"api.{format}"
             toc.append(output_relpath)
```

### Comparing `talondoc-0.5.1/src/talondoc/_autogen/resources/conf.py.jinja2` & `talondoc-0.6.0/src/talondoc/_autogen/resources/conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `talondoc-0.5.1/src/talondoc/_cache_builtin/__init__.py` & `talondoc-0.6.0/src/talondoc/_cache_builtin/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from typing import Mapping
+from collections.abc import Mapping
 
 from .._util.logging import getLogger
 from ..analysis.live import TalonRepl
 
 _LOGGER = getLogger(__name__)
 
 
@@ -14,11 +14,11 @@
         _LOGGER.info(f"Found Talon {version}")
         _LOGGER.info(f"Getting builtin declarations...")
         builtin = repl.builtin_registry.to_dict()
         if isinstance(builtin, Mapping):
             for cls, objs in builtin.items():
                 if isinstance(objs, Mapping):
                     _LOGGER.info(f"Found {len(objs)} {cls.lower()}s")
-        output_path = os.path.join(output_dir, f"talon-{version}.json")
+        output_path = os.path.join(output_dir, f"talon.json")
         with open(output_path, "w") as f:
             json.dump(builtin, f)
         _LOGGER.info(f"Wrote {output_path}")
```

### Comparing `talondoc-0.5.1/src/talondoc/_util/io.py` & `talondoc-0.6.0/src/talondoc/_util/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import io
 import queue
 import threading
-from typing import Callable, Iterator, Optional
+from collections.abc import Callable, Iterator
+from typing import Optional
 
 
 class NonBlockingTextIOWrapper:
     _stream: io.TextIOWrapper
     _queue: queue.Queue[str]
     _daemon: threading.Thread
```

### Comparing `talondoc-0.5.1/src/talondoc/_util/logging.py` & `talondoc-0.6.0/src/talondoc/_util/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from logging import basicConfig as basicConfig  # type: ignore[no-redef]
 else:
     from colorlog import basicConfig as basicConfig  # type: ignore[no-redef]
 
 if "sphinx" not in sys.modules:
     import colorlog
 
-    class PrettyColoredFormatter(colorlog.ColoredFormatter):
+    class PrettyColoredFormatter(colorlog.ColoredFormatter):  # type: ignore[misc]
         def format(self, record: LogRecord) -> str:
             if record.levelno == INFO:
                 return record.getMessage()
             else:
                 return super().format(record)  # type: ignore[no-any-return]
 
     _FORMATTER = PrettyColoredFormatter(
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/live/__init__.py` & `talondoc-0.6.0/src/talondoc/analysis/live/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import importlib.resources
 import io
 import json
 import os
 import platform
 import subprocess
+from collections.abc import Sequence
 from contextlib import AbstractContextManager
-from functools import cached_property
 from importlib.resources import Resource
 from types import TracebackType
-from typing import Optional, Sequence
+from typing import Optional
 
 from packaging.version import Version
 from typing_extensions import Self
 
 from ..._util.io import NonBlockingTextIOWrapper
 from ..._util.logging import getLogger
 from ..registry import Registry, data
 
 _LOGGER = getLogger(__name__)
 
 
-class TalonRepl(AbstractContextManager):
+class TalonRepl(AbstractContextManager["TalonRepl"]):
     _session: Optional[subprocess.Popen[bytes]]
     _session_stdout: Optional[NonBlockingTextIOWrapper]
     _session_stderr: Optional[NonBlockingTextIOWrapper]
 
     @property
     def executable_path(self) -> str:
         if platform.system() == "Windows":
@@ -94,105 +94,105 @@
         self.close()
 
     def close(self) -> None:
         if self._session:
             self.eval("exit()")
             self._session.wait()
 
-    @cached_property
+    @property
     def version(self) -> Version:
         parts = self.eval_resource("get_version.py").split("-", maxsplit=3)
         pep440_version = parts[0]
         if len(parts) >= 2:
             pep440_version += f"b{parts[1]}"
         if len(parts) >= 3:
             pep440_version += f"+{parts[2]}"
         return Version(pep440_version)
 
-    @cached_property
+    @property
     def actions(self) -> Sequence[data.Action]:
         actions_json = self.eval_resource("get_actions.py")
         try:
             actions_fields = json.loads(actions_json)
         except json.JSONDecodeError as e:
             _LOGGER.error(e)
             return ()
         return tuple(map(data.Action.from_dict, actions_fields))
 
     @property
     def builtin_actions(self) -> Sequence[data.Action]:
         return tuple(filter(lambda action: action.builtin, self.actions))
 
-    @cached_property
+    @property
     def captures(self) -> Sequence[data.Capture]:
         captures_json = self.eval_resource("get_captures.py")
         try:
             captures_fields = json.loads(captures_json)
         except json.JSONDecodeError as e:
             _LOGGER.error(e)
             return ()
         return tuple(map(data.Capture.from_dict, captures_fields))
 
     @property
     def builtin_captures(self) -> Sequence[data.Capture]:
         return tuple(filter(lambda capture: capture.builtin, self.captures))
 
-    @cached_property
+    @property
     def commands(self) -> Sequence[data.Command]:
         commands_json = self.eval_resource("get_commands.py")
         try:
             commands_fields = json.loads(commands_json)
         except json.JSONDecodeError as e:
             _LOGGER.error(e)
             return ()
         return tuple(map(data.Command.from_dict, commands_fields))
 
-    @cached_property
+    @property
     def lists(self) -> Sequence[data.List]:
         lists_json = self.eval_resource("get_lists.py")
         try:
             lists_fields = json.loads(lists_json)
         except json.JSONDecodeError as e:
             _LOGGER.error(e)
             return ()
         return tuple(map(data.List.from_dict, lists_fields))
 
     @property
     def builtin_lists(self) -> Sequence[data.List]:
         return tuple(filter(lambda list: list.builtin, self.lists))
 
-    @cached_property
+    @property
     def settings(self) -> Sequence[data.Setting]:
         settings_json = self.eval_resource("get_settings.py")
         try:
             settings_fields = json.loads(settings_json)
         except json.JSONDecodeError as e:
             _LOGGER.error(e)
             return ()
         return tuple(map(data.Setting.from_dict, settings_fields))
 
     @property
     def builtin_settings(self) -> Sequence[data.Setting]:
         return tuple(filter(lambda setting: setting.builtin, self.settings))
 
-    @cached_property
+    @property
     def modes(self) -> Sequence[data.Mode]:
         modes_json = self.eval_resource("get_modes.py")
         try:
             modes_fields = json.loads(modes_json)
         except json.JSONDecodeError as e:
             _LOGGER.error(e)
             return ()
         return tuple(map(data.Mode.from_dict, modes_fields))
 
     @property
     def builtin_modes(self) -> Sequence[data.Mode]:
         return tuple(filter(lambda mode: mode.builtin, self.modes))
 
-    @cached_property
+    @property
     def tags(self) -> Sequence[data.Tag]:
         tags_json = self.eval_resource("get_tags.py")
         try:
             tags_fields = json.loads(tags_json)
         except json.JSONDecodeError as e:
             _LOGGER.error(e)
             return ()
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/live/resources/get_actions.py` & `talondoc-0.6.0/src/talondoc/analysis/live/resources/get_actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     def asdict_class(cls: type) -> typing.Optional[str]:
         if cls in (inspect.Signature.empty, inspect.Parameter.empty):
             return None
         if hasattr(cls, "__name__"):
             return cls.__name__
         return repr(cls)
 
-    def asdict_parameter(par: inspect.Parameter) -> typing.Dict:
+    def asdict_parameter(par: inspect.Parameter) -> typing.Dict[str, typing.Any]:
         return {
             "name": par.name,
             "kind": par.kind,
             "default": asdict_pickle(par.default),
             "annotation": asdict_class(par.annotation),
         }
 
-    def asdict_signature(sig: inspect.Signature) -> typing.Dict:
+    def asdict_signature(sig: inspect.Signature) -> typing.Dict[str, typing.Any]:
         return {
             "parameters": [asdict_parameter(par) for par in sig.parameters.values()],
             "return_annotation": asdict_class(sig.return_annotation),
         }
 
     for action_impls in talon.registry.actions.values():
         for action_impl in action_impls:
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/live/resources/get_captures.py` & `talondoc-0.6.0/src/talondoc/analysis/live/resources/get_captures.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     def asdict_class(cls: type) -> typing.Optional[str]:
         if cls in (inspect.Signature.empty, inspect.Parameter.empty):
             return None
         if hasattr(cls, "__name__"):
             return cls.__name__
         return repr(cls)
 
-    def asdict_parameter(par: inspect.Parameter) -> typing.Dict:
+    def asdict_parameter(par: inspect.Parameter) -> typing.Dict[str, typing.Any]:
         return {
             "name": par.name,
             "kind": par.kind,
             "default": asdict_pickle(par.default),
             "annotation": asdict_class(par.annotation),
         }
 
-    def asdict_signature(sig: inspect.Signature) -> typing.Dict:
+    def asdict_signature(sig: inspect.Signature) -> typing.Dict[str, typing.Any]:
         return {
             "parameters": [asdict_parameter(par) for par in sig.parameters.values()],
             "return_annotation": asdict_class(sig.return_annotation),
         }
 
     for capture_impls in talon.registry.captures.values():
         for capture_impl in capture_impls:
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/live/resources/get_commands.py` & `talondoc-0.6.0/src/talondoc/analysis/live/resources/get_commands.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.5.1/src/talondoc/analysis/live/resources/get_lists.py` & `talondoc-0.6.0/src/talondoc/analysis/live/resources/get_lists.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.5.1/src/talondoc/analysis/live/resources/get_settings.py` & `talondoc-0.6.0/src/talondoc/analysis/live/resources/get_settings.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.5.1/src/talondoc/analysis/registry/__init__.py` & `talondoc-0.6.0/src/talondoc/analysis/registry/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,52 @@
 import inspect
-from dataclasses import dataclass
+import itertools
+import json
+from collections.abc import Callable, Iterator, Mapping, Sequence
+from dataclasses import asdict, dataclass, fields
 from functools import singledispatchmethod
-from typing import (
-    Any,
-    Callable,
-    ClassVar,
-    Dict,
-    Iterator,
-    List,
-    Mapping,
-    Optional,
-    Sequence,
-    Union,
-    cast,
-    overload,
-)
+from typing import Any, ClassVar, Optional, Union, cast, overload
 
+import importlib_resources
+from more_itertools import partition
 from talonfmt import talonfmt
 from typing_extensions import Final
 
-from talondoc.analysis.registry.data.serialise import JsonValue
-
 from ..._util.logging import getLogger
 from . import data
 from .data import CallbackVar
 from .data.abc import (
     Data,
     DataVar,
     DuplicateData,
     GroupData,
     GroupDataHasFunction,
     GroupDataVar,
     SimpleData,
     SimpleDataVar,
     UnknownReference,
 )
+from .data.serialise import JsonValue, parse_dict, parse_list
 
 _LOGGER = getLogger(__name__)
 
 
 @dataclass
 class Registry:
-    _data: Final[Dict[str, Any]]
-    _temp_data: Final[Dict[str, Any]]
+    _data: Final[dict[str, Any]]
+    _temp_data: Final[dict[str, Any]]
 
     _active_package: Optional[data.Package] = None
     _active_file: Optional[data.File] = None
 
     def __init__(
         self,
         *,
-        data: Dict[str, Any] = {},
-        temp_data: Dict[str, Any] = {},
+        data: dict[str, Any] = {},
+        temp_data: dict[str, Any] = {},
         continue_on_error: bool = True,
     ):
         self._data = data
         self._temp_data = temp_data
         self._active_package = None
         self._active_file = None
         self._continue_on_error = continue_on_error
@@ -270,20 +261,26 @@
             value = cast(Optional[DataVar], self.lookup(cls, name))
             # For files, try various alternatives:
             if value is None and issubclass(cls, data.File):
                 value = cast(
                     Optional[DataVar],
                     # Try the search again with ".talon" suffixed:
                     self.lookup(cls, f"{name}.talon") or
+                    # Try the search again with ".py" suffixed:
+                    self.lookup(cls, f"{name}.py") or
                     # Try the search again assuming name is a path:
                     self.lookup(cls, f"user.{name.replace('/', '.')}"),
                 )
 
         elif issubclass(cls, GroupData):
-            value = cast(Optional[DataVar], self.lookup_default(cls, name))
+            declaration, defaults, others = self.lookup_partition(cls, name)
+            for obj in itertools.chain((declaration,), defaults, others):
+                if obj:
+                    value = cast(DataVar, obj)
+                    break
         elif issubclass(cls, data.Callback):
             raise ValueError(f"Registry.get does not support callbacks")
         if value is not None:
             return value
         else:
             raise UnknownReference(
                 cls,
@@ -301,106 +298,152 @@
         ...
 
     @overload
     def lookup(
         self,
         cls: type[GroupDataVar],
         name: str,
-    ) -> Optional[List[GroupDataVar]]:
+    ) -> Optional[list[GroupDataVar]]:
         ...
 
     @overload
     def lookup(
         self,
         cls: type[data.Callback],
         name: data.EventCode,
     ) -> Optional[Sequence[data.Callback]]:
         ...
 
     def lookup(self, cls: type[Data], name: Any) -> Optional[Any]:
         return self._typed_store(cls).get(self.resolve_name(name), None)
 
+    def lookup_default(
+        self, cls: type[GroupDataVar], name: str
+    ) -> Optional[GroupDataVar]:
+        declaration, default_overrides, _ = self.lookup_partition(cls, name)
+        return self._combine(cls, itertools.chain((declaration,), default_overrides))
+
+    def _combine(
+        self, cls: type[GroupDataVar], data: Iterator[Optional[GroupDataVar]]
+    ) -> Optional[GroupDataVar]:
+        init_keys: set[str] = {field.name for field in fields(cls) if field.init}
+        init_args: dict[str, Any] = {}
+        for datum in data:
+            if isinstance(datum, cls):
+                for name in init_keys:
+                    init_args[name] = init_args.get(name, getattr(datum, name))
+        if init_args:
+            return cls(**init_args)
+        else:
+            return None
+
     def lookup_description(self, cls: type[Data], name: Any) -> Optional[str]:
         if issubclass(cls, SimpleData):
             simple = self.lookup(cls, name)
             if simple:
                 return simple.description
         if issubclass(cls, GroupData):
-            group = self.lookup_default(cls, name)
-            if group:
-                return group.description
+            default = self.lookup_default(cls, name)
+            if default:
+                return default.description
         return None
 
-    def lookup_default(
-        self, cls: type[GroupDataVar], name: str
-    ) -> Optional[GroupDataVar]:
+    def lookup_partition(
+        self,
+        cls: type[GroupDataVar],
+        name: str,
+    ) -> tuple[Optional[GroupDataVar], Sequence[GroupDataVar], Sequence[GroupDataVar]]:
         group = self.lookup(cls, name)
         if group:
             _IS_DECLARATION: int = 0
             _IS_ALWAYS_ON: int = 1
 
             def _complexity(obj: GroupDataVar) -> int:
                 if issubclass(obj.parent_type, data.Module):
                     return _IS_DECLARATION
                 else:
-                    ctx = self.get(data.Context, obj.parent_name, referenced_by=obj)
-                    return _IS_ALWAYS_ON + len(ctx.matches)
+                    ctx = self.lookup(data.Context, obj.parent_name)
+                    if ctx is None:
+                        return _IS_ALWAYS_ON
+                    else:
+                        return _IS_ALWAYS_ON + len(ctx.matches)
 
+            # Sort all objects in the group by the complexity of their matches:
             sorted_group = [(_complexity(obj), obj) for obj in group]
             sorted_group.sort(key=lambda tup: tup[0])
-            declarations = [obj for c, obj in sorted_group if c == _IS_DECLARATION]
+
+            # Extract all declarations:
+            declarations_iter, overrides_iter = partition(
+                lambda tup: tup[0] != _IS_DECLARATION, sorted_group
+            )
+            declarations = tuple(declarations_iter)
             if len(declarations) >= 2:
-                _LOGGER.warning(DuplicateData(declarations))
-            return sorted_group[0][1]
-        return None
+                _LOGGER.warning(DuplicateData([tup[1] for tup in declarations]))
+            declaration = declarations[0][1] if len(declarations) >= 1 else None
+
+            # Extract all overrides that are always on:
+            default_overrides_iter, other_overrides_iter = partition(
+                lambda tup: tup[0] == _IS_ALWAYS_ON, overrides_iter
+            )
+
+            default_overrides = tuple((tup[1] for tup in default_overrides_iter))
+            other_overrides = tuple((tup[1] for tup in other_overrides_iter))
+            if len(default_overrides) >= 2:
+                # NOTE: We warn the user if there are multiple overrides which
+                #       are always on, but suppress this warning for commands.
+                if not issubclass(cls, data.Command):
+                    _LOGGER.warning(DuplicateData(default_overrides))
+            return (declaration, default_overrides, other_overrides)
+        return (None, (), ())
 
     def lookup_default_function(
         self, cls: type[GroupDataHasFunction], name: str
     ) -> Optional[Callable[..., Any]]:
-        value = self.lookup_default(cls, name)
-        if value and value.function_name:
-            function = self.lookup(data.Function, value.function_name)
+        # Find the default object:
+        default = self.lookup_default(cls, name)
+
+        # Find the associated function:
+        if default is not None and default.function_name is not None:
+            function = self.lookup(data.Function, default.function_name)
             if function is not None:
                 # Create copy for _function_wrapper
                 func = function.function
 
                 def _function_wrapper(*args: Any, **kwargs: Any) -> Any:
                     func_name = func.__name__
                     func_type = inspect.signature(func)
                     act_argc = len(args) + len(kwargs)
                     exp_argc = len(func_type.parameters)
                     if act_argc != exp_argc:
-                        act_argv: List[str] = []
+                        act_argv: list[str] = []
                         act_argv.extend(map(str, args))
                         act_argv.extend(f"{key}={val}" for key, val in kwargs.items())
                         _LOGGER.warning(
                             f"mismatch in number of parameters for {func_name}\n"
                             f"expected: {func_type}\n"
                             f"found: ({', '.join(act_argv)})"
                         )
                     return func(*args, **kwargs)
 
                 return _function_wrapper
-            else:
-                return None
         return None
 
     def resolve_name(self, name: str, *, package: Optional[data.Package] = None) -> str:
         try:
             if package is None:
                 package = self.get_active_package()
             parts = name.split(".")
             if len(parts) >= 1 and parts[0] == "self":
                 name = ".".join((package.name, *parts[1:]))
         except NoActivePackage:
             pass
         return name
 
     ######################################################################
-    # Typed Access To Data
+    # typed Access To Data
     ######################################################################
 
     @property
     def packages(self) -> Mapping[str, data.Package]:
         return self._typed_store(data.Package)
 
     @property
@@ -408,90 +451,137 @@
         return self._typed_store(data.File)
 
     @property
     def functions(self) -> Mapping[str, data.Function]:
         return self._typed_store(data.Function)
 
     @property
-    def callbacks(self) -> Mapping[data.EventCode, List[data.Callback]]:
+    def callbacks(self) -> Mapping[data.EventCode, list[data.Callback]]:
         return self._typed_store(data.Callback)
 
     @property
     def modules(self) -> Mapping[str, data.Module]:
         return self._typed_store(data.Module)
 
     @property
     def contexts(self) -> Mapping[str, data.Context]:
         return self._typed_store(data.Context)
 
     @property
-    def commands(self) -> Mapping[str, List[data.Command]]:
+    def commands(self) -> Mapping[str, list[data.Command]]:
         return self._typed_store(data.Command)
 
     @property
-    def actions(self) -> Mapping[str, List[data.Action]]:
+    def actions(self) -> Mapping[str, list[data.Action]]:
         return self._typed_store(data.Action)
 
     @property
-    def captures(self) -> Mapping[str, List[data.Capture]]:
+    def captures(self) -> Mapping[str, list[data.Capture]]:
         return self._typed_store(data.Capture)
 
     @property
-    def lists(self) -> Mapping[str, List[data.List]]:
+    def lists(self) -> Mapping[str, list[data.List]]:
         return self._typed_store(data.List)
 
     @property
-    def settings(self) -> Mapping[str, List[data.Setting]]:
+    def settings(self) -> Mapping[str, list[data.Setting]]:
         return self._typed_store(data.Setting)
 
     @property
     def modes(self) -> Mapping[str, data.Mode]:
         return self._typed_store(data.Mode)
 
     @property
     def tags(self) -> Mapping[str, data.Tag]:
         return self._typed_store(data.Tag)
 
     ######################################################################
-    # Internal Typed Access To Data
+    # Internal typed Access To Data
     ######################################################################
 
     @overload
-    def _typed_store(self, cls: type[SimpleDataVar]) -> Dict[str, SimpleDataVar]:
+    def _typed_store(self, cls: type[SimpleDataVar]) -> dict[str, SimpleDataVar]:
         ...
 
     @overload
-    def _typed_store(self, cls: type[GroupDataVar]) -> Dict[str, List[GroupDataVar]]:
+    def _typed_store(self, cls: type[GroupDataVar]) -> dict[str, list[GroupDataVar]]:
         ...
 
     @overload
     def _typed_store(
         self, cls: type[data.Callback]
-    ) -> Dict[data.EventCode, List[data.Callback]]:
+    ) -> dict[data.EventCode, list[data.Callback]]:
         ...
 
     @overload
-    def _typed_store(self, cls: type[Data]) -> Dict[Any, Any]:
+    def _typed_store(self, cls: type[Data]) -> dict[Any, Any]:
         ...
 
-    def _typed_store(self, cls: type[Data]) -> Dict[Any, Any]:
+    def _typed_store(self, cls: type[Data]) -> dict[Any, Any]:
         # If the data is not serialisable, store it in temp_data:
         if cls.serialisable:
             data = self._data
         else:
             data = self._temp_data
         # Store the data in a dictionary indexed by its type name.
         store = data.setdefault(cls.__name__, {})
         assert isinstance(store, dict)
         return store
 
     ##################################################
     # Encoder/Decoder
     ##################################################
 
+    def load_builtin(self) -> None:
+        self._load_from_dict(
+            json.loads(
+                importlib_resources.open_text(
+                    "talondoc._cache_builtin.resources", "talon.json"
+                ).read()
+            )
+        )
+
+    def _load_from_dict(self, registry: JsonValue) -> None:
+        registry = parse_dict(registry)
+        for cls in (
+            data.Command,
+            data.Action,
+            data.Capture,
+            data.List,
+            data.Setting,
+            data.Mode,
+            data.Tag,
+        ):
+            _LOGGER.debug(f"Loading builtin {cls.__name__} objects...")
+            store = parse_dict(registry.get(cls.__name__, {}))
+            if issubclass(cls, GroupData):
+                for name, group in store.items():
+                    _LOGGER.debug(
+                        f"Found {len(group)} {cls.__name__} objects with {name}"
+                    )
+                    for value in parse_list(group):
+                        parsed_group_value = cls.from_dict(value)
+                        if name != parsed_group_value.name:
+                            _LOGGER.warning(
+                                f"Found {cls.__name__} {parsed_group_value.name} in group for {name}"
+                            )
+                        self.register(parsed_group_value)
+
+            elif issubclass(cls, (data.Mode, data.Tag)):
+                for name, value in store.items():
+                    _LOGGER.debug(f"Found {cls.__name__} object with {name}")
+                    parsed_simple_value = cls.from_dict(value)
+                    if name != parsed_simple_value.name:
+                        _LOGGER.warning(
+                            f"Found {cls.__name__} {parsed_simple_value.name} in group for {name}"
+                        )
+                    self.register(parsed_simple_value)
+            else:
+                raise TypeError(f"Unexpected data class {cls.__name__}")
+
     def to_dict(self) -> JsonValue:
         return {
             data.Command.__name__: {
                 name: [command.to_dict() for command in group]
                 for name, group in self.commands.items()
             },
             data.Action.__name__: {
@@ -527,21 +617,21 @@
         try:
             if Registry._active_global_registry:
                 return Registry._active_global_registry
         except AttributeError:
             pass
         raise NoActiveRegistry()
 
-    def activate(self: "Registry"):
+    def activate(self: "Registry") -> None:
         """
         Activate this registry.
         """
         Registry._active_global_registry = self
 
-    def deactivate(self: "Registry"):
+    def deactivate(self: "Registry") -> None:
         """
         Deactivate this registry.
         """
         if self is not None and self != Registry._active_global_registry:
             _LOGGER.warning(f"attempted to deactivate registry that is inactive")
         Registry._active_global_registry = None
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/registry/data/__init__.py` & `talondoc-0.6.0/src/talondoc/analysis/registry/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import textwrap
-import typing
-from collections.abc import Callable
+from collections.abc import Callable, Mapping, Sequence
 from dataclasses import dataclass, field
 from functools import partial
 from inspect import Signature
-from typing import Any, Mapping, Optional, Sequence, Union
+from typing import Any, Optional, Union
 
 import tree_sitter_talon
 from tree_sitter_talon import Node as Node
 from tree_sitter_talon import Point as Point
 from tree_sitter_talon import TalonBlock, TalonMatch, TalonRule
 from typing_extensions import Literal, TypeAlias, TypeVar, final
 
@@ -58,15 +57,15 @@
 ListName: TypeAlias = str
 SettingName: TypeAlias = str
 ModeName: TypeAlias = str
 TagName: TypeAlias = str
 
 EventCode: TypeAlias = Union[int, str]
 Script: TypeAlias = TalonBlock
-ListValue: TypeAlias = Union[typing.Dict[str, Any], typing.List[str]]
+ListValue: TypeAlias = Union[dict[str, Any], list[str]]
 SettingValue: TypeAlias = Any
 Match: TypeAlias = TalonMatch
 Rule: TypeAlias = TalonRule
 
 
 ##############################################################################
 # Decoders - Common
@@ -155,15 +154,15 @@
         return {
             key: parse_pickle(val, context=context)
             for key, val in parse_dict(value).items()
         }
     if isinstance(value, Sequence):
         return list(map(parse_str, value))
     raise TypeError(
-        f"Expected dict[str, any] or list[str], found {type(value).__name__}"
+        f"Expected dict[str, any] or List[str], found {type(value).__name__}"
     )
 
 
 def field_list_value(value: JsonValue) -> Optional[ListValue]:
     context: dict[str, str] = {
         "object_type": "list",
         "field_name": "value",
@@ -227,15 +226,15 @@
     name: FileName = field(init=False)
     description: None = field(default=None, init=False)
     location: Location
     parent_name: PackageName
     parent_type: type[Package] = field(default=Package, init=False)
     serialisable: bool = field(default=True, init=False)
 
-    def __post_init__(self, *_args, **_kwargs) -> None:
+    def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         self.name = ".".join((self.parent_name, *self.location.path.parts))
 
 
 ##############################################################################
 # Modules and Contexts
 ##############################################################################
 
@@ -248,15 +247,15 @@
     name: ModuleName = field(init=False)
     description: Optional[str]
     location: Location
     parent_name: FileName
     parent_type: type[File] = field(default=File, init=False)
     serialisable: bool = field(default=True, init=False)
 
-    def __post_init__(self, *_args, **_kwargs) -> None:
+    def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         if self.index == 0:
             self.name = f"{self.parent_name}"
         else:
             self.name = f"{self.parent_name}.{self.index}"
 
 
 @final
@@ -269,15 +268,15 @@
     name: ContextName = field(init=False)
     description: Optional[str]
     location: Location
     parent_name: FileName
     parent_type: type[File] = field(default=File, init=False)
     serialisable: bool = field(default=True, init=False)
 
-    def __post_init__(self, *_args, **_kwargs) -> None:
+    def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         if self.index == 0:
             self.name = f"{self.parent_name}"
         else:
             self.name = f"{self.parent_name}.{self.index}"
 
     @property
     def always_on(self) -> bool:
@@ -307,15 +306,15 @@
     location: Location
     parent_name: Union[ModuleName, ContextName]
     parent_type: Union[type[Module], type[Context]]
     serialisable: bool = field(default=False, init=False)
 
     function: Callable[..., Any] = field(repr=False)
 
-    def __post_init__(self, *_args, **_kwargs) -> None:
+    def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         self.name = f"{self.parent_name}:{self.namespace}.{self.function.__name__}"
         self.description = self.function.__doc__
 
 
 ##############################################################################
 # Callbacks
 ##############################################################################
@@ -330,15 +329,15 @@
     parent_name: FileName
     parent_type: type[File] = field(default=File, init=False)
     serialisable: bool = field(default=False, init=False)
 
     event_code: EventCode
     function: Callable[..., Any] = field(repr=False)
 
-    def __post_init__(self, *_args, **_kwargs) -> None:
+    def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         self.name = f"{self.parent_name}:{self.function.__name__}"
         self.description = self.function.__doc__
 
 
 CallbackVar = TypeVar("CallbackVar", bound=Callback)
 
 ##############################################################################
@@ -355,28 +354,28 @@
     name: str = field(init=False)
     description: Optional[str]
     location: Location
     parent_name: ContextName
     parent_type: type[Context] = field(default=Context, init=False)
     serialisable: bool = field(default=True, init=False)
 
-    def __post_init__(self, *_args, **_kwargs) -> None:
+    def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         self.name = rule_name(self.rule)
 
     @classmethod
     def from_dict(cls, value: JsonValue) -> "Command":
         return Command(
             rule=field_rule(value),
             script=field_script(value),
             description=field_description(value),
             location=parse_field("location", Location.from_dict)(value),
             parent_name=field_parent_name(value),
         )
 
-    def to_dict(self) -> JsonValue:
+    def to_dict(self) -> dict[str, JsonValue]:
         return {
             "rule": self.rule.text,
             "script": self.script.text,
             "description": self.description,
             "location": asdict_location(self.location),
             "parent_name": self.parent_name,
         }
@@ -420,15 +419,15 @@
             name=field_name(value),
             description=field_description(value),
             location=field_location(value),
             parent_name=field_parent_name(value),
             parent_type=field_parent_type(value),
         )
 
-    def to_dict(self) -> JsonValue:
+    def to_dict(self) -> dict[str, JsonValue]:
         return {
             "function_name": None,
             "function_signature": asdict_opt(asdict_signature)(self.function_signature),
             "name": self.name,
             "description": self.description,
             "location": asdict_location(self.location),
             "parent_name": self.parent_name,
@@ -472,15 +471,15 @@
             name=field_name(value),
             description=field_description(value),
             location=field_location(value),
             parent_name=field_parent_name(value),
             parent_type=field_parent_type(value),
         )
 
-    def to_dict(self) -> JsonValue:
+    def to_dict(self) -> dict[str, JsonValue]:
         return {
             "rule": self.rule.text,
             "function_name": None,
             "function_signature": asdict_opt(asdict_signature)(self.function_signature),
             "name": self.name,
             "description": self.description,
             "location": asdict_location(self.location),
@@ -489,24 +488,24 @@
         }
 
 
 @final
 @dataclass
 class List(GroupData):
     value: Optional[ListValue]
-    value_type_hint: Optional[type]
+    value_type_hint: Optional[type[Any]]
 
     name: ListName
     description: Optional[str]
     location: Union[None, Literal["builtin"], Location]
     parent_name: Union[ModuleName, ContextName]
     parent_type: Union[type[Module], type[Context]]
     serialisable: bool = field(default=True, init=False)
 
-    def __post_init__(self, *args, **kwargs) -> None:
+    def __post_init__(self, *_args: Any, **_kwargs: Any) -> None:
         if isinstance(self.value, Mapping):
             self.value = dict(self.value)
         elif isinstance(self.value, Sequence):
             self.value = list(self.value)
         else:
             if type(self.value).__name__ != "ObjectShim" and self.value is not None:
                 _LOGGER.warning(  # type: ignore[unreachable]
@@ -522,15 +521,15 @@
             name=field_name(value),
             description=field_description(value),
             location=field_optlocation(value),
             parent_name=field_parent_name(value),
             parent_type=field_parent_type(value),
         )
 
-    def to_dict(self) -> JsonValue:
+    def to_dict(self) -> dict[str, JsonValue]:
         return {
             "value": asdict_opt(asdict_list_value)(self.value),
             "value_type_hint": asdict_opt(asdict_class)(self.value_type_hint),
             "name": self.name,
             "description": self.description,
             "location": asdict_opt(asdict_location)(self.location),
             "parent_name": self.parent_name,
@@ -538,15 +537,15 @@
         }
 
 
 @final
 @dataclass
 class Setting(GroupData):
     value: Optional[SettingValue]
-    value_type_hint: Optional[type]
+    value_type_hint: Optional[type[Any]]
 
     name: SettingName
     description: Optional[str]
     location: Union[None, Literal["builtin"], Location]
     parent_name: Union[ModuleName, ContextName]
     parent_type: Union[type[Module], type[Context]]
     serialisable: bool = field(default=True, init=False)
@@ -559,15 +558,15 @@
             name=field_name(value),
             description=field_description(value),
             location=field_optlocation(value),
             parent_name=field_parent_name(value),
             parent_type=field_parent_type(value),
         )
 
-    def to_dict(self) -> JsonValue:
+    def to_dict(self) -> dict[str, JsonValue]:
         return {
             "value": asdict_opt(asdict_pickle)(self.value),
             "value_type_hint": asdict_opt(asdict_class)(self.value_type_hint),
             "name": self.name,
             "description": self.description,
             "location": asdict_opt(asdict_location)(self.location),
             "parent_name": self.parent_name,
@@ -590,15 +589,15 @@
         return Mode(
             name=field_name(value),
             description=field_description(value),
             location=field_optlocation(value),
             parent_name=field_parent_name(value),
         )
 
-    def to_dict(self) -> JsonValue:
+    def to_dict(self) -> dict[str, JsonValue]:
         return {
             "name": self.name,
             "description": self.description,
             "location": asdict_opt(asdict_location)(self.location),
             "parent_name": self.parent_name,
         }
 
@@ -618,14 +617,14 @@
         return Tag(
             name=field_name(value),
             description=field_description(value),
             location=field_optlocation(value),
             parent_name=field_parent_name(value),
         )
 
-    def to_dict(self) -> JsonValue:
+    def to_dict(self) -> dict[str, JsonValue]:
         return {
             "name": self.name,
             "description": self.description,
             "location": asdict_opt(asdict_location)(self.location),
             "parent_name": self.parent_name,
         }
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/registry/data/abc.py` & `talondoc-0.6.0/src/talondoc/analysis/registry/data/abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import abstractmethod
+from collections.abc import Callable, Mapping, Sequence
 from dataclasses import asdict, dataclass
 from functools import singledispatch
 from inspect import Signature
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 import editdistance
 from tree_sitter_talon import Node as Node
 from tree_sitter_talon import Point as Point
 from tree_sitter_talon import (
     TalonCapture,
     TalonChoice,
@@ -61,30 +62,31 @@
     end_line: Optional[int] = None
     end_column: Optional[int] = None
 
     @staticmethod
     def _str_from_point(line: Optional[int], column: Optional[int]) -> Optional[str]:
         if line is not None:
             if column is not None:
-                return f"{line}"
-            else:
                 return f"{line}:{column}"
+            else:
+                return f"{line}"
         else:
             return None
 
     def __str__(self) -> str:
+        resolved_path = self.path.resolve().relative_to(Path.cwd())
         start_position = Location._str_from_point(self.start_line, self.start_column)
-        if start_position:
+        if start_position is not None:
             end_position = Location._str_from_point(self.end_line, self.end_column)
-            if end_position:
-                return f"{self.path}:{start_position}-{end_position}"
+            if end_position is not None:
+                return f"{resolved_path}:{start_position}-{end_position}"
             else:
-                return f"{self.path}:{start_position}"
+                return f"{resolved_path}:{start_position}"
         else:
-            return f"{self.path}"
+            return f"{resolved_path}"
 
     @staticmethod
     def from_ast(path: Path, node: Node) -> "Location":
         return Location(
             path=path,
             start_line=node.start_position.line,
             start_column=node.start_position.column,
@@ -100,15 +102,15 @@
 
     @staticmethod
     def from_path(path: Path) -> "Location":
         return Location(path=path)
 
     @staticmethod
     def from_dict(value: JsonValue) -> "Location":
-        if isinstance(value, Dict):
+        if isinstance(value, Mapping):
             return Location(
                 path=Path(parse_field("path", parse_str)(value)),
                 start_line=parse_optfield("start_line", parse_int)(value),
                 start_column=parse_optfield("start_column", parse_int)(value),
                 end_line=parse_optfield("end_line", parse_int)(value),
                 end_column=parse_optfield("end_column", parse_int)(value),
             )
@@ -183,15 +185,15 @@
 
     @classmethod
     @abstractmethod
     def from_dict(cls, value: JsonValue) -> Self:
         ...
 
     @abstractmethod
-    def to_dict(self) -> JsonValue:
+    def to_dict(self) -> dict[str, JsonValue]:
         ...
 
 
 GroupDataVar = TypeVar(
     "GroupDataVar",
     bound=GroupData,
 )
@@ -245,20 +247,25 @@
 @dataclass
 class UnknownReference(Exception):
     """Raised when an entry is defined in multiple modules."""
 
     ref_type: type[Data]
     ref_name: str
 
-    referenced_by: Optional[Data]
-    known_references: Optional[Sequence[str]]
+    location: Optional[str] = None
+    referenced_by: Optional[Data] = None
+    known_references: Optional[Sequence[str]] = None
 
     def __str__(self) -> str:
         buffer = []
 
+        # If location is set, include it:
+        if self.location is not None:
+            buffer.append(f"{self.location}:")
+
         # If referenced_by is set, include it:
         if self.referenced_by is not None:
             referenced_by_type_name = self.referenced_by.__class__.__name__.lower()
             buffer.append(
                 f"{referenced_by_type_name} '{self.referenced_by.name}' references"
             )
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/registry/data/serialise.py` & `talondoc-0.6.0/src/talondoc/analysis/registry/data/serialise.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import pickle
-from collections.abc import Callable
+from collections.abc import Callable, Mapping, Sequence
 from functools import partial
 from inspect import Parameter, Signature
 from logging import WARNING
-from typing import Any, Dict, Mapping, Optional, Sequence, Union
+from typing import Any, Optional, Union
 
 from typing_extensions import TypeAlias, TypeVar
 
 from ...._util.logging import getLogger
 
 _LOGGER = getLogger(__name__)
 
@@ -166,15 +166,15 @@
 
     return _parser
 
 
 _EnumType = TypeVar("_EnumType", bound=int)
 
 
-def parse_enum(options: tuple[_EnumType, ...]) -> Callable[[JsonValue], _EnumType]:
+def parse_enum(options: Sequence[_EnumType]) -> Callable[[JsonValue], _EnumType]:
     OPTIONS_DICT = {int(opt): opt for opt in options}
     return lambda value: OPTIONS_DICT[parse_int(value)]
 
 
 def parse_class(*options: type[_T]) -> Callable[[JsonValue], type[_T]]:
     return lambda value: {opt.__name__: opt for opt in options}[parse_str(value)]
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/static/__init__.py` & `talondoc-0.6.0/src/talondoc/analysis/static/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,39 @@
+from collections.abc import Sequence
 from pathlib import Path
 from typing import Optional
 
 from ..registry import Registry
 from ..registry.data import Package
 from ..registry.data.abc import Location
 from .python import analyse_files as analyse_python_files
 from .talon import analyse_files as analyse_talon_files
 
 
 def _include_file(
     file_path: Path,
     *,
-    include: tuple[str, ...] = (),
-    exclude: tuple[str, ...] = (),
+    include: Sequence[str] = (),
+    exclude: Sequence[str] = (),
 ) -> bool:
     return (
         not exclude
         or not any(file_path.match(exclude_pattern) for exclude_pattern in exclude)
         or any(file_path.match(include_pattern) for include_pattern in include)
     )
 
 
 def analyse_package(
     registry: Registry,
     package_dir: Path,
     *,
     package_name: Optional[str] = None,
-    include: tuple[str, ...] = (),
-    exclude: tuple[str, ...] = (),
-    trigger: tuple[str, ...] = (),
+    include: Sequence[str] = (),
+    exclude: Sequence[str] = (),
+    trigger: Sequence[str] = (),
     show_progress: bool = False,
     continue_on_error: bool = True,
 ) -> None:
     # Activate the registry:
     registry.activate()
 
     # Retrieve or create package entry:
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/static/python/__init__.py` & `talondoc-0.6.0/src/talondoc/analysis/static/python/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import importlib
 import sys
-from collections.abc import Iterator
+from collections.abc import Iterator, Sequence
 from contextlib import contextmanager
 from importlib.abc import Loader, MetaPathFinder
 from importlib.machinery import ModuleSpec, PathFinder, SourceFileLoader
 from pathlib import Path
 from types import ModuleType
-from typing import ClassVar, Optional, Sequence, cast
+from typing import ClassVar, Optional
 
 from ...._util.logging import getLogger
 from ...._util.progress_bar import ProgressBar
 from ...registry import Registry, data
 from ...registry.data.abc import Location
 from .shims import ModuleShim, TalonShim
 
@@ -18,24 +18,24 @@
 
 
 class TalonShimFinder(MetaPathFinder):
     """
     Makes the shims available under 'talon' and 'talon_plugins'.
     """
 
-    PACKAGES: ClassVar[tuple[str, ...]] = ("talon", "talon_plugins")
+    PACKAGES: ClassVar[Sequence[str]] = ("talon", "talon_plugins")
 
     class TalonShimLoader(Loader):
         def create_module(cls, spec: ModuleSpec) -> ModuleType:
-            return cast(ModuleType, cls.load_module(spec.name))
+            return cls.load_module(spec.name)
 
-        def exec_module(cls, module: ModuleType):
+        def exec_module(cls, module: ModuleType) -> None:
             pass
 
-        def load_module(cls, fullname: str):
+        def load_module(cls, fullname: str) -> ModuleType:
             if fullname == "talon":
                 return TalonShim()
             else:
                 return ModuleShim(fullname)
 
     @classmethod
     def _is_module(cls, fullname: str) -> bool:
@@ -69,21 +69,21 @@
 
     class PackagePathFinder(PathFinder):
         """
         Makes the package available.
         """
 
         class ImplicitInitLoader(Loader):
-            def create_module(cls, spec: ModuleSpec):
+            def create_module(cls, spec: ModuleSpec) -> ModuleType:
                 return cls.load_module(spec.name)
 
-            def exec_module(cls, _module: ModuleType):
+            def exec_module(cls, _module: ModuleType) -> None:
                 pass
 
-            def load_module(cls, fullname: str):
+            def load_module(cls, fullname: str) -> ModuleType:
                 return ModuleType(fullname)
 
         @classmethod
         def _is_module(cls, fullname: str) -> bool:
             return fullname == package_name or fullname.startswith(f"{package_name}.")
 
         @classmethod
@@ -92,15 +92,20 @@
             return Path(package_path, *fullname.split(".")[1:])
 
         @classmethod
         def _is_subpackage(cls, fullname: str) -> bool:
             return cls._is_module(fullname) and cls._module_path(fullname).is_dir()
 
         @classmethod
-        def find_spec(cls, fullname: str, path=None, _target=None):
+        def find_spec(
+            cls,
+            fullname: str,
+            path: Optional[Sequence[str]] = None,
+            target: Optional[ModuleType] = None,
+        ) -> Optional[ModuleSpec]:
             if cls._is_module(fullname):
                 if cls._is_subpackage(fullname):
                     module_spec = ModuleSpec(
                         name=fullname, loader=cls.ImplicitInitLoader(), is_package=True
                     )
                     submodule_search_location = str(cls._module_path(fullname))
                     if not module_spec.submodule_search_locations:
@@ -127,15 +132,17 @@
     try:
         yield None
     finally:
         sys.meta_path.remove(PackagePathFinder)
 
 
 @contextmanager
-def talon_shims(registry: Registry, *, package: Optional[data.Package] = None):
+def talon_shims(
+    registry: Registry, *, package: Optional[data.Package] = None
+) -> Iterator[None]:
     sys.meta_path.insert(0, TalonShimFinder)
     try:
         if package:
             with talon_package_shims(package):
                 yield None
         else:
             yield None
@@ -157,15 +164,15 @@
 
 
 def analyse_files(
     registry: Registry,
     paths: Sequence[Path],
     package: data.Package,
     *,
-    trigger: tuple[str, ...] = (),
+    trigger: Sequence[str] = (),
     show_progress: bool = False,
     continue_on_error: bool = True,
 ) -> None:
     # Retrieve or create package entry:
     with talon_shims(registry, package=package):
         bar = ProgressBar(total=len(paths), show=show_progress)
         for file_path in paths:
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/static/python/shims.py` & `talondoc-0.6.0/src/talondoc/analysis/static/python/shims.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import inspect
 import platform
-from collections.abc import Callable, Iterator
+from collections.abc import Callable, Iterator, Mapping, Sequence
 from io import TextIOWrapper
 from types import ModuleType
-from typing import Any, Mapping, Optional, Sequence, cast
+from typing import Any, Optional, Union, cast, overload
 
 from tree_sitter_talon import Point
 
 from ...._util.logging import getLogger
 from ...registry import Registry, data
-from ...registry.data.abc import Location
+from ...registry.data.abc import Location, UnknownReference
 
 _LOGGER = getLogger(__name__)
 
 
 class ObjectShim:
     """
     A simple shim which responds to any method.
     """
 
-    def register(self, event_code: data.EventCode, func: Callable[..., Any]):
+    def register(self, event_code: data.EventCode, func: Callable[..., Any]) -> None:
         if inspect.isfunction(func):
             registry = Registry.get_active_global_registry()
             registry.register(
                 data.Callback(
                     event_code=event_code,
                     function=func,
                     location=Location.from_function(func),
@@ -31,75 +31,75 @@
                 )
             )
         else:
             _LOGGER.debug(
                 f"skip register {data.Callback.__name__}: callback of type {func.__class__.__qualname__} is not a function"
             )
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *_args: Any, **_kwargs: Any) -> None:
         pass
 
     def __getattr__(self, name: str) -> Any:
         try:
             return object.__getattribute__(self, name)
         except AttributeError:
             return self
 
-    def __setattr__(self, name: str, value: Any):
+    def __setattr__(self, name: str, value: Any) -> None:
         object.__setattr__(self, name, value)
 
     def __getitem__(self, name: str) -> Any:
         return self
 
-    def __setitem__(self, name: str, value: Any):
+    def __setitem__(self, name: str, value: Any) -> None:
         pass
 
     def __enter__(self) -> Any:
         return self
 
-    def __exit__(self, *args):
+    def __exit__(self, *_args: Any) -> None:
         pass
 
-    def __add__(self, other) -> Any:
+    def __add__(self, other: Any) -> Any:
         return self
 
-    def __sub__(self, other) -> Any:
+    def __sub__(self, other: Any) -> Any:
         return self
 
-    def __mul__(self, other) -> Any:
+    def __mul__(self, other: Any) -> Any:
         return self
 
-    def __pow__(self, other) -> Any:
+    def __pow__(self, other: Any) -> Any:
         return self
 
-    def __mod__(self, other) -> Any:
+    def __mod__(self, other: Any) -> Any:
         return self
 
-    def __floordiv__(self, other) -> Any:
+    def __floordiv__(self, other: Any) -> Any:
         return self
 
-    def __truediv__(self, other) -> Any:
+    def __truediv__(self, other: Any) -> Any:
         return self
 
-    def __radd__(self, other) -> Any:
+    def __radd__(self, other: Any) -> Any:
         return self
 
-    def __rsub__(self, other) -> Any:
+    def __rsub__(self, other: Any) -> Any:
         return self
 
-    def __rmul__(self, other) -> Any:
+    def __rmul__(self, other: Any) -> Any:
         return self
 
-    def __rmod__(self, other) -> Any:
+    def __rmod__(self, other: Any) -> Any:
         return self
 
-    def __rfloordiv__(self, other) -> Any:
+    def __rfloordiv__(self, other: Any) -> Any:
         return self
 
-    def __rtruediv__(self, other) -> Any:
+    def __rtruediv__(self, other: Any) -> Any:
         return self
 
     def __abs__(self) -> Any:
         return self
 
     def __neg__(self) -> Any:
         return self
@@ -109,51 +109,51 @@
 
     def __floor__(self) -> Any:
         return self
 
     def __ceil__(self) -> Any:
         return self
 
-    def __and__(self, other) -> Any:
+    def __and__(self, other: Any) -> Any:
         return self
 
-    def __rand__(self, other) -> Any:
+    def __rand__(self, other: Any) -> Any:
         return self
 
-    def __or__(self, other) -> Any:
+    def __or__(self, other: Any) -> Any:
         return self
 
-    def __ror__(self, other) -> Any:
+    def __ror__(self, other: Any) -> Any:
         return self
 
-    def __xor__(self, other) -> Any:
+    def __xor__(self, other: Any) -> Any:
         return self
 
-    def __rxor__(self, other) -> Any:
+    def __rxor__(self, other: Any) -> Any:
         return self
 
     def __invert__(self) -> Any:
         return self
 
-    def __lshift__(self, other) -> Any:
+    def __lshift__(self, other: Any) -> Any:
         return self
 
-    def __rlshift__(self, other) -> Any:
+    def __rlshift__(self, other: Any) -> Any:
         return self
 
-    def __rshift__(self, other) -> Any:
+    def __rshift__(self, other: Any) -> Any:
         return self
 
-    def __rrshift__(self, other) -> Any:
+    def __rrshift__(self, other: Any) -> Any:
         return self
 
-    def __call__(self, *args, **kwargs) -> Any:
+    def __call__(self, *_args: Any, **_kwargs: Any) -> Any:
         return self
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[Any]:
         return ().__iter__()
 
 
 class ModuleShim(ModuleType):
     """
     A module shim which defines any value.
     """
@@ -173,15 +173,21 @@
         try:
             return cast(
                 Optional[Callable[..., Any]],
                 object.__getattribute__(self, name),
             )
         except AttributeError:
             registry = Registry.get_active_global_registry()
-            return registry.lookup_default_function(data.Action, name) or ObjectShim()
+            try:
+                default = registry.lookup_default_function(data.Action, name)
+                if default:
+                    return default
+            except UnknownReference as e:
+                _LOGGER.warning(e)
+            return ObjectShim()
 
 
 class TalonAppShim(ObjectShim):
     @property
     def platform(self) -> str:
         system = platform.system()
         if system == "Linux":
@@ -193,15 +199,15 @@
         raise ValueError(system)
 
 
 class TalonContextListsShim(Mapping[str, data.ListValue]):
     def __init__(self, context: "TalonShim.Context"):
         self._context = context
 
-    def _add_list_value(self, name: str, value: data.ListValue):
+    def _add_list_value(self, name: str, value: data.ListValue) -> None:
         self._context._registry.register(
             data.List(
                 value=value,
                 value_type_hint=None,
                 # NOTE: list names on contexts are fully qualified
                 name=self._context._registry.resolve_name(
                     name, package=self._context._package
@@ -209,36 +215,36 @@
                 description=None,
                 location=self._context._context.location,
                 parent_name=self._context._context.name,
                 parent_type=data.Context,
             )
         )
 
-    def __setitem__(self, name: str, value: data.ListValue):
+    def __setitem__(self, name: str, value: data.ListValue) -> None:
         self._add_list_value(name, value)
 
-    def update(self, values: Mapping[str, data.ListValue]):
+    def update(self, values: Mapping[str, data.ListValue]) -> None:
         for name, value in values.items():
             self._add_list_value(name, value)
 
-    def __getitem__(self):
-        raise NotImplementedError
+    def __getitem__(self, key: str) -> Union[dict[str, Any], list[str]]:
+        raise NotImplementedError()
 
-    def __iter__(self):
-        raise NotImplementedError
+    def __iter__(self) -> Iterator[Any]:
+        raise NotImplementedError()
 
-    def __len__(self):
-        raise NotImplementedError
+    def __len__(self) -> int:
+        raise NotImplementedError()
 
 
-class TalonContextSettingsShim(Mapping):
+class TalonContextSettingsShim(Mapping[str, data.SettingValue]):
     def __init__(self, context: "TalonShim.Context"):
         self._context = context
 
-    def _add_setting_value(self, name: str, value: data.SettingValue):
+    def _add_setting_value(self, name: str, value: data.SettingValue) -> None:
         self._context._registry.register(
             data.Setting(
                 value=value,
                 value_type_hint=None,
                 # NOTE: setting names on contexts are fully qualified
                 name=self._context._registry.resolve_name(
                     name, package=self._context._package
@@ -246,95 +252,103 @@
                 description=None,
                 location=self._context._context.location,
                 parent_name=self._context._context.name,
                 parent_type=data.Context,
             )
         )
 
-    def __setitem__(self, name: str, value: data.SettingValue):
+    def __setitem__(self, name: str, value: data.SettingValue) -> None:
         self._add_setting_value(name, value)
 
-    def update(self, values: Mapping[str, data.SettingValue]):
+    def update(self, values: Mapping[str, data.SettingValue]) -> None:
         for name, value in values.items():
             self._add_setting_value(name, value)
 
-    def __getitem__(self):
-        raise NotImplementedError
+    def __getitem__(self, key: str) -> data.SettingValue:
+        raise NotImplementedError()
 
-    def __iter__(self):
-        raise NotImplementedError
+    def __iter__(self) -> Iterator[data.SettingValue]:
+        raise NotImplementedError()
 
-    def __len__(self):
-        raise NotImplementedError
+    def __len__(self) -> int:
+        raise NotImplementedError()
 
 
-class TalonContextTagsShim(Sequence):
+class TalonContextTagsShim(Sequence[str]):
     def __init__(self, context: "TalonShim.Context"):
         self._context = context
 
-    def _add_tag_import(self, name: str):
+    def _add_tag_import(self, name: str) -> None:
         # TODO: add use entries
         pass
 
-    def __setitem__(self, name: str):
+    def __setitem__(self, name: str) -> None:
         self._add_tag_import(name)
 
-    def update(self, values: Sequence[str]):
+    def update(self, values: Sequence[str]) -> None:
         for name in values:
             self._add_tag_import(name)
 
-    def __getitem__(self):
-        raise NotImplementedError
+    @overload
+    def __getitem__(self, index: int) -> str:
+        ...
+
+    @overload
+    def __getitem__(self, index: slice) -> Sequence[str]:
+        ...
+
+    def __getitem__(self, _index: Any) -> Sequence[Any]:
+        raise NotImplementedError()
 
-    def __iter__(self):
-        raise NotImplementedError
+    def __iter__(self) -> Iterator[str]:
+        raise NotImplementedError()
 
-    def __len__(self):
-        raise NotImplementedError
+    def __len__(self) -> int:
+        raise NotImplementedError()
 
 
 class TalonResourceShim(ObjectShim):
     def open(self, file: str, mode: str = "r") -> TextIOWrapper:
         return cast(TextIOWrapper, open(file, mode))
 
     def read(self, file: str) -> str:
-        raise NotImplementedError
+        raise NotImplementedError()
 
-    def write(self, file: str, contents: str) -> str:
-        raise NotImplementedError
+    def write(self, _file: str, _contents: str) -> str:
+        raise NotImplementedError()
 
 
 class TalonShim(ModuleShim):
     """
     A shim for the 'talon' module.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("talon")
         self.actions = TalonActionsShim()
         self.app = TalonAppShim()
         self.resource = TalonResourceShim()
         # TODO: app
         # TODO: ui
 
     class Module(ObjectShim):
-        def __init__(self, desc: Optional[str] = None):
+        def __init__(self, desc: Optional[str] = None) -> None:
             self._registry = Registry.get_active_global_registry()
             self._package = self._registry.get_active_package()
             self._file = self._registry.get_active_file()
             self._module = data.Module(
                 index=len(self._file.modules),
                 description=desc,
                 location=self._file.location,
                 parent_name=self._file.name,
             )
             self._file.modules.append(self._module.name)
             self._registry.register(self._module)
 
-        def action_class(self, cls: type):
+        def action_class(self, cls: type[Any]) -> type[Any]:
             for name, func in inspect.getmembers(cls, inspect.isfunction):
                 assert callable(func)
                 package = self._registry.get_active_package()
                 function = data.Function(
                     namespace=package.name,
                     function=func,
                     location=Location.from_function(func),
@@ -348,14 +362,15 @@
                     name=f"{package.name}.{name}",
                     description=func.__doc__,
                     location=function.location,
                     parent_name=self._module.name,
                     parent_type=data.Module,
                 )
                 self._registry.register(action)
+            return cls
 
         def action(self, name: str) -> Optional[Callable[..., Any]]:
             function = self._registry.lookup_default_function(data.Action, name)
             return function or ObjectShim()
 
         def capture(
             self, rule: str
@@ -388,15 +403,15 @@
 
         def setting(
             self,
             name: str,
             type: type,
             default: data.SettingValue = None,
             desc: Optional[str] = None,
-        ):
+        ) -> None:
             self._registry.register(
                 data.Setting(
                     value=default,
                     value_type_hint=type,
                     # NOTE: list names passed to modules are unqualified
                     name=f"{self._package.name}.{name}",
                     description=desc,
@@ -406,15 +421,15 @@
                 )
             )
 
         def list(
             self,
             name: str,
             desc: Optional[str] = None,
-        ):
+        ) -> None:
             self._registry.register(
                 data.List(
                     value=None,
                     value_type_hint=None,
                     # NOTE: list names passed to modules are unqualified
                     name=f"{self._package.name}.{name}",
                     description=desc,
@@ -424,43 +439,43 @@
                 )
             )
 
         def mode(
             self,
             name: str,
             desc: Optional[str] = None,
-        ):
+        ) -> None:
             self._registry.register(
                 data.Mode(
                     name=f"{self._package.name}.{name}",
                     description=desc,
                     location=self._module.location,
                     parent_name=self._module.name,
                 )
             )
 
         def tag(
             self,
             name: str,
             desc: Optional[str] = None,
-        ):
+        ) -> None:
             self._registry.register(
                 data.Tag(
                     name=f"{self._package.name}.{name}",
                     description=desc,
                     location=self._module.location,
                     parent_name=self._module.name,
                 )
             )
 
         # TODO: apps
         # TODO: scope
 
     class Context(ObjectShim):
-        def __init__(self, desc: Optional[str] = None):
+        def __init__(self, desc: Optional[str] = None) -> None:
             self._registry = Registry.get_active_global_registry()
             self._package = self._registry.get_active_package()
             self._file = self._registry.get_active_file()
             self._context = data.Context(
                 matches=[],
                 index=len(self._file.contexts),
                 description=desc,
@@ -484,27 +499,27 @@
             self._lists.update(lists)
 
         @property
         def settings(self) -> Mapping[str, data.SettingValue]:
             return self._settings
 
         @settings.setter
-        def settings(self, values: Mapping[str, data.SettingValue]):
+        def settings(self, values: Mapping[str, data.SettingValue]) -> None:
             self._settings.update(values)
 
         @property
         def tags(self) -> Sequence[str]:
             return self._tags
 
         @tags.setter
-        def tags(self, values: Sequence[str]):
+        def tags(self, values: Sequence[str]) -> None:
             self._tags.update(values)
 
-        def action_class(self, namespace: str) -> Callable[[type], type]:
-            def __decorator(cls: type):
+        def action_class(self, namespace: str) -> Callable[[type[Any]], type[Any]]:
+            def __decorator(cls: type[Any]) -> type[Any]:
                 for name, func in inspect.getmembers(cls, inspect.isfunction):
                     # LINT: check if function on decorated class is a function
                     assert callable(func)
 
                     location = Location.from_function(func)
                     function = data.Function(
                         namespace=namespace,
@@ -521,21 +536,22 @@
                         name=f"{namespace}.{name}",
                         description=func.__doc__,
                         location=location,
                         parent_name=self._context.name,
                         parent_type=data.Context,
                     )
                     self._registry.register(action)
+                return cls
 
             return __decorator
 
         def action(
             self, name: str
         ) -> Optional[Callable[[Callable[..., Any]], Callable[..., Any]]]:
-            def __decorator(func: Callable[..., Any]):
+            def __decorator(func: Callable[..., Any]) -> Callable[..., Any]:
                 # LINT: check if function on decorated class is a function
                 assert callable(func)
                 namespace = name.split(".")[0]
 
                 location = Location.from_function(func)
                 function = data.Function(
                     namespace=namespace,
@@ -552,14 +568,15 @@
                     name=name,
                     description=func.__doc__,
                     location=location,
                     parent_name=self._context.name,
                     parent_type=data.Context,
                 )
                 self._registry.register(action)
+                return func
 
             return __decorator
 
         def capture(
             self, name: Optional[str] = None, rule: Optional[str] = None
         ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
             def __decorator(func: Callable[..., Any]) -> Callable[..., Any]:
```

### Comparing `talondoc-0.5.1/src/talondoc/analysis/static/talon.py` & `talondoc-0.6.0/src/talondoc/analysis/static/talon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Iterator, List, Optional, Sequence
+from typing import Iterator, Sequence
 
 from tree_sitter_talon import (
     ParseError,
     TalonAssignmentStatement,
     TalonCommandDeclaration,
     TalonDeclaration,
     TalonDeclarations,
```

### Comparing `talondoc-0.5.1/src/talondoc/description/__init__.py` & `talondoc-0.6.0/src/talondoc/description/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import dataclasses
 import re
-from collections.abc import Iterable
+from collections.abc import Iterable, Sequence
+from dataclasses import dataclass, field
 from typing import Optional, Union
 
 import docstring_parser
 
 from .._util.logging import getLogger
 
 _LOGGER = getLogger(__name__)
 
 
-@dataclasses.dataclass
+@dataclass
 class InvalidInterpolation(Exception):
     """Exception raised when attempting to interpolate a multiline doc string."""
 
     argument: Optional["Description"]
     template: Optional["StepsTemplate"] = None
 
     def __str__(self) -> str:
@@ -31,74 +31,74 @@
         """
         return Steps(())
 
 
 DescLike = Union[None, str, Description, Iterable[Description]]
 
 
-@dataclasses.dataclass
+@dataclass
 class Value(Description):
     """
     The description of a value.
     """
 
     desc: str
 
     def __str__(self) -> str:
         return self.desc
 
     def as_steps(self) -> "Steps":
         return Steps(steps=(Step(self),))
 
 
-@dataclasses.dataclass
+@dataclass
 class Step(Description):
     """
     The description of one step in a series of steps.
     """
 
     desc: Union[str, Value]
 
     def __str__(self) -> str:
         return str(self.desc)
 
     def as_steps(self) -> "Steps":
         return Steps(steps=(self,))
 
 
-@dataclasses.dataclass
+@dataclass
 class Steps(Description):
     """
     The description of a series of steps.
     """
 
-    steps: tuple[Step, ...] = dataclasses.field(default_factory=tuple)
+    steps: Sequence[Step] = field(default_factory=tuple)
 
     def __str__(self) -> str:
         return "\n".join(str(step) for step in self.steps)
 
     def as_steps(self) -> "Steps":
         return self
 
 
-@dataclasses.dataclass
+@dataclass
 class StepsTemplate(Description):
     template: str
-    names: tuple[str, ...]
+    names: Sequence[str]
 
-    def __call__(self, values: tuple[Optional[Description], ...]) -> Steps:
+    def __call__(self, values: Sequence[Optional[Description]]) -> Steps:
         ret = self.template
         for name, value in zip(self.names, values):
             if isinstance(value, Value):
                 ret = ret.replace(f"<{name}>", value.desc)
             else:
                 raise InvalidInterpolation(argument=value, template=self)
         return Steps(steps=tuple(Step(desc=desc) for desc in ret.splitlines()))
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.template
 
     def as_steps(self) -> "Steps":
         return Steps(steps=(Step(desc=str(self)),))
 
 
 def and_then(
```

### Comparing `talondoc-0.5.1/src/talondoc/description/describer.py` & `talondoc-0.6.0/src/talondoc/description/describer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Callable
 from functools import singledispatchmethod
-from typing import Optional, TypeVar
+from typing import Any, Optional, TypeVar
 
 from tree_sitter_talon import (
     Node,
     TalonAction,
     TalonAssignmentStatement,
     TalonBinaryOperator,
     TalonBlock,
@@ -83,15 +83,15 @@
         return Value(f"<{ast.text}>")
 
     @describe.register
     def _(self, ast: TalonKeyAction) -> Optional[Description]:
         return Step(f"Press {ast.arguments.text.strip()}.")
 
     @describe.register
-    def _(self, ast: TalonSleepAction, **kwargs) -> Optional[Description]:
+    def _(self, ast: TalonSleepAction, **kwargs: Any) -> Optional[Description]:
         return None
 
     def get_docstring(
         self,
         cls: type[Data],
         name: str,
     ) -> Optional[str]:
```

### Comparing `talondoc-0.5.1/src/talondoc/sphinx/__init__.py` & `talondoc-0.6.0/src/talondoc/sphinx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from collections.abc import Callable
+from collections.abc import Callable, Sequence
 from pathlib import Path
-from typing import Any, Optional, Sequence, Union, cast
+from typing import Any, Optional, Union, cast
 
 from sphinx.application import BuildEnvironment, Sphinx
 from typing_extensions import TypeGuard
 
 from .._util.logging import getLogger
 from .._version import __version__
 from ..analysis.registry import NoActiveFile, NoActivePackage, NoActiveRegistry
@@ -81,15 +81,15 @@
                     for talon_package in talon_packages
                 ),
             )
         )
     raise TypeError(type(talon_packages))
 
 
-def _canonicalize_vararg(vararg: Union[None, str, Sequence[str]]) -> tuple[str, ...]:
+def _canonicalize_vararg(vararg: Union[None, str, Sequence[str]]) -> Sequence[str]:
     if vararg is None:
         return ()
     if type(vararg) == str:
         return (vararg,)
     if isinstance(vararg, Sequence):
         return tuple(vararg)
     raise TypeError(type(vararg))
@@ -107,15 +107,15 @@
     talon_packages = _canonicalize_talon_packages(env.config["talon_packages"])
     if talon_packages:
         buffer.extend(talon_packages)
 
     return buffer
 
 
-def _talondoc_load_package(app: Sphinx, env: BuildEnvironment, *args):
+def _talondoc_load_package(app: Sphinx, env: BuildEnvironment, *args: Any) -> None:
     try:
         talon_domain = cast(TalonDomain, env.get_domain("talon"))
         talon_packages = _talon_packages(env)
         srcdir = Path(env.srcdir)
         for talon_package in talon_packages:
             package_dir = srcdir / talon_package["path"]
 
@@ -164,15 +164,15 @@
 
     app.add_config_value(
         name="talon_packages",
         default=None,
         rebuild="env",
         types=[
             list,  # list[TalonPackage]
-            tuple,  # tuple[TalonPackage]
+            tuple,  # Tuple[TalonPackage]
         ],
     )
 
     app.connect("env-before-read-docs", _talondoc_load_package)
 
     return {
         "version": __version__,
```

### Comparing `talondoc-0.5.1/src/talondoc/sphinx/_util/addnodes.py` & `talondoc-0.6.0/src/talondoc/sphinx/_util/addnodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from collections.abc import Iterable
-from typing import Any, Sequence, TypeVar, Union
+from collections.abc import Iterable, Sequence
+from typing import Any, TypeVar, Union
 
 from docutils import nodes
 from sphinx import addnodes
 
 NodeVar = TypeVar("NodeVar", bound=nodes.Node)
 
 AttributeValue = Union[Any, Sequence[Any]]
```

### Comparing `talondoc-0.5.1/src/talondoc/sphinx/directives/__init__.py` & `talondoc-0.6.0/src/talondoc/sphinx/directives/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from collections.abc import Callable
 from typing import TYPE_CHECKING, Any, Optional, cast
 
 import sphinx.directives
+from docutils import nodes
+from sphinx import addnodes
+from talonfmt import talonfmt
+from typing_extensions import final
+
+from ...analysis.registry import data
 
 if TYPE_CHECKING:
     from ..domains import TalonDomain
 else:
     TalonDomain = Any
 
 
-class TalonDocDirective(sphinx.directives.SphinxDirective):
+class TalonDocDirective(sphinx.directives.SphinxDirective):  # type: ignore[misc, name-defined]
     @property
     def talon(self) -> TalonDomain:
         return cast(TalonDomain, self.env.get_domain("talon"))
 
     @property
     def docstring_hook(self) -> Callable[[str, str], Optional[str]]:
         docstring_hook = self.env.config["talon_docstring_hook"]
@@ -37,9 +43,15 @@
                 value = docstring_hook(sort, name)
                 assert value is None or isinstance(value, str)
                 return value
 
             return __docstring_hook
 
 
-class TalonDocObjectDescription(sphinx.directives.ObjectDescription, TalonDocDirective):
+class TalonDocObjectDescription(
+    sphinx.directives.ObjectDescription[str], TalonDocDirective  # type: ignore[misc]
+):
     pass
+
+    @final
+    def describe_rule(self, rule: data.Rule) -> nodes.Text:
+        return nodes.Text(talonfmt(rule, safe=False))
```

### Comparing `talondoc-0.5.1/src/talondoc/sphinx/directives/command/__init__.py` & `talondoc-0.6.0/src/talondoc/sphinx/directives/command/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sys
-from typing import List
 
 from sphinx import addnodes
 from sphinx.util.typing import OptionSpec
 from typing_extensions import override
 
 from ...._util.logging import getLogger
+from ....analysis.registry.data.abc import UnknownReference
 from ..._util.typing import flag, optional_strlist
-from ..errors import AmbiguousSignature, UnmatchedSignature
+from ..errors import AmbiguousSignature
 from .abc import TalonDocCommandDescription
 
 _LOGGER = getLogger(__name__)
 
 
 class TalonCommandDirective(TalonDocCommandDescription):
     has_content = True
@@ -21,24 +21,24 @@
         "context": optional_strlist,
         "contexts": optional_strlist,
         "always_include_script": flag,
     }
     final_argument_whitespace = False
 
     @override
-    def get_signatures(self) -> List[str]:
+    def get_signatures(self) -> list[str]:
         return [" ".join(self.arguments)]
 
     @override
-    def handle_signature(self, sig: str, signode: addnodes.desc_signature):
+    def handle_signature(self, sig: str, signode: addnodes.desc_signature) -> str:
         try:
             command = self.find_command(sig, fullmatch=False, restrict_to=self.contexts)
             signode = self.describe_command(
                 command,
                 signode,
                 always_include_script=self.always_include_script,
                 docstring_hook=self.docstring_hook,
             )
             return command.name
-        except (UnmatchedSignature, AmbiguousSignature) as e:
+        except (UnknownReference, AmbiguousSignature) as e:
             _LOGGER.error(e)
             raise ValueError(e)
```

### Comparing `talondoc-0.5.1/src/talondoc/sphinx/directives/command/abc.py` & `talondoc-0.6.0/src/talondoc/sphinx/directives/command/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 from sphinx import addnodes
 from talonfmt import talonfmt
 from tree_sitter_talon import TalonComment
 from typing_extensions import final
 
 from ...._util.logging import getLogger
 from ....analysis.registry import data
+from ....analysis.registry.data.abc import UnknownReference
 from ....description import InvalidInterpolation
 from ....description.describer import TalonScriptDescriber
 from ....sphinx.directives import TalonDocObjectDescription
 from ....sphinx.typing import TalonDocstringHook_Callable
 from ..._util.addnodes import desc_content, desc_name, paragraph
-from ..errors import AmbiguousSignature, UnmatchedSignature
+from ..errors import AmbiguousSignature
 
 _LOGGER = getLogger(__name__)
 
 
 class TalonDocCommandDescription(TalonDocObjectDescription):
     @property
     def contexts(self) -> Optional[Iterator[str]]:
@@ -37,15 +38,17 @@
         fullmatch: bool = False,
         restrict_to: Optional[Iterator[str]] = None,
     ) -> data.Command:
         commands = list(
             self.find_commands(text, fullmatch=fullmatch, restrict_to=restrict_to)
         )
         if len(commands) == 0:
-            raise UnmatchedSignature(self.get_location(), text)
+            raise UnknownReference(
+                ref_type=data.Command, ref_name=text, location=self.get_location()
+            )
         if len(commands) >= 2:
             raise AmbiguousSignature(
                 self.get_location(),
                 text,
                 [
                     f"{command.location}: {talonfmt(command.rule, safe=False)}"
                     for command in commands
@@ -100,18 +103,14 @@
                 always_include_script=always_include_script,
                 docstring_hook=docstring_hook,
             )
         )
         return signode
 
     @final
-    def describe_rule(self, rule: data.Rule) -> nodes.Text:
-        return nodes.Text(talonfmt(rule, safe=False))
-
-    @final
     def describe_script(
         self,
         command: data.Command,
         *,
         always_include_script: bool,
         docstring_hook: Optional[TalonDocstringHook_Callable],
     ) -> Sequence[nodes.Element]:
```

### Comparing `talondoc-0.5.1/src/talondoc/sphinx/directives/command/hlist.py` & `talondoc-0.6.0/src/talondoc/sphinx/directives/command/hlist.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.5.1/src/talondoc/sphinx/directives/command/table.py` & `talondoc-0.6.0/src/talondoc/sphinx/directives/command/table.py`

 * *Files identical despite different names*

### Comparing `talondoc-0.5.1/src/talondoc/sphinx/typing.py` & `talondoc-0.6.0/src/talondoc/sphinx/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from collections.abc import Callable
-from typing import Optional, Sequence, Union
+from collections.abc import Callable, Sequence
+from typing import Optional, Union
 
 from typing_extensions import NotRequired, Required, TypeAlias, TypedDict
 
 TalonEvent = str
 
 TalonPackage = TypedDict(
     "TalonPackage",
```

### Comparing `talondoc-0.5.1/src/talondoc.egg-info/PKG-INFO` & `talondoc-0.6.0/src/talondoc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talondoc
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Sphinx extension for Talon user directories.
 Author-email: Wen Kokke <wenkokke@users.noreply.github.com>
 Keywords: talon,sphinx
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `talondoc-0.5.1/src/talondoc.egg-info/SOURCES.txt` & `talondoc-0.6.0/src/talondoc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 src/talondoc/_autogen/resources/index.md.jinja2
 src/talondoc/_autogen/resources/index.rst.jinja2
 src/talondoc/_autogen/resources/python_file.md.jinja2
 src/talondoc/_autogen/resources/python_file.rst.jinja2
 src/talondoc/_autogen/resources/talon_file.md.jinja2
 src/talondoc/_autogen/resources/talon_file.rst.jinja2
 src/talondoc/_cache_builtin/__init__.py
+src/talondoc/_cache_builtin/resources/talon.json
 src/talondoc/_util/__init__.py
 src/talondoc/_util/io.py
 src/talondoc/_util/logging.py
 src/talondoc/_util/progress_bar.py
 src/talondoc/analysis/__init__.py
 src/talondoc/analysis/live/__init__.py
 src/talondoc/analysis/live/resources/get_actions.py
 src/talondoc/analysis/live/resources/get_captures.py
 src/talondoc/analysis/live/resources/get_commands.py
 src/talondoc/analysis/live/resources/get_lists.py
 src/talondoc/analysis/live/resources/get_modes.py
 src/talondoc/analysis/live/resources/get_settings.py
 src/talondoc/analysis/live/resources/get_tags.py
 src/talondoc/analysis/live/resources/get_version.py
-src/talondoc/analysis/live/resources/talon_actions_dict-0.3.1-437-g8fea.json
 src/talondoc/analysis/registry/__init__.py
 src/talondoc/analysis/registry/data/__init__.py
 src/talondoc/analysis/registry/data/abc.py
 src/talondoc/analysis/registry/data/serialise.py
 src/talondoc/analysis/static/__init__.py
 src/talondoc/analysis/static/talon.py
 src/talondoc/analysis/static/python/__init__.py
```

