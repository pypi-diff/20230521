# Comparing `tmp/allianceauth-securegroups-0.5.1.tar.gz` & `tmp/allianceauth-securegroups-0.5.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-securegroups-0.5.1.tar", last modified: Fri Mar 31 13:18:47 2023, max compression
+gzip compressed data, was "allianceauth-securegroups-0.5.2b1.tar", last modified: Sun May 21 01:53:20 2023, max compression
```

## Comparing `allianceauth-securegroups-0.5.1.tar` & `allianceauth-securegroups-0.5.2b1.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.911789 allianceauth-securegroups-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-03-31 13:18:47.911789 allianceauth-securegroups-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.903788 allianceauth-securegroups-0.5.1/allianceauth_securegroups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-03-31 13:18:47.000000 allianceauth-securegroups-0.5.1/allianceauth_securegroups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-31 13:18:47.000000 allianceauth-securegroups-0.5.1/allianceauth_securegroups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 13:18:47.000000 allianceauth-securegroups-0.5.1/allianceauth_securegroups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-31 13:18:47.000000 allianceauth-securegroups-0.5.1/allianceauth_securegroups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-31 13:18:47.000000 allianceauth-securegroups-0.5.1/allianceauth_securegroups.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.907788 allianceauth-securegroups-0.5.1/securegroups/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.907788 allianceauth-securegroups-0.5.1/securegroups/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/cogs/groupcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.903788 allianceauth-securegroups-0.5.1/securegroups/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.907788 allianceauth-securegroups-0.5.1/securegroups/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/management/commands/setup_securegroup_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.907788 allianceauth-securegroups-0.5.1/securegroups/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0002_auto_20210103_2237.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0003_smartfilter_grace_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0004_auto_20210104_0317.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0005_auto_20210104_1525.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0006_useringroupfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0007_auto_20210105_0735.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0008_auto_20210117_0219.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0009_auto_20210218_0908.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0010_perms_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0011_smartgroup_notify_on_add_smartgroup_notify_on_grace_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/0012_alter_pendingnotification_notified.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14151 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.903788 allianceauth-securegroups-0.5.1/securegroups/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.911789 allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/audit.html
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/audit_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/filter_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/groups.html
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/user_check.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.911789 allianceauth-securegroups-0.5.1/securegroups/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/templatetags/sg_audit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.911789 allianceauth-securegroups-0.5.1/securegroups/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/tests/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/tests/test_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/securegroups/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 13:18:47.911789 allianceauth-securegroups-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:18:47.911789 allianceauth-securegroups-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/tests/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 13:18:10.000000 allianceauth-securegroups-0.5.1/tests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.856435 allianceauth-securegroups-0.5.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-05-21 01:53:20.856435 allianceauth-securegroups-0.5.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.852435 allianceauth-securegroups-0.5.2b1/allianceauth_securegroups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-05-21 01:53:20.000000 allianceauth-securegroups-0.5.2b1/allianceauth_securegroups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-21 01:53:20.000000 allianceauth-securegroups-0.5.2b1/allianceauth_securegroups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 01:53:20.000000 allianceauth-securegroups-0.5.2b1/allianceauth_securegroups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 01:53:20.000000 allianceauth-securegroups-0.5.2b1/allianceauth_securegroups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 01:53:20.000000 allianceauth-securegroups-0.5.2b1/allianceauth_securegroups.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.852435 allianceauth-securegroups-0.5.2b1/securegroups/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/auth_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.852435 allianceauth-securegroups-0.5.2b1/securegroups/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/cogs/groupcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.848435 allianceauth-securegroups-0.5.2b1/securegroups/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.852435 allianceauth-securegroups-0.5.2b1/securegroups/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/management/commands/setup_securegroup_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.856435 allianceauth-securegroups-0.5.2b1/securegroups/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0002_auto_20210103_2237.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0003_smartfilter_grace_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0004_auto_20210104_0317.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0005_auto_20210104_1525.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0006_useringroupfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0007_auto_20210105_0735.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0008_auto_20210117_0219.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0009_auto_20210218_0908.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0010_perms_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0011_smartgroup_notify_on_add_smartgroup_notify_on_grace_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0012_alter_pendingnotification_notified.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/0013_useringroupfilter_reversed_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14151 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.852435 allianceauth-securegroups-0.5.2b1/securegroups/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.856435 allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/audit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/audit_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/filter_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/user_check.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.856435 allianceauth-securegroups-0.5.2b1/securegroups/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/templatetags/sg_audit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.856435 allianceauth-securegroups-0.5.2b1/securegroups/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/tests/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/tests/test_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/securegroups/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 01:53:20.856435 allianceauth-securegroups-0.5.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:53:20.856435 allianceauth-securegroups-0.5.2b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/tests/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 01:52:51.000000 allianceauth-securegroups-0.5.2b1/tests/views.py
```

### Comparing `allianceauth-securegroups-0.5.1/PKG-INFO` & `allianceauth-securegroups-0.5.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-securegroups
-Version: 0.5.1
+Version: 0.5.2b1
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/pvyParts/allianceauth-secure-groups
 Author: ak
 Author-email: ak@ak.auth
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `allianceauth-securegroups-0.5.1/README.md` & `allianceauth-securegroups-0.5.2b1/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/allianceauth_securegroups.egg-info/PKG-INFO` & `allianceauth-securegroups-0.5.2b1/allianceauth_securegroups.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-securegroups
-Version: 0.5.1
+Version: 0.5.2b1
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/pvyParts/allianceauth-secure-groups
 Author: ak
 Author-email: ak@ak.auth
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `allianceauth-securegroups-0.5.1/allianceauth_securegroups.egg-info/SOURCES.txt` & `allianceauth-securegroups-0.5.2b1/allianceauth_securegroups.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 securegroups/migrations/0006_useringroupfilter.py
 securegroups/migrations/0007_auto_20210105_0735.py
 securegroups/migrations/0008_auto_20210117_0219.py
 securegroups/migrations/0009_auto_20210218_0908.py
 securegroups/migrations/0010_perms_update.py
 securegroups/migrations/0011_smartgroup_notify_on_add_smartgroup_notify_on_grace_and_more.py
 securegroups/migrations/0012_alter_pendingnotification_notified.py
