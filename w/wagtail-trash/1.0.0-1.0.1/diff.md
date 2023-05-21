# Comparing `tmp/wagtail-trash-1.0.0.tar.gz` & `tmp/wagtail-trash-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-trash-1.0.0.tar", last modified: Thu Mar 23 18:04:23 2023, max compression
+gzip compressed data, was "wagtail-trash-1.0.1.tar", last modified: Sun May 21 13:26:47 2023, max compression
```

## Comparing `wagtail-trash-1.0.0.tar` & `wagtail-trash-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.569398 wagtail-trash-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-03-23 18:04:23.569398 wagtail-trash-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 18:04:23.569398 wagtail-trash-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.565399 wagtail-trash-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/tests/test_management_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.565399 wagtail-trash-1.0.0/wagtail_trash/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.561399 wagtail-trash-1.0.0/wagtail_trash/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.561399 wagtail-trash-1.0.0/wagtail_trash/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.565399 wagtail-trash-1.0.0/wagtail_trash/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.561399 wagtail-trash-1.0.0/wagtail_trash/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.565399 wagtail-trash-1.0.0/wagtail_trash/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.561399 wagtail-trash-1.0.0/wagtail_trash/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.569398 wagtail-trash-1.0.0/wagtail_trash/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.561399 wagtail-trash-1.0.0/wagtail_trash/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.569398 wagtail-trash-1.0.0/wagtail_trash/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.569398 wagtail-trash-1.0.0/wagtail_trash/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.569398 wagtail-trash-1.0.0/wagtail_trash/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/management/commands/delete_stray_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/management/commands/empty_trash.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.569398 wagtail-trash-1.0.0/wagtail_trash/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/migrations/0002_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.565399 wagtail-trash-1.0.0/wagtail_trash/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.569398 wagtail-trash-1.0.0/wagtail_trash/templates/wagtail_trash/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/templates/wagtail_trash/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/templates/wagtail_trash/move.html
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-03-23 18:04:02.000000 wagtail-trash-1.0.0/wagtail_trash/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:04:23.565399 wagtail-trash-1.0.0/wagtail_trash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-03-23 18:04:23.000000 wagtail-trash-1.0.0/wagtail_trash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-23 18:04:23.000000 wagtail-trash-1.0.0/wagtail_trash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 18:04:23.000000 wagtail-trash-1.0.0/wagtail_trash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 18:04:23.000000 wagtail-trash-1.0.0/wagtail_trash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-23 18:04:23.000000 wagtail-trash-1.0.0/wagtail_trash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-23 18:04:23.000000 wagtail-trash-1.0.0/wagtail_trash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.578742 wagtail-trash-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-21 13:26:47.578742 wagtail-trash-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 13:26:47.578742 wagtail-trash-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.574742 wagtail-trash-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/tests/test_management_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.574742 wagtail-trash-1.0.1/wagtail_trash/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.570742 wagtail-trash-1.0.1/wagtail_trash/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.570742 wagtail-trash-1.0.1/wagtail_trash/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.574742 wagtail-trash-1.0.1/wagtail_trash/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.570742 wagtail-trash-1.0.1/wagtail_trash/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.578742 wagtail-trash-1.0.1/wagtail_trash/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.570742 wagtail-trash-1.0.1/wagtail_trash/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.578742 wagtail-trash-1.0.1/wagtail_trash/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.570742 wagtail-trash-1.0.1/wagtail_trash/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.578742 wagtail-trash-1.0.1/wagtail_trash/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.578742 wagtail-trash-1.0.1/wagtail_trash/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.578742 wagtail-trash-1.0.1/wagtail_trash/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/management/commands/delete_stray_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/management/commands/empty_trash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.578742 wagtail-trash-1.0.1/wagtail_trash/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/migrations/0002_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.574742 wagtail-trash-1.0.1/wagtail_trash/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.578742 wagtail-trash-1.0.1/wagtail_trash/templates/wagtail_trash/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/templates/wagtail_trash/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/templates/wagtail_trash/move.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-21 13:26:29.000000 wagtail-trash-1.0.1/wagtail_trash/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:26:47.574742 wagtail-trash-1.0.1/wagtail_trash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-21 13:26:47.000000 wagtail-trash-1.0.1/wagtail_trash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-21 13:26:47.000000 wagtail-trash-1.0.1/wagtail_trash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:26:47.000000 wagtail-trash-1.0.1/wagtail_trash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:26:47.000000 wagtail-trash-1.0.1/wagtail_trash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-21 13:26:47.000000 wagtail-trash-1.0.1/wagtail_trash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 13:26:47.000000 wagtail-trash-1.0.1/wagtail_trash.egg-info/top_level.txt
```

### Comparing `wagtail-trash-1.0.0/LICENSE` & `wagtail-trash-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/PKG-INFO` & `wagtail-trash-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-trash
-Version: 1.0.0
+Version: 1.0.1
 Summary: Make deleted pages only temporarily deleted.
 Author: Andreas Bernacca
 Author-email: ante.bernacca@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/Frojd/wagtail-trash/
 Project-URL: Changelog, https://github.com/Frojd/wagtail-trash/blob/main/CHANGELOG.md
 Classifier: Environment :: Web Environment
