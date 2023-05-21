# Comparing `tmp/embykeeper-2.0.9.tar.gz` & `tmp/embykeeper-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.0.9.tar", last modified: Fri Apr 21 22:15:30 2023, max compression
+gzip compressed data, was "embykeeper-2.1.0.tar", last modified: Sun May 21 21:04:36 2023, max compression
```

## Comparing `embykeeper-2.0.9.tar` & `embykeeper-2.1.0.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.964925 embykeeper-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 22:15:17.000000 embykeeper-2.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18790 2023-04-21 22:15:30.964925 embykeeper-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-04-21 22:15:17.000000 embykeeper-2.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.956925 embykeeper-2.0.9/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.960925 embykeeper-2.0.9/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.960925 embykeeper-2.0.9/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.960925 embykeeper-2.0.9/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.964925 embykeeper-2.0.9/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.964925 embykeeper-2.0.9/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/pornemby_exam.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-21 22:15:17.000000 embykeeper-2.0.9/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.956925 embykeeper-2.0.9/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18790 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 22:15:30.000000 embykeeper-2.0.9/embykeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-21 22:15:17.000000 embykeeper-2.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 22:15:30.964925 embykeeper-2.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:15:30.964925 embykeeper-2.0.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-21 22:15:17.000000 embykeeper-2.0.9/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.032250 embykeeper-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 21:04:25.000000 embykeeper-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-05-21 21:04:36.032250 embykeeper-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19758 2023-05-21 21:04:25.000000 embykeeper-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.020250 embykeeper-2.1.0/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.024250 embykeeper-2.1.0/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.024250 embykeeper-2.1.0/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.028250 embykeeper-2.1.0/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.028250 embykeeper-2.1.0/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.032250 embykeeper-2.1.0/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13927 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-21 21:04:25.000000 embykeeper-2.1.0/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.024250 embykeeper-2.1.0/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:04:35.000000 embykeeper-2.1.0/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 21:04:36.000000 embykeeper-2.1.0/embykeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-21 21:04:25.000000 embykeeper-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:04:36.032250 embykeeper-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:04:36.032250 embykeeper-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-21 21:04:25.000000 embykeeper-2.1.0/tests/test_cli.py
```

### Comparing `embykeeper-2.0.9/LICENSE` & `embykeeper-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.9/PKG-INFO` & `embykeeper-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.0.9
+Version: 2.1.0
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper) [![telegram badge](https://img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
+[![build status](https://img.shields.io/github/actions/workflow/status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
 
 <p align="center">
   <a href='https://github.com/embykeeper/embykeeper'>
-    <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
+    <img src="https://github.com/embykeeper/embykeeper/raw/main/images/logo.svg" alt="Embykeeper" />
   </a>
 </p>
 <p align="center">
     <b>自动签到 定时保号 按需水群</b>
 </p>
 
 ---
@@ -35,50 +35,54 @@
 
 ## 声明
 
 本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
 本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
-本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Telegram 讨论组](https://t.me/embykeeper_chat) 与开发团队进行交流.
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论.
 
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
-  - 支持群组
-    - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
-    - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
-    - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
-    - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
-    - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
-    - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
-    - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
-    - Pornemby (_测试中_): [频道](https://t.me/pornembyservice) [机器人](https://t.me/PronembyTGBot2_bot)
-    - 其他非 Emby 相关:
-      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_): [机器人](https://t.me/sosdbot)
-    - 默认禁用:
-      - Pornemby 科举考试 (_测试中_): [活动频道](https://t.me/PornembyFun)
-      - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-      - ~~垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)~~ (无响应)
-  - 特性
-    - 验证码识别与自动重试
-    - 多账户签到
-    - 网页类型签到
+  - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
+  - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
+  - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
+  - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
+  - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+  - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
+  - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
+  - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
+  - 其他非 Emby 相关:
+    - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
+  - 默认禁用:
+    - ~~卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)~~ (机器人逻辑频繁变动, 暂时禁用)
+    - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
+    - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
+
 - Emby 保活
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
+
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
-  - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
+  - 默认禁用:
+    - ~~NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)~~ (停服)
+
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
+  - Pornemby 科举考试: [活动频道](https://t.me/PornembyFun) (由于需要使用 OpenAI API 进行回答, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime), 回答准确率一般请谨慎使用)
   - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
+  - Viper 抢邀请码: [频道](https://t.me/viper_emby_channel) [群组](https://t.me/Viper_Emby_Chat) [机器人](https://t.me/viper_emby_bot)
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+  - Misty 开注自动注册: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
+  - 默认禁用:
+    - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
 ### 从 PyPi 安装
 
 Embykeeper 可以通过 `python` 运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
 
@@ -90,15 +94,34 @@
 
 随后, 您需要执行:
 
 ```bash
 embykeeper
 ```
 
-命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)).
+命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = 1080
+scheme = "socks5"
+
+[[telegram]]
+api_id = "27894236"
+api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899"
+
+[[emby]]
+url = "https://weiss-griffin.com/"
+username = "carrie19"
+password = "s*D7MMCpS$"
+```
+
+对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
 
 随后, 您需要再次执行:
 
 ```bash
 embykeeper
 ```
 
@@ -124,144 +147,147 @@
 
 ```
 pip install -U embykeeper
 ```
 
 然后重新运行应用.
 
-### 从 Docker 安装
+### 从源码构建
 
-Embykeeper 可以通过 `docker` 运行, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
 
 ```bash
-touch config.toml
-docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
+git clone https://github.com/embykeeper/embykeeper.git
+cd embykeeper
+pip install -e .
 ```
 
-命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+然后即可执行 Embykeeper:
 
-```toml
-[proxy]
-hostname = "127.0.0.1"
-port = "1080"
-scheme = "socks5"
+```bash
+embykeeper
+```
 
-[[telegram]]
-api_id = "27894236"
-api_hash = "622159182fdd4b15b627eeb3ac695271"
-phone = "+8612109347899"
+详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
+
+当版本更新时, 您需要执行:
 
-[[emby]]
-url = "https://weiss-griffin.com/"
-username = "carrie19"
-password = "s*D7MMCpS$"
+```
+git pull
 ```
 
-对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
+然后重新运行应用.
 
-随后, 您需要再次执行:
+### 从 Docker 部署
+
+Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
-docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
-您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息 (详见[从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)).
 
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+随后, 您需要再次执行:
 
 ```bash
-docker run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
-或者使用 [docker-compose](https://docs.docker.com/compose/) ([watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务):
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper.
+
+### 通过 Docker Compose 部署
+
+您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
+
+**注意**: 您需要先进行过 [从 Docker 部署](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
+
+您需要新建一个文件 `docker-compose.yml`:
 
 ```yaml
 version: '3'
 services:
   embykeeper:
     container_name: embykeeper
-    image: cembykeeper/embykeeper
+    image: embykeeper/embykeeper
     restart: unless-stopped
     volumes:
-      - ./config.toml:/app/config.toml
+      - ./embykeeper:/app
+    network_mode: host
   watchtower:
     container_name: watchtower
     image: containrrr/watchtower
     restart: unless-stopped
     volumes:
       - /var/run/docker.sock:/var/run/docker.sock:rw
 ```
 
-即可在后台启动 embykeeper.
-
-您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
-
-如果您需要使用主机上的代理服务器 (例如 `https://localhost:1080`), 您可能需要使用 `--net=host` 参数以使用主机网络模式.
-
-### 从源码构建
-
-和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
-
-```bash
-git clone https://github.com/embykeeper/embykeeper.git
-cd embykeeper
-pip install -e .
-```
+其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务.
 
-然后即可执行 Embykeeper:
+然后运行以下命令以启动:
 
 ```bash
-embykeeper
+docker-compose up -d
 ```
 
-详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
-
-当版本更新时, 您需要执行:
-
-```
-git pull
-```
+即可在后台启动 embykeeper.
 
-然后重新运行应用.
+您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
 
 ## 命令行帮助
 
 您可以通过运行 `embykeeper -h` 以获取帮助:
 
 ```bash
 $ embykeeper -h
 
 欢迎使用 Embykeeper. 🎦 无参数默认开启全部功能.
 
 参数:
     config  配置文件 (置空以生成)
 模块开关:
-    --checkin     -c   启用每日指定时间签到 (不指定值时默认为6:00PM)
+    --checkin     -c   启用每日签到 (不指定值时默认为<8:00PM,9:00PM>随机时间)
     --emby        -e   启用每隔天数Emby自动保活 (不指定值时默认为每7天)
     --monitor     -m   启用群聊监视
     --send        -s   启用自动水群
 调试参数:
     --no-instant  -I   不立刻执行一次计划任务
-    --debug       -d   开启调试模式, 错误将会导致程序停止运行
+    --once        -o   仅执行一次任务而不计划执行
+    --debug       -d   开启调试输出, 错误将会导致程序停止运行
     --version     -v   打印 Embykeeper 版本
     --follow      -f   仅启动消息调试
     --analyze     -a   仅启动历史信息分析
+    --basedir          设定输出文件默认位置
 ```
 
 例如:
 
 ```bash
+# 启动所有功能 (在各账号配置中进一步设置功能开启/关闭)
+$ embykeeper config.toml
+
 # 仅启动每日签到
 $ embykeeper config.toml -c
 
 # 仅启动每日 8:00 PM 签到
 $ embykeeper config.toml -c 8:00PM
 
+# 仅启动每日 8:00 PM - 9:00 PM 随机时间签到
+$ embykeeper config.toml -c <8:00PM,9:00PM>
+
 # 启动所有功能, 同时调整签到时间为 8:00 AM, 调整保活间隔天数为 14
 $ embykeeper config.toml -c 8:00PM -e 14 -m -s
+
+# 启动所有功能, 只运行一次
+$ embykeeper config.toml --once
+
+# 启动所有功能, 不立即执行一次签到/保活
+$ embykeeper config.toml -I
 ```
 
 您也可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
 
 ```bash
 # 启动历史信息分析
 $ embykeeper config.toml -a
@@ -296,24 +322,24 @@
 
 ##### 开发者团队
 
 - [jackzzs](https://github.com/jackzzs)
 
 ##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
 
-![kitty](images/kitty.gif)
+![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
 
 ## 配置项
 
 | 设置项       | 值类型             | 简介                                         | 默认值  |
 | ------------ | ------------------ | -------------------------------------------- | ------- |
 | `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `10`    |
+| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`    |
 | `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
-| `random`     | `int`              | Telegram 机器人签到定时任务时间随机量 (分钟) | `15`    |
+| `random`     | `int`              | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
 | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
 | `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
 | `proxy`      | `dict`             | 代理设置                                     | `{}`    |
 | `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
 | `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
 
 `service`设置可以为:
@@ -331,15 +357,15 @@
 | 站点 | 名称 | | 站点 | 名称 |
 | --- | --- | --- |--- | --- |
 | 垃圾影音 | `ljyy` | | 搜书神器 | `sosdbot` |
 | 卷毛鼠 IPTV | `jms_iptv` | | 终点站 | `terminus` |
 | Pornemby | `pornemby` | | Singularity | `singularity` |
 | Peach | `peach` | | Nebula | `nebula` |
 | Bluesea | `bluesea` | | Embyhub | `embyhub` |
-| 卷毛鼠 | `jms` | | | |
+| 卷毛鼠 | `jms` | | 卡戎 | `charon` |
 
 `proxy` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                    | 默认值      |
 | ---------- | ------ | --------------------------------------- | ----------- |
 | `hostname` | `str`  | 代理服务器地址                          | `localhost` |
 | `port`     | `int`  | 代理端口号                              | `1080`      |
@@ -361,14 +387,25 @@
 | ---------- | ------ | --------------------------------------------------------- | ------ |
 | `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
 | `username` | `str`  | Emby 服务器用户名                                         |        |
 | `password` | `str`  | Emby 服务器密码                                           |        |
 | `time`     | `int`  | 模拟观看的时间 (秒)                                       | `800`  |
 | `progress` | `int`  | 观看后模拟进度条保存的时间 (秒)                           | `1000` |
 
+服务可以进行特定配置, 如下所示:
+
+```toml
+
+[monitor.bgk] # 支持 bgk, embyhub, polo
+unique_name = "your_username_for_registeration" # 自动抢注时使用的用户名
+
+[monitor.pornemby]
+only_history = true # 仅当问题历史中找到答案时自动回答
+```
+
 ## 代码重用与开发
 
 代码架构如下:
 
 ```mermaid
 flowchart TD
     A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
@@ -415,7 +452,11 @@
                 await self.retry()
                 break
 ```
 
 上述代码实现每次按对应一个字符按键的功能.
 
 当您实现一个新的签到器时, 欢迎您提出 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 以帮助更多人使用!
+
+## 趋势
+
+[![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

#### html2text {}

```diff
@@ -1,29 +1,31 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.0.9 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.1.0 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
 :: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: <3.11,>=3.7 Description-Content-Type: text/markdown License-
-File: LICENSE [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https:/
-/pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/
-dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
+Requires-Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-
+File: LICENSE [![build status](https://img.shields.io/github/actions/workflow/
+status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/
+embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/
+v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https:
+//img.shields.io/pypi/dm/
+embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
 embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
 embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
 embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
 [telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
 embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
-channel-green)](https://t.me/embykeeper) [![telegram badge](https://
-img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
+channel-green)](https://t.me/embykeeper)
                                  [Embykeeper]
                     èªå¨ç­¾å° å®æ¶ä¿å· æéæ°´ç¾¤
 --- Embykeeper æ¯ä¸ä¸ªå¨ä¸­æç¤¾ç¾¤è§åä¸ç¨äº Emby
 å½±è§æå¡å¨çç­¾å°åä¿å·çèªå¨æ§è¡å·¥å·, åºäº Pyrogram
 ç¼åå¹¶å·æå¯æå±æ§. ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
 æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³, å¨ä½¿ç¨ Embykeeper
 æ¶é æçä¸åæå¤± (åæ¬ä½ä¸éäº Emby æ Telegram
@@ -36,127 +38,143 @@
 å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
 å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
 æ¬é¡¹ç®ä»æä¾å·¥å·,
 å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
 å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
-æ¨ä¹å¯ä»¥éè¿ [Telegram è®¨è®ºç»](https://t.me/embykeeper_chat)
-ä¸å¼åå¢éè¿è¡äº¤æµ. å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½,
-è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper Auth Bot](https://t.me/
-embykeeper_auth_bot)" åéå³é®çæå/å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper
-Bot](https://t.me/embykeeper_bot)" åæ¨æ¨é,
-æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
+å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
+Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
+å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
+åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
-æºå¨äººç­¾å° - æ¯æç¾¤ç» - ç»ç¹ç«: [é¢é](https://t.me/embypub)
-[ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) -
-å·æ¯é¼ : [é¢é]() [ç¾¤ç»](https://t.me/Curly_Mouse) [æºå¨äºº](https://
-t.me/jmsembybot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»](https://
-t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
-(ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
-t.me/embykeeper_bot?start=__prime)) - BlueSea: [ç¾¤ç»](https://t.me/
-blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot) - Singularity: [é¢é]
-(https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/
-Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach:
-[é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
+æºå¨äººç­¾å° - ç»ç¹ç«: [é¢é](https://t.me/embypub) [ç¾¤ç»](https://
+t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) - Nebula: [é¢é]
+(https://t.me/Nebula_Emby) [ç¾¤ç»](https://t.me/NebulaEmbyUser) [æºå¨äºº]
+(https://t.me/Nebula_Account_bot) (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare
+éªè¯ç , éè¦[é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) -
+Singularity: [é¢é](https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://
+t.me/Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) -
+Peach: [é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
 peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
 (https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
-t.me/EdHubot) - Pornemby (_æµè¯ä¸­_): [é¢é](https://t.me/pornembyservice)
-[æºå¨äºº](https://t.me/PronembyTGBot2_bot) - å¶ä»é Emby ç¸å³: -
-æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/pull/8)
-å¢å ) (_æµè¯ä¸­_): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
-Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_): [æ´»å¨é¢é](https://t.me/PornembyFun) -
+t.me/EdHubot) - Pornemby: [é¢é](https://t.me/pornembyservice) [ç¾¤ç»]
+(https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
+åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
+t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
+t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
+ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
+pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
+~~å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https://t.me/
+Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot)~~
+(æºå¨äººé»è¾é¢ç¹åå¨, ææ¶ç¦ç¨) - ~~BlueSea: [ç¾¤ç»](https://t.me/
+blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~ (æ ååº) -
 ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/
-Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) -
-~~åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
-t.me/zckllflbot)~~ (æ ååº) - ç¹æ§ - éªè¯ç è¯å«ä¸èªå¨éè¯ -
-å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby ä¿æ´» -
-å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
-èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
-è¯·è°¨æä½¿ç¨) - NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork)
-[æºå¨äºº](https://t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦
-[è¶çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç
-æ¢éè¯·ç : [ç¾¤ç»](https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/
-UnknownEmbyBot) - Embyhub å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub)
-[ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) ##
-å®è£ä¸ä½¿ç¨ ### ä» PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡,
-æ¨å¯ä»¥éè¿ [conda](https://github.com/conda/conda) æ [virtualvenv]
-(https://virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿
-`pip` å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
-embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
-github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)). éå,
-æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) - Emby
+ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
+Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
+t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
+Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
+embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
+t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
+[é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime),
+åç­åç¡®çä¸è¬è¯·è°¨æä½¿ç¨) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»](https:
+//t.me/Ephemeralemby) [æºå¨äºº](https://t.me/UnknownEmbyBot) - Viper
+æ¢éè¯·ç : [é¢é](https://t.me/viper_emby_channel) [ç¾¤ç»](https://t.me/
+Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
+å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
+emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
+[é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
+[æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
+[é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
+(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### ä»
+PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡, æ¨å¯ä»¥éè¿ [conda]
+(https://github.com/conda/conda) æ [virtualvenv](https://virtualenv.pypa.io/
+) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip` å®è£ `embykeeper`
+(éè¦ `python >= 3.7, < 3.11`): ```bash pip install embykeeper ``` éå,
+æ¨éè¦æ§è¡: ```bash embykeeper ``` å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿
+`config.toml` æä»¶, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
+(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [proxy] hostname =
+"127.0.0.1" port = 1080 scheme = "socks5" [[telegram]] api_id = "27894236"
+api_hash = "622159182fdd4b15b627eeb3ac695271" phone = "+8612109347899" [[emby]]
+url = "https://weiss-griffin.com/" username = "carrie19" password =
+"s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿ [Telegram å®ç½]
+(https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
+development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
+æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
+æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
+æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡:
+```bash embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
+ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
 Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
 ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿
-`docker` è¿è¡, æ¨é [å®è£ docker](https://yeasy.gitbook.io/
-docker_practice/install), ç¶åæ§è¡: ```bash touch config.toml docker run -
-v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
-```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme = "socks5" [
-[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
-phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
-"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
-[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
-ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
-è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
-"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
-æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
-éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/config.toml:/app/
-config.toml --rm -it embykeeper/embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º åä» PyPi
+å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python ç¯å¢, ç¶åæå Github
+å¹¶å®è£: ```bash git clone https://github.com/embykeeper/embykeeper.git cd
+embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash
+embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/
+embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ### ä» Docker
+é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://
+yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡: ```bash docker run -
+v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
+å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯ (è¯¦è§[ä» Pypi å®è£](https://github.com/
+embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)). éå,
+æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
+net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
+ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash docker
-run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper ```
-æèä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) ([watchtower]
-(https://github.com/containrrr/watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡):
-```yaml version: '3' services: embykeeper: container_name: embykeeper image:
-cembykeeper/embykeeper restart: unless-stopped volumes: - ./config.toml:/app/
-config.toml watchtower: container_name: watchtower image: containrrr/watchtower
-restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/docker.sock:rw
-``` å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -
-f embykeeper` æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿.
-å¦ææ¨éè¦ä½¿ç¨ä¸»æºä¸çä»£çæå¡å¨ (ä¾å¦ `https://localhost:
-1080`), æ¨å¯è½éè¦ä½¿ç¨ `--net=host` åæ°ä»¥ä½¿ç¨ä¸»æºç½ç»æ¨¡å¼.
-### ä»æºç æå»º åä» PyPi å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python
-ç¯å¢, ç¶åæå Github å¹¶å®è£: ```bash git clone https://github.com/
-embykeeper/embykeeper.git cd embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡
-Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£]
-(https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
-å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
-## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
-```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. ### éè¿ Docker Compose
+é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/compose/
+) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker é¨ç½²]
+(https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2)
+æè½éè¿ `docker-compose` é¨ç½²,
+è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
+ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
+compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
+version: '3' services: embykeeper: container_name: embykeeper image:
+embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
+network_mode: host watchtower: container_name: watchtower image: containrrr/
+watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
+docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
+watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡.
+ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨: ```bash docker-compose up -d ```
+å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -f embykeeper`
+æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿. ##
+å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash
+$ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
 æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
-(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å°
-(ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´»
-(ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --monitor -m å¯ç¨ç¾¤èçè§ --send -
-s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-instant -
-I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
+(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
+(ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
+e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
+instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
+o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
-follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ ```
-ä¾å¦: ```bash # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
+follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ --
+basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® ``` ä¾å¦: ```bash # å¯å¨ææåè½
+(å¨åè´¦å·éç½®ä¸­è¿ä¸æ­¥è®¾ç½®åè½å¼å¯/å³é­) $ embykeeper
+config.toml # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
-å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
-è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -
-s ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
+ä»å¯å¨æ¯æ¥ 8:00 PM - 9:00 PM éæºæ¶é´ç­¾å° $ embykeeper config.toml -
+c <8:00PM,9:00PM> # å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
+è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -s #
+å¯å¨ææåè½, åªè¿è¡ä¸æ¬¡ $ embykeeper config.toml --once #
+å¯å¨ææåè½, ä¸ç«å³æ§è¡ä¸æ¬¡ç­¾å°/ä¿æ´» $ embykeeper config.toml
+-I ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
 ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
 config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
 10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
 "åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
 è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
 ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
 å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
@@ -170,21 +188,22 @@
 (ä¾å¦èªå¨æ¢éè¯·ç )å°éè¦é«çº§ç¨æ·, æ¨å¯ä»¥éè¿ [Embykeeper
 Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
-(https://afdian.net/a/jackzzs)èµå© ![kitty](images/kitty.gif) ## éç½®é¡¹ |
-è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ------------ | -----------------
-- | -------------------------------------------- | ------- | | `timeout` |
-`int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | | `retries` | `int` |
-Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `10` | | `concurrent` | `int` |
-Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random` | `int` | Telegram
-æºå¨äººç­¾å°å®æ¶ä»»å¡æ¶é´éæºé (åé) | `15` | | `notifier` |
+(https://afdian.net/a/jackzzs)èµå© ![Kitty](https://github.com/embykeeper/
+embykeeper/raw/main/images/kitty.gif) ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å |
+ç®ä» | é»è®¤å¼ | | ------------ | ------------------ | --------------------
+------------------------ | ------- | | `timeout` | `int` | Telegram
+æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | | `retries` | `int` | Telegram
+æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | | `concurrent` | `int` | Telegram
+æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random` | `int` | Telegram
+æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` | | `notifier` |
 `int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/ææºå·) |
 `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/çè§åè½å¼å¯ç«ç¹è®¾ç½® |
 `{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `{}` | | `telegram` | `list` |
 Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | | `emby` | `list` | Emby
 è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
 å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------- | ------ | -------------- | ----
 ---------------- | | `checkiner` | `list` | å¯ç¨çç­¾å°ç«ç¹ |
@@ -195,18 +214,18 @@
 æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
 è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
 æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
 ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | --- | --- | --- |--- | --- | |
 åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` | | å·æ¯é¼  IPTV |
 `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby | `pornemby` | | Singularity
 | `singularity` | | Peach | `peach` | | Nebula | `nebula` | | Bluesea |
-`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | | | `proxy`
-è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
------- | --------------------------------------- | ----------- | | `hostname` |
-`str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
+`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | å¡æ | `charon` |
+`proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | -----
+----- | ------ | --------------------------------------- | ----------- | |
+`hostname` | `str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
 ä»£çç«¯å£å· | `1080` | | `scheme` | `str` | ä»£çåè®®, å¯ä»¥ä¸º
 "`socks5`" æ "`http`" | `socks5` | `telegram` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
 å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
 -------------------------------------------- | ------- | | `api_id` | `str` |
 ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID | | |
 `api_hash` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç
 Application Hash | | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
@@ -214,29 +233,34 @@
 | `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: |
 è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------
 ----------------------------------------------- | ------ | | `url` | `str` |
 Emby æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | |
 `username` | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
-## ä»£ç éç¨ä¸å¼å ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-
-terminal cli) --> B(fa:fa-telegram telechecker) A --> C(fa:fa-play embywatcher)
-B --checker--> E[fa:fa-robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --
-messager--> F[fa:fa-message Messager] C --watcher--> H[fa:fa-circle-play
-EmbyWatcher] F ---- |schedule| A ``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: -
-`embykeeper.telechecker.bots` - `embykeeper.telechecker.monitor` -
-`embykeeper.telechecker.messager` éå¸¸æ¥è¯´,
-å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
+æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
+bgk, embyhub, polo unique_name = "your_username_for_registeration" #
+èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
+ä»å½é®é¢åå²ä¸­æ¾å°ç­æ¡æ¶èªå¨åç­ ``` ## ä»£ç éç¨ä¸å¼å
+ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-
+telegram telechecker) A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-
+robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message
+Messager] C --watcher--> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A
+``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
+`embykeeper.telechecker.monitor` - `embykeeper.telechecker.messager`
+éå¸¸æ¥è¯´, å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
 ä¸­å¢å ä¸ä¸ªæä»¶ `dummy.py`: ```python from .base import BotCheckin class
 DummyCheckin(BotCheckin): name = "Dummy" bot_username = "dummy" bot_captcha_len
 = 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨, å°ä¼åç¨æ·åä¸º
 "`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4 ä½çéªè¯ç ,
 è¯å«éªè¯ç åå°åé. è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®,
 æ¨å¯ä»¥ä½¿ç¨ `AnswerBotCheckin`, æ¨ä¹å¯ä»¥éå `on_captcha`
 å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from .base import AnswerBotCheckin
 class DummyCheckin(AnswerBotCheckin): .... async def on_captcha(self, message:
 Message, captcha: str): for l in captcha: try: await self.message.click(l)
 except ValueError: self.log.info(f'æªè½æ¾å°å¯¹åº "{l}" çæé®,
 æ­£å¨éè¯.') await self.retry() break ```
 ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
 å½æ¨å®ç°ä¸ä¸ªæ°çç­¾å°å¨æ¶, æ¬¢è¿æ¨æåº [Pull Requests](https://
-github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨!
+github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! ## è¶å¿ [!
+[Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
+embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

### Comparing `embykeeper-2.0.9/README.md` & `embykeeper-2.1.0/embykeeper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,32 @@
-[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper) [![telegram badge](https://img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
+Metadata-Version: 2.1
+Name: embykeeper
+Version: 2.1.0
+Summary: Daily checkin automator for emby bots in telegram.
+Author-email: jackzzs <jackzzs@outlook.com>
+Project-URL: Homepage, https://github.com/embykeeper/embykeeper
+Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: <3.11,>=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![build status](https://img.shields.io/github/actions/workflow/status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
 
 <p align="center">
   <a href='https://github.com/embykeeper/embykeeper'>
-    <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
+    <img src="https://github.com/embykeeper/embykeeper/raw/main/images/logo.svg" alt="Embykeeper" />
   </a>
 </p>
 <p align="center">
     <b>自动签到 定时保号 按需水群</b>
 </p>
 
 ---
@@ -15,50 +35,54 @@
 
 ## 声明
 
 本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
 本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
-本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Telegram 讨论组](https://t.me/embykeeper_chat) 与开发团队进行交流.
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论.
 
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
-  - 支持群组
-    - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
-    - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
-    - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
-    - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
-    - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
-    - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
-    - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
-    - Pornemby (_测试中_): [频道](https://t.me/pornembyservice) [机器人](https://t.me/PronembyTGBot2_bot)
-    - 其他非 Emby 相关:
-      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_): [机器人](https://t.me/sosdbot)
-    - 默认禁用:
-      - Pornemby 科举考试 (_测试中_): [活动频道](https://t.me/PornembyFun)
-      - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-      - ~~垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)~~ (无响应)
-  - 特性
-    - 验证码识别与自动重试
-    - 多账户签到
-    - 网页类型签到
+  - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
+  - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
+  - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
+  - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
+  - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+  - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
+  - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
+  - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
+  - 其他非 Emby 相关:
+    - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
+  - 默认禁用:
+    - ~~卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)~~ (机器人逻辑频繁变动, 暂时禁用)
+    - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
+    - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
+
 - Emby 保活
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
+
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
-  - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
+  - 默认禁用:
+    - ~~NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)~~ (停服)
+
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
+  - Pornemby 科举考试: [活动频道](https://t.me/PornembyFun) (由于需要使用 OpenAI API 进行回答, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime), 回答准确率一般请谨慎使用)
   - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
+  - Viper 抢邀请码: [频道](https://t.me/viper_emby_channel) [群组](https://t.me/Viper_Emby_Chat) [机器人](https://t.me/viper_emby_bot)
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+  - Misty 开注自动注册: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
+  - 默认禁用:
+    - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
 ### 从 PyPi 安装
 
 Embykeeper 可以通过 `python` 运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
 
@@ -70,15 +94,34 @@
 
 随后, 您需要执行:
 
 ```bash
 embykeeper
 ```
 
-命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)).
+命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = 1080
+scheme = "socks5"
+
+[[telegram]]
+api_id = "27894236"
+api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899"
+
+[[emby]]
+url = "https://weiss-griffin.com/"
+username = "carrie19"
+password = "s*D7MMCpS$"
+```
+
+对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
 
 随后, 您需要再次执行:
 
 ```bash
 embykeeper
 ```
 
@@ -104,144 +147,147 @@
 
 ```
 pip install -U embykeeper
 ```
 
 然后重新运行应用.
 
-### 从 Docker 安装
+### 从源码构建
 
-Embykeeper 可以通过 `docker` 运行, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
 
 ```bash
-touch config.toml
-docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
+git clone https://github.com/embykeeper/embykeeper.git
+cd embykeeper
+pip install -e .
 ```
 
-命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+然后即可执行 Embykeeper:
 
-```toml
-[proxy]
-hostname = "127.0.0.1"
-port = "1080"
-scheme = "socks5"
+```bash
+embykeeper
+```
 
-[[telegram]]
-api_id = "27894236"
-api_hash = "622159182fdd4b15b627eeb3ac695271"
-phone = "+8612109347899"
+详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
+
+当版本更新时, 您需要执行:
 
-[[emby]]
-url = "https://weiss-griffin.com/"
-username = "carrie19"
-password = "s*D7MMCpS$"
+```
+git pull
 ```
 
-对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
+然后重新运行应用.
 
-随后, 您需要再次执行:
+### 从 Docker 部署
+
+Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
-docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
-您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息 (详见[从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)).
 
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+随后, 您需要再次执行:
 
 ```bash
-docker run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
-或者使用 [docker-compose](https://docs.docker.com/compose/) ([watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务):
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper.
+
+### 通过 Docker Compose 部署
+
+您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
+
+**注意**: 您需要先进行过 [从 Docker 部署](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
+
+您需要新建一个文件 `docker-compose.yml`:
 
 ```yaml
 version: '3'
 services:
   embykeeper:
     container_name: embykeeper
-    image: cembykeeper/embykeeper
+    image: embykeeper/embykeeper
     restart: unless-stopped
     volumes:
-      - ./config.toml:/app/config.toml
+      - ./embykeeper:/app
+    network_mode: host
   watchtower:
     container_name: watchtower
     image: containrrr/watchtower
     restart: unless-stopped
     volumes:
       - /var/run/docker.sock:/var/run/docker.sock:rw
 ```
 
-即可在后台启动 embykeeper.
-
-您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
-
-如果您需要使用主机上的代理服务器 (例如 `https://localhost:1080`), 您可能需要使用 `--net=host` 参数以使用主机网络模式.
-
-### 从源码构建
-
-和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
-
-```bash
-git clone https://github.com/embykeeper/embykeeper.git
-cd embykeeper
-pip install -e .
-```
+其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务.
 
-然后即可执行 Embykeeper:
+然后运行以下命令以启动:
 
 ```bash
-embykeeper
+docker-compose up -d
 ```
 
-详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
-
-当版本更新时, 您需要执行:
-
-```
-git pull
-```
+即可在后台启动 embykeeper.
 
-然后重新运行应用.
+您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
 
 ## 命令行帮助
 
 您可以通过运行 `embykeeper -h` 以获取帮助:
 
 ```bash
 $ embykeeper -h
 
 欢迎使用 Embykeeper. 🎦 无参数默认开启全部功能.
 
 参数:
     config  配置文件 (置空以生成)
 模块开关:
-    --checkin     -c   启用每日指定时间签到 (不指定值时默认为6:00PM)
+    --checkin     -c   启用每日签到 (不指定值时默认为<8:00PM,9:00PM>随机时间)
     --emby        -e   启用每隔天数Emby自动保活 (不指定值时默认为每7天)
     --monitor     -m   启用群聊监视
     --send        -s   启用自动水群
 调试参数:
     --no-instant  -I   不立刻执行一次计划任务
-    --debug       -d   开启调试模式, 错误将会导致程序停止运行
+    --once        -o   仅执行一次任务而不计划执行
+    --debug       -d   开启调试输出, 错误将会导致程序停止运行
     --version     -v   打印 Embykeeper 版本
     --follow      -f   仅启动消息调试
     --analyze     -a   仅启动历史信息分析
+    --basedir          设定输出文件默认位置
 ```
 
 例如:
 
 ```bash
+# 启动所有功能 (在各账号配置中进一步设置功能开启/关闭)
+$ embykeeper config.toml
+
 # 仅启动每日签到
 $ embykeeper config.toml -c
 
 # 仅启动每日 8:00 PM 签到
 $ embykeeper config.toml -c 8:00PM
 
+# 仅启动每日 8:00 PM - 9:00 PM 随机时间签到
+$ embykeeper config.toml -c <8:00PM,9:00PM>
+
 # 启动所有功能, 同时调整签到时间为 8:00 AM, 调整保活间隔天数为 14
 $ embykeeper config.toml -c 8:00PM -e 14 -m -s
+
+# 启动所有功能, 只运行一次
+$ embykeeper config.toml --once
+
+# 启动所有功能, 不立即执行一次签到/保活
+$ embykeeper config.toml -I
 ```
 
 您也可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
 
 ```bash
 # 启动历史信息分析
 $ embykeeper config.toml -a
@@ -276,24 +322,24 @@
 
 ##### 开发者团队
 
 - [jackzzs](https://github.com/jackzzs)
 
 ##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
 
-![kitty](images/kitty.gif)
+![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
 
 ## 配置项
 
 | 设置项       | 值类型             | 简介                                         | 默认值  |
 | ------------ | ------------------ | -------------------------------------------- | ------- |
 | `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `10`    |
+| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`    |
 | `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
-| `random`     | `int`              | Telegram 机器人签到定时任务时间随机量 (分钟) | `15`    |
+| `random`     | `int`              | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
 | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
 | `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
 | `proxy`      | `dict`             | 代理设置                                     | `{}`    |
 | `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
 | `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
 
 `service`设置可以为:
@@ -311,15 +357,15 @@
 | 站点 | 名称 | | 站点 | 名称 |
 | --- | --- | --- |--- | --- |
 | 垃圾影音 | `ljyy` | | 搜书神器 | `sosdbot` |
 | 卷毛鼠 IPTV | `jms_iptv` | | 终点站 | `terminus` |
 | Pornemby | `pornemby` | | Singularity | `singularity` |
 | Peach | `peach` | | Nebula | `nebula` |
 | Bluesea | `bluesea` | | Embyhub | `embyhub` |
-| 卷毛鼠 | `jms` | | | |
+| 卷毛鼠 | `jms` | | 卡戎 | `charon` |
 
 `proxy` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                    | 默认值      |
 | ---------- | ------ | --------------------------------------- | ----------- |
 | `hostname` | `str`  | 代理服务器地址                          | `localhost` |
 | `port`     | `int`  | 代理端口号                              | `1080`      |
@@ -341,14 +387,25 @@
 | ---------- | ------ | --------------------------------------------------------- | ------ |
 | `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
 | `username` | `str`  | Emby 服务器用户名                                         |        |
 | `password` | `str`  | Emby 服务器密码                                           |        |
 | `time`     | `int`  | 模拟观看的时间 (秒)                                       | `800`  |
 | `progress` | `int`  | 观看后模拟进度条保存的时间 (秒)                           | `1000` |
 
+服务可以进行特定配置, 如下所示:
+
+```toml
+
+[monitor.bgk] # 支持 bgk, embyhub, polo
+unique_name = "your_username_for_registeration" # 自动抢注时使用的用户名
+
+[monitor.pornemby]
+only_history = true # 仅当问题历史中找到答案时自动回答
+```
+
 ## 代码重用与开发
 
 代码架构如下:
 
 ```mermaid
 flowchart TD
     A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
@@ -395,7 +452,11 @@
                 await self.retry()
                 break
 ```
 
 上述代码实现每次按对应一个字符按键的功能.
 
 当您实现一个新的签到器时, 欢迎您提出 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 以帮助更多人使用!
+
+## 趋势
+
+[![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

#### html2text {}

```diff
@@ -1,18 +1,31 @@
-[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/
-project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/
+Metadata-Version: 2.1 Name: embykeeper Version: 2.1.0 Summary: Daily checkin
+automator for emby bots in telegram. Author-email: jackzzs
+outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
+Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
+Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
+:: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-
+File: LICENSE [![build status](https://img.shields.io/github/actions/workflow/
+status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/
+embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/
+v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https:
+//img.shields.io/pypi/dm/
 embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
 embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
 embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
 embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
 [telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
 embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
-channel-green)](https://t.me/embykeeper) [![telegram badge](https://
-img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
+channel-green)](https://t.me/embykeeper)
                                  [Embykeeper]
                     èªå¨ç­¾å° å®æ¶ä¿å· æéæ°´ç¾¤
 --- Embykeeper æ¯ä¸ä¸ªå¨ä¸­æç¤¾ç¾¤è§åä¸ç¨äº Emby
 å½±è§æå¡å¨çç­¾å°åä¿å·çèªå¨æ§è¡å·¥å·, åºäº Pyrogram
 ç¼åå¹¶å·æå¯æå±æ§. ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
 æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³, å¨ä½¿ç¨ Embykeeper
 æ¶é æçä¸åæå¤± (åæ¬ä½ä¸éäº Emby æ Telegram
@@ -25,127 +38,143 @@
 å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
 å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
 æ¬é¡¹ç®ä»æä¾å·¥å·,
 å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
 å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
-æ¨ä¹å¯ä»¥éè¿ [Telegram è®¨è®ºç»](https://t.me/embykeeper_chat)
-ä¸å¼åå¢éè¿è¡äº¤æµ. å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½,
-è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper Auth Bot](https://t.me/
-embykeeper_auth_bot)" åéå³é®çæå/å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper
-Bot](https://t.me/embykeeper_bot)" åæ¨æ¨é,
-æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
+å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
+Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
+å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
+åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
-æºå¨äººç­¾å° - æ¯æç¾¤ç» - ç»ç¹ç«: [é¢é](https://t.me/embypub)
-[ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) -
-å·æ¯é¼ : [é¢é]() [ç¾¤ç»](https://t.me/Curly_Mouse) [æºå¨äºº](https://
-t.me/jmsembybot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»](https://
-t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
-(ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
-t.me/embykeeper_bot?start=__prime)) - BlueSea: [ç¾¤ç»](https://t.me/
-blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot) - Singularity: [é¢é]
-(https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/
-Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach:
-[é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
+æºå¨äººç­¾å° - ç»ç¹ç«: [é¢é](https://t.me/embypub) [ç¾¤ç»](https://
+t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) - Nebula: [é¢é]
+(https://t.me/Nebula_Emby) [ç¾¤ç»](https://t.me/NebulaEmbyUser) [æºå¨äºº]
+(https://t.me/Nebula_Account_bot) (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare
+éªè¯ç , éè¦[é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) -
+Singularity: [é¢é](https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://
+t.me/Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) -
+Peach: [é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
 peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
 (https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
-t.me/EdHubot) - Pornemby (_æµè¯ä¸­_): [é¢é](https://t.me/pornembyservice)
-[æºå¨äºº](https://t.me/PronembyTGBot2_bot) - å¶ä»é Emby ç¸å³: -
-æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/pull/8)
-å¢å ) (_æµè¯ä¸­_): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
-Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_): [æ´»å¨é¢é](https://t.me/PornembyFun) -
+t.me/EdHubot) - Pornemby: [é¢é](https://t.me/pornembyservice) [ç¾¤ç»]
+(https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
+åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
+t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
+t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
+ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
+pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
+~~å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https://t.me/
+Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot)~~
+(æºå¨äººé»è¾é¢ç¹åå¨, ææ¶ç¦ç¨) - ~~BlueSea: [ç¾¤ç»](https://t.me/
+blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~ (æ ååº) -
 ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/
-Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) -
-~~åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
-t.me/zckllflbot)~~ (æ ååº) - ç¹æ§ - éªè¯ç è¯å«ä¸èªå¨éè¯ -
-å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby ä¿æ´» -
-å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
-èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
-è¯·è°¨æä½¿ç¨) - NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork)
-[æºå¨äºº](https://t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦
-[è¶çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç
-æ¢éè¯·ç : [ç¾¤ç»](https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/
-UnknownEmbyBot) - Embyhub å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub)
-[ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) ##
-å®è£ä¸ä½¿ç¨ ### ä» PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡,
-æ¨å¯ä»¥éè¿ [conda](https://github.com/conda/conda) æ [virtualvenv]
-(https://virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿
-`pip` å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
-embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
-github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)). éå,
-æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) - Emby
+ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
+Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
+t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
+Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
+embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
+t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
+[é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime),
+åç­åç¡®çä¸è¬è¯·è°¨æä½¿ç¨) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»](https:
+//t.me/Ephemeralemby) [æºå¨äºº](https://t.me/UnknownEmbyBot) - Viper
+æ¢éè¯·ç : [é¢é](https://t.me/viper_emby_channel) [ç¾¤ç»](https://t.me/
+Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
+å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
+emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
+[é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
+[æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
+[é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
+(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### ä»
+PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡, æ¨å¯ä»¥éè¿ [conda]
+(https://github.com/conda/conda) æ [virtualvenv](https://virtualenv.pypa.io/
+) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip` å®è£ `embykeeper`
+(éè¦ `python >= 3.7, < 3.11`): ```bash pip install embykeeper ``` éå,
+æ¨éè¦æ§è¡: ```bash embykeeper ``` å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿
+`config.toml` æä»¶, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
+(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [proxy] hostname =
+"127.0.0.1" port = 1080 scheme = "socks5" [[telegram]] api_id = "27894236"
+api_hash = "622159182fdd4b15b627eeb3ac695271" phone = "+8612109347899" [[emby]]
+url = "https://weiss-griffin.com/" username = "carrie19" password =
+"s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿ [Telegram å®ç½]
+(https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
+development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
+æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
+æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
+æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡:
+```bash embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
+ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
 Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
 ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿
-`docker` è¿è¡, æ¨é [å®è£ docker](https://yeasy.gitbook.io/
-docker_practice/install), ç¶åæ§è¡: ```bash touch config.toml docker run -
-v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
-```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme = "socks5" [
-[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
-phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
-"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
-[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
-ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
-è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
-"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
-æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
-éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/config.toml:/app/
-config.toml --rm -it embykeeper/embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º åä» PyPi
+å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python ç¯å¢, ç¶åæå Github
+å¹¶å®è£: ```bash git clone https://github.com/embykeeper/embykeeper.git cd
+embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash
+embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/
+embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ### ä» Docker
+é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://
+yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡: ```bash docker run -
+v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
+å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯ (è¯¦è§[ä» Pypi å®è£](https://github.com/
+embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)). éå,
+æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
+net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
+ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash docker
-run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper ```
-æèä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) ([watchtower]
-(https://github.com/containrrr/watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡):
-```yaml version: '3' services: embykeeper: container_name: embykeeper image:
-cembykeeper/embykeeper restart: unless-stopped volumes: - ./config.toml:/app/
-config.toml watchtower: container_name: watchtower image: containrrr/watchtower
-restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/docker.sock:rw
-``` å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -
-f embykeeper` æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿.
-å¦ææ¨éè¦ä½¿ç¨ä¸»æºä¸çä»£çæå¡å¨ (ä¾å¦ `https://localhost:
-1080`), æ¨å¯è½éè¦ä½¿ç¨ `--net=host` åæ°ä»¥ä½¿ç¨ä¸»æºç½ç»æ¨¡å¼.
-### ä»æºç æå»º åä» PyPi å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python
-ç¯å¢, ç¶åæå Github å¹¶å®è£: ```bash git clone https://github.com/
-embykeeper/embykeeper.git cd embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡
-Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£]
-(https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
-å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
-## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
-```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. ### éè¿ Docker Compose
+é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/compose/
+) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker é¨ç½²]
+(https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2)
+æè½éè¿ `docker-compose` é¨ç½²,
+è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
+ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
+compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
+version: '3' services: embykeeper: container_name: embykeeper image:
+embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
+network_mode: host watchtower: container_name: watchtower image: containrrr/
+watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
+docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
+watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡.
+ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨: ```bash docker-compose up -d ```
+å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -f embykeeper`
+æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿. ##
+å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash
+$ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
 æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
-(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å°
-(ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´»
-(ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --monitor -m å¯ç¨ç¾¤èçè§ --send -
-s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-instant -
-I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
+(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
+(ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
+e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
+instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
+o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
-follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ ```
-ä¾å¦: ```bash # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
+follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ --
+basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® ``` ä¾å¦: ```bash # å¯å¨ææåè½
+(å¨åè´¦å·éç½®ä¸­è¿ä¸æ­¥è®¾ç½®åè½å¼å¯/å³é­) $ embykeeper
+config.toml # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
-å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
-è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -
-s ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
+ä»å¯å¨æ¯æ¥ 8:00 PM - 9:00 PM éæºæ¶é´ç­¾å° $ embykeeper config.toml -
+c <8:00PM,9:00PM> # å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
+è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -s #
+å¯å¨ææåè½, åªè¿è¡ä¸æ¬¡ $ embykeeper config.toml --once #
+å¯å¨ææåè½, ä¸ç«å³æ§è¡ä¸æ¬¡ç­¾å°/ä¿æ´» $ embykeeper config.toml
+-I ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
 ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
 config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
 10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
 "åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
 è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
 ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
 å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
@@ -159,21 +188,22 @@
 (ä¾å¦èªå¨æ¢éè¯·ç )å°éè¦é«çº§ç¨æ·, æ¨å¯ä»¥éè¿ [Embykeeper
 Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
-(https://afdian.net/a/jackzzs)èµå© ![kitty](images/kitty.gif) ## éç½®é¡¹ |
-è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ------------ | -----------------
-- | -------------------------------------------- | ------- | | `timeout` |
-`int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | | `retries` | `int` |
-Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `10` | | `concurrent` | `int` |
-Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random` | `int` | Telegram
-æºå¨äººç­¾å°å®æ¶ä»»å¡æ¶é´éæºé (åé) | `15` | | `notifier` |
+(https://afdian.net/a/jackzzs)èµå© ![Kitty](https://github.com/embykeeper/
+embykeeper/raw/main/images/kitty.gif) ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å |
+ç®ä» | é»è®¤å¼ | | ------------ | ------------------ | --------------------
+------------------------ | ------- | | `timeout` | `int` | Telegram
+æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | | `retries` | `int` | Telegram
+æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | | `concurrent` | `int` | Telegram
+æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random` | `int` | Telegram
+æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` | | `notifier` |
 `int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/ææºå·) |
 `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/çè§åè½å¼å¯ç«ç¹è®¾ç½® |
 `{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `{}` | | `telegram` | `list` |
 Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | | `emby` | `list` | Emby
 è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
 å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------- | ------ | -------------- | ----
 ---------------- | | `checkiner` | `list` | å¯ç¨çç­¾å°ç«ç¹ |
@@ -184,18 +214,18 @@
 æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
 è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
 æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
 ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | --- | --- | --- |--- | --- | |
 åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` | | å·æ¯é¼  IPTV |
 `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby | `pornemby` | | Singularity
 | `singularity` | | Peach | `peach` | | Nebula | `nebula` | | Bluesea |
-`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | | | `proxy`
-è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
------- | --------------------------------------- | ----------- | | `hostname` |
-`str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
+`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | å¡æ | `charon` |
+`proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | -----
+----- | ------ | --------------------------------------- | ----------- | |
+`hostname` | `str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
 ä»£çç«¯å£å· | `1080` | | `scheme` | `str` | ä»£çåè®®, å¯ä»¥ä¸º
 "`socks5`" æ "`http`" | `socks5` | `telegram` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
 å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
 -------------------------------------------- | ------- | | `api_id` | `str` |
 ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID | | |
 `api_hash` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç
 Application Hash | | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
@@ -203,29 +233,34 @@
 | `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: |
 è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------
 ----------------------------------------------- | ------ | | `url` | `str` |
 Emby æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | |
 `username` | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
-## ä»£ç éç¨ä¸å¼å ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-
-terminal cli) --> B(fa:fa-telegram telechecker) A --> C(fa:fa-play embywatcher)
-B --checker--> E[fa:fa-robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --
-messager--> F[fa:fa-message Messager] C --watcher--> H[fa:fa-circle-play
-EmbyWatcher] F ---- |schedule| A ``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: -
-`embykeeper.telechecker.bots` - `embykeeper.telechecker.monitor` -
-`embykeeper.telechecker.messager` éå¸¸æ¥è¯´,
-å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
+æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
+bgk, embyhub, polo unique_name = "your_username_for_registeration" #
+èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
+ä»å½é®é¢åå²ä¸­æ¾å°ç­æ¡æ¶èªå¨åç­ ``` ## ä»£ç éç¨ä¸å¼å
+ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-
+telegram telechecker) A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-
+robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message
+Messager] C --watcher--> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A
+``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
+`embykeeper.telechecker.monitor` - `embykeeper.telechecker.messager`
+éå¸¸æ¥è¯´, å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
 ä¸­å¢å ä¸ä¸ªæä»¶ `dummy.py`: ```python from .base import BotCheckin class
 DummyCheckin(BotCheckin): name = "Dummy" bot_username = "dummy" bot_captcha_len
 = 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨, å°ä¼åç¨æ·åä¸º
 "`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4 ä½çéªè¯ç ,
 è¯å«éªè¯ç åå°åé. è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®,
 æ¨å¯ä»¥ä½¿ç¨ `AnswerBotCheckin`, æ¨ä¹å¯ä»¥éå `on_captcha`
 å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from .base import AnswerBotCheckin
 class DummyCheckin(AnswerBotCheckin): .... async def on_captcha(self, message:
 Message, captcha: str): for l in captcha: try: await self.message.click(l)
 except ValueError: self.log.info(f'æªè½æ¾å°å¯¹åº "{l}" çæé®,
 æ­£å¨éè¯.') await self.retry() break ```
 ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
 å½æ¨å®ç°ä¸ä¸ªæ°çç­¾å°å¨æ¶, æ¬¢è¿æ¨æåº [Pull Requests](https://
-github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨!
+github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! ## è¶å¿ [!
+[Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
+embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

### Comparing `embykeeper-2.0.9/embykeeper/cli.py` & `embykeeper-2.1.0/embykeeper/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 from pathlib import Path
 from datetime import datetime, timedelta
+import re
 import sys
 
-import tomli as tomllib
 import typer
 import asyncio
 from appdirs import user_data_dir
-from schedule import Scheduler
 from dateutil import parser
 
 from . import __author__, __name__, __url__, __version__
 from .utils import Flagged, FlagValueCommand, AsyncTyper, AsyncTaskPool
 from .settings import prepare_config
 
 app = AsyncTyper(
     pretty_exceptions_show_locals=False,
     rich_markup_mode="rich",
     add_completion=False,
     context_settings={"help_option_names": ["-h", "--help"]},
 )
 
 
-async def run_pending(scheduler: Scheduler):
-    while True:
-        scheduler.run_pending()
-        await asyncio.sleep(1)
-
-
 def version(version):
     if version:
         print(__version__)
         raise typer.Exit()
 
 
 @app.async_command(
@@ -42,15 +35,15 @@
         envvar=f"{__name__.upper()}_CONFIG",
         dir_okay=False,
         allow_dash=True,
         rich_help_panel="参数",
         help="配置文件 (置空以生成)",
     ),
     checkin: str = typer.Option(
-        Flagged("", "6:00PM"),
+        Flagged("", "<10:00AM,9:00PM>"),
         "--checkin",
         "-c",
         rich_help_panel="模块开关",
         show_default="不指定值时默认为6:00PM",
         help="启用每日指定时间签到",
     ),
     emby: int = typer.Option(
@@ -76,44 +69,61 @@
         rich_help_panel="调试参数",
         callback=version,
         is_eager=True,
         help=f"打印 {__name__.capitalize()} 版本",
     ),
     follow: bool = typer.Option(False, "--follow", "-f", rich_help_panel="调试参数", help="仅启动消息调试"),
     analyze: bool = typer.Option(False, "--analyze", "-a", rich_help_panel="调试参数", help="仅启动历史信息分析"),
+    basedir: Path = typer.Option(None, rich_help_panel="调试参数", help="设定输出文件位置"),
 ):
     from .log import logger, initialize
 
     initialize(level="DEBUG" if debug else "INFO")
 
     config: dict = prepare_config(config)
 
     if debug:
-        config.setdefault("nofail", False)
+        config["nofail"] = False
         logger.warning("您当前处于调试模式, 错误将会导致程序停止运行.")
+    if debug_cron:
+        logger.warning("您当前处于计划任务调试模式, 将在 3 秒后运行计划任务.")
 
     if emby < 0:
         emby = -emby
 
     if not checkin and not monitor and not emby and not send:
-        checkin = "08:00"
+        checkin = "<5:00PM,8:00PM>"
         emby = 7
         monitor = True
         send = True
 
     logger.info(f"欢迎使用 [orange3]{__name__.capitalize()}[/]! 正在启动, 请稍等. 您可以通过 Ctrl+C 以结束运行.")
     logger.info(f'当前版本 ({__version__}) 活跃贡献者: {", ".join(__author__)}.')
+    logger.debug(f'命令行参数: "{" ".join(sys.argv[1:])}".')
 
-    session_dir = Path(user_data_dir(__name__))
-    session_dir.mkdir(parents=True, exist_ok=True)
-    session_dir_spec = Path("~") / session_dir.relative_to(Path.home())
-    logger.info(f'您的 Telegram 会话将存储至 "{session_dir_spec}", 请注意保管.')
-
-    from .embywatcher.main import watcher
-    from .telechecker.main import analyzer, checkiner, follower, messager, monitorer, notifier
+    basedir = Path(basedir or user_data_dir(__name__))
+    basedir.mkdir(parents=True, exist_ok=True)
+    config["basedir"] = basedir
+    try:
+        session_dir_spec = Path("~") / basedir.relative_to(Path.home())
+    except ValueError:
+        session_dir_spec = basedir
+    if not basedir == Path("/app"):
+        logger.info(f'您的 Telegram 会话将存储至 "{session_dir_spec}", 请注意保管.')
+
+    from .embywatcher.main import watcher, watcher_schedule
+    from .telechecker.main import (
+        analyzer,
+        checkiner,
+        checkiner_schedule,
+        follower,
+        messager,
+        monitorer,
+        notifier,
+    )
 
     if follow:
         return await follower(config)
 
     if analyze:
         indent = " " * 29
         chats = typer.prompt(indent + "请输入群组用户名 (以空格分隔)").split()
@@ -127,48 +137,48 @@
     if instant and not debug_cron:
         instants = []
         if emby:
             instants.append(watcher(config))
         if checkin:
             instants.append(checkiner(config, instant=True))
         await asyncio.gather(*instants)
+        logger.debug("启动时立刻执行签到和保活: 已完成.")
 
     if not once:
+        await notifier(config)
         pool = AsyncTaskPool()
-
-        pool.add(notifier(config))
-
         debug_time = datetime.now() + timedelta(seconds=3) if debug_cron else None
         if emby:
-            schedule_emby = Scheduler()
-            pool.add(run_pending(schedule_emby))
-            schedule_emby.every(1 if debug_cron else emby).days.at(
-                (debug_time or datetime.now()).strftime("%H:%M:%S")
-            ).do(lambda: pool.add(watcher(config)))
-            logger.bind(scheme="embywatcher").info(
-                f"下一次保活将在 {schedule_emby.next_run.strftime('%m-%d %H:%M %p')} 进行."
-            )
+            pool.add(watcher_schedule(config, 1 if debug_cron else emby))
         if checkin:
-            schedule_checkin = Scheduler()
-            pool.add(run_pending(schedule_checkin))
-            checkin = (debug_time or parser.parse(checkin).time()).strftime("%H:%M:%S")
-            schedule_checkin.every().day.at(checkin).do(
-                lambda: pool.add(checkiner(config, instant=debug_cron))
-            )
-            logger.bind(scheme="telechecker").info(
-                f"下一次签到将在 {schedule_checkin.next_run.strftime('%m-%d %H:%M %p')} 进行."
-            )
-        if send:
-            schedule_send = Scheduler()
-            pool.add(run_pending(schedule_send))
-            pool.add(messager(config, schedule_send))
+            if debug_time:
+                start_time = end_time = debug_time.time()
+            else:
+                checkin_range_match = re.match(r"<\s*(.*),\s*(.*)\s*>", checkin)
+                if checkin_range_match:
+                    start_time, end_time = [parser.parse(checkin_range_match.group(i)).time() for i in (1, 2)]
+                else:
+                    start_time = end_time = parser.parse(checkin).time()
+            pool.add(checkiner_schedule(config, instant=debug_cron, start_time=start_time, end_time=end_time))
         if monitor:
             pool.add(monitorer(config))
+        if send:
+            pool.add(messager(config))
 
         async for t in pool.as_completed():
+            msg = f"任务 {t.get_name()} "
+            try:
+                e = t.exception()
+                if e:
+                    msg += f"发生错误并退出: {e}"
+                else:
+                    msg += f"成功结束."
+            except asyncio.CancelledError:
+                msg += f"被取消."
+            logger.debug(msg)
             try:
                 await t
             except Exception as e:
                 if debug:
                     raise
                 else:
                     logger.opt(exception=e).error("出现错误, 模块可能停止运行:")
```

### Comparing `embykeeper-2.0.9/embykeeper/embywatcher/emby.py` & `embykeeper-2.1.0/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.9/embykeeper/embywatcher/main.py` & `embykeeper-2.1.0/embykeeper/embywatcher/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import asyncio
 import random
 import string
 from typing import Union
-from datetime import datetime
+from datetime import datetime, time
 
-from aiohttp import ClientError
+from aiohttp import ClientError, ClientConnectionError
 from loguru import logger
 from embypy.objects import Episode, Movie
 
+from ..utils import next_random_datetime
 from .emby import Emby, Connector, EmbyObject
 
 logger = logger.bind(scheme="embywatcher")
 
 
 class PlayError(Exception):
     pass
@@ -24,16 +25,16 @@
 def is_ok(co):
     if isinstance(co, tuple):
         co, *_ = co
     if 200 <= co < 300:
         return True
 
 
-async def get_oldest(emby: Emby, n=10):
-    items = await emby.get_items(["Movie", "Episode"], limit=n, sort="DateCreated")
+async def get_latest(emby: Emby, n=10):
+    items = await emby.get_items(["Movie", "Episode"], limit=n, sort="DateCreated", ascending=False)
     i: Union[Movie, Episode]
     for i in items:
         yield i
 
 
 async def set_played(obj: EmbyObject):
     c: Connector = obj.connector
@@ -52,16 +53,18 @@
 
 async def send_playing(obj: EmbyObject, playing_info: dict):
     c: Connector = obj.connector
     try:
         while True:
             try:
                 await asyncio.wait_for(c.post("/Sessions/Playing", **playing_info), 10)
-            except (ClientError, ConnectionError, TimeoutError, asyncio.TimeoutError):
-                pass
+            except (ClientError, ConnectionError, TimeoutError, asyncio.TimeoutError) as e:
+                logger.debug(f"播放状态设定错误: {e}")
+            else:
+                break
             await asyncio.sleep(10)
     except asyncio.CancelledError:
         pass
 
 
 async def play(obj: EmbyObject, time=800, progress=1000):
     c: Connector = obj.connector
@@ -113,32 +116,31 @@
             password=a["password"],
             device_id=_gen_random_device_id(),
             jellyfin=a.get("jellyfin", False),
             proxy=config.get("proxy", None),
         )
         try:
             info = await emby.info()
-        except ConnectionError:
+        except (ConnectionError, RuntimeError, ClientConnectionError):
             logger.error(f'Emby ({a["url"]}) 连接错误, 请重新检查配置.')
             continue
-
         if info:
             loggeruser = logger.bind(server=info["ServerName"], username=a["username"])
             loggeruser.info(f'成功登录 ({"Jellyfin" if a.get("jellyfin", False) else "Emby"} {info["Version"]}).')
             yield emby, a.get("time", 800), a.get("progress", 1000), loggeruser
         else:
             logger.error(f'Emby ({a["url"]}) 无法获取元信息而跳过, 请重新检查配置.')
             continue
 
 
 async def watch(emby, time, progress, logger, retries=5):
     retry = 0
     while True:
         try:
-            async for obj in get_oldest(emby):
+            async for obj in get_latest(emby):
                 logger.info(f'开始尝试播放 "{obj.name}" ({time} 秒).')
                 while True:
                     try:
                         if await play(obj, time, progress):
                             await obj.update()
                             if obj.play_count < 1:
                                 raise PlayError("尝试播放后播放数低于1")
@@ -159,15 +161,16 @@
                             return False
                         else:
                             logger.info(f"连接失败, 正在重试.")
                     except PlayError as e:
                         logger.info(f"发生错误: {e}, 正在重试其他视频.")
                         break
                     finally:
-                        await hide_from_resume(obj)
+                        if not await hide_from_resume(obj):
+                            logger.debug(f"未能成功从最近播放中隐藏视频.")
             else:
                 logger.warning(f"由于没有成功播放视频, 保活失败, 请重新检查配置.")
                 return False
         except (ClientError, OSError):
             retry += 1
             if retry > retries:
                 logger.warning(f"超过最大重试次数, 保活失败.")
@@ -177,22 +180,30 @@
         except asyncio.CancelledError:
             raise
         except Exception as e:
             logger.opt(exception=e).warning("发生错误:")
             return False
 
 
-async def watcher(config):
+async def watcher(config: dict):
     async def wrapper(emby, time, progress, logger):
         try:
             return await asyncio.wait_for(watch(emby, time, progress, logger), max(time * 3, 180))
         except asyncio.TimeoutError:
             logger.warning(f"一定时间内未完成播放, 保活失败.")
             return False
 
     tasks = []
     async for emby, time, progress, logger in login(config):
         tasks.append(wrapper(emby, time, progress, logger))
     results = await asyncio.gather(*tasks)
     fails = len(tasks) - sum(results)
     if fails:
         logger.error(f"保活失败 ({fails}/{len(tasks)}).")
+
+
+async def watcher_schedule(config: dict, days: int = 7):
+    dt = next_random_datetime(time(11, 0), time(23, 0), interval_days=days)
+    while True:
+        logger.bind(scheme="embywatcher").info(f"下一次保活将在 {dt.strftime('%m-%d %H:%M %p')} 进行.")
+        await asyncio.sleep((dt - datetime.now()).seconds)
+        await watcher(config)
```

### Comparing `embykeeper-2.0.9/embykeeper/log.py` & `embykeeper-2.1.0/embykeeper/log.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from logging import Formatter
 from loguru import logger
 from rich.logging import Console, RichHandler
 import asyncio
 
 from .utils import to_iterable
 
 
@@ -12,27 +13,38 @@
     def ifextra(keys, pattern="{}"):
         keys = to_iterable(keys)
         if all(k in extra for k in keys):
             return pattern.format(*[f"{{extra[{k}]}}" for k in keys])
         else:
             return ""
 
+    scheme_names = {
+        "telegram": "Telegram",
+        "telechecker": "每日签到",
+        "telemonitor": "消息监控",
+        "telemessager": "定时水群",
+        "telelink": "账号服务",
+        "telenotifier": "消息推送",
+        "embywatcher": "Emby保活",
+        "datamanager": "下载器",
+    }
+
     if scheme in ("telegram", "telechecker", "telemonitor", "telemessager", "telelink"):
         username = ifextra("username", " ([cyan]{}[/])")
         name = ifextra("name", "([magenta]{}[/]) ")
-        return f"[blue]{scheme.capitalize()}[/]{username}: {name}{{message}}"
+        return f"[blue]{scheme_names[scheme]}[/]{username}: {name}{{message}}"
     elif scheme == "embywatcher":
         ident = ifextra(["server", "username"], " ([cyan]{}:{}[/])")
-        return f"[blue]Embywatcher[/]{ident}: {{message}}"
+        return f"[blue]{scheme_names[scheme]}[/]{ident}: {{message}}"
+    elif scheme == "datamanager":
+        return f"[blue]{scheme_names[scheme]}[/]: {{message}}"
     else:
         return "{message}"
 
 
 def initialize(level="INFO"):
     logger.remove()
-    logger.add(
-        RichHandler(
-            console=Console(stderr=True), markup=True, rich_tracebacks=True, tracebacks_suppress=[asyncio]
-        ),
-        format=formatter,
-        level=level,
+    handler = RichHandler(
+        console=Console(stderr=True), markup=True, rich_tracebacks=True, tracebacks_suppress=[asyncio]
     )
+    handler.setFormatter(Formatter(None, "[%m/%d %H:%M]"))
+    logger.add(handler, format=formatter, level=level, colorize=False)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `embykeeper-2.0.9/embykeeper/settings.py` & `embykeeper-2.1.0/embykeeper/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 from pathlib import Path
 import sys
 from loguru import logger
 
 import tomli as tomllib
-from schema import And, Optional, Or, Regex, Schema, SchemaError, Use
+from schema import And, Optional, Or, Regex, Schema, SchemaError
 
 
 def check_config(config):
-    PositiveInt = lambda: And(Use(int), lambda n: n > 0)
+    PositiveInt = lambda: And(int, lambda n: n > 0)
     schema = Schema(
         {
             Optional("timeout"): PositiveInt(),
             Optional("retries"): PositiveInt(),
             Optional("concurrent"): PositiveInt(),
             Optional("random"): PositiveInt(),
             Optional("notifier"): Or(str, bool),
             Optional("nofail"): bool,
             Optional("proxy"): Schema(
                 {
                     Optional("hostname"): Regex(
                         r"^(?=.{1,255}$)[0-9A-Za-z](?:(?:[0-9A-Za-z]|-){0,61}[0-9A-Za-z])?(?:\.[0-9A-Za-z](?:(?:[0-9A-Za-z]|-){0,61}[0-9A-Za-z])?)*\.?$"
                     ),
-                    Optional("port"): And(Use(int), lambda n: n > 1024 and n < 65536),
+                    Optional("port"): And(int, lambda n: n > 1024 and n < 65536),
                     Optional("scheme"): Schema(Or("socks5", "http")),
                 }
             ),
             Optional("service"): Schema(
                 {
-                    Optional("checkiner"): [Use(str)],
-                    Optional("monitor"): [Use(str)],
-                    Optional("messager"): [Use(str)],
+                    Optional("checkiner"): [str],
+                    Optional("monitor"): [str],
+                    Optional("messager"): [str],
                 }
             ),
             Optional("telegram"): [
                 Schema(
                     {
                         "api_id": Regex(r"^\d+$"),
                         "api_hash": Regex(r"^[a-z0-9]+$"),
-                        "phone": Use(str),
+                        "phone": str,
                         Optional("monitor"): bool,
                         Optional("send"): bool,
                     }
                 )
             ],
             Optional("emby"): [
                 Schema(
                     {
                         "url": Regex(
                             r"(http|https):\/\/([\w_-]+(?:(?:\.[\w_-]+)+))([\w.,@?^=%&:\/~+#-]*[\w@?^=%&\/~+#-])"
                         ),
-                        "username": Use(str),
-                        "password": Use(str),
+                        "username": str,
+                        "password": str,
                         Optional("time"): PositiveInt(),
                         Optional("progress"): PositiveInt(),
                     }
                 )
             ],
+            Optional("monitor"): Schema({str: Schema({}, ignore_extra_keys=True)}),
         }
     )
     try:
         schema.validate(config)
     except SchemaError as e:
         return e
     else:
@@ -91,24 +92,24 @@
     doc.add(comment("将关键信息发送到第一个 Telegram 账号, 设为N以发送到第 N 个."))
     doc["notifier"] = True
     doc.add(nl())
     doc.add(comment("每个 Telegram Bot 签到的最大尝试时间."))
     doc["timeout"] = 120
     doc.add(nl())
     doc.add(comment("每个 Telegram Bot 签到的最大尝试次数."))
-    doc["retries"] = 10
+    doc["retries"] = 4
     doc.add(nl())
     doc.add(comment("最大可同时进行的 Telegram Bot 签到."))
     doc["concurrent"] = 1
     doc.add(nl())
     doc.add(comment("计划任务时, 各签到器启动前等待的随机时间 (分钟)."))
     doc["random"] = 15
     doc["proxy"] = {
         "hostname": "127.0.0.1",
-        "port": "1080",
+        "port": 1080,
         "scheme": "socks5",
     }
     doc["proxy"]["scheme"].comment("可选: http / socks5")
     doc.add(nl())
     doc.add(comment(f"服务设置, 当您需要禁用某些站点时, 请将该段取消注释并修改."))
     doc.add(comment(f"该部分内容是根据 {__name__.capitalize()} {__version__} 生成的."))
     service = item(
@@ -191,9 +192,9 @@
     if error:
         logger.error(f"配置文件错误, 请检查配置文件:\n{error}.")
         sys.exit(253)
     proxy: dict = config.get("proxy", None)
     if proxy:
         proxy.setdefault("scheme", "socks5")
         proxy.setdefault("hostname", "127.0.0.1")
-        proxy.setdefault("port", "1080")
+        proxy.setdefault("port", 1080)
     return config
```

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/bots/base.py` & `embykeeper-2.1.0/embykeeper/telechecker/bots/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 import asyncio
 import re
 from abc import ABC, abstractmethod
 from contextlib import asynccontextmanager
 from enum import Flag, auto
 import string
+import time
 from typing import Iterable, List, Union
 
-import ddddocr
+from ddddocr import DdddOcr
+from appdirs import user_data_dir
 from loguru import logger
 from PIL import Image
 from pyrogram import filters
-from pyrogram.errors import UsernameNotOccupied
+from pyrogram.errors import UsernameNotOccupied, FloodWait
 from pyrogram.handlers import EditedMessageHandler, MessageHandler
 from pyrogram.types import InlineKeyboardMarkup, Message, ReplyKeyboardMarkup
 from thefuzz import fuzz
 
+from ...data import get_datas
 from ...utils import to_iterable, AsyncCountPool
 from ..tele import Client
 
 __ignore__ = True
 
-ocr = ddddocr.DdddOcr(beta=True, show_ad=False)
+default_ocr = DdddOcr(beta=True, show_ad=False)
 
 
 class MessageType(Flag):
     TEXT = auto()
     CAPTION = auto()
     CAPTCHA = auto()
     ANSWER = auto()
 
 
 class BaseBotCheckin(ABC):
     name = None
 
-    def __init__(self, client: Client, retries=10, timeout=120, nofail=True):
+    def __init__(self, client: Client, retries=4, timeout=120, nofail=True, basedir=None, proxy=None):
         self.client = client
         self.retries = retries
         self.timeout = timeout
         self.nofail = nofail
+        self.basedir = basedir or user_data_dir(__name__)
+        self.proxy = proxy
         self.finished = asyncio.Event()
         self.log = logger.bind(scheme="telechecker", name=self.name, username=client.me.name)
 
     async def _start(self):
         try:
             return await self.start()
         except asyncio.CancelledError:
@@ -58,37 +63,43 @@
         pass
 
 
 class BotCheckin(BaseBotCheckin):
     """签到类, 用于回复模式签到."""
 
     group_pool = AsyncCountPool(base=2000)
+    ocr = default_ocr
+    lock = asyncio.Lock()
 
     name: str = None  # 签到器的名称
     bot_id: int = None  # Bot 的 UserID
     bot_username: str = None  # Bot 的 用户名
     bot_checkin_cmd: Union[str, List[str]] = ["/checkin"]  # Bot 依次执行的签到命令
+    bot_send_interval: int = 1  # 签到命令间等待的秒数
     bot_checkin_caption_pat: str = None  # 当 Bot 返回图片时, 仅当符合该 regex 才识别为验证码
     bot_text_ignore: Union[str, List[str]] = []  # 当含有列表中的关键词, 即忽略该消息
-    bot_captcha_len: Iterable = range(2, 7)  # 验证码的可能范围
+    bot_captcha_len: Iterable = None  # 验证码的可能范围
     bot_success_pat: str = r"(\d+)[^\d]*(\d+)"  # 当接收到成功消息后, 从消息中提取数字的模式
     bot_retry_wait: int = 2  # 失败时等待的秒数
     bot_use_history: int = None  # 首先尝试识别历史记录中最后一个验证码图片, 最多识别 N 条
     bot_allow_from_scratch: bool = False  # 允许从未聊天情况下启动
     chat_name: str = None  # 在群聊中向机器人签到
 
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
         self._is_archived = False
         self._retries = 0
+        self._waiting = {}
 
     def get_filter(self):
         filter = filters.user(self.bot_id or self.bot_username)
         if self.chat_name:
             filter = filter & filters.chat(self.chat_name)
+        else:
+            filter = filter & filters.private
         return filter
 
     def get_handlers(self):
         return [
             MessageHandler(self._message_handler, self.get_filter()),
             EditedMessageHandler(self._message_handler, self.get_filter()),
         ]
@@ -104,55 +115,88 @@
             try:
                 self.client.remove_handler(h, group=group)
             except ValueError:
                 pass
 
     async def start(self):
         ident = self.chat_name or self.bot_id or self.bot_username
-        try:
-            chat = await self.client.get_chat(ident)
-        except UsernameNotOccupied:
-            self.log.warning(f'初始化错误: 会话 "{ident}" 不存在.')
-            return False
+        while True:
+            try:
+                chat = await self.client.get_chat(ident)
+            except UsernameNotOccupied:
+                self.log.warning(f'初始化错误: 会话 "{ident}" 不存在.')
+                return False
+            except KeyError as e:
+                self.log.info(f"初始化错误: 无法访问, 您可能已被封禁: {e}.")
+                return False
+            except FloodWait as e:
+                self.log.info(f"初始化信息: Telegram 要求等待 {e.value} 秒.")
+                await asyncio.sleep(e.value)
+            else:
+                break
         async for d in self.client.get_dialogs(folder_id=1):
             if d.chat.id == chat.id:
                 self._is_archived = True
                 break
         else:
             async for d in self.client.get_dialogs(folder_id=0):
                 if d.chat.id == chat.id:
                     break
             else:
                 if not self.bot_allow_from_scratch:
                     self.log.info(f'跳过签到: 从未与 "{ident}" 交流.')
                     return None
+
+        async with self.lock:
+            if isinstance(self.ocr, str):
+                data = []
+                files = (f"{self.ocr}.onnx", f"{self.ocr}.json")
+                async for p in get_datas(self.basedir, files, proxy=self.proxy, caller=self.name):
+                    if p is None:
+                        self.log.warning(f"初始化错误: 无法下载所需文件.")
+                        return None
+                    else:
+                        data.append(p)
+                self.__class__.ocr = DdddOcr(
+                    show_ad=False, import_onnx_path=str(data[0]), charsets_path=str(data[1])
+                )
+
         bot = await self.client.get_users(self.bot_id or self.bot_username)
         msg = f"开始执行签到: [green]{bot.name}[/] [gray50](@{bot.username})[/]"
         if chat.title:
             msg += f" @ [green]{chat.title}[/] [gray50](@{chat.username})[/]"
         self.log.info(msg + ".")
+
+        if not self.chat_name:
+            self.log.debug(f"[gray50]禁用提醒 {self.timeout} 秒: {bot.username}[/]")
+            await self.client.mute_chat(ident, time.time() + self.timeout + 10)
+
         try:
             async with self.listener():
                 if self.bot_use_history is None:
                     await self.send_checkin()
                 elif not await self.walk_history(self.bot_use_history):
                     await self.send_checkin()
                 try:
                     await asyncio.wait_for(self.finished.wait(), self.timeout)
                 except asyncio.TimeoutError:
                     pass
                 finally:
                     if self._is_archived:
+                        self.log.debug(f"[gray50]将会话重新归档: {bot.username}[/]")
                         try:
                             await asyncio.shield(asyncio.wait_for(chat.archive(), 0.5))
                         except asyncio.TimeoutError:
                             pass
         except OSError as e:
             self.log.warning(f'初始化错误: "{e}".')
             return False
+        finally:
+            if not self.chat_name:
+                await self.client.read_chat_history(ident)
         if not self.finished.is_set():
             self.log.warning("无法在时限内完成签到.")
             return False
         else:
             return self._retries <= self.retries
 
     async def walk_history(self, limit=0):
@@ -167,18 +211,21 @@
     async def send(self, cmd):
         if self.chat_name:
             bot = await self.client.get_users(self.bot_id or self.bot_username)
             await self.client.send_message(self.chat_name, f"{cmd}@{bot.username}")
         else:
             await self.client.send_message(self.bot_id or self.bot_username, cmd)
 
-    async def send_checkin(self):
-        for i, cmd in enumerate(to_iterable(self.bot_checkin_cmd)):
-            if not i:
+    async def send_checkin(self, retry=False):
+        cmds = to_iterable(self.bot_checkin_cmd)
+        for i, cmd in enumerate(cmds):
+            if retry and not i:
                 await asyncio.sleep(self.bot_retry_wait)
+            if i < len(cmds):
+                await asyncio.sleep(self.bot_send_interval)
             await self.send(cmd)
 
     async def _message_handler(self, client: Client, message: Message):
         try:
             await self.message_handler(client, message)
         except OSError as e:
             self.log.info(f'发生错误: "{e}", 正在重试.')
@@ -192,14 +239,20 @@
             else:
                 await self.fail()
                 raise
         finally:
             message.continue_propagation()
 
     async def message_handler(self, client: Client, message: Message, type=None):
+        text = message.text or message.caption
+        if text:
+            for p, k in self._waiting.items():
+                if re.search(p, text):
+                    k.set()
+                    self._waiting[p] = message
         type = type or self.message_type(message)
         if MessageType.TEXT in type:
             await self.on_text(message, message.text)
         if MessageType.CAPTION in type:
             await self.on_text(message, message.caption)
         if MessageType.CAPTCHA in type:
             await self.on_photo(message)
@@ -219,18 +272,20 @@
         elif message.text:
             return MessageType.TEXT
 
     async def on_photo(self, message: Message):
         data = await self.client.download_media(message, in_memory=True)
         image = Image.open(data)
         captcha = (
-            ocr.classification(image).translate(str.maketrans("", "", string.punctuation)).replace(" ", "")
+            self.ocr.classification(image)
+            .translate(str.maketrans("", "", string.punctuation))
+            .replace(" ", "")
         )
         if captcha:
-            self.log.info(f"[gray50]接收验证码: {captcha}.[/]")
+            self.log.debug(f"[gray50]接收验证码: {captcha}.[/]")
             if self.bot_captcha_len and len(captcha) not in to_iterable(self.bot_captcha_len):
                 self.log.info(f"签到失败: 验证码低于设定长度, 正在重试.")
                 await self.retry()
             else:
                 await asyncio.sleep(1)
                 await self.on_captcha(message, captcha)
         else:
@@ -239,47 +294,66 @@
 
     async def on_captcha(self, message: Message, captcha: str):
         await message.reply(captcha)
 
     async def on_text(self, message: Message, text: str):
         if any(s in text for s in to_iterable(self.bot_text_ignore)):
             pass
-        elif any(s in text for s in ("失败", "错误", "超时", "拉黑", "黑名单", "冻结")):
+        elif any(s in text for s in ("拉黑", "黑名单", "冻结", "未找到用户", "无资格", "退出群", "退群", "加群", "加入群聊", "请先关注")):
+            self.log.warning(f"签到失败: 账户错误.")
+            await self.fail()
+        elif any(s in text for s in ("已尝试", "过多")):
+            self.log.warning(f"签到失败: 尝试次数过多.")
+            await self.fail()
+        elif any(s in text for s in ("失败", "错误", "超时")):
             self.log.info(f"签到失败: 验证码错误, 正在重试.")
             await self.retry()
-        elif any(s in text for s in ("成功", "通过", "完成")):
+        elif any(s in text for s in ("成功", "通过", "完成", "获得")):
             matches = re.search(self.bot_success_pat, text)
             if matches:
-                self.log.info(f"[yellow]签到成功[/]: + {matches.group(1)} 分 -> {matches.group(2)} 分.")
+                try:
+                    self.log.info(f"[yellow]签到成功[/]: + {matches.group(1)} 分 -> {matches.group(2)} 分.")
+                except IndexError:
+                    self.log.info(f"[yellow]签到成功[/]: 当前/增加 {matches.group(0)} 分.")
             else:
                 matches = re.search(r"\d+", text)
                 if matches:
-                    self.log.info(f"[yellow]签到成功[/]: 当前 {matches.group(0)} 分.")
+                    self.log.info(f"[yellow]签到成功[/]: 当前/增加 {matches.group(0)} 分.")
                 else:
                     self.log.info(f"[yellow]签到成功[/].")
             self.finished.set()
         elif any(s in text for s in ("只能", "已经", "下次", "过了", "签过", "明日再来")):
             self.log.info(f"今日已经签到过了.")
             self.finished.set()
         else:
             self.log.warning(f"接收到异常返回信息: {text}")
 
     async def retry(self):
         self._retries += 1
         if self._retries <= self.retries:
             await asyncio.sleep(self.bot_retry_wait)
-            await self.send_checkin()
+            await self.send_checkin(retry=True)
         else:
             self.log.warning("超过最大重试次数.")
             self.finished.set()
 
     async def fail(self, message=None):
         self.finished.set()
         self._retries = float("inf")
 
+    async def wait_until(self, pattern: str = ".", timeout: float = None):
+        self._waiting[pattern] = e = asyncio.Event()
+        try:
+            await asyncio.wait_for(e.wait(), timeout)
+        except asyncio.TimeoutError:
+            return None
+        else:
+            msg: Message = self._waiting[pattern]
+            return msg
+
 
 class AnswerBotCheckin(BotCheckin):
     """签到类, 用于按钮模式签到."""
 
     bot_checkin_button_pat: str = None  # 所有按键需要满足的 regex 条件
 
     def __init__(self, *args, **kw):
```

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.1.0/embykeeper/telechecker/monitor/embyhub.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from pyrogram.types import Message
 
-from .base import AnswerBotCheckin
+from .base import Monitor
 
 
-class JMSCheckin(AnswerBotCheckin):
-    name = "卷毛鼠"
-    bot_username = "jmsembybot"
-    bot_captcha_len = 4
+class EmbyhubMonitor(Monitor):
+    name = "EmbyHub"
+    chat_name = "emby_hub"
+    chat_user = "ednovas"
+    chat_keyword = r"注册已开放"
+    bot_username = "EdHubot"
+    notify_create_name = True
 
-    async def on_captcha(self, message: Message, captcha: str):
-        async with self.operable:
-            if not self.message:
-                await self.operable.wait()
-            for l in captcha:
-                try:
-                    await self.message.click(l)
-                except ValueError:
-                    self.log.info(f'未能找到对应 "{l}" 的按键, 正在重试.')
-                    await self.retry()
-                    break
+    async def on_trigger(self, message: Message, key, reply):
+        await self.client.send_message(self.bot_username, f"/create {self.unique_name}")
+        self.log.bind(notify=True).info(f'已向Bot发送用户注册申请: "{self.unique_name}", 请检查结果.')
```

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.1.0/embykeeper/telechecker/bots/nebula.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,17 +64,20 @@
         query["token"] = token
         url_checkin = scheme._replace(query=urlencode(query, True)).geturl()
         connector = ProxyConnector.from_url(proxy)
         async with ClientSession(connector=connector) as session:
             async with session.get(url_checkin, headers={"User-Agent": useragent}) as resp:
                 results = await resp.json()
             message = results["message"]
+            if any(s in message for s in ("未找到用户", "权限错误")):
+                self.log.info("签到失败: 账户错误.")
+                await self.fail()
             if "失败" in message:
                 self.log.info("签到失败.")
-                return self.fail()
+                await self.fail()
             if "重复" in message:
                 self.log.info("今日已经签到过了.")
                 self.finished.set()
             elif "成功" in message:
                 self.log.info(f"[yellow]签到成功[/]: + {results['get_credit']} 分 -> {results['credit']} 分.")
                 self.finished.set()
             else:
```

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.1.0/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.1.0/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/link.py` & `embykeeper-2.1.0/embykeeper/telechecker/link.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import asyncio
-import io
 import random
-from typing import Callable, List, Optional, Tuple
+import time
+from typing import Callable, Coroutine, List, Optional, Tuple, Union
 import uuid
 
 import tomli
 from loguru import logger
-from pyrogram import Client, filters
+from pyrogram import filters
 from pyrogram.handlers import MessageHandler
 from pyrogram.types import Message
-from rich.text import Text
+
+from ..utils import async_partial, truncate_str
+from .tele import Client
 
 
 class Link:
     bot = "embykeeper_auth_bot"
 
     def __init__(self, client: Client):
         self.client = client
@@ -21,38 +23,47 @@
 
     @property
     def instance(self):
         rd = random.Random()
         rd.seed(uuid.getnode())
         return uuid.UUID(int=rd.getrandbits(128))
 
-    @staticmethod
-    async def delete_messages(messages: List[Message]):
+    async def delete_messages(self, messages: List[Message]):
         async def delete(m: Message):
             try:
                 await m.delete(revoke=True)
+                text = m.text or m.caption or "图片或其他内容"
+                text = truncate_str(text.replace("\n", ""), 30)
+                self.log.debug(f"[gray50]删除了API消息记录: {text}[/]")
             except asyncio.CancelledError:
                 pass
 
         return await asyncio.gather(*[delete(m) for m in messages])
 
     async def post(
         self, cmd, condition: Callable = None, timeout: int = 10, name: str = None
     ) -> Tuple[Optional[str], Optional[str]]:
-        results = {}
-        ok = asyncio.Event()
-        handler = self.get_handler(cmd, results, ok, condition)
-        handler = MessageHandler(handler, filters.text & filters.bot & filters.user(self.bot))
-        self.client.add_handler(handler)
+        self.log.debug(f"[gray50]禁用提醒 {timeout} 秒: {self.bot}[/]")
+        await self.client.mute_chat(self.bot, time.time() + timeout + 5)
+        future = asyncio.Future()
+        handler = MessageHandler(
+            async_partial(self._handler, cmd=cmd, future=future, condition=condition),
+            filters.text & filters.bot & filters.user(self.bot),
+        )
+        groups = self.client.dispatcher.groups
+        if 1 not in groups:
+            groups[1] = [handler]
+        else:
+            groups[1].append(handler)
         messages = []
         messages.append(await self.client.send_message(self.bot, f"/start quiet"))
         await asyncio.sleep(0.5)
         messages.append(await self.client.send_message(self.bot, cmd))
         try:
-            await asyncio.wait_for(ok.wait(), timeout=timeout)
+            results = await asyncio.wait_for(future, timeout=timeout)
         except asyncio.CancelledError:
             try:
                 await asyncio.wait_for(self.delete_messages(messages), 1.0)
             except asyncio.TimeoutError:
                 pass
             finally:
                 raise
@@ -68,77 +79,64 @@
                 return None
             elif status == "ok":
                 return results
             else:
                 self.log.warning(f"{name}出现未知错误.")
                 return None
         finally:
-            self.client.remove_handler(handler)
+            groups[1].remove(handler)
 
-    @staticmethod
-    def get_handler(cmd, results, ok, condition=None):
-        async def _handler(client: Client, message: Message):
+    async def _handler(
+        self,
+        client: Client,
+        message: Message,
+        cmd: str,
+        future: asyncio.Future,
+        condition: Union[bool, Callable[..., Coroutine], Callable] = None,
+    ):
+        try:
+            toml = tomli.loads(message.text)
+        except tomli.TOMLDecodeError:
+            self.delete_messages([message])
+        else:
             try:
-                toml = tomli.loads(message.text)
-            except tomli.TOMLDecodeError:
-                await message.delete(revoke=False)
-                return
-            else:
+                if toml.get("command", None) == cmd:
+                    if condition is None:
+                        cond = True
+                    elif asyncio.iscoroutinefunction(condition):
+                        cond = await condition(toml)
+                    elif callable(condition):
+                        cond = condition(toml)
+                    if cond:
+                        future.set_result(toml)
+                        await asyncio.sleep(0.5)
+                        await self.delete_messages([message])
+                        return
+            except asyncio.CancelledError as e:
                 try:
-                    if toml.get("command", None) == cmd:
-                        if condition is None:
-                            cond = True
-                        elif asyncio.iscoroutinefunction(condition):
-                            cond = await condition(toml)
-                        elif callable(condition):
-                            cond = condition(toml)
-                        if cond:
-                            results.update(toml)
-                            ok.set()
-                            await asyncio.sleep(0.5)
-                            await message.delete(revoke=False)
-                            return
-                except asyncio.CancelledError:
-                    try:
-                        await asyncio.wait_for(message.delete(revoke=False), 1.0)
-                    except asyncio.TimeoutError:
-                        pass
-                    finally:
-                        raise
-                else:
-                    message.continue_propagation()
-
-        return _handler
+                    await asyncio.wait_for(self.delete_messages([message]), 1)
+                except asyncio.TimeoutError:
+                    pass
+                finally:
+                    future.set_exception(e)
+            finally:
+                message.continue_propagation()
 
     async def auth(self, service: str):
         results = await self.post(f"/auth {service} {self.instance}", name=f"服务 {service.capitalize()} 认证")
         return bool(results)
 
     async def captcha(self):
         results = await self.post(f"/captcha {self.instance}", timeout=240, name="请求跳过验证码")
         if results:
             return [results.get(p, None) for p in ("token", "proxy", "useragent")]
         else:
             return None, None, None
 
     async def answer(self, question: str):
-        results = await self.post(f"/answer {self.instance} {question}", timeout=60, name="请求问题回答")
+        results = await self.post(f"/answer {self.instance} {question}", timeout=10, name="请求问题回答")
         if results:
             return results.get("answer", None)
 
-    async def sendlog(self, message):
-        results = await self.post(f"/log {self.instance} {message}", name="发送日志到 Telegram ")
+    async def send_log(self, message):
+        results = await self.post(f"/log {self.instance} {message}", name="发送日志到 Telegram")
         return bool(results)
-
-
-class TelegramStream(io.TextIOWrapper):
-    def __init__(self, link: Link = None):
-        super().__init__(io.BytesIO(), line_buffering=True)
-        self.link = link
-
-    def write(self, message):
-        message = Text.from_markup(message).plain
-        if message.endswith("\n"):
-            message = message[:-1]
-        if message:
-            asyncio.create_task(self.link.sendlog(message))
-        super().write(message + "\n")
```

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/main.py` & `embykeeper-2.1.0/embykeeper/telechecker/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import asyncio
+from datetime import datetime
 import inspect
 import logging
 import operator
 import pkgutil
 import random
-from logging import StreamHandler
 from typing import List, Type
 from importlib import import_module
 
 from dateutil import parser
 from pyrogram.enums import ChatType
 from pyrogram.handlers import MessageHandler
-from pyrogram.types import Message, Update
+from pyrogram.types import Message
 from rich import box
 from rich.live import Live
 from rich.panel import Panel
 from rich.progress import MofNCompleteColumn, Progress, SpinnerColumn
 from rich.table import Column, Table
 from rich.text import Text
-from rich.pretty import pprint
 
-from ..utils import batch, flatten, idle, time_in_range, async_partial
+from ..utils import batch, flatten, idle, time_in_range, async_partial, next_random_datetime
 from ..log import logger, formatter
 from . import __name__
-from .link import Link, TelegramStream
+from .link import Link
+from .log import TelegramStream
 from .tele import Client, ClientsSession
 from .bots.base import BaseBotCheckin
 
 logger = logger.bind(scheme="telegram")
 
 
 def get_spec(type: str):
@@ -127,48 +127,57 @@
         sender_id,
         "│",
         text,
     )
 
 
 async def checkin_task(checkiner: BaseBotCheckin, sem, wait=0):
-    await asyncio.sleep(wait)
+    if wait > 0:
+        checkiner.log.debug(f"随机启动等待: 将等待 {wait} 分钟以启动.")
+    await asyncio.sleep(wait * 60)
     async with sem:
         return await checkiner._start()
 
 
 async def gather_task(tasks, username):
     return username, await asyncio.gather(*tasks)
 
 
 async def checkiner(config: dict, instant=False):
+    logger.debug("正在启动每日签到模块, 请等待登录.")
     async with ClientsSession.from_config(config) as clients:
         coros = []
         async for tg in clients:
             log = logger.bind(scheme="telechecker", username=tg.me.name)
             if not await Link(tg).auth("checkiner"):
                 log.error(f"功能初始化失败: 权限校验不通过.")
                 continue
             sem = asyncio.Semaphore(int(config.get("concurrent", 1)))
             clses = extract(get_cls("checkiner", names=config.get("service", {}).get("checkiner", None)))
             checkiners = [
                 cls(
                     tg,
-                    retries=config.get("retries", 10),
+                    retries=config.get("retries", 4),
                     timeout=config.get("timeout", 120),
                     nofail=config.get("nofail", True),
+                    basedir=config.get("basedir", None),
+                    proxy=config.get("proxy", None),
                 )
                 for cls in clses
             ]
             tasks = []
+            names = []
             for c in checkiners:
+                names.append(c.name)
                 wait = 0 if instant else random.randint(0, 60 * config.get("random", 15))
                 task = asyncio.create_task(checkin_task(c, sem, wait))
                 tasks.append(task)
             coros.append(gather_task(tasks, username=tg.me.name))
+            if names:
+                log.debug(f'已启用签到器: {", ".join(names)}')
         while coros:
             done, coros = await asyncio.wait(coros, return_when=asyncio.FIRST_COMPLETED)
             for t in done:
                 username, results = await t
                 log = logger.bind(scheme="telechecker", username=username)
                 failed = []
                 ignored = []
@@ -179,58 +188,83 @@
                     elif results[i] is None:
                         ignored.append(c)
                     else:
                         successful.append(c)
                 spec = f"共{len(checkiners)}个"
                 if successful:
                     spec += f", {len(successful)}成功"
-                elif failed:
+                if failed:
                     spec += f", {len(failed)}失败"
-                elif ignored:
+                if ignored:
                     spec += f", {len(ignored)}跳过"
                 if failed:
                     log.error(f"签到失败 ({spec}): {','.join([f.name for f in failed])}")
                 else:
                     log.bind(notify=True).info(f"签到成功 ({spec}).")
 
 
+async def checkiner_schedule(config: dict, start_time=None, end_time=None, instant=False):
+    dt = next_random_datetime(start_time, end_time, 0)
+    while True:
+        logger.bind(scheme="telechecker").info(f"下一次签到将在 {dt.strftime('%m-%d %H:%M %p')} 进行.")
+        await asyncio.sleep((dt - datetime.now()).seconds)
+        await checkiner(config, instant=instant)
+
+
 async def monitorer(config: dict):
+    logger.debug("正在启动消息监控模块, 请等待登录.")
     jobs = []
     async with ClientsSession.from_config(config, monitor=True) as clients:
         async for tg in clients:
             log = logger.bind(scheme="telemonitor", username=tg.me.name)
             if not await Link(tg).auth("monitorer"):
                 log.error(f"功能初始化失败: 权限校验不通过.")
                 continue
             clses = extract(get_cls("monitor", names=config.get("service", {}).get("monitor", None)))
             names = []
             for cls in clses:
-                jobs.append(asyncio.create_task(cls(tg, nofail=config.get("nofail", True))._start()))
+                cls_config = config.get("monitor", {}).get(cls.__module__.rsplit(".", 1)[-1], {})
+                jobs.append(
+                    asyncio.create_task(
+                        cls(
+                            tg,
+                            nofail=config.get("nofail", True),
+                            basedir=config.get("basedir", None),
+                            proxy=config.get("proxy", None),
+                            config=cls_config,
+                        )._start()
+                    )
+                )
                 names.append(cls.name)
             if names:
-                log.info(f'已启用监控器: {",".join(names)}')
+                log.debug(f'已启用监控器: {", ".join(names)}')
         await asyncio.gather(*jobs)
 
 
-async def messager(config: dict, scheduler):
+async def messager(config: dict):
+    logger.debug("正在启动自动水群模块.")
+    messagers = []
     async with ClientsSession.from_config(config, send=True) as clients:
         async for tg in clients:
             log = logger.bind(scheme="telemessager", username=tg.me.name)
             if not await Link(tg).auth("messager"):
                 log.error(f"功能初始化失败: 权限校验不通过.")
                 continue
             clses = extract(get_cls("messager", names=config.get("service", {}).get("messager", None)))
             for cls in clses:
-                cls(
-                    {"api_id": tg.api_id, "api_hash": tg.api_hash, "phone": tg.phone_number},
-                    scheduler,
-                    username=tg.me.name,
-                    proxy=config.get("proxy", None),
-                    nofail=config.get("nofail", True),
-                ).start()
+                messagers.append(
+                    cls(
+                        {"api_id": tg.api_id, "api_hash": tg.api_hash, "phone": tg.phone_number},
+                        username=tg.me.name,
+                        nofail=config.get("nofail", True),
+                        proxy=config.get("proxy", None),
+                        basedir=config.get("basedir", None),
+                    )
+                )
+    await asyncio.gather(*[m.start() for m in messagers])
 
 
 async def follower(config: dict):
     columns = [
         Column("用户", style="cyan", justify="center"),
         Column("", max_width=1, style="white"),
         Column("", max_width=2, overflow="crop"),
@@ -340,12 +374,15 @@
                         notifier = a
                         break
             else:
                 notifier = None
         except IndexError:
             notifier = None
     if notifier:
-        async with ClientsSession([notifier], proxy=config.get("proxy", None)) as clients:
-            async for tg in clients:
-                logger.info(f'计划任务的关键消息将通过 Embykeeper Bot 发送至 "{tg.phone_number}" 账号.')
-                logger.add(StreamHandler(TelegramStream(link=Link(tg))), format=_formatter, filter=_filter)
-            await idle()
+        logger.info(f'计划任务的关键消息将通过 Embykeeper Bot 发送至 "{notifier["phone"]}" 账号.')
+        logger.add(
+            TelegramStream(
+                account=notifier, proxy=config.get("proxy", None), basedir=config.get("basedir", None)
+            ),
+            format=_formatter,
+            filter=_filter,
+        )
```

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/messager/common.py` & `embykeeper-2.1.0/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.1.0/embykeeper/telechecker/monitor/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import asyncio
 import random
 import re
 from contextlib import asynccontextmanager
 import string
-from typing import List, Sized, Union
+from typing import Iterable, List, Sized, Union
 
 from loguru import logger
+from appdirs import user_data_dir
 from pyrogram import filters
 from pyrogram.enums import ChatMemberStatus
-from pyrogram.errors import UsernameNotOccupied, UserNotParticipant
+from pyrogram.errors import UsernameNotOccupied, UserNotParticipant, FloodWait
 from pyrogram.handlers import EditedMessageHandler, MessageHandler
 from pyrogram.types import Message, User
 
 from ...utils import to_iterable, truncate_str, AsyncCountPool
 from ..tele import Client
 
 __ignore__ = True
@@ -78,53 +79,57 @@
         else:
             unique: str = user.name.lower()
         unique = re.sub(r"[^A-Za-z0-9]", "", unique)
         random_bits = 10 - len(unique)
         if random_bits:
             random_bits = "".join(random.choice(string.digits) for _ in range(random_bits))
             unique = unique + random_bits
-        log.info(f'当监控到开注时, 将以用户名 "{unique}" 注册, 请[yellow]保证[/]具有一定独特性以避免注册失败.')
+        log.info(f'([magenta]默认[/]) 当监控到开注时, 将以用户名 "{unique}" 注册, 请[yellow]保证[/]具有一定独特性以避免注册失败.')
         return unique
 
 
 class Monitor:
     group_pool = AsyncCountPool(base=1000)
     unique_cache = UniqueUsername()
 
     name: str = None  # 监控器名称
-    chat_name: str = None  # 群聊名称
+    chat_name: Union[str, List[str]] = []  # 群聊名称
     chat_allow_outgoing: bool = False  # 是否支持自己发言触发
     chat_user: Union[str, List[str]] = []  # 仅被列表中用户的发言触发
     chat_keyword: Union[str, List[str]] = []  # 仅当消息含有列表中的关键词时触发, 支持 regex
     chat_probability: float = 1.0  # 发信概率
     chat_delay: int = 0  # 发信延迟
     chat_follow_user: int = 0  # 需要等待 N 个用户发送 {chat_reply} 方可回复
     chat_reply: str = None  # 回复的内容, 可以通过 @property 类属性重写.
     notify_create_name: bool = False  # 启动时生成 unique name 并提示
+    allow_edit: bool = True  # 检测编辑消息内容
 
-    def __init__(self, client: Client, nofail=True):
+    def __init__(self, client: Client, nofail=True, basedir=None, proxy=None, config: dict = {}):
         self.client = client
         self.nofail = nofail
+        self.basedir = basedir or user_data_dir(__name__)
+        self.proxy = proxy
+        self.config = config
         self.log = logger.bind(scheme="telemonitor", name=self.name, username=client.me.name)
         self.session = None
         self.failed = asyncio.Event()
 
     def get_filter(self):
         filter = filters.caption | filters.text
         if self.chat_name:
-            filter = filter & filters.chat(self.chat_name)
+            filter = filter & filters.chat(to_iterable(self.chat_name))
         if not self.chat_allow_outgoing:
             filter = filter & (~filters.outgoing)
         return filter
 
     def get_handlers(self):
-        return [
-            MessageHandler(self._message_handler, self.get_filter()),
-            EditedMessageHandler(self._message_handler, self.get_filter()),
-        ]
+        handlers = [MessageHandler(self._message_handler, self.get_filter())]
+        if self.allow_edit:
+            handlers.append(EditedMessageHandler(self._message_handler, self.get_filter()))
+        return handlers
 
     @asynccontextmanager
     async def listener(self):
         group = await self.group_pool.append(self)
         handlers = self.get_handlers()
         for h in handlers:
             self.client.add_handler(h, group=group)
@@ -144,72 +149,89 @@
             if self.nofail:
                 self.log.opt(exception=e).warning(f"初始化错误:")
                 return False
             else:
                 raise
 
     async def start(self):
-        try:
-            chat = await self.client.get_chat(self.chat_name)
-            self.chat_name = chat.id
-        except UsernameNotOccupied:
-            self.log.warning(f'初始化错误: 群组 "{self.chat_name}" 不存在.')
-            return False
+        chat_ids = []
+        for cn in to_iterable(self.chat_name):
+            while True:
+                try:
+                    chat = await self.client.get_chat(cn)
+                    chat_ids.append(chat.id)
+                except UsernameNotOccupied:
+                    self.log.warning(f'初始化错误: 群组 "{self.chat_name}" 不存在.')
+                    return False
+                except KeyError as e:
+                    self.log.info(f"初始化错误: 无法访问, 您可能已被封禁: {e}.")
+                    return False
+                except FloodWait as e:
+                    self.log.info(f"初始化信息: Telegram 要求等待 {e.value} 秒.")
+                    await asyncio.sleep(e.value)
+                else:
+                    break
+        self.chat_name = chat_ids
         try:
             me = await chat.get_member("me")
         except UserNotParticipant:
-            self.log.warning(f'初始化错误: 尚未加入群组 "{chat.title}".')
+            self.log.warning(f'跳过监控: 尚未加入群组 "{chat.title}".')
             return False
         if me.status in (ChatMemberStatus.LEFT, ChatMemberStatus.RESTRICTED):
             self.log.warning(f'初始化错误: 被群组 "{chat.title}" 禁言.')
             return False
         if self.notify_create_name:
             self.unique_name = self.get_unique_name()
+
         spec = f"[green]{chat.title}[/] [gray50](@{chat.username})[/]"
-        self.log.info(f"开始监视: {spec}.")
-        async with self.listener():
-            await self.failed.wait()
-            self.log.error(f"发生错误, 不再监视: {spec}.")
+        if await self.init():
+            self.log.info(f"开始监视: {spec}.")
+            async with self.listener():
+                await self.failed.wait()
+                self.log.error(f"发生错误, 不再监视: {spec}.")
+                return False
+        else:
+            self.log.bind(notify=True).warning(f"机器人状态初始化失败, 监控将停止.")
             return False
 
-    def get_key(self, message: Message):
+    async def init(self):
+        return True
+
+    @classmethod
+    def keys(cls, message: Message):
         sender = message.from_user
         if (
             sender
-            and self.chat_user
-            and not any(i in to_iterable(self.chat_user) for i in (sender.id, sender.username))
+            and cls.chat_user
+            and not any(i in to_iterable(cls.chat_user) for i in (sender.id, sender.username))
         ):
             return False
         text = message.text or message.caption
-        if self.chat_keyword:
-            for k in to_iterable(self.chat_keyword):
-                match = re.search(k, text, re.IGNORECASE)
-                if match:
-                    return match.groups() or match.group(0)
-            else:
-                return False
+        if cls.chat_keyword:
+            for k in to_iterable(cls.chat_keyword):
+                for m in re.findall(k, text, re.IGNORECASE):
+                    yield m
         else:
             return text
 
-    async def get_reply(self, message: Message, keys: str):
+    async def get_reply(self, message: Message, key: Union[str, List[str]]):
         if callable(self.chat_reply):
-            result = self.chat_reply(message, keys)
+            result = self.chat_reply(message, key)
             if asyncio.iscoroutinefunction(self.chat_reply):
                 return await result
             else:
                 return result
         else:
             return self.chat_reply
 
     @staticmethod
     def get_spec(keys):
-        if isinstance(keys, str):
-            return truncate_str(keys.replace("\n", " "), 30)
-        else:
-            return ", ".join(keys)
+        if isinstance(keys, Iterable) and not isinstance(keys, str):
+            keys = " ".join([str(k).strip() for k in keys])
+        return truncate_str(keys.replace("\n", " ").strip(), 30)
 
     async def _message_handler(self, client: Client, message: Message):
         try:
             await self.message_handler(client, message)
         except OSError as e:
             self.log.info(f'发生错误: "{e}", 忽略.')
         except asyncio.CancelledError:
@@ -220,39 +242,42 @@
                 self.log.opt(exception=e).warning(f"发生错误:")
             else:
                 raise
         finally:
             message.continue_propagation()
 
     async def message_handler(self, client: Client, message: Message):
-        keys = self.get_key(message)
-        if keys:
-            spec = self.get_spec(keys)
-            self.log.info(f'监听到关键信息: "{spec}".')
+        for key in self.keys(message):
+            spec = self.get_spec(key)
+            self.log.debug(f"监听到关键信息: {spec}.")
             if random.random() >= self.chat_probability:
-                self.log.info(f'由于概率设置, 不予回应: "{spec}".')
+                self.log.info(f"由于概率设置, 不予回应: {spec}.")
                 return False
-            reply = await self.get_reply(message, keys)
+            reply = await self.get_reply(message, key)
             if self.session:
                 await self.session.cancel()
             if self.chat_follow_user:
                 self.log.info(f"将等待{self.chat_follow_user}个人回复: {reply}")
             self.session = Session(reply, follows=self.chat_follow_user, delays=self.chat_delay)
             if await self.session.wait():
                 self.session = None
-                self.log.info(f'执行监听响应: "{spec}".')
-                await self.on_trigger(message, keys, reply)
+                await self.on_trigger(message, key, reply)
         else:
             if self.session and not self.session.followed.is_set():
                 text = message.text or message.caption
                 if self.session.reply == text:
                     now = await self.session.follow()
                     self.log.info(
                         f'从众计数 ({self.chat_follow_user - now}/{self.chat_follow_user}): "{message.from_user.name}"'
                     )
 
     async def on_trigger(self, message: Message, keys: Union[List[str], str], reply: str):
         if reply:
             return await self.client.send_message(message.chat.id, reply)
 
     def get_unique_name(self):
-        return Monitor.unique_cache[self.client.me]
+        unique_name = self.config.get("unique_name", None)
+        if unique_name:
+            self.log.info(f'根据您的设置, 当监控到开注时, 该站点将以用户名 "{unique_name}" 注册.')
+            return unique_name
+        else:
+            return Monitor.unique_cache[self.client.me]
```

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.1.0/embykeeper/telechecker/monitor/bgk.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 
 class BGKMonitor(Monitor):
     name = "不给看"
     chat_name = "Ephemeralemby"
     chat_keyword = r"(?:^|\s)([a-zA-Z0-9]{32})(?!\S)"
     bot_username = "UnknownEmbyBot"
     notify_create_name = True
+    allow_edit = False
 
-    async def on_trigger(self, message: Message, keys, reply):
+    async def on_trigger(self, message: Message, key, reply):
         await self.client.send_message(self.bot_username, "/invite")
-        await self.client.send_message(self.bot_username, keys[0])
+        await self.client.send_message(self.bot_username, key)
         await self.client.send_message(self.bot_username, self.unique_name)
-        self.log.bind(notify=True).info(f'已向Bot发送邀请码: "{keys[0]}", 请查看.')
+        self.log.bind(notify=True).info(f'已向Bot发送邀请码: "{key}", 请查看.')
```

### Comparing `embykeeper-2.0.9/embykeeper/telechecker/tele.py` & `embykeeper-2.1.0/embykeeper/telechecker/tele.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+from datetime import datetime
+import time
 import asyncio
 from typing import AsyncGenerator, Optional, Union
 
 from rich.prompt import Prompt
 from appdirs import user_data_dir
 from loguru import logger
 from pyrogram import Client as _Client
-from pyrogram import raw, types, utils
+from pyrogram import raw, types, utils, filters
 from pyrogram.enums import SentCodeType
-from pyrogram.errors import BadRequest, RPCError, Unauthorized, SessionPasswordNeeded
+from pyrogram.errors import (
+    BadRequest,
+    RPCError,
+    Unauthorized,
+    SessionPasswordNeeded,
+    CodeInvalid,
+    PhoneCodeInvalid,
+)
+from pyrogram.handlers import MessageHandler
 from aiocache import Cache
 
 from .. import __name__, __version__
-from ..utils import to_iterable
+from ..utils import async_partial, to_iterable
 
 logger = logger.bind(scheme="telegram")
 
 
 def _name(self: Union[types.User, types.Chat]):
     return " ".join([n for n in (self.first_name, self.last_name) if n])
 
@@ -49,31 +59,31 @@
                     SentCodeType.CALL: "来电",
                     SentCodeType.FLASH_CALL: "闪存呼叫",
                     SentCodeType.FRAGMENT_SMS: "Fragment短信",
                     SentCodeType.EMAIL_CODE: "邮件",
                 }
                 if not self.phone_code:
                     if retry:
-                        msg = f'验证码错误, 请在重新输入 "{self.phone_number}" 的登录验证码: '
+                        msg = f'验证码错误, 请重新输入 "{self.phone_number}" 的登录验证码'
                     else:
-                        msg = f'请在{code_target[sent_code.type]}接收 "{self.phone_number}" 的登录验证码: '
-                    self.phone_code = Prompt.ask(" " * 29 + msg)
+                        msg = f'请从{code_target[sent_code.type]}接收 "{self.phone_number}" 的登录验证码'
+                    self.phone_code = Prompt.ask(" " * 23 + msg)
                 signed_in = await self.sign_in(self.phone_number, sent_code.phone_code_hash, self.phone_code)
-            except BadRequest:
+            except (CodeInvalid, PhoneCodeInvalid):
                 self.phone_code = None
                 retry = True
             except SessionPasswordNeeded:
                 retry = False
                 while True:
                     if not self.password:
                         if retry:
-                            msg = f'密码错误, 请重新输入 "{self.phone_number}" 的两步验证密码 (不显示, 按回车确认):'
+                            msg = f'密码错误, 请重新输入 "{self.phone_number}" 的两步验证密码 (不显示, 按回车确认)'
                         else:
-                            msg = f'需要输入 "{self.phone_number}" 的两步验证密码 (不显示, 按回车确认): '
-                        self.password = Prompt.ask(" " * 29 + msg, password=True)
+                            msg = f'需要输入 "{self.phone_number}" 的两步验证密码 (不显示, 按回车确认)'
+                        self.password = Prompt.ask(" " * 23 + msg, password=True)
                     try:
                         return await self.check_password(self.password)
                     except BadRequest:
                         self.password = None
                         retry = True
             else:
                 break
@@ -149,49 +159,86 @@
                 yield dialog
 
                 current += 1
 
                 if current >= total:
                     return
 
+    async def wait_reply(
+        self, chat_id: Union[int, str], text: str = None, timeout: float = 3, outgoing=False
+    ):
+        async def handler_func(client, message, future: asyncio.Future):
+            future.set_result(message)
+
+        future = asyncio.Future()
+        filter = filters.chat(chat_id)
+        if not outgoing:
+            filter = filter & (~filters.outgoing)
+        handler = MessageHandler(async_partial(handler_func, future=future), filter)
+        groups = self.dispatcher.groups
+        if 0 not in groups:
+            groups[0] = [handler]
+        else:
+            groups[0].append(handler)
+        try:
+            if text:
+                await self.send_message(chat_id, text)
+            msg: types.Message = await asyncio.wait_for(future, timeout)
+            return msg
+        finally:
+            groups[0].remove(handler)
+
+    async def mute_chat(self, chat_id: Union[int, str], until: Union[int, datetime]):
+        if isinstance(until, datetime):
+            until = until.timestamp()
+
+        return await self.invoke(
+            raw.functions.account.UpdateNotifySettings(
+                peer=raw.types.InputNotifyPeer(peer=await self.resolve_peer(chat_id)),
+                settings=raw.types.InputPeerNotifySettings(
+                    show_previews=False,
+                    mute_until=int(until),
+                ),
+            )
+        )
+
 
 class ClientsSession:
     pool = {}
     lock = asyncio.Lock()
     watch = None
 
     @classmethod
     def from_config(cls, config, **kw):
         accounts = config.get("telegram", [])
         for k, v in kw.items():
             accounts = [a for a in accounts if a.get(k, None) in to_iterable(v)]
-        return cls(accounts=accounts, proxy=config.get("proxy", None))
+        return cls(accounts=accounts, proxy=config.get("proxy", None), basedir=config.get("basedir", None))
 
     @classmethod
     async def watchdog(cls, timeout=120):
         logger.debug("Telegram 账号池 watchdog 启动.")
         try:
             counter = {}
             while True:
                 await asyncio.sleep(10)
-                for p, v in cls.pool.items():
+                for p in list(cls.pool):
                     try:
-                        if v[1] <= 0:
+                        if cls.pool[p][1] <= 0:
                             if p in counter:
                                 counter[p] += 1
                                 if counter[p] >= timeout / 10:
                                     await cls.clean(p)
                             else:
                                 counter[p] = 1
                         else:
                             counter.pop(p, None)
-                    except TypeError:
+                    except (TypeError, KeyError):
                         pass
         except asyncio.CancelledError:
-            print("\r正在停止... ", end="")
             await cls.shutdown()
 
     @classmethod
     async def clean(cls, phone):
         async with cls.lock:
             entry = cls.pool.get(phone, None)
             if not entry:
@@ -202,39 +249,46 @@
                 return
             if not ref:
                 logger.debug(f'登出账号 "{client.phone_number}".')
                 await client.stop()
                 cls.pool.pop(phone, None)
 
     @classmethod
+    async def clean_all(cls):
+        for phone in list(cls.pool):
+            await cls.clean(phone)
+
+    @classmethod
     async def shutdown(cls):
+        print("\r正在停止...\r", end="", flush=True)
         for v in cls.pool.values():
             if isinstance(v, asyncio.Task):
                 v.cancel()
             else:
                 client, ref = v
                 client.dispatcher.updates_queue.put_nowait(None)
                 for t in client.dispatcher.handler_worker_tasks:
                     try:
                         await t
                     except asyncio.CancelledError:
                         pass
         while len(asyncio.all_tasks()) > 1:
             await asyncio.sleep(0.1)
-        print(f"Telegram 账号池停止.", end="")
+        print(f"Telegram 账号池停止.\r", end="")
         for v in cls.pool.values():
             if isinstance(v, tuple):
                 client: Client = v[0]
                 await client.storage.save()
                 await client.storage.close()
-                # print(f'登出账号 "{client.phone_number}".')
+                logger.debug(f'登出账号 "{client.phone_number}".')
 
-    def __init__(self, accounts, proxy=None, quiet=False):
+    def __init__(self, accounts, proxy=None, basedir=None, quiet=False):
         self.accounts = accounts
         self.proxy = proxy
+        self.basedir = basedir or user_data_dir(__name__)
         self.phones = []
         self.done = asyncio.Queue()
         self.quiet = quiet
         if not self.watch:
             self.__class__.watch = asyncio.create_task(self.watchdog())
 
     async def login(self, account, proxy):
@@ -247,67 +301,83 @@
                         app_version=f"{__name__.capitalize()} {__version__}",
                         name=account["phone"],
                         api_id=account["api_id"],
                         api_hash=account["api_hash"],
                         phone_number=account["phone"],
                         proxy=proxy,
                         lang_code="zh",
-                        workdir=user_data_dir(__name__),
+                        workdir=self.basedir,
                     )
                     await client.start()
                 except Unauthorized:
                     await client.storage.delete()
+                except KeyError:
+                    logger.warning(f'登录账号 "{client.phone_number}" 时发生异常, 可能是由于网络错误, 将在 3 秒后重试.')
+                    await asyncio.sleep(3)
                 else:
                     break
         except asyncio.CancelledError:
             raise
         except RPCError as e:
             logger.error(f'登录账号 "{client.phone_number}" 失败 ({e.MESSAGE.format(value=e.value)}), 将被跳过.')
         except Exception as e:
-            logger.exception(f'登录账号 "{client.phone_number}" 时发生异常, 将被跳过:')
+            logger.opt(exception=e).error(f'登录账号 "{client.phone_number}" 时发生异常, 将被跳过:')
         else:
+            logger.debug(f'登录账号 "{client.phone_number}" 成功.')
             return client
 
     async def loginer(self, account):
         client = await self.login(account, self.proxy)
         if isinstance(client, Client):
             async with self.lock:
                 phone = account["phone"]
                 self.pool[phone] = (client, 1)
                 self.phones.append(phone)
                 await self.done.put(client)
+                logger.debug(f"Telegram 账号池计数增加: {phone} => 1")
+        else:
+            await self.done.put(None)
 
     async def __aenter__(self):
         for a in self.accounts:
             phone = a["phone"]
-            async with self.lock:
+            try:
+                await self.lock.acquire()
                 if phone in self.pool:
                     if isinstance(self.pool[phone], asyncio.Task):
                         self.lock.release()
                         await self.pool[phone]
                         await self.lock.acquire()
+                    if isinstance(self.pool[phone], asyncio.Task):
+                        continue
                     client, ref = self.pool[phone]
                     ref += 1
                     self.pool[phone] = (client, ref)
+                    self.phones.append(phone)
                     await self.done.put(client)
+                    logger.debug(f"Telegram 账号池计数增加: {phone} => {ref}")
                 else:
                     self.pool[phone] = asyncio.create_task(self.loginer(a))
+            finally:
+                try:
+                    self.lock.release()
+                except RuntimeError:
+                    pass
         return self
 
     def __aiter__(self):
         async def aiter():
             for _ in range(len(self.accounts)):
                 client: Client = await self.done.get()
-                if client == None:
-                    break
-                yield client
+                if client:
+                    yield client
 
         return aiter()
 
     async def __aexit__(self, type, value, tb):
         async with self.lock:
             for phone in self.phones:
                 entry = self.pool.get(phone, None)
                 client, ref = entry
                 ref -= 1
                 self.pool[phone] = (client, ref)
-                # print(f"Telegram 账号池计数 {client.phone_number} => {ref}.")
+                logger.debug(f"Telegram 账号池计数降低: {phone} => {ref}")
```

### Comparing `embykeeper-2.0.9/embykeeper/utils.py` & `embykeeper-2.1.0/embykeeper/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import asyncio
 from collections import namedtuple
+from datetime import date, datetime, time, timedelta
 from functools import wraps
+import random
 import sys
-from typing import Any, Iterable, Union
+from typing import Any, Coroutine, Iterable, Union
 
 from loguru import logger
 import click
-from typer import Typer, Exit
+from typer import Typer
 from typer.core import TyperCommand
 
 from . import __url__, __name__
 
 Flagged = namedtuple("Flagged", ("noflag", "flag"))
 
 
@@ -22,22 +24,24 @@
 
 class AsyncTyper(Typer):
     def async_command(self, *args, **kwargs):
         def decorator(async_func):
             @wraps(async_func)
             def sync_func(*_args, **_kwargs):
                 try:
-                    return asyncio.run(async_func(*_args, **_kwargs))
+                    asyncio.run(async_func(*_args, **_kwargs))
                 except KeyboardInterrupt:
-                    print("\r", end="")
+                    print("\r", end="", flush=True)
                     logger.info("所有客户端已停止, 欢迎您再次使用 Embykeeper.")
                 except Exception as e:
-                    print("\r", end="")
+                    print("\r", end="", flush=True)
                     fail_message(e)
                     sys.exit(1)
+                else:
+                    logger.info("所有任务已完成, 欢迎您再次使用 Embykeeper.")
 
             self.command(*args, **kwargs)(sync_func)
             return async_func
 
         return decorator
 
 
@@ -76,27 +80,28 @@
 
 
 class AsyncTaskPool:
     def __init__(self):
         self.waiter = asyncio.Condition()
         self.tasks = []
 
-    def add(self, coro):
+    def add(self, coro: Coroutine):
         async def wrapper():
             task = asyncio.ensure_future(coro)
             await asyncio.wait([task])
             async with self.waiter:
                 self.waiter.notify()
                 return await task
 
         t = asyncio.create_task(wrapper())
+        t.set_name(coro.__name__)
         self.tasks.append(t)
 
     async def as_completed(self):
-        while True:
+        while self.tasks:
             async with self.waiter:
                 await self.waiter.wait()
                 for t in self.tasks:
                     if t.done():
                         yield t
                         self.tasks.remove(t)
 
@@ -154,7 +159,50 @@
         return await f(*args1, *args2, **kw1, **kw2)
 
     return func
 
 
 async def idle():
     await asyncio.Event().wait()
+
+
+def random_time(start_time: time = None, end_time: time = None):
+    start_datetime = datetime.combine(date.today(), start_time or time(0, 0))
+    end_datetime = datetime.combine(date.today(), end_time or time(23, 59, 59))
+    if end_datetime < start_datetime:
+        end_datetime += timedelta(days=1)
+    time_diff_seconds = (end_datetime - start_datetime).seconds
+    random_seconds = random.randint(0, time_diff_seconds)
+    random_time = (start_datetime + timedelta(seconds=random_seconds)).time()
+    return random_time
+
+
+def next_random_datetime(start_time: time = None, end_time: time = None, interval_days=1):
+    min_datetime = datetime.now() + timedelta(days=interval_days)
+    target_time = random_time(start_time, end_time)
+    offset_date = 0
+    while True:
+        offset_date += 1
+        t = datetime.combine(datetime.now() + timedelta(days=offset_date), target_time)
+        if t >= min_datetime:
+            break
+    return t
+
+
+def humanbytes(B: float):
+    """Return the given bytes as a human friendly KB, MB, GB, or TB string."""
+    B = float(B)
+    KB = float(1024)
+    MB = float(KB**2)  # 1,048,576
+    GB = float(KB**3)  # 1,073,741,824
+    TB = float(KB**4)  # 1,099,511,627,776
+
+    if B < KB:
+        return "{0} {1}".format(B, "Bytes" if 0 == B > 1 else "Byte")
+    elif KB <= B < MB:
+        return "{0:.2f} KB".format(B / KB)
+    elif MB <= B < GB:
+        return "{0:.2f} MB".format(B / MB)
+    elif GB <= B < TB:
+        return "{0:.2f} GB".format(B / GB)
+    elif TB <= B:
+        return "{0:.2f} TB".format(B / TB)
```

### Comparing `embykeeper-2.0.9/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,12 @@
-Metadata-Version: 2.1
-Name: embykeeper
-Version: 2.0.9
-Summary: Daily checkin automator for emby bots in telegram.
-Author-email: jackzzs <jackzzs@outlook.com>
-Project-URL: Homepage, https://github.com/embykeeper/embykeeper
-Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: <3.11,>=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper) [![telegram badge](https://img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
+[![build status](https://img.shields.io/github/actions/workflow/status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
 
 <p align="center">
   <a href='https://github.com/embykeeper/embykeeper'>
-    <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
+    <img src="https://github.com/embykeeper/embykeeper/raw/main/images/logo.svg" alt="Embykeeper" />
   </a>
 </p>
 <p align="center">
     <b>自动签到 定时保号 按需水群</b>
 </p>
 
 ---
@@ -35,50 +15,54 @@
 
 ## 声明
 
 本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关.
 
 本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关.
 
-本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Telegram 讨论组](https://t.me/embykeeper_chat) 与开发团队进行交流.
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论.
 
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
-  - 支持群组
-    - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
-    - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
-    - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
-    - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
-    - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
-    - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
-    - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
-    - Pornemby (_测试中_): [频道](https://t.me/pornembyservice) [机器人](https://t.me/PronembyTGBot2_bot)
-    - 其他非 Emby 相关:
-      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_): [机器人](https://t.me/sosdbot)
-    - 默认禁用:
-      - Pornemby 科举考试 (_测试中_): [活动频道](https://t.me/PornembyFun)
-      - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-      - ~~垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)~~ (无响应)
-  - 特性
-    - 验证码识别与自动重试
-    - 多账户签到
-    - 网页类型签到
+  - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
+  - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
+  - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
+  - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
+  - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+  - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
+  - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
+  - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
+  - 其他非 Emby 相关:
+    - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
+  - 默认禁用:
+    - ~~卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)~~ (机器人逻辑频繁变动, 暂时禁用)
+    - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
+    - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
+
 - Emby 保活
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
+
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
-  - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
+  - 默认禁用:
+    - ~~NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)~~ (停服)
+
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
+  - Pornemby 科举考试: [活动频道](https://t.me/PornembyFun) (由于需要使用 OpenAI API 进行回答, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime), 回答准确率一般请谨慎使用)
   - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
+  - Viper 抢邀请码: [频道](https://t.me/viper_emby_channel) [群组](https://t.me/Viper_Emby_Chat) [机器人](https://t.me/viper_emby_bot)
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+  - Misty 开注自动注册: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
+  - 默认禁用:
+    - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
 ### 从 PyPi 安装
 
 Embykeeper 可以通过 `python` 运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
 
@@ -90,15 +74,34 @@
 
 随后, 您需要执行:
 
 ```bash
 embykeeper
 ```
 
-命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)).
+命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = 1080
+scheme = "socks5"
+
+[[telegram]]
+api_id = "27894236"
+api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899"
+
+[[emby]]
+url = "https://weiss-griffin.com/"
+username = "carrie19"
+password = "s*D7MMCpS$"
+```
+
+对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
 
 随后, 您需要再次执行:
 
 ```bash
 embykeeper
 ```
 
@@ -124,144 +127,147 @@
 
 ```
 pip install -U embykeeper
 ```
 
 然后重新运行应用.
 
-### 从 Docker 安装
+### 从源码构建
 
-Embykeeper 可以通过 `docker` 运行, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
 
 ```bash
-touch config.toml
-docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
+git clone https://github.com/embykeeper/embykeeper.git
+cd embykeeper
+pip install -e .
 ```
 
-命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+然后即可执行 Embykeeper:
 
-```toml
-[proxy]
-hostname = "127.0.0.1"
-port = "1080"
-scheme = "socks5"
+```bash
+embykeeper
+```
 
-[[telegram]]
-api_id = "27894236"
-api_hash = "622159182fdd4b15b627eeb3ac695271"
-phone = "+8612109347899"
+详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
+
+当版本更新时, 您需要执行:
 
-[[emby]]
-url = "https://weiss-griffin.com/"
-username = "carrie19"
-password = "s*D7MMCpS$"
+```
+git pull
 ```
 
-对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
+然后重新运行应用.
 
-随后, 您需要再次执行:
+### 从 Docker 部署
+
+Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
-docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
-您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息 (详见[从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)).
 
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+随后, 您需要再次执行:
 
 ```bash
-docker run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
-或者使用 [docker-compose](https://docs.docker.com/compose/) ([watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务):
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper.
+
+### 通过 Docker Compose 部署
+
+您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
+
+**注意**: 您需要先进行过 [从 Docker 部署](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
+
+您需要新建一个文件 `docker-compose.yml`:
 
 ```yaml
 version: '3'
 services:
   embykeeper:
     container_name: embykeeper
-    image: cembykeeper/embykeeper
+    image: embykeeper/embykeeper
     restart: unless-stopped
     volumes:
-      - ./config.toml:/app/config.toml
+      - ./embykeeper:/app
+    network_mode: host
   watchtower:
     container_name: watchtower
     image: containrrr/watchtower
     restart: unless-stopped
     volumes:
       - /var/run/docker.sock:/var/run/docker.sock:rw
 ```
 
-即可在后台启动 embykeeper.
-
-您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
-
-如果您需要使用主机上的代理服务器 (例如 `https://localhost:1080`), 您可能需要使用 `--net=host` 参数以使用主机网络模式.
-
-### 从源码构建
-
-和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
-
-```bash
-git clone https://github.com/embykeeper/embykeeper.git
-cd embykeeper
-pip install -e .
-```
+其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务.
 
-然后即可执行 Embykeeper:
+然后运行以下命令以启动:
 
 ```bash
-embykeeper
+docker-compose up -d
 ```
 
-详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
-
-当版本更新时, 您需要执行:
-
-```
-git pull
-```
+即可在后台启动 embykeeper.
 
-然后重新运行应用.
+您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
 
 ## 命令行帮助
 
 您可以通过运行 `embykeeper -h` 以获取帮助:
 
 ```bash
 $ embykeeper -h
 
 欢迎使用 Embykeeper. 🎦 无参数默认开启全部功能.
 
 参数:
     config  配置文件 (置空以生成)
 模块开关:
-    --checkin     -c   启用每日指定时间签到 (不指定值时默认为6:00PM)
+    --checkin     -c   启用每日签到 (不指定值时默认为<8:00PM,9:00PM>随机时间)
     --emby        -e   启用每隔天数Emby自动保活 (不指定值时默认为每7天)
     --monitor     -m   启用群聊监视
     --send        -s   启用自动水群
 调试参数:
     --no-instant  -I   不立刻执行一次计划任务
-    --debug       -d   开启调试模式, 错误将会导致程序停止运行
+    --once        -o   仅执行一次任务而不计划执行
+    --debug       -d   开启调试输出, 错误将会导致程序停止运行
     --version     -v   打印 Embykeeper 版本
     --follow      -f   仅启动消息调试
     --analyze     -a   仅启动历史信息分析
+    --basedir          设定输出文件默认位置
 ```
 
 例如:
 
 ```bash
+# 启动所有功能 (在各账号配置中进一步设置功能开启/关闭)
+$ embykeeper config.toml
+
 # 仅启动每日签到
 $ embykeeper config.toml -c
 
 # 仅启动每日 8:00 PM 签到
 $ embykeeper config.toml -c 8:00PM
 
+# 仅启动每日 8:00 PM - 9:00 PM 随机时间签到
+$ embykeeper config.toml -c <8:00PM,9:00PM>
+
 # 启动所有功能, 同时调整签到时间为 8:00 AM, 调整保活间隔天数为 14
 $ embykeeper config.toml -c 8:00PM -e 14 -m -s
+
+# 启动所有功能, 只运行一次
+$ embykeeper config.toml --once
+
+# 启动所有功能, 不立即执行一次签到/保活
+$ embykeeper config.toml -I
 ```
 
 您也可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
 
 ```bash
 # 启动历史信息分析
 $ embykeeper config.toml -a
@@ -296,24 +302,24 @@
 
 ##### 开发者团队
 
 - [jackzzs](https://github.com/jackzzs)
 
 ##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
 
-![kitty](images/kitty.gif)
+![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
 
 ## 配置项
 
 | 设置项       | 值类型             | 简介                                         | 默认值  |
 | ------------ | ------------------ | -------------------------------------------- | ------- |
 | `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `10`    |
+| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`    |
 | `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
-| `random`     | `int`              | Telegram 机器人签到定时任务时间随机量 (分钟) | `15`    |
+| `random`     | `int`              | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
 | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
 | `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
 | `proxy`      | `dict`             | 代理设置                                     | `{}`    |
 | `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
 | `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
 
 `service`设置可以为:
@@ -331,15 +337,15 @@
 | 站点 | 名称 | | 站点 | 名称 |
 | --- | --- | --- |--- | --- |
 | 垃圾影音 | `ljyy` | | 搜书神器 | `sosdbot` |
 | 卷毛鼠 IPTV | `jms_iptv` | | 终点站 | `terminus` |
 | Pornemby | `pornemby` | | Singularity | `singularity` |
 | Peach | `peach` | | Nebula | `nebula` |
 | Bluesea | `bluesea` | | Embyhub | `embyhub` |
-| 卷毛鼠 | `jms` | | | |
+| 卷毛鼠 | `jms` | | 卡戎 | `charon` |
 
 `proxy` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                    | 默认值      |
 | ---------- | ------ | --------------------------------------- | ----------- |
 | `hostname` | `str`  | 代理服务器地址                          | `localhost` |
 | `port`     | `int`  | 代理端口号                              | `1080`      |
@@ -361,14 +367,25 @@
 | ---------- | ------ | --------------------------------------------------------- | ------ |
 | `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
 | `username` | `str`  | Emby 服务器用户名                                         |        |
 | `password` | `str`  | Emby 服务器密码                                           |        |
 | `time`     | `int`  | 模拟观看的时间 (秒)                                       | `800`  |
 | `progress` | `int`  | 观看后模拟进度条保存的时间 (秒)                           | `1000` |
 
+服务可以进行特定配置, 如下所示:
+
+```toml
+
+[monitor.bgk] # 支持 bgk, embyhub, polo
+unique_name = "your_username_for_registeration" # 自动抢注时使用的用户名
+
+[monitor.pornemby]
+only_history = true # 仅当问题历史中找到答案时自动回答
+```
+
 ## 代码重用与开发
 
 代码架构如下:
 
 ```mermaid
 flowchart TD
     A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
@@ -415,7 +432,11 @@
                 await self.retry()
                 break
 ```
 
 上述代码实现每次按对应一个字符按键的功能.
 
 当您实现一个新的签到器时, 欢迎您提出 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 以帮助更多人使用!
+
+## 趋势
+
+[![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

#### html2text {}

```diff
@@ -1,29 +1,20 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.0.9 Summary: Daily checkin
-automator for emby bots in telegram. Author-email: jackzzs
-outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
-Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
-Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
-:: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: <3.11,>=3.7 Description-Content-Type: text/markdown License-
-File: LICENSE [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https:/
-/pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/
-dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
+[![build status](https://img.shields.io/github/actions/workflow/status/
+embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/
+embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/
+embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://
+img.shields.io/pypi/dm/
+embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
 embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
 embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
 embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
 [telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
 embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
-channel-green)](https://t.me/embykeeper) [![telegram badge](https://
-img.shields.io/badge/telegram-group-blue)](https://t.me/embykeeper_chat)
+channel-green)](https://t.me/embykeeper)
                                  [Embykeeper]
                     èªå¨ç­¾å° å®æ¶ä¿å· æéæ°´ç¾¤
 --- Embykeeper æ¯ä¸ä¸ªå¨ä¸­æç¤¾ç¾¤è§åä¸ç¨äº Emby
 å½±è§æå¡å¨çç­¾å°åä¿å·çèªå¨æ§è¡å·¥å·, åºäº Pyrogram
 ç¼åå¹¶å·æå¯æå±æ§. ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
 æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³, å¨ä½¿ç¨ Embykeeper
 æ¶é æçä¸åæå¤± (åæ¬ä½ä¸éäº Emby æ Telegram
@@ -36,127 +27,143 @@
 å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
 å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
 æ¬é¡¹ç®ä»æä¾å·¥å·,
 å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
 å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
-æ¨ä¹å¯ä»¥éè¿ [Telegram è®¨è®ºç»](https://t.me/embykeeper_chat)
-ä¸å¼åå¢éè¿è¡äº¤æµ. å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½,
-è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper Auth Bot](https://t.me/
-embykeeper_auth_bot)" åéå³é®çæå/å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper
-Bot](https://t.me/embykeeper_bot)" åæ¨æ¨é,
-æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
+å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
+Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
+å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
+åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
-æºå¨äººç­¾å° - æ¯æç¾¤ç» - ç»ç¹ç«: [é¢é](https://t.me/embypub)
-[ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) -
-å·æ¯é¼ : [é¢é]() [ç¾¤ç»](https://t.me/Curly_Mouse) [æºå¨äºº](https://
-t.me/jmsembybot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»](https://
-t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
-(ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
-t.me/embykeeper_bot?start=__prime)) - BlueSea: [ç¾¤ç»](https://t.me/
-blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot) - Singularity: [é¢é]
-(https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/
-Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach:
-[é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
+æºå¨äººç­¾å° - ç»ç¹ç«: [é¢é](https://t.me/embypub) [ç¾¤ç»](https://
+t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) - Nebula: [é¢é]
+(https://t.me/Nebula_Emby) [ç¾¤ç»](https://t.me/NebulaEmbyUser) [æºå¨äºº]
+(https://t.me/Nebula_Account_bot) (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare
+éªè¯ç , éè¦[é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) -
+Singularity: [é¢é](https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://
+t.me/Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) -
+Peach: [é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
 peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
 (https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
-t.me/EdHubot) - Pornemby (_æµè¯ä¸­_): [é¢é](https://t.me/pornembyservice)
-[æºå¨äºº](https://t.me/PronembyTGBot2_bot) - å¶ä»é Emby ç¸å³: -
-æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/pull/8)
-å¢å ) (_æµè¯ä¸­_): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
-Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_): [æ´»å¨é¢é](https://t.me/PornembyFun) -
+t.me/EdHubot) - Pornemby: [é¢é](https://t.me/pornembyservice) [ç¾¤ç»]
+(https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
+åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
+t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
+t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
+ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
+pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
+~~å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https://t.me/
+Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot)~~
+(æºå¨äººé»è¾é¢ç¹åå¨, ææ¶ç¦ç¨) - ~~BlueSea: [ç¾¤ç»](https://t.me/
+blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~ (æ ååº) -
 ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/
-Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) -
-~~åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
-t.me/zckllflbot)~~ (æ ååº) - ç¹æ§ - éªè¯ç è¯å«ä¸èªå¨éè¯ -
-å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby ä¿æ´» -
-å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
-èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
-è¯·è°¨æä½¿ç¨) - NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork)
-[æºå¨äºº](https://t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦
-[è¶çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç
-æ¢éè¯·ç : [ç¾¤ç»](https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/
-UnknownEmbyBot) - Embyhub å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub)
-[ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) ##
-å®è£ä¸ä½¿ç¨ ### ä» PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡,
-æ¨å¯ä»¥éè¿ [conda](https://github.com/conda/conda) æ [virtualvenv]
-(https://virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿
-`pip` å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
-embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
-github.com/embykeeper/embykeeper#%E4%BB%8E-docker-%E5%AE%89%E8%A3%85)). éå,
-æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) - Emby
+ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
+Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
+t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
+Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
+embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
+t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
+[é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime),
+åç­åç¡®çä¸è¬è¯·è°¨æä½¿ç¨) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»](https:
+//t.me/Ephemeralemby) [æºå¨äºº](https://t.me/UnknownEmbyBot) - Viper
+æ¢éè¯·ç : [é¢é](https://t.me/viper_emby_channel) [ç¾¤ç»](https://t.me/
+Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
+å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
+emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
+[é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
+[æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
+[é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
+(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### ä»
+PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡, æ¨å¯ä»¥éè¿ [conda]
+(https://github.com/conda/conda) æ [virtualvenv](https://virtualenv.pypa.io/
+) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip` å®è£ `embykeeper`
+(éè¦ `python >= 3.7, < 3.11`): ```bash pip install embykeeper ``` éå,
+æ¨éè¦æ§è¡: ```bash embykeeper ``` å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿
+`config.toml` æä»¶, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
+(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [proxy] hostname =
+"127.0.0.1" port = 1080 scheme = "socks5" [[telegram]] api_id = "27894236"
+api_hash = "622159182fdd4b15b627eeb3ac695271" phone = "+8612109347899" [[emby]]
+url = "https://weiss-griffin.com/" username = "carrie19" password =
+"s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿ [Telegram å®ç½]
+(https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
+development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
+æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
+æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
+æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡:
+```bash embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
+ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
 é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
 Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
 ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿
-`docker` è¿è¡, æ¨é [å®è£ docker](https://yeasy.gitbook.io/
-docker_practice/install), ç¶åæ§è¡: ```bash touch config.toml docker run -
-v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
-```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme = "socks5" [
-[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
-phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
-"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
-[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
-ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
-è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
-"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
-æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
-éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/config.toml:/app/
-config.toml --rm -it embykeeper/embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º åä» PyPi
+å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python ç¯å¢, ç¶åæå Github
+å¹¶å®è£: ```bash git clone https://github.com/embykeeper/embykeeper.git cd
+embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash
+embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/
+embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ### ä» Docker
+é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://
+yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡: ```bash docker run -
+v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
+å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯ (è¯¦è§[ä» Pypi å®è£](https://github.com/
+embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)). éå,
+æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
+net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
+ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash docker
-run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper ```
-æèä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) ([watchtower]
-(https://github.com/containrrr/watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡):
-```yaml version: '3' services: embykeeper: container_name: embykeeper image:
-cembykeeper/embykeeper restart: unless-stopped volumes: - ./config.toml:/app/
-config.toml watchtower: container_name: watchtower image: containrrr/watchtower
-restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/docker.sock:rw
-``` å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -
-f embykeeper` æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿.
-å¦ææ¨éè¦ä½¿ç¨ä¸»æºä¸çä»£çæå¡å¨ (ä¾å¦ `https://localhost:
-1080`), æ¨å¯è½éè¦ä½¿ç¨ `--net=host` åæ°ä»¥ä½¿ç¨ä¸»æºç½ç»æ¨¡å¼.
-### ä»æºç æå»º åä» PyPi å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python
-ç¯å¢, ç¶åæå Github å¹¶å®è£: ```bash git clone https://github.com/
-embykeeper/embykeeper.git cd embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡
-Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£]
-(https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
-å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨.
-## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©:
-```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. ### éè¿ Docker Compose
+é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/compose/
+) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker é¨ç½²]
+(https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2)
+æè½éè¿ `docker-compose` é¨ç½²,
+è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
+ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
+compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
+version: '3' services: embykeeper: container_name: embykeeper image:
+embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
+network_mode: host watchtower: container_name: watchtower image: containrrr/
+watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
+docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
+watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡.
+ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨: ```bash docker-compose up -d ```
+å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -f embykeeper`
+æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿. ##
+å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash
+$ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
 æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
-(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å°
-(ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´»
-(ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --monitor -m å¯ç¨ç¾¤èçè§ --send -
-s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-instant -
-I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
+(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
+(ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
+e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
+instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
+o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
-follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ ```
-ä¾å¦: ```bash # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
+follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ --
+basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® ``` ä¾å¦: ```bash # å¯å¨ææåè½
+(å¨åè´¦å·éç½®ä¸­è¿ä¸æ­¥è®¾ç½®åè½å¼å¯/å³é­) $ embykeeper
+config.toml # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
-å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
-è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -
-s ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
+ä»å¯å¨æ¯æ¥ 8:00 PM - 9:00 PM éæºæ¶é´ç­¾å° $ embykeeper config.toml -
+c <8:00PM,9:00PM> # å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
+è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -s #
+å¯å¨ææåè½, åªè¿è¡ä¸æ¬¡ $ embykeeper config.toml --once #
+å¯å¨ææåè½, ä¸ç«å³æ§è¡ä¸æ¬¡ç­¾å°/ä¿æ´» $ embykeeper config.toml
+-I ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
 ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
 config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
 10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
 "åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
 è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
 ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
 å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
@@ -170,21 +177,22 @@
 (ä¾å¦èªå¨æ¢éè¯·ç )å°éè¦é«çº§ç¨æ·, æ¨å¯ä»¥éè¿ [Embykeeper
 Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
-(https://afdian.net/a/jackzzs)èµå© ![kitty](images/kitty.gif) ## éç½®é¡¹ |
-è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ------------ | -----------------
-- | -------------------------------------------- | ------- | | `timeout` |
-`int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | | `retries` | `int` |
-Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `10` | | `concurrent` | `int` |
-Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random` | `int` | Telegram
-æºå¨äººç­¾å°å®æ¶ä»»å¡æ¶é´éæºé (åé) | `15` | | `notifier` |
+(https://afdian.net/a/jackzzs)èµå© ![Kitty](https://github.com/embykeeper/
+embykeeper/raw/main/images/kitty.gif) ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å |
+ç®ä» | é»è®¤å¼ | | ------------ | ------------------ | --------------------
+------------------------ | ------- | | `timeout` | `int` | Telegram
+æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | | `retries` | `int` | Telegram
+æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | | `concurrent` | `int` | Telegram
+æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random` | `int` | Telegram
+æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` | | `notifier` |
 `int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/ææºå·) |
 `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/çè§åè½å¼å¯ç«ç¹è®¾ç½® |
 `{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `{}` | | `telegram` | `list` |
 Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | | `emby` | `list` | Emby
 è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
 å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------- | ------ | -------------- | ----
 ---------------- | | `checkiner` | `list` | å¯ç¨çç­¾å°ç«ç¹ |
@@ -195,18 +203,18 @@
 æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
 è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
 æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
 ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | --- | --- | --- |--- | --- | |
 åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` | | å·æ¯é¼  IPTV |
 `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby | `pornemby` | | Singularity
 | `singularity` | | Peach | `peach` | | Nebula | `nebula` | | Bluesea |
-`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | | | `proxy`
-è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
------- | --------------------------------------- | ----------- | | `hostname` |
-`str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
+`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | å¡æ | `charon` |
+`proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | -----
+----- | ------ | --------------------------------------- | ----------- | |
+`hostname` | `str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
 ä»£çç«¯å£å· | `1080` | | `scheme` | `str` | ä»£çåè®®, å¯ä»¥ä¸º
 "`socks5`" æ "`http`" | `socks5` | `telegram` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
 å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
 -------------------------------------------- | ------- | | `api_id` | `str` |
 ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID | | |
 `api_hash` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç
 Application Hash | | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
@@ -214,29 +222,34 @@
 | `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: |
 è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------
 ----------------------------------------------- | ------ | | `url` | `str` |
 Emby æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | |
 `username` | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
-## ä»£ç éç¨ä¸å¼å ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-
-terminal cli) --> B(fa:fa-telegram telechecker) A --> C(fa:fa-play embywatcher)
-B --checker--> E[fa:fa-robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --
-messager--> F[fa:fa-message Messager] C --watcher--> H[fa:fa-circle-play
-EmbyWatcher] F ---- |schedule| A ``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: -
-`embykeeper.telechecker.bots` - `embykeeper.telechecker.monitor` -
-`embykeeper.telechecker.messager` éå¸¸æ¥è¯´,
-å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
+æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
+bgk, embyhub, polo unique_name = "your_username_for_registeration" #
+èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
+ä»å½é®é¢åå²ä¸­æ¾å°ç­æ¡æ¶èªå¨åç­ ``` ## ä»£ç éç¨ä¸å¼å
+ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-
+telegram telechecker) A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-
+robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message
+Messager] C --watcher--> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A
+``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
+`embykeeper.telechecker.monitor` - `embykeeper.telechecker.messager`
+éå¸¸æ¥è¯´, å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
 ä¸­å¢å ä¸ä¸ªæä»¶ `dummy.py`: ```python from .base import BotCheckin class
 DummyCheckin(BotCheckin): name = "Dummy" bot_username = "dummy" bot_captcha_len
 = 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨, å°ä¼åç¨æ·åä¸º
 "`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4 ä½çéªè¯ç ,
 è¯å«éªè¯ç åå°åé. è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®,
 æ¨å¯ä»¥ä½¿ç¨ `AnswerBotCheckin`, æ¨ä¹å¯ä»¥éå `on_captcha`
 å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from .base import AnswerBotCheckin
 class DummyCheckin(AnswerBotCheckin): .... async def on_captcha(self, message:
 Message, captcha: str): for l in captcha: try: await self.message.click(l)
 except ValueError: self.log.info(f'æªè½æ¾å°å¯¹åº "{l}" çæé®,
 æ­£å¨éè¯.') await self.retry() break ```
 ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
 å½æ¨å®ç°ä¸ä¸ªæ°çç­¾å°å¨æ¶, æ¬¢è¿æ¨æåº [Pull Requests](https://
-github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨!
+github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! ## è¶å¿ [!
+[Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
+embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

### Comparing `embykeeper-2.0.9/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.1.0/embykeeper.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 LICENSE
 README.md
 pyproject.toml
 embykeeper/__init__.py
 embykeeper/cli.py
+embykeeper/data.py
 embykeeper/log.py
-embykeeper/loop.py
 embykeeper/settings.py
 embykeeper/utils.py
 embykeeper.egg-info/PKG-INFO
 embykeeper.egg-info/SOURCES.txt
 embykeeper.egg-info/dependency_links.txt
 embykeeper.egg-info/entry_points.txt
 embykeeper.egg-info/not-zip-safe
 embykeeper.egg-info/requires.txt
 embykeeper.egg-info/top_level.txt
 embykeeper/embywatcher/__init__.py
 embykeeper/embywatcher/emby.py
 embykeeper/embywatcher/main.py
 embykeeper/telechecker/__init__.py
 embykeeper/telechecker/link.py
+embykeeper/telechecker/log.py
 embykeeper/telechecker/main.py
 embykeeper/telechecker/tele.py
 embykeeper/telechecker/bots/__init__.py
 embykeeper/telechecker/bots/base.py
 embykeeper/telechecker/bots/bluesea.py
+embykeeper/telechecker/bots/charon.py
 embykeeper/telechecker/bots/embyhub.py
 embykeeper/telechecker/bots/jms.py
 embykeeper/telechecker/bots/jms_iptv.py
 embykeeper/telechecker/bots/ljyy.py
 embykeeper/telechecker/bots/nebula.py
 embykeeper/telechecker/bots/peach.py
 embykeeper/telechecker/bots/pornemby.py
@@ -39,10 +41,13 @@
 embykeeper/telechecker/messager/common.py
 embykeeper/telechecker/messager/nakonako.py
 embykeeper/telechecker/messager/test.py
 embykeeper/telechecker/monitor/__init__.py
 embykeeper/telechecker/monitor/base.py
 embykeeper/telechecker/monitor/bgk.py
 embykeeper/telechecker/monitor/embyhub.py
-embykeeper/telechecker/monitor/pornemby_exam.py
+embykeeper/telechecker/monitor/misty.py
+embykeeper/telechecker/monitor/polo.py
+embykeeper/telechecker/monitor/pornemby.py
 embykeeper/telechecker/monitor/test.py
-test/test_cli.py
+embykeeper/telechecker/monitor/viper.py
+tests/test_cli.py
```

### Comparing `embykeeper-2.0.9/pyproject.toml` & `embykeeper-2.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.0.9"
+version = "2.1.0"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
@@ -25,24 +25,24 @@
     "Natural Language :: Chinese (Simplified)",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
 ]
-requires-python = ">=3.7,<3.11"
+requires-python = ">=3.8,<3.11"
 dependencies = [
     "tomli",
     "tomlkit",
     "rich",
     "typer",
-    "schedule",
     "appdirs",
     "loguru",
     "faker",
+    "aiofiles",
     "aiohttp",
     "aiohttp_socks",
     "python-dateutil",
     "ddddocr",
     "embypy",
     "pyrogram",
     "tgcrypto",
@@ -63,24 +63,11 @@
 [project.scripts]
 embykeeper = "embykeeper.cli:app"
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.packages]
-find = {}
-
-[tool.bumpversion]
-current_version = "2.0.9"
-commit = "True"
-tag = "True"
-
-[tool.bumpversion.file.setup.py]
-search = 'version="{current_version}"'
-replace = 'version="{new_version}"'
-
-[tool.bumpversion.file."embykeeper/__init__".py]
-search = '__version__ = "{current_version}"'
-replace = '__version__ = "{new_version}"'
+find = {namespaces = false}
 
 [tool.black]
 line-length = 110
```

### Comparing `embykeeper-2.0.9/test/test_cli.py` & `embykeeper-2.1.0/tests/test_cli.py`

 * *Files identical despite different names*