+securegroups/migrations/0013_useringroupfilter_reversed_logic.py
 securegroups/migrations/__init__.py
 securegroups/templates/smartgroups/audit.html
 securegroups/templates/smartgroups/audit_list.html
 securegroups/templates/smartgroups/filter_list.html
 securegroups/templates/smartgroups/groups.html
 securegroups/templates/smartgroups/menu.html
 securegroups/templates/smartgroups/user_check.html
```

### Comparing `allianceauth-securegroups-0.5.1/securegroups/admin.py` & `allianceauth-securegroups-0.5.2b1/securegroups/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 
 admin.site.register(AltCorpFilter, AltCorpAdmin)
 
 
 class UserInGroupFilterAdmin(admin.ModelAdmin):
     list_select_related = ["group"]
-    list_display = ["__str__", "group"]
+    list_display = ["__str__", "group", "reversed_logic"]
     filter_horizontal = ["exempt_alliances", "exempt_corporations"]
 
 
 admin.site.register(UserInGroupFilter, UserInGroupFilterAdmin)
 
 
 class AltAlliAdmin(admin.ModelAdmin):
```

### Comparing `allianceauth-securegroups-0.5.1/securegroups/auth_hooks.py` & `allianceauth-securegroups-0.5.2b1/securegroups/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/cogs/groupcheck.py` & `allianceauth-securegroups-0.5.2b1/securegroups/cogs/groupcheck.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/filter.py` & `allianceauth-securegroups-0.5.2b1/securegroups/filter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/management/commands/setup_securegroup_task.py` & `allianceauth-securegroups-0.5.2b1/securegroups/management/commands/setup_securegroup_task.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/migrations/0001_initial.py` & `allianceauth-securegroups-0.5.2b1/securegroups/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/migrations/0004_auto_20210104_0317.py` & `allianceauth-securegroups-0.5.2b1/securegroups/migrations/0004_auto_20210104_0317.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/migrations/0005_auto_20210104_1525.py` & `allianceauth-securegroups-0.5.2b1/securegroups/migrations/0005_auto_20210104_1525.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/migrations/0006_useringroupfilter.py` & `allianceauth-securegroups-0.5.2b1/securegroups/migrations/0006_useringroupfilter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/migrations/0008_auto_20210117_0219.py` & `allianceauth-securegroups-0.5.2b1/securegroups/migrations/0008_auto_20210117_0219.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/migrations/0009_auto_20210218_0908.py` & `allianceauth-securegroups-0.5.2b1/securegroups/migrations/0009_auto_20210218_0908.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/migrations/0011_smartgroup_notify_on_add_smartgroup_notify_on_grace_and_more.py` & `allianceauth-securegroups-0.5.2b1/securegroups/migrations/0011_smartgroup_notify_on_add_smartgroup_notify_on_grace_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/models.py` & `allianceauth-securegroups-0.5.2b1/securegroups/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,26 +144,29 @@
 
     # sometimes there are double standards.
     exempt_alliances = models.ManyToManyField(
         EveAllianceInfo, related_name="group_exempt_alliances", blank=True)
     exempt_corporations = models.ManyToManyField(
         EveCorporationInfo, related_name="group_exempt_corporations", blank=True)
 