@@ -14,19 +14,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 [![Run tests, lint and publish](https://github.com/Frojd/wagtail-trash/actions/workflows/main.yml/badge.svg)](https://github.com/Frojd/wagtail-trash/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/wagtail-trash.svg)](https://badge.fury.io/py/wagtail-trash)
```

### Comparing `wagtail-trash-1.0.0/README.md` & `wagtail-trash-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/setup.py` & `wagtail-trash-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,19 +38,21 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Framework :: Wagtail",
         "Framework :: Wagtail :: 4",
+        "Framework :: Wagtail :: 5",
         "License :: OSI Approved :: MIT License",
     ],
     project_urls={
         "Source": "https://github.com/Frojd/wagtail-trash/",
         "Changelog": "https://github.com/Frojd/wagtail-trash/blob/main/CHANGELOG.md",
     },
 )
```

### Comparing `wagtail-trash-1.0.0/tests/test_admin.py` & `wagtail-trash-1.0.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/tests/test_management_commands.py` & `wagtail-trash-1.0.1/tests/test_management_commands.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/tests/test_managers.py` & `wagtail-trash-1.0.1/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/tests/test_permissions.py` & `wagtail-trash-1.0.1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/tests/test_utils.py` & `wagtail-trash-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/locale/en/LC_MESSAGES/django.po` & `wagtail-trash-1.0.1/wagtail_trash/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/locale/es_AR/LC_MESSAGES/django.mo` & `wagtail-trash-1.0.1/wagtail_trash/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/locale/es_AR/LC_MESSAGES/django.po` & `wagtail-trash-1.0.1/wagtail_trash/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/locale/pt_BR/LC_MESSAGES/django.mo` & `wagtail-trash-1.0.1/wagtail_trash/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/locale/pt_BR/LC_MESSAGES/django.po` & `wagtail-trash-1.0.1/wagtail_trash/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/locale/sv/LC_MESSAGES/django.mo` & `wagtail-trash-1.0.1/wagtail_trash/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/locale/sv/LC_MESSAGES/django.po` & `wagtail-trash-1.0.1/wagtail_trash/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/management/commands/delete_stray_pages.py` & `wagtail-trash-1.0.1/wagtail_trash/management/commands/delete_stray_pages.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/management/commands/empty_trash.py` & `wagtail-trash-1.0.1/wagtail_trash/management/commands/empty_trash.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/managers.py` & `wagtail-trash-1.0.1/wagtail_trash/managers.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/migrations/0001_initial.py` & `wagtail-trash-1.0.1/wagtail_trash/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/migrations/0002_translation.py` & `wagtail-trash-1.0.1/wagtail_trash/migrations/0002_translation.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/models.py` & `wagtail-trash-1.0.1/wagtail_trash/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/templates/wagtail_trash/move.html` & `wagtail-trash-1.0.1/wagtail_trash/templates/wagtail_trash/move.html`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/utils.py` & `wagtail-trash-1.0.1/wagtail_trash/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/views.py` & `wagtail-trash-1.0.1/wagtail_trash/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash/wagtail_hooks.py` & `wagtail-trash-1.0.1/wagtail_trash/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-trash-1.0.0/wagtail_trash.egg-info/PKG-INFO` & `wagtail-trash-1.0.1/wagtail_trash.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-trash
-Version: 1.0.0
+Version: 1.0.1
 Summary: Make deleted pages only temporarily deleted.
 Author: Andreas Bernacca
 Author-email: ante.bernacca@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/Frojd/wagtail-trash/
 Project-URL: Changelog, https://github.com/Frojd/wagtail-trash/blob/main/CHANGELOG.md
 Classifier: Environment :: Web Environment
@@ -14,19 +14,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 [![Run tests, lint and publish](https://github.com/Frojd/wagtail-trash/actions/workflows/main.yml/badge.svg)](https://github.com/Frojd/wagtail-trash/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/wagtail-trash.svg)](https://badge.fury.io/py/wagtail-trash)
```

### Comparing `wagtail-trash-1.0.0/wagtail_trash.egg-info/SOURCES.txt` & `wagtail-trash-1.0.1/wagtail_trash.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 tests/test_admin.py
 tests/test_management_commands.py
 tests/test_managers.py
```