+    reversed_logic = models.BooleanField(default=False)
+
     def process_filter(self, user: User):
         return smart_filters.check_group_on_account(user, self.group,
                                                     exempt_allis=self.exempt_alliances.all().values_list("alliance_id", flat=True),
                                                     exempt_corps=self.exempt_corporations.all().values_list("corporation_id", flat=True)
                                                     )
 
     def audit_filter(self, users):
         cl = users.prefetch_related('groups').filter(
             groups__id__in=[self.group.id, ])
-        chars = defaultdict(lambda: {"message": "", "check": False})
+        chars = defaultdict(
+            lambda: {"message": "", "check": self.reversed_logic})
         for c in cl:
-            chars[c.id] = {"message": "", "check": True}
+            chars[c.id] = {"message": "", "check": not self.reversed_logic}
         return chars
 
 
 class SmartGroup(models.Model):
     group = models.OneToOneField(Group, on_delete=models.CASCADE)
     description = models.CharField(max_length=500, default="", blank=True)
     filters = models.ManyToManyField(SmartFilter)
```

### Comparing `allianceauth-securegroups-0.5.1/securegroups/signals.py` & `allianceauth-securegroups-0.5.2b1/securegroups/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/tasks.py` & `allianceauth-securegroups-0.5.2b1/securegroups/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/audit.html` & `allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/audit.html`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/audit_list.html` & `allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/audit_list.html`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/filter_list.html` & `allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/filter_list.html`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/groups.html` & `allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/groups.html`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/menu.html` & `allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/templates/smartgroups/user_check.html` & `allianceauth-securegroups-0.5.2b1/securegroups/templates/smartgroups/user_check.html`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/templatetags/sg_audit.py` & `allianceauth-securegroups-0.5.2b1/securegroups/templatetags/sg_audit.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/tests/test_transactions.py` & `allianceauth-securegroups-0.5.2b1/securegroups/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/tests/test_user_filters.py` & `allianceauth-securegroups-0.5.2b1/securegroups/tests/test_user_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,17 @@
                                                executor_corp_id=3)
         cls.alli_filter = gb_models.AltAllianceFilter.objects.create(
             name="Test Alli 1 Alt", description="Have Alt in TSTA2", alt_alli_id=_alli.pk
         )
         cls.grp_filter = gb_models.UserInGroupFilter.objects.create(
             name="Test Group", description="Test Group", group=cls.test_group
         )
+        cls.grp_filter_inverted = gb_models.UserInGroupFilter.objects.create(
+            name="Test Group", description="Test Group", group=cls.test_group, reversed_logic=True
+        )
 
     def test_user_alt_corp(self):
         users = {}
         for user in User.objects.all():
             print
             users[user.pk] = None
 
@@ -226,14 +229,36 @@
         self.assertFalse(tests[5]['check'])
         self.assertFalse(tests[6]['check'])
         self.assertTrue(tests[7]['check'])
         self.assertFalse(tests[8]['check'])
         self.assertFalse(tests[9]['check'])
         self.assertFalse(tests[10]['check'])
 
+    def test_user_group_filter_audit_inverted(self):
+        User.objects.get(id=1).groups.add(self.test_group)
+        User.objects.get(id=7).groups.add(self.test_group)
+
+        users = []
+        for user in User.objects.all():
+            users.append(user.pk)
+
+        tests = self.grp_filter_inverted.audit_filter(
+            User.objects.filter(pk__in=users))
+
+        self.assertFalse(tests[1]['check'])
+        self.assertTrue(tests[2]['check'])
+        self.assertTrue(tests[3]['check'])
+        self.assertTrue(tests[4]['check'])
+        self.assertTrue(tests[5]['check'])
+        self.assertTrue(tests[6]['check'])
+        self.assertFalse(tests[7]['check'])
+        self.assertTrue(tests[8]['check'])
+        self.assertTrue(tests[9]['check'])
+        self.assertTrue(tests[10]['check'])
+
     def test_generic_smart_group_task(self):
         cache.clear()
         reset_time = timezone.now() - timedelta(days=5)
         User.objects.get(id=1).groups.add(self.test_group)
         User.objects.get(id=10).groups.add(self.test_group)
         User.objects.get(id=9).groups.add(self.test_group)
         User.objects.get(id=7).groups.add(self.test_group)
```

### Comparing `allianceauth-securegroups-0.5.1/securegroups/urls.py` & `allianceauth-securegroups-0.5.2b1/securegroups/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/securegroups/views.py` & `allianceauth-securegroups-0.5.2b1/securegroups/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/setup.py` & `allianceauth-securegroups-0.5.2b1/setup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/tests/celery.py` & `allianceauth-securegroups-0.5.2b1/tests/celery.py`

 * *Files identical despite different names*

### Comparing `allianceauth-securegroups-0.5.1/tests/test_settings.py` & `allianceauth-securegroups-0.5.2b1/tests/test_settings.py`

 * *Files identical despite different names*

