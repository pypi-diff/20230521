# Comparing `tmp/aa-fleetpings-2.8.0.tar.gz` & `tmp/aa-fleetpings-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-fleetpings-2.8.0.tar", last modified: Sun Jan  2 02:26:57 2022, max compression
+gzip compressed data, was "aa-fleetpings-2.9.0.tar", last modified: Tue Jan 11 14:51:31 2022, max compression
```

## Comparing `aa-fleetpings-2.8.0.tar` & `aa-fleetpings-2.9.0.tar`

### file list

```diff
@@ -1,88 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.332825 aa-fleetpings-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9238 2022-01-02 02:26:57.332825 aa-fleetpings-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6304 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.324825 aa-fleetpings-2.8.0/aa_fleetpings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9238 2022-01-02 02:26:57.000000 aa-fleetpings-2.8.0/aa_fleetpings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-01-02 02:26:57.000000 aa-fleetpings-2.8.0/aa_fleetpings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-02 02:26:57.000000 aa-fleetpings-2.8.0/aa_fleetpings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-01-02 02:26:57.000000 aa-fleetpings-2.8.0/aa_fleetpings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-02 02:26:57.000000 aa-fleetpings-2.8.0/aa_fleetpings.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.324825 aa-fleetpings-2.8.0/fleetpings/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6395 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.328825 aa-fleetpings-2.8.0/fleetpings/docs/
--rw-r--r--   0 runner    (1001) docker     (121)   368124 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/docs/aa-view.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    96246 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/docs/discord-ping-embedded.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   107317 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/docs/discord-ping.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    99225 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/docs/slack-ping.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/form.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.312825 aa-fleetpings-2.8.0/fleetpings/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.312825 aa-fleetpings-2.8.0/fleetpings/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.328825 aa-fleetpings-2.8.0/fleetpings/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     7942 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    11690 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.312825 aa-fleetpings-2.8.0/fleetpings/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.328825 aa-fleetpings-2.8.0/fleetpings/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     8715 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.328825 aa-fleetpings-2.8.0/fleetpings/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    12856 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/migrations/0002_webhook_is_embed_description_change.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/migrations/0003_fleetdoctrine_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/migrations/0004_auto_20200915_1617.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/migrations/0005_fleettype_restricted_to_group.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     2064 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/migrations/0008_auto_20210114_1733.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12035 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.312825 aa-fleetpings-2.8.0/fleetpings/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.312825 aa-fleetpings-2.8.0/fleetpings/static/fleetpings/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.328825 aa-fleetpings-2.8.0/fleetpings/static/fleetpings/css/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/static/fleetpings/css/fleetpings.css
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/static/fleetpings/css/fleetpings.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.328825 aa-fleetpings-2.8.0/fleetpings/static/fleetpings/js/
--rw-r--r--   0 runner    (1001) docker     (121)    24583 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/static/fleetpings/js/fleetpings.js
--rw-r--r--   0 runner    (1001) docker     (121)    12693 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/static/fleetpings/js/fleetpings.min.js
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.316825 aa-fleetpings-2.8.0/fleetpings/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.328825 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.332825 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/additionalInformation.html
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/createOptimer.html
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/createSrpLink.html
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/fleetCommander.html
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/fleetComms.html
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/fleetDoctrine.html
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/fleetName.html
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/fleetType.html
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/formupLocation.html
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/formupTime.html
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/pingChannel.html
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/pingTargets.html
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/prePing.html
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/srp.html
--rw-r--r--   0 runner    (1001) docker     (121)     2513 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form.html
--rw-r--r--   0 runner    (1001) docker     (121)     2999 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/ping.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.332825 aa-fleetpings-2.8.0/fleetpings/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (121)     3425 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/tests/test_installed_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7079 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/fleetpings/views.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-02 02:26:57.336825 aa-fleetpings-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 02:26:57.332825 aa-fleetpings-2.8.0/testauth/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/testauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/testauth/celery.py
--rw-r--r--   0 runner    (1001) docker     (121)     9432 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/testauth/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/testauth/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-01-02 02:26:47.000000 aa-fleetpings-2.8.0/testauth/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.172436 aa-fleetpings-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9238 2022-01-11 14:51:31.172436 aa-fleetpings-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6304 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.164436 aa-fleetpings-2.9.0/aa_fleetpings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9238 2022-01-11 14:51:30.000000 aa-fleetpings-2.9.0/aa_fleetpings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2677 2022-01-11 14:51:31.000000 aa-fleetpings-2.9.0/aa_fleetpings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-11 14:51:30.000000 aa-fleetpings-2.9.0/aa_fleetpings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-01-11 14:51:30.000000 aa-fleetpings-2.9.0/aa_fleetpings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-11 14:51:30.000000 aa-fleetpings-2.9.0/aa_fleetpings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.168436 aa-fleetpings-2.9.0/fleetpings/
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6395 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/auth_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.168436 aa-fleetpings-2.9.0/fleetpings/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)   368124 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/docs/aa-view.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    96246 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/docs/discord-ping-embedded.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   107317 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/docs/discord-ping.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    99225 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/docs/slack-ping.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/form.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.164436 aa-fleetpings-2.9.0/fleetpings/locale/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.164436 aa-fleetpings-2.9.0/fleetpings/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.168436 aa-fleetpings-2.9.0/fleetpings/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     7942 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    11690 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.164436 aa-fleetpings-2.9.0/fleetpings/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.168436 aa-fleetpings-2.9.0/fleetpings/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     8715 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.168436 aa-fleetpings-2.9.0/fleetpings/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)    12856 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/migrations/0002_webhook_is_embed_description_change.py
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/migrations/0003_fleetdoctrine_link.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/migrations/0004_auto_20200915_1617.py
+-rw-r--r--   0 runner    (1001) docker     (121)      672 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/migrations/0005_fleettype_restricted_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2064 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/migrations/0008_auto_20210114_1733.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12035 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.164436 aa-fleetpings-2.9.0/fleetpings/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.164436 aa-fleetpings-2.9.0/fleetpings/static/fleetpings/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.168436 aa-fleetpings-2.9.0/fleetpings/static/fleetpings/css/
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/static/fleetpings/css/fleetpings.css
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/static/fleetpings/css/fleetpings.min.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.168436 aa-fleetpings-2.9.0/fleetpings/static/fleetpings/js/
+-rw-r--r--   0 runner    (1001) docker     (121)    24841 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/static/fleetpings/js/fleetpings.js
+-rw-r--r--   0 runner    (1001) docker     (121)    12702 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/static/fleetpings/js/fleetpings.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.164436 aa-fleetpings-2.9.0/fleetpings/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.168436 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.172436 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/additionalInformation.html
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/createOptimer.html
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/createSrpLink.html
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/fleetCommander.html
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/fleetComms.html
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/fleetDoctrine.html
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/fleetName.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/fleetType.html
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/formupLocation.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/formupTime.html
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/pingChannel.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/pingTargets.html
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/prePing.html
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/srp.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/ping.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.172436 aa-fleetpings-2.9.0/fleetpings/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/templatetags/fleetpings_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.172436 aa-fleetpings-2.9.0/fleetpings/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3425 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/tests/test_installed_modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7079 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/fleetpings/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-11 14:51:31.172436 aa-fleetpings-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:51:31.172436 aa-fleetpings-2.9.0/testauth/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/testauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/testauth/celery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9432 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/testauth/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/testauth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-01-11 14:51:22.000000 aa-fleetpings-2.9.0/testauth/wsgi.py
```

### Comparing `aa-fleetpings-2.8.0/LICENSE` & `aa-fleetpings-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/PKG-INFO` & `aa-fleetpings-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aa-fleetpings
-Version: 2.8.0
+Version: 2.9.0
 Summary: Fleet Ping Tool for Alliance Auth supporting pings via webhooks to Discord and Slack.
 Home-page: https://github.com/ppfeufer/aa-fleetpings
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
 License: GPLv3
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-fleetpings/issues
 Project-URL: Changelog, https://github.com/ppfeufer/aa-fleetpings/blob/master/CHANGELOG.md
-Project-URL: Release Notes, https://github.com/ppfeufer/aa-fleetpings/releases/tag/v2.8.0
+Project-URL: Release Notes, https://github.com/ppfeufer/aa-fleetpings/releases/tag/v2.9.0
 Project-URL: Git Repository, https://github.com/ppfeufer/aa-fleetpings
 Description: # AA Fleet Pings
         
         [![Version](https://img.shields.io/pypi/v/aa-fleetpings?label=release)](https://pypi.org/project/aa-fleetpings/)
         [![License](https://img.shields.io/github/license/ppfeufer/aa-fleetpings)](https://github.com/ppfeufer/aa-fleetpings/blob/master/LICENSE)
         [![Python](https://img.shields.io/pypi/pyversions/aa-fleetpings)](https://pypi.org/project/aa-fleetpings/)
         [![Django](https://img.shields.io/pypi/djversions/aa-fleetpings?label=django)](https://pypi.org/project/aa-fleetpings/)
```

### Comparing `aa-fleetpings-2.8.0/README.md` & `aa-fleetpings-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/aa_fleetpings.egg-info/PKG-INFO` & `aa-fleetpings-2.9.0/aa_fleetpings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aa-fleetpings
-Version: 2.8.0
+Version: 2.9.0
 Summary: Fleet Ping Tool for Alliance Auth supporting pings via webhooks to Discord and Slack.
 Home-page: https://github.com/ppfeufer/aa-fleetpings
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
 License: GPLv3
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-fleetpings/issues
 Project-URL: Changelog, https://github.com/ppfeufer/aa-fleetpings/blob/master/CHANGELOG.md
-Project-URL: Release Notes, https://github.com/ppfeufer/aa-fleetpings/releases/tag/v2.8.0
+Project-URL: Release Notes, https://github.com/ppfeufer/aa-fleetpings/releases/tag/v2.9.0
 Project-URL: Git Repository, https://github.com/ppfeufer/aa-fleetpings
 Description: # AA Fleet Pings
         
         [![Version](https://img.shields.io/pypi/v/aa-fleetpings?label=release)](https://pypi.org/project/aa-fleetpings/)
         [![License](https://img.shields.io/github/license/ppfeufer/aa-fleetpings)](https://github.com/ppfeufer/aa-fleetpings/blob/master/LICENSE)
         [![Python](https://img.shields.io/pypi/pyversions/aa-fleetpings)](https://pypi.org/project/aa-fleetpings/)
         [![Django](https://img.shields.io/pypi/djversions/aa-fleetpings?label=django)](https://pypi.org/project/aa-fleetpings/)
```

### Comparing `aa-fleetpings-2.8.0/aa_fleetpings.egg-info/SOURCES.txt` & `aa-fleetpings-2.9.0/aa_fleetpings.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -52,16 +52,19 @@
 fleetpings/templates/fleetpings/form/fleetType.html
 fleetpings/templates/fleetpings/form/formupLocation.html
 fleetpings/templates/fleetpings/form/formupTime.html
 fleetpings/templates/fleetpings/form/pingChannel.html
 fleetpings/templates/fleetpings/form/pingTargets.html
 fleetpings/templates/fleetpings/form/prePing.html
 fleetpings/templates/fleetpings/form/srp.html
+fleetpings/templatetags/__init__.py
+fleetpings/templatetags/fleetpings_versioned_static.py
 fleetpings/tests/__init__.py
 fleetpings/tests/test_access.py
 fleetpings/tests/test_installed_modules.py
+fleetpings/tests/test_templatetags.py
 fleetpings/tests/utils.py
 testauth/__init__.py
 testauth/celery.py
 testauth/settings.py
 testauth/urls.py
 testauth/wsgi.py
```

### Comparing `aa-fleetpings-2.8.0/fleetpings/admin.py` & `aa-fleetpings-2.9.0/fleetpings/admin.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/app_settings.py` & `aa-fleetpings-2.9.0/fleetpings/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/auth_hooks.py` & `aa-fleetpings-2.9.0/fleetpings/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/docs/aa-view.jpg` & `aa-fleetpings-2.9.0/fleetpings/docs/aa-view.jpg`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/docs/discord-ping-embedded.jpg` & `aa-fleetpings-2.9.0/fleetpings/docs/discord-ping-embedded.jpg`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/docs/discord-ping.jpg` & `aa-fleetpings-2.9.0/fleetpings/docs/discord-ping.jpg`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/docs/slack-ping.jpg` & `aa-fleetpings-2.9.0/fleetpings/docs/slack-ping.jpg`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/locale/de/LC_MESSAGES/django.mo` & `aa-fleetpings-2.9.0/fleetpings/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/locale/de/LC_MESSAGES/django.po` & `aa-fleetpings-2.9.0/fleetpings/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/locale/en/LC_MESSAGES/django.po` & `aa-fleetpings-2.9.0/fleetpings/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/migrations/0001_initial.py` & `aa-fleetpings-2.9.0/fleetpings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/migrations/0002_webhook_is_embed_description_change.py` & `aa-fleetpings-2.9.0/fleetpings/migrations/0002_webhook_is_embed_description_change.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/migrations/0003_fleetdoctrine_link.py` & `aa-fleetpings-2.9.0/fleetpings/migrations/0003_fleetdoctrine_link.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/migrations/0004_auto_20200915_1617.py` & `aa-fleetpings-2.9.0/fleetpings/migrations/0004_auto_20200915_1617.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/migrations/0005_fleettype_restricted_to_group.py` & `aa-fleetpings-2.9.0/fleetpings/migrations/0005_fleettype_restricted_to_group.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py` & `aa-fleetpings-2.9.0/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py` & `aa-fleetpings-2.9.0/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/migrations/0008_auto_20210114_1733.py` & `aa-fleetpings-2.9.0/fleetpings/migrations/0008_auto_20210114_1733.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/models.py` & `aa-fleetpings-2.9.0/fleetpings/models.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/static/fleetpings/js/fleetpings.js` & `aa-fleetpings-2.9.0/fleetpings/static/fleetpings/js/fleetpings.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,114 +1,104 @@
 /* global fleetpingsSettings, fleetpingsTranslations, ClipboardJS */
 
 jQuery(document).ready(function($) {
     'use strict';
 
     /* Functions
     ----------------------------------------------------------------------------------------------------------------- */
-
     /**
-     * convert line breaks into <br>
+     * Convert line breaks into <br>
      *
      * @param {string} string
      * @param {bool} isXhtml
      */
-    var nl2br = function(string, isXhtml) {
-        var breakTag = isXhtml || typeof isXhtml === 'undefined' ? '<br />' : '<br>';
+    const nl2br = function(string, isXhtml) {
+        const breakTag = isXhtml || typeof isXhtml === 'undefined' ? '<br />' : '<br>';
 
         return (string + '').replace(/([^>\r\n]?)(\r\n|\n\r|\r|\n)/g, '$1' + breakTag + '$2');
     };
 
     /**
-     * closing the message
+     * Closing the message
      *
      * @param {string} element
-     * @returns {void}
      */
-    var closeCopyMessageElement = function(element) {
+    const closeCopyMessageElement = function(element) {
         /**
-         * close after 10 seconds
+         * Close after 10 seconds
          */
         $(element).fadeTo(10000, 500).slideUp(500, function() {
             $(this).slideUp(500, function() {
                 $(this).remove();
             });
         });
     };
 
     /**
-     * show message when copy action was successful
+     * Show message when copy action was successful
      *
      * @param {string} message
      * @param {string} element
-     * @returns {undefined}
      */
-    var showSuccess = function(message, element) {
+    const showSuccess = function(message, element) {
         $(element).html(
             '<div class="alert alert-success alert-dismissable alert-copy-success">' +
             '<button type="button" class="close" data-dismiss="alert" aria-hidden="true">&times;</button>' + message +
             '</div>'
         );
 
         closeCopyMessageElement('.alert-copy-success');
-
-        return;
     };
 
     /**
-     * show message when copy action was not successful
+     * Show message when copy action was not successful
      *
      * @param {string} message
      * @param {string} element
-     * @returns {undefined}
      */
-    var showError = function(message, element) {
+    const showError = function(message, element) {
         $(element).html(
             '<div class="alert alert-danger alert-dismissable alert-copy-error">' +
             '<button type="button" class="close" data-dismiss="alert" aria-hidden="true">&times;</button>' + message +
             '</div>'
         );
 
         closeCopyMessageElement('.alert-copy-error');
-
-        return;
     };
 
     /**
-     * sanitize input string
+     * Sanitize input string
      *
-     * @param {string} input string to sanitize
-     * @returns {string} sanitized string
+     * @param {string} input String to sanitize
+     * @returns {string} Sanitized string
      */
-    var sanitizeInput = function(input) {
+    const sanitizeInput = function(input) {
         if (input) {
-            var returnValue = input
+            return input
                 .replace(
                     /<(|\/|[^>\/bi]|\/[^>bi]|[^\/>][^>]+|\/[^>][^>]+)>/g,
                     ''
                 );
-
-            return returnValue;
         } else {
             return input;
         }
     };
 
     /**
-     * escape input string
+     * Escape input string
      *
-     * @param {string} input string to escape
-     * @param {boolean} quotesToEntities transform quotes into entities
-     * @returns {string} escaped string
+     * @param {string} input String to escape
+     * @param {boolean} quotesToEntities Transform quotes into entities
+     * @returns {string} Escaped string
      */
-    var escapeInput = function(input, quotesToEntities) {
+    const escapeInput = function(input, quotesToEntities) {
         quotesToEntities = quotesToEntities || false;
 
         if (input) {
-            var returnValue = sanitizeInput(input)
+            let returnValue = sanitizeInput(input)
                 .replace(
                     /&/g,
                     '&amp;'
                 );
 
             if (quotesToEntities === true) {
                 returnValue = returnValue.replace(
@@ -127,153 +117,154 @@
             return returnValue;
         } else {
             return input;
         }
     };
 
     /**
-     * send an embedded message to a Discord webhook
+     * Send an embedded message to a Discord webhook
      *
-     * @param {string} webhookUrl
-     * @param {string} content
-     * @param {object} embeds
+     * @param {string} webhookUrl Discord webhook URL
+     * @param {string} content Message to send to Discord
+     * @param {object} embeds Embedded content » https://discohook.org/ - https://leovoel.github.io/embed-visualizer/
      */
-    var sendEmbeddedDiscordPing = function(webhookUrl, content, embeds) {
-        var request = new XMLHttpRequest();
+    const sendEmbeddedDiscordPing = function(webhookUrl, content, embeds) {
+        const request = new XMLHttpRequest();
 
         request.open('POST', webhookUrl);
         request.setRequestHeader('Content-type', 'application/json');
 
-        var params = {
+        const params = {
             username: '',
             avatar_url: '',
             content: content,
             embeds: [embeds]
         };
 
         request.send(JSON.stringify(params));
     };
 
     /**
-     * send a message to a Discord webhook
+     * Send a message to a Discord webhook
      *
-     * @param {string} webhookUrl
-     * @param {string} pingText
+     * @param {string} webhookUrl Discord webhook URL
+     * @param {string} pingText Message to send to Discord
      */
-    var sendDiscordPing = function(webhookUrl, pingText) {
-        var request = new XMLHttpRequest();
+    const sendDiscordPing = function(webhookUrl, pingText) {
+        const request = new XMLHttpRequest();
 
         request.open('POST', webhookUrl);
         request.setRequestHeader('Content-type', 'application/json');
 
-        var params = {
+        const params = {
             username: '',
             avatar_url: '',
             content: pingText
         };
 
         request.send(JSON.stringify(params));
     };
 
     /**
-     * send a message to a Slack webhook
+     * Send a message to a Slack webhook
      *
-     * @param {string} webhookUrl
-     * @param {object} payload
+     * @param {string} webhookUrl Slack webhook URL
+     * @param {object} payload Message to send to Slack
      */
-    var sendSlackPing = function(webhookUrl, payload) {
+    const sendSlackPing = function(webhookUrl, payload) {
         $.ajax({
             data: 'payload=' + JSON.stringify(payload),
             dataType: 'json',
             processData: false,
             type: 'POST',
             url: webhookUrl
         });
     };
 
     /**
-     * convert hex color code in something Discord can handle
+     * Convert hex color code in something Discord can handle
      *
      * @param {string} hexValue
      */
-    var hexToDecimal = function(hexValue) {
+    const hexToDecimal = function(hexValue) {
         return parseInt(hexValue.replace('#', ''), 16);
     };
 
     /**
-     * convert the datepicker info into an URL that the
-     * aa-tomezones module understands
+     * Convert the datepicker info into an URL that the aa-timezones module understands
      *
      * @param {string} formupTime
      */
-    var getTimezonesUrl = function(formupTime) {
-        var formupDateTime = new Date(formupTime);
-        var formupTimestamp = (formupDateTime.getTime() - formupDateTime.getTimezoneOffset() * 60 * 1000) / 1000;
-        var timezonesUrl = '';
-
-        if (fleetpingsSettings.useNewTimezoneLinks === true) {
-            timezonesUrl = fleetpingsSettings.siteUrl + 'timezones/' + formupTimestamp + '/';
-        } else {
-            timezonesUrl = fleetpingsSettings.siteUrl + 'timezones/?#' + formupTimestamp;
-        }
+    const getTimezonesUrl = function(formupTime) {
+        const formupDateTime = new Date(formupTime);
+        const formupTimestamp = (formupDateTime.getTime() - formupDateTime.getTimezoneOffset() * 60 * 1000) / 1000;
 
-        return timezonesUrl;
+        return fleetpingsSettings.siteUrl + 'timezones/' + formupTimestamp + '/';
     };
 
     /**
-     * create the ping text
+     * Create the ping text
+     *
+     * @param {string} fleetSrpCode SRP code for the fleet, if available
      */
-    var generateFleetPing = function(fleetSrpCode) {
-        var pingTarget = sanitizeInput($('select#pingTarget option:selected').val());
-        var pingTargetText = sanitizeInput($('select#pingTarget option:selected').text());
+    const generateFleetPing = function(fleetSrpCode) {
+        const pingTargetSelected = $('select#pingTarget option:selected');
+        const pingTarget = sanitizeInput(pingTargetSelected.val());
+        const pingTargetText = sanitizeInput(pingTargetSelected.text());
+
+        const pingChannelSelected = $('select#pingChannel option:selected');
+        const webhookType = sanitizeInput(pingChannelSelected.data('webhook-type'));
+        const webhookEmbedPing = sanitizeInput(pingChannelSelected.data('webhook-embed'));
 
-        var webhookType = sanitizeInput($('select#pingChannel option:selected').data('webhook-type'));
-        var webhookEmbedPing = sanitizeInput($('select#pingChannel option:selected').data('webhook-embed'));
+        const fleetTypeSelected = $('select#fleetType option:selected');
+        const fleetType = sanitizeInput(fleetTypeSelected.val());
+        const webhookEmbedColor = sanitizeInput(fleetTypeSelected.data('embed-color'));
 
-        var fleetType = sanitizeInput($('select#fleetType option:selected').val());
-        var webhookEmbedColor = sanitizeInput($('select#fleetType option:selected').data('embed-color'));
+        const fcName = sanitizeInput($('input#fcName').val());
+        const fleetName = sanitizeInput($('input#fleetName').val());
+        const formupLocation = sanitizeInput($('input#formupLocation').val());
+        const formupTime = sanitizeInput($('input#formupTime').val());
+        const fleetComms = sanitizeInput($('input#fleetComms').val());
+        const fleetDoctrine = sanitizeInput($('input#fleetDoctrine').val());
+        const fleetSrp = sanitizeInput($('select#fleetSrp option:selected').val());
+        const additionalInformation = sanitizeInput($('textarea#additionalInformation').val());
 
-        var fcName = sanitizeInput($('input#fcName').val());
-        var fleetName = sanitizeInput($('input#fleetName').val());
-        var formupLocation = sanitizeInput($('input#formupLocation').val());
-        var formupTime = sanitizeInput($('input#formupTime').val());
-        var fleetComms = sanitizeInput($('input#fleetComms').val());
-        var fleetDoctrine = sanitizeInput($('input#fleetDoctrine').val());
-        var fleetSrp = sanitizeInput($('select#fleetSrp option:selected').val());
-        var additionalInformation = sanitizeInput($('textarea#additionalInformation').val());
+        const checkboxPrePing = $('input#prePing');
+        const checkboxFormupTimeNow = $('input#formupTimeNow');
+        const checkboxCreateOptimer = $('input#createOptimer');
 
-        // let's see if we can find a doctrine link
-        var fleetDoctrineLink = null;
+        // Let's see if we can find a doctrine link
+        let fleetDoctrineLink = null;
         if (fleetDoctrine !== '') {
-            var selectedLink = $('#fleetDoctrineList [value="' + escapeInput(fleetDoctrine, false) + '"]').data('doctrine-url');
+            const selectedLink = $('#fleetDoctrineList [value="' + escapeInput(fleetDoctrine, false) + '"]').data('doctrine-url');
 
             if (undefined !== selectedLink && selectedLink !== '') {
                 // Houston, we have a link!
                 fleetDoctrineLink = selectedLink;
             }
         }
 
-        // ping webhooks, if configured
-        var webhookUrl = false;
+        // Ping webhooks, if configured
+        let webhookUrl = false;
 
         if ($('select#pingChannel').length) {
-            webhookUrl = sanitizeInput($('select#pingChannel option:selected').val());
+            webhookUrl = sanitizeInput(pingChannelSelected.val());
         }
 
         $('.aa-fleetpings-no-ping').hide('fast');
         $('.aa-fleetpings-ping').show('fast');
 
-        var webhookPingTextHeader = '';
-        var webhookPingTextContent = '';
-        var webhookPingTextFooter = '';
-        var pingText = '';
-
-        // determine pingTarget and pingTargetText
-        var discordPingTarget = '';
-        var webhookPingTarget = '';
+        let webhookPingTextHeader = '';
+        let webhookPingTextContent = '';
+        let webhookPingTextFooter = '';
+        let pingText = '';
+
+        // Determine pingTarget and pingTargetText
+        let discordPingTarget = '';
+        let webhookPingTarget = '';
 
         if (pingTarget !== '') {
             // pingTarget
             if (pingTarget.indexOf('@') > -1) {
                 webhookPingTarget = pingTarget;
             } else {
                 webhookPingTarget = '<@&' + pingTarget + '>';
@@ -282,23 +273,23 @@
             // pingTargetText
             if (pingTargetText.indexOf('@') > -1) {
                 discordPingTarget = pingTargetText;
             } else {
                 discordPingTarget = '@' + pingTargetText;
             }
 
-            // separator
+            // Separator
             pingText += ' :: ';
         }
 
-        // fleet announcement
+        // Fleet announcement
         pingText += '**';
 
-        // check if it's a pre-ping or not
-        if ($('input#prePing').is(':checked')) {
+        // Check if it's a pre-ping or not
+        if (checkboxPrePing.is(':checked')) {
             pingText += '### PRE PING ###';
             webhookPingTextHeader += '### PRE PING ###';
 
             if (fleetType !== '') {
                 pingText += ' / ' + fleetType + ' Fleet';
                 webhookPingTextHeader += ' / ' + fleetType + ' Fleet';
             }
@@ -314,42 +305,42 @@
 
             pingText += 'Fleet is up';
             webhookPingTextHeader += 'Fleet is up';
         }
 
         pingText += '**' + '\n';
 
-        // check if FC name is available
+        // Check if FC name is available
         if (fcName !== '') {
             pingText += '\n' + '**FC:** ' + fcName;
             webhookPingTextContent += '\n' + '**FC:** ' + fcName;
         }
 
-        // check if fleet name is available
+        // Check if fleet name is available
         if (fleetName !== '') {
             pingText += '\n' + '**Fleet Name:** ' + fleetName;
             webhookPingTextContent += '\n' + '**Fleet Name:** ' + fleetName;
         }
 
-        // check if form-up location is available
+        // Check if form-up location is available
         if (formupLocation !== '') {
             pingText += '\n' + '**Formup Location:** ' + formupLocation;
             webhookPingTextContent += '\n' + '**Formup Location:** ' + formupLocation;
         }
 
-        // check if form-up time is available
-        if ($('input#formupTimeNow').is(':checked')) {
+        // Check if form-up time is available
+        if (checkboxFormupTimeNow.is(':checked')) {
             pingText += '\n' + '**Formup Time:** NOW';
             webhookPingTextContent += '\n' + '**Formup Time:** NOW';
         } else {
             if (formupTime !== '') {
                 pingText += '\n' + '**Formup Time:** ' + formupTime;
                 webhookPingTextContent += '\n' + '**Formup Time:** ' + formupTime;
 
-                // get the timestamp and build the link to the timezones module if it's installed
+                // Get the timestamp and build the link to the timezones module if it's installed
                 if (fleetpingsSettings.timezonesInstalled === true) {
                     var timezonesUrl = getTimezonesUrl(formupTime);
 
                     pingText += ' - ' + timezonesUrl;
 
                     if (webhookType === 'Discord') {
                         webhookPingTextContent += ' ([Time Zone Conversion](' + timezonesUrl + '))';
@@ -358,51 +349,51 @@
                     if (webhookType === 'Slack') {
                         webhookPingTextContent += ' (<' + timezonesUrl + '|Time Zone Conversion>)';
                     }
                 }
             }
         }
 
-        // check if fleet comms is available
+        // Check if fleet comms is available
         if (fleetComms !== '') {
             pingText += '\n' + '**Comms:** ' + fleetComms;
             webhookPingTextContent += '\n' + '**Comms:** ' + fleetComms;
         }
 
-        // check if doctrine is available
+        // Check if doctrine is available
         if (fleetDoctrine !== '') {
             pingText += '\n' + '**Ships / Doctrine:** ' + fleetDoctrine;
             webhookPingTextContent += '\n' + '**Ships / Doctrine:** ' + fleetDoctrine;
 
-            // grab the doctrine link if there is one
+            // Grab the doctrine link if there is one
             if (fleetDoctrineLink !== null) {
                 pingText += ' - ' + fleetDoctrineLink;
 
                 if (webhookType === 'Discord') {
                     webhookPingTextContent += ' ([Doctrine Link](' + fleetDoctrineLink + '))';
                 }
 
                 if (webhookType === 'Slack') {
                     webhookPingTextContent += ' (<' + fleetDoctrineLink + '|Doctrine Link>)';
                 }
             }
         }
 
-        // check if srp is available
+        // Check if srp is available
         if (fleetSrp !== '') {
             pingText += '\n' + '**SRP:** ' + fleetSrp;
             webhookPingTextContent += '\n' + '**SRP:** ' + fleetSrp;
 
             if (fleetSrp === 'Yes' && fleetSrpCode !== '') {
                 pingText += ' (SRP Code: ' + fleetSrpCode + ')';
                 webhookPingTextContent += ' (SRP Code: ' + fleetSrpCode + ')';
             }
         }
 
-        // check if additional information is available
+        // Check if additional information is available
         if (additionalInformation !== '') {
             pingText += '\n\n' + '**Additional Information**:' + '\n' + additionalInformation;
             webhookPingTextContent += '\n\n' + '**Additional Information**:' + '\n' + additionalInformation;
         }
 
         if (fleetpingsSettings.platformUsed === 'Discord') {
             $('.aa-fleetpings-ping-text').html(
@@ -412,99 +403,97 @@
 
         if (fleetpingsSettings.platformUsed === 'Slack') {
             $('.aa-fleetpings-ping-text').html(
                 '<p>' + nl2br(discordPingTarget + pingText.split('**').join('*')) + '</p>'
             );
         }
 
-        // ping it directly if a webhook is selected
+        // Ping it directly if a webhook is selected
         if (webhookUrl !== false && webhookUrl !== '') {
             // add ping creator at the end
             if (fleetpingsSettings.pingCreator !== '') {
                 pingText += '\n\n' + '*(Ping sent by: ' + fleetpingsSettings.pingCreator + ')*';
                 webhookPingTextFooter = '(Ping sent by: ' + fleetpingsSettings.pingCreator + ')';
             }
 
-            // default embed color
-            var embedColor = '#faa61a';
+            // Default embed color
+            let embedColor = '#faa61a';
 
             if (fleetType !== '' && embedColor !== '') {
                 embedColor = webhookEmbedColor;
             }
 
-            // add fcName if we have one
+            // Add fcName if we have one
             if (fcName !== '') {
                 webhookPingTextHeader += ' under ' + fcName;
             }
 
-            var copyPasteText = '';
-
-            // send the ping to Discord
+            // Send the ping to Discord
             if (webhookType === 'Discord') {
                 if (undefined !== webhookEmbedPing && webhookEmbedPing === 'True') {
                     if (pingTarget !== '') {
                         webhookPingTarget += ' :: ';
                     }
 
                     sendEmbeddedDiscordPing(
                         webhookUrl,
                         webhookPingTarget + '**' + webhookPingTextHeader + '**' + '\n' + '** **',
-                        // embedded content » https://discohook.org/ - https://leovoel.github.io/embed-visualizer/
+                        // Embedded content » https://discohook.org/ - https://leovoel.github.io/embed-visualizer/
                         {
                             'title': '**.: Fleet Details :.**',
                             'description': webhookPingTextContent,
                             'color': hexToDecimal(embedColor),
                             'footer': {
                                 'text': webhookPingTextFooter
                             }
                         }
                     );
                 } else {
                     sendDiscordPing(webhookUrl, webhookPingTarget + pingText);
                 }
             }
 
-            // send the ping to Discord
+            // Send the ping to Discord
             if (webhookType === 'Slack') {
-                var slackEmbedPingTarget = '';
+                let slackEmbedPingTarget = '';
 
                 if (pingTarget !== '') {
                     slackEmbedPingTarget = '<' + webhookPingTarget.replace('@', '!') + '> :: ';
                 }
 
                 /**
-                 * payload to send to Slack
+                 * Payload to send to Slack
                  *
                  * @type {{attachments: [{color: string, footer: string, pretext: string, text: string, fallback: string}]}}
                  */
                 var payload = {
                     'attachments': [{
                         'fallback': pingText,
                         'color': embedColor,
                         'pretext': slackEmbedPingTarget + '*' + webhookPingTextHeader + '*',
                         'text': '*.: Fleet Details :.*' + '\n' + webhookPingTextContent.split('**').join('*'),
-                        'footer': webhookPingTextFooter,
+                        'footer': webhookPingTextFooter
                         //                            'footer_icon': 'https://platform.slack-edge.com/img/default_application_icon.png'
                     }]
                 };
 
                 sendSlackPing(webhookUrl, payload);
             }
 
-            // tell the FC that it's already pinged
+            // Tell the FC that it's already pinged
             showSuccess(
                 fleetpingsTranslations.ping.success,
                 '.aa-fleetpings-ping-copyresult'
             );
         }
 
-        // create optimer if needed
+        // Create optimer if needed
         if (fleetpingsSettings.optimerInstalled === true) {
-            if ($('input#prePing').is(':checked') && $('input#createOptimer').is(':checked') && formupTime !== '') {
-                var optimerAjaxUrl = fleetpingsSettings.optimerAjaxUrl;
+            if (checkboxPrePing.is(':checked') && checkboxCreateOptimer.is(':checked') && formupTime !== '') {
+                const optimerAjaxUrl = fleetpingsSettings.optimerAjaxUrl;
 
                 $.ajax({
                     url: optimerAjaxUrl,
                     type: 'post',
                     data: {
                         fleet_doctrine: fleetDoctrine,
                         formup_location: formupLocation,
@@ -513,168 +502,170 @@
                         fleet_commander: fcName
                     },
                     headers: {
                         'X-CSRFToken': $('input[name="csrfmiddlewaretoken"]').val()
                     }
                 });
 
-                // re-set checkbox
-                $('input#createOptimer').removeAttr('checked');
+                // Re-set checkbox
+                checkboxCreateOptimer.prop('checked', false);
 
-                // let the user know that an optimer has been created
+                // Let the user know that an optimer has been created
                 showSuccess(
                     fleetpingsTranslations.optimer.created,
                     '.fleetpings-create-optimer-message'
                 );
             }
         }
     };
 
     /**
-     * copy the fleet ping to clipboard
+     * Copy the fleet ping to clipboard
      */
-    var copyFleetPing = function() {
+    const copyFleetPing = function() {
         /**
-         * copy text to clipboard
+         * Copy text to clipboard
          *
          * @type Clipboard
          */
-        var clipboardFleetPingData = new ClipboardJS('button#copyFleetPing');
+        const clipboardFleetPingData = new ClipboardJS('button#copyFleetPing');
 
         /**
-         * copy success
+         * Copy success
          *
          * @param {type} e
          */
         clipboardFleetPingData.on('success', function(e) {
             showSuccess(
                 fleetpingsTranslations.copyToClipboard.success,
                 '.aa-fleetpings-ping-copyresult'
             );
 
             e.clearSelection();
             clipboardFleetPingData.destroy();
         });
 
         /**
-         * copy error
+         * Copy error
          */
         clipboardFleetPingData.on('error', function() {
             showError(
                 fleetpingsTranslations.copyToClipboard.error,
                 '.aa-fleetpings-ping-copyresult'
             );
 
             clipboardFleetPingData.destroy();
         });
     };
 
     /* Events
     ----------------------------------------------------------------------------------------------------------------- */
-
+    /**
+     * Toggle "Create SRP Link" checkbox
+     */
     if (fleetpingsSettings.srpModuleAvailableToUser === true) {
         if (sanitizeInput($('select#fleetSrp option:selected').val()) === 'Yes' && $('input#formupTimeNow').is(':checked')) {
             $('.fleetpings-create-srp-link').show('fast');
         } else {
-            $('input#createSrpLink').removeAttr('checked');
+            $('input#createSrpLink').prop('checked', false);
             $('.fleetpings-create-srp-link').hide('fast');
         }
 
         $('select#fleetSrp').change(function() {
             if (sanitizeInput($('select#fleetSrp option:selected').val()) === 'Yes' && $('input#formupTimeNow').is(':checked')) {
                 $('.fleetpings-create-srp-link').show('fast');
             } else {
-                $('input#createSrpLink').removeAttr('checked');
+                $('input#createSrpLink').prop('checked', false);
                 $('.fleetpings-create-srp-link').hide('fast');
             }
         });
     }
 
     /**
-     * toggle "Formup NOW" checkbox when "Pre-Ping" is toggled
+     * Toggle "Formup NOW" checkbox when "Pre-Ping" is toggled
      *
      * Behaviour:
      *  Pre-Ping checked
      *      » Formup NOW unchecked
      *      » Create Optimer is unchecked and hidden
      *      » Create SRP Link is displayed
      *  Pre-Ping unchecked
      *      » Formup NOW checked
      *      » Create Optimer is displayed
      *      » Create SRP Link is hidden and unchecked
      */
     $('#prePing').on('change', function() {
         if ($('input#prePing').is(':checked')) {
-            $('input#formupTimeNow').removeAttr('checked');
+            $('input#formupTimeNow').prop('checked', false);
             $('input#formupTime').removeAttr('disabled');
 
             if (fleetpingsSettings.optimerInstalled === true) {
                 $('.fleetpings-create-optimer').show('fast');
             }
 
             if (fleetpingsSettings.srpModuleAvailableToUser === true) {
-                $('input#createSrpLink').removeAttr('checked');
+                $('input#createSrpLink').prop('checked', false);
                 $('.fleetpings-create-srp-link').hide('fast');
             }
         } else {
-            $('input#formupTimeNow').prop('checked', true).removeAttr('disabled');
+            $('input#formupTimeNow').prop('checked', true);
             $('input#formupTime').prop('disabled', true);
 
             if (fleetpingsSettings.optimerInstalled === true) {
-                $('input#createOptimer').removeAttr('checked');
+                $('input#createOptimer').prop('checked', false);
                 $('.fleetpings-create-optimer').hide('fast');
             }
 
             if (fleetpingsSettings.srpModuleAvailableToUser === true && sanitizeInput($('select#fleetSrp option:selected').val()) === 'Yes') {
                 $('.fleetpings-create-srp-link').show('fast');
             }
         }
     });
 
     $('input#formupTimeNow').on('change', function() {
         if ($(this).is(':checked')) {
-            $('input#prePing').removeAttr('checked');
-            // $('input#prePing').prop('disabled', true);
+            $('input#prePing').prop('checked', false);
             $('input#formupTime').prop('disabled', true);
 
             if (fleetpingsSettings.optimerInstalled === true) {
-                $('input#createOptimer').removeAttr('checked');
+                $('input#createOptimer').prop('checked', false);
                 $('.fleetpings-create-optimer').hide('fast');
             }
 
             if (fleetpingsSettings.srpModuleAvailableToUser === true && sanitizeInput($('select#fleetSrp option:selected').val()) === 'Yes') {
                 $('.fleetpings-create-srp-link').show('fast');
             }
         } else {
-            $('input#prePing').prop('checked', true).removeAttr('disabled');
+            $('input#prePing').prop('checked', true);
             $('input#formupTime').removeAttr('disabled');
 
             if (fleetpingsSettings.optimerInstalled === true) {
                 $('.fleetpings-create-optimer').show('fast');
             }
 
             if (fleetpingsSettings.srpModuleAvailableToUser === true) {
-                $('input#createSrpLink').removeAttr('checked');
+                $('input#createSrpLink').prop('checked', false);
                 $('.fleetpings-create-srp-link').hide('fast');
             }
         }
     });
 
     /**
-     * generate ping text
+     * Generate ping text
      */
     $('button#createPingText').on('click', function() {
-        var fleetSrp = sanitizeInput($('select#fleetSrp option:selected').val());
-        var fleetName = sanitizeInput($('input#fleetName').val());
-        var fleetDoctrine = sanitizeInput($('input#fleetDoctrine').val());
-
-        if ($('input#createSrpLink').is(':checked') && $('input#formupTimeNow').is(':checked')) {
-            // create SRP link
-            var srpAjaxUrl = fleetpingsSettings.srpAjaxUrl;
-            var srpCode = '';
+        const fleetName = sanitizeInput($('input#fleetName').val());
+        const fleetDoctrine = sanitizeInput($('input#fleetDoctrine').val());
+        const checkboxCreateSrpLink = $('input#createSrpLink');
+        const checkboxFormupTimeNow = $('input#formupTimeNow');
+
+        if (checkboxCreateSrpLink.is(':checked') && checkboxFormupTimeNow.is(':checked')) {
+            // Create SRP link
+            const srpAjaxUrl = fleetpingsSettings.srpAjaxUrl;
+            let srpCode = '';
 
             $.ajax({
                 url: srpAjaxUrl,
                 type: 'post',
                 data: {
                     fleet_doctrine: fleetDoctrine,
                     fleet_name: fleetName
@@ -685,30 +676,30 @@
                     )
                 }
             }).done(function(result) {
                 srpCode = result.srp_code;
 
                 generateFleetPing(srpCode);
 
-                // let the user know that an optimer has been created
+                // Let the user know that an optimer has been created
                 showSuccess(
                     fleetpingsTranslations.srp.created,
                     '.fleetpings-create-srp-link-message'
                 );
             });
 
-            // re-set checkbox
-            $('input#createSrpLink').removeAttr('checked');
+            // Re-set checkbox
+            checkboxCreateSrpLink.prop('checked', false);
         } else {
             generateFleetPing('');
         }
 
         return false;
     });
 
     /**
-     * copy ping text
+     * Copy ping text
      */
     $('button#copyFleetPing').on('click', function() {
         copyFleetPing();
     });
 });
```

### Comparing `aa-fleetpings-2.8.0/fleetpings/static/fleetpings/js/fleetpings.min.js` & `aa-fleetpings-2.9.0/fleetpings/static/fleetpings/js/fleetpings.min.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,148 +1,145 @@
 jQuery(document).ready(function($) {
     "use strict";
-    var nl2br = function(string, isXhtml) {
-        var breakTag = isXhtml || typeof isXhtml === "undefined" ? "<br />" : "<br>";
+    const nl2br = function(string, isXhtml) {
+        const breakTag = isXhtml || typeof isXhtml === "undefined" ? "<br />" : "<br>";
         return (string + "").replace(/([^>\r\n]?)(\r\n|\n\r|\r|\n)/g, "$1" + breakTag + "$2")
     };
-    var closeCopyMessageElement = function(element) {
+    const closeCopyMessageElement = function(element) {
         $(element).fadeTo(1e4, 500).slideUp(500, function() {
             $(this).slideUp(500, function() {
                 $(this).remove()
             })
         })
     };
-    var showSuccess = function(message, element) {
+    const showSuccess = function(message, element) {
         $(element).html('<div class="alert alert-success alert-dismissable alert-copy-success">' + '<button type="button" class="close" data-dismiss="alert" aria-hidden="true">&times;</button>' + message + "</div>");
-        closeCopyMessageElement(".alert-copy-success");
-        return
+        closeCopyMessageElement(".alert-copy-success")
     };
-    var showError = function(message, element) {
+    const showError = function(message, element) {
         $(element).html('<div class="alert alert-danger alert-dismissable alert-copy-error">' + '<button type="button" class="close" data-dismiss="alert" aria-hidden="true">&times;</button>' + message + "</div>");
-        closeCopyMessageElement(".alert-copy-error");
-        return
+        closeCopyMessageElement(".alert-copy-error")
     };
-    var sanitizeInput = function(input) {
+    const sanitizeInput = function(input) {
         if (input) {
-            var returnValue = input.replace(/<(|\/|[^>\/bi]|\/[^>bi]|[^\/>][^>]+|\/[^>][^>]+)>/g, "");
-            return returnValue
+            return input.replace(/<(|\/|[^>\/bi]|\/[^>bi]|[^\/>][^>]+|\/[^>][^>]+)>/g, "")
         } else {
             return input
         }
     };
-    var escapeInput = function(input, quotesToEntities) {
+    const escapeInput = function(input, quotesToEntities) {
         quotesToEntities = quotesToEntities || false;
         if (input) {
-            var returnValue = sanitizeInput(input).replace(/&/g, "&amp;");
+            let returnValue = sanitizeInput(input).replace(/&/g, "&amp;");
             if (quotesToEntities === true) {
                 returnValue = returnValue.replace(/"/g, "&quot;")
             }
             if (quotesToEntities === false) {
                 returnValue = returnValue.replace(/"/g, '\\"')
             }
             return returnValue
         } else {
             return input
         }
     };
-    var sendEmbeddedDiscordPing = function(webhookUrl, content, embeds) {
-        var request = new XMLHttpRequest;
+    const sendEmbeddedDiscordPing = function(webhookUrl, content, embeds) {
+        const request = new XMLHttpRequest;
         request.open("POST", webhookUrl);
         request.setRequestHeader("Content-type", "application/json");
-        var params = {
+        const params = {
             username: "",
             avatar_url: "",
             content: content,
             embeds: [embeds]
         };
         request.send(JSON.stringify(params))
     };
-    var sendDiscordPing = function(webhookUrl, pingText) {
-        var request = new XMLHttpRequest;
+    const sendDiscordPing = function(webhookUrl, pingText) {
+        const request = new XMLHttpRequest;
         request.open("POST", webhookUrl);
         request.setRequestHeader("Content-type", "application/json");
-        var params = {
+        const params = {
             username: "",
             avatar_url: "",
             content: pingText
         };
         request.send(JSON.stringify(params))
     };
-    var sendSlackPing = function(webhookUrl, payload) {
+    const sendSlackPing = function(webhookUrl, payload) {
         $.ajax({
             data: "payload=" + JSON.stringify(payload),
             dataType: "json",
             processData: false,
             type: "POST",
             url: webhookUrl
         })
     };
-    var hexToDecimal = function(hexValue) {
+    const hexToDecimal = function(hexValue) {
         return parseInt(hexValue.replace("#", ""), 16)
     };
-    var getTimezonesUrl = function(formupTime) {
-        var formupDateTime = new Date(formupTime);
-        var formupTimestamp = (formupDateTime.getTime() - formupDateTime.getTimezoneOffset() * 60 * 1e3) / 1e3;
-        var timezonesUrl = "";
-        if (fleetpingsSettings.useNewTimezoneLinks === true) {
-            timezonesUrl = fleetpingsSettings.siteUrl + "timezones/" + formupTimestamp + "/"
-        } else {
-            timezonesUrl = fleetpingsSettings.siteUrl + "timezones/?#" + formupTimestamp
-        }
-        return timezonesUrl
-    };
-    var generateFleetPing = function(fleetSrpCode) {
-        var pingTarget = sanitizeInput($("select#pingTarget option:selected").val());
-        var pingTargetText = sanitizeInput($("select#pingTarget option:selected").text());
-        var webhookType = sanitizeInput($("select#pingChannel option:selected").data("webhook-type"));
-        var webhookEmbedPing = sanitizeInput($("select#pingChannel option:selected").data("webhook-embed"));
-        var fleetType = sanitizeInput($("select#fleetType option:selected").val());
-        var webhookEmbedColor = sanitizeInput($("select#fleetType option:selected").data("embed-color"));
-        var fcName = sanitizeInput($("input#fcName").val());
-        var fleetName = sanitizeInput($("input#fleetName").val());
-        var formupLocation = sanitizeInput($("input#formupLocation").val());
-        var formupTime = sanitizeInput($("input#formupTime").val());
-        var fleetComms = sanitizeInput($("input#fleetComms").val());
-        var fleetDoctrine = sanitizeInput($("input#fleetDoctrine").val());
-        var fleetSrp = sanitizeInput($("select#fleetSrp option:selected").val());
-        var additionalInformation = sanitizeInput($("textarea#additionalInformation").val());
-        var fleetDoctrineLink = null;
+    const getTimezonesUrl = function(formupTime) {
+        const formupDateTime = new Date(formupTime);
+        const formupTimestamp = (formupDateTime.getTime() - formupDateTime.getTimezoneOffset() * 60 * 1e3) / 1e3;
+        return fleetpingsSettings.siteUrl + "timezones/" + formupTimestamp + "/"
+    };
+    const generateFleetPing = function(fleetSrpCode) {
+        const pingTargetSelected = $("select#pingTarget option:selected");
+        const pingTarget = sanitizeInput(pingTargetSelected.val());
+        const pingTargetText = sanitizeInput(pingTargetSelected.text());
+        const pingChannelSelected = $("select#pingChannel option:selected");
+        const webhookType = sanitizeInput(pingChannelSelected.data("webhook-type"));
+        const webhookEmbedPing = sanitizeInput(pingChannelSelected.data("webhook-embed"));
+        const fleetTypeSelected = $("select#fleetType option:selected");
+        const fleetType = sanitizeInput(fleetTypeSelected.val());
+        const webhookEmbedColor = sanitizeInput(fleetTypeSelected.data("embed-color"));
+        const fcName = sanitizeInput($("input#fcName").val());
+        const fleetName = sanitizeInput($("input#fleetName").val());
+        const formupLocation = sanitizeInput($("input#formupLocation").val());
+        const formupTime = sanitizeInput($("input#formupTime").val());
+        const fleetComms = sanitizeInput($("input#fleetComms").val());
+        const fleetDoctrine = sanitizeInput($("input#fleetDoctrine").val());
+        const fleetSrp = sanitizeInput($("select#fleetSrp option:selected").val());
+        const additionalInformation = sanitizeInput($("textarea#additionalInformation").val());
+        const checkboxPrePing = $("input#prePing");
+        const checkboxFormupTimeNow = $("input#formupTimeNow");
+        const checkboxCreateOptimer = $("input#createOptimer");
+        let fleetDoctrineLink = null;
         if (fleetDoctrine !== "") {
-            var selectedLink = $('#fleetDoctrineList [value="' + escapeInput(fleetDoctrine, false) + '"]').data("doctrine-url");
+            const selectedLink = $('#fleetDoctrineList [value="' + escapeInput(fleetDoctrine, false) + '"]').data("doctrine-url");
             if (undefined !== selectedLink && selectedLink !== "") {
                 fleetDoctrineLink = selectedLink
             }
         }
-        var webhookUrl = false;
+        let webhookUrl = false;
         if ($("select#pingChannel").length) {
-            webhookUrl = sanitizeInput($("select#pingChannel option:selected").val())
+            webhookUrl = sanitizeInput(pingChannelSelected.val())
         }
         $(".aa-fleetpings-no-ping").hide("fast");
         $(".aa-fleetpings-ping").show("fast");
-        var webhookPingTextHeader = "";
-        var webhookPingTextContent = "";
-        var webhookPingTextFooter = "";
-        var pingText = "";
-        var discordPingTarget = "";
-        var webhookPingTarget = "";
+        let webhookPingTextHeader = "";
+        let webhookPingTextContent = "";
+        let webhookPingTextFooter = "";
+        let pingText = "";
+        let discordPingTarget = "";
+        let webhookPingTarget = "";
         if (pingTarget !== "") {
             if (pingTarget.indexOf("@") > -1) {
                 webhookPingTarget = pingTarget
             } else {
                 webhookPingTarget = "<@&" + pingTarget + ">"
             }
             if (pingTargetText.indexOf("@") > -1) {
                 discordPingTarget = pingTargetText
             } else {
                 discordPingTarget = "@" + pingTargetText
             }
             pingText += " :: "
         }
         pingText += "**";
-        if ($("input#prePing").is(":checked")) {
+        if (checkboxPrePing.is(":checked")) {
             pingText += "### PRE PING ###";
             webhookPingTextHeader += "### PRE PING ###";
             if (fleetType !== "") {
                 pingText += " / " + fleetType + " Fleet";
                 webhookPingTextHeader += " / " + fleetType + " Fleet"
             }
         } else {
@@ -162,15 +159,15 @@
             pingText += "\n" + "**Fleet Name:** " + fleetName;
             webhookPingTextContent += "\n" + "**Fleet Name:** " + fleetName
         }
         if (formupLocation !== "") {
             pingText += "\n" + "**Formup Location:** " + formupLocation;
             webhookPingTextContent += "\n" + "**Formup Location:** " + formupLocation
         }
-        if ($("input#formupTimeNow").is(":checked")) {
+        if (checkboxFormupTimeNow.is(":checked")) {
             pingText += "\n" + "**Formup Time:** NOW";
             webhookPingTextContent += "\n" + "**Formup Time:** NOW"
         } else {
             if (formupTime !== "") {
                 pingText += "\n" + "**Formup Time:** " + formupTime;
                 webhookPingTextContent += "\n" + "**Formup Time:** " + formupTime;
                 if (fleetpingsSettings.timezonesInstalled === true) {
@@ -221,22 +218,21 @@
             $(".aa-fleetpings-ping-text").html("<p>" + nl2br(discordPingTarget + pingText.split("**").join("*")) + "</p>")
         }
         if (webhookUrl !== false && webhookUrl !== "") {
             if (fleetpingsSettings.pingCreator !== "") {
                 pingText += "\n\n" + "*(Ping sent by: " + fleetpingsSettings.pingCreator + ")*";
                 webhookPingTextFooter = "(Ping sent by: " + fleetpingsSettings.pingCreator + ")"
             }
-            var embedColor = "#faa61a";
+            let embedColor = "#faa61a";
             if (fleetType !== "" && embedColor !== "") {
                 embedColor = webhookEmbedColor
             }
             if (fcName !== "") {
                 webhookPingTextHeader += " under " + fcName
             }
-            var copyPasteText = "";
             if (webhookType === "Discord") {
                 if (undefined !== webhookEmbedPing && webhookEmbedPing === "True") {
                     if (pingTarget !== "") {
                         webhookPingTarget += " :: "
                     }
                     sendEmbeddedDiscordPing(webhookUrl, webhookPingTarget + "**" + webhookPingTextHeader + "**" + "\n" + "** **", {
                         title: "**.: Fleet Details :.**",
@@ -247,15 +243,15 @@
                         }
                     })
                 } else {
                     sendDiscordPing(webhookUrl, webhookPingTarget + pingText)
                 }
             }
             if (webhookType === "Slack") {
-                var slackEmbedPingTarget = "";
+                let slackEmbedPingTarget = "";
                 if (pingTarget !== "") {
                     slackEmbedPingTarget = "<" + webhookPingTarget.replace("@", "!") + "> :: "
                 }
                 var payload = {
                     attachments: [{
                         fallback: pingText,
                         color: embedColor,
@@ -265,116 +261,117 @@
                     }]
                 };
                 sendSlackPing(webhookUrl, payload)
             }
             showSuccess(fleetpingsTranslations.ping.success, ".aa-fleetpings-ping-copyresult")
         }
         if (fleetpingsSettings.optimerInstalled === true) {
-            if ($("input#prePing").is(":checked") && $("input#createOptimer").is(":checked") && formupTime !== "") {
-                var optimerAjaxUrl = fleetpingsSettings.optimerAjaxUrl;
+            if (checkboxPrePing.is(":checked") && checkboxCreateOptimer.is(":checked") && formupTime !== "") {
+                const optimerAjaxUrl = fleetpingsSettings.optimerAjaxUrl;
                 $.ajax({
                     url: optimerAjaxUrl,
                     type: "post",
                     data: {
                         fleet_doctrine: fleetDoctrine,
                         formup_location: formupLocation,
                         formup_time: formupTime,
                         fleet_name: fleetName,
                         fleet_commander: fcName
                     },
                     headers: {
                         "X-CSRFToken": $('input[name="csrfmiddlewaretoken"]').val()
                     }
                 });
-                $("input#createOptimer").removeAttr("checked");
+                checkboxCreateOptimer.prop("checked", false);
                 showSuccess(fleetpingsTranslations.optimer.created, ".fleetpings-create-optimer-message")
             }
         }
     };
-    var copyFleetPing = function() {
-        var clipboardFleetPingData = new ClipboardJS("button#copyFleetPing");
+    const copyFleetPing = function() {
+        const clipboardFleetPingData = new ClipboardJS("button#copyFleetPing");
         clipboardFleetPingData.on("success", function(e) {
             showSuccess(fleetpingsTranslations.copyToClipboard.success, ".aa-fleetpings-ping-copyresult");
             e.clearSelection();
             clipboardFleetPingData.destroy()
         });
         clipboardFleetPingData.on("error", function() {
             showError(fleetpingsTranslations.copyToClipboard.error, ".aa-fleetpings-ping-copyresult");
             clipboardFleetPingData.destroy()
         })
     };
     if (fleetpingsSettings.srpModuleAvailableToUser === true) {
         if (sanitizeInput($("select#fleetSrp option:selected").val()) === "Yes" && $("input#formupTimeNow").is(":checked")) {
             $(".fleetpings-create-srp-link").show("fast")
         } else {
-            $("input#createSrpLink").removeAttr("checked");
+            $("input#createSrpLink").prop("checked", false);
             $(".fleetpings-create-srp-link").hide("fast")
         }
         $("select#fleetSrp").change(function() {
             if (sanitizeInput($("select#fleetSrp option:selected").val()) === "Yes" && $("input#formupTimeNow").is(":checked")) {
                 $(".fleetpings-create-srp-link").show("fast")
             } else {
-                $("input#createSrpLink").removeAttr("checked");
+                $("input#createSrpLink").prop("checked", false);
                 $(".fleetpings-create-srp-link").hide("fast")
             }
         })
     }
     $("#prePing").on("change", function() {
         if ($("input#prePing").is(":checked")) {
-            $("input#formupTimeNow").removeAttr("checked");
+            $("input#formupTimeNow").prop("checked", false);
             $("input#formupTime").removeAttr("disabled");
             if (fleetpingsSettings.optimerInstalled === true) {
                 $(".fleetpings-create-optimer").show("fast")
             }
             if (fleetpingsSettings.srpModuleAvailableToUser === true) {
-                $("input#createSrpLink").removeAttr("checked");
+                $("input#createSrpLink").prop("checked", false);
                 $(".fleetpings-create-srp-link").hide("fast")
             }
         } else {
-            $("input#formupTimeNow").prop("checked", true).removeAttr("disabled");
+            $("input#formupTimeNow").prop("checked", true);
             $("input#formupTime").prop("disabled", true);
             if (fleetpingsSettings.optimerInstalled === true) {
-                $("input#createOptimer").removeAttr("checked");
+                $("input#createOptimer").prop("checked", false);
                 $(".fleetpings-create-optimer").hide("fast")
             }
             if (fleetpingsSettings.srpModuleAvailableToUser === true && sanitizeInput($("select#fleetSrp option:selected").val()) === "Yes") {
                 $(".fleetpings-create-srp-link").show("fast")
             }
         }
     });
     $("input#formupTimeNow").on("change", function() {
         if ($(this).is(":checked")) {
-            $("input#prePing").removeAttr("checked");
+            $("input#prePing").prop("checked", false);
             $("input#formupTime").prop("disabled", true);
             if (fleetpingsSettings.optimerInstalled === true) {
-                $("input#createOptimer").removeAttr("checked");
+                $("input#createOptimer").prop("checked", false);
                 $(".fleetpings-create-optimer").hide("fast")
             }
             if (fleetpingsSettings.srpModuleAvailableToUser === true && sanitizeInput($("select#fleetSrp option:selected").val()) === "Yes") {
                 $(".fleetpings-create-srp-link").show("fast")
             }
         } else {
-            $("input#prePing").prop("checked", true).removeAttr("disabled");
+            $("input#prePing").prop("checked", true);
             $("input#formupTime").removeAttr("disabled");
             if (fleetpingsSettings.optimerInstalled === true) {
                 $(".fleetpings-create-optimer").show("fast")
             }
             if (fleetpingsSettings.srpModuleAvailableToUser === true) {
-                $("input#createSrpLink").removeAttr("checked");
+                $("input#createSrpLink").prop("checked", false);
                 $(".fleetpings-create-srp-link").hide("fast")
             }
         }
     });
     $("button#createPingText").on("click", function() {
-        var fleetSrp = sanitizeInput($("select#fleetSrp option:selected").val());
-        var fleetName = sanitizeInput($("input#fleetName").val());
-        var fleetDoctrine = sanitizeInput($("input#fleetDoctrine").val());
-        if ($("input#createSrpLink").is(":checked") && $("input#formupTimeNow").is(":checked")) {
-            var srpAjaxUrl = fleetpingsSettings.srpAjaxUrl;
-            var srpCode = "";
+        const fleetName = sanitizeInput($("input#fleetName").val());
+        const fleetDoctrine = sanitizeInput($("input#fleetDoctrine").val());
+        const checkboxCreateSrpLink = $("input#createSrpLink");
+        const checkboxFormupTimeNow = $("input#formupTimeNow");
+        if (checkboxCreateSrpLink.is(":checked") && checkboxFormupTimeNow.is(":checked")) {
+            const srpAjaxUrl = fleetpingsSettings.srpAjaxUrl;
+            let srpCode = "";
             $.ajax({
                 url: srpAjaxUrl,
                 type: "post",
                 data: {
                     fleet_doctrine: fleetDoctrine,
                     fleet_name: fleetName
                 },
@@ -382,15 +379,15 @@
                     "X-CSRFToken": sanitizeInput($('input[name="csrfmiddlewaretoken"]').val())
                 }
             }).done(function(result) {
                 srpCode = result.srp_code;
                 generateFleetPing(srpCode);
                 showSuccess(fleetpingsTranslations.srp.created, ".fleetpings-create-srp-link-message")
             });
-            $("input#createSrpLink").removeAttr("checked")
+            checkboxCreateSrpLink.prop("checked", false)
         } else {
             generateFleetPing("")
         }
         return false
     });
     $("button#copyFleetPing").on("click", function() {
         copyFleetPing()
```

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/createOptimer.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/createOptimer.html`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/createSrpLink.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/createSrpLink.html`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/fleetComms.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/fleetComms.html`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/fleetDoctrine.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/fleetDoctrine.html`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/fleetType.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/fleetType.html`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/formupLocation.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/formupLocation.html`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/formupTime.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/formupTime.html`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/pingChannel.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/pingChannel.html`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form/pingTargets.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form/pingTargets.html`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/form.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/form.html`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         <div class="col-md-4">
             <button id="createPingText" name="createPingText" class="btn btn-primary">{% translate "Create Ping" %}</button>
         </div>
     </div>
 </fieldset>
 
 <script type="application/javascript">
-    var fleetpingsSettings = {
+    const fleetpingsSettings = {
         platformUsed: '{{ platform_used }}',
         timezonesInstalled: {{ timezones_installed|yesno:"true,false" }},
         optimerInstalled: {{ optimer_installed|yesno:"true,false" }},
         srpModuleAvailableToUser: {{ srp_module_available_to_user|yesno:"true,false" }},
         useNewTimezoneLinks: {{ use_new_timezone_links|yesno:"true,false" }},
         siteUrl: '{{ site_url }}/',
         pingCreator: '{{ main_character|safe|addslashes }}',
```

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/index.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% extends 'fleetpings/base.html' %}
 
 {% load i18n %}
-{% load static %}
+{% load fleetpings_versioned_static %}
 
 {% block details %}
     <div class="aa-fleetpings row">
         <div class="col-md-6">
             <div class="panel panel-default">
                 <div class="panel-heading aa-fleetpings-ping-header">
                     <span class="panel-title">{% translate "Fleet Information" %}</span>
@@ -24,15 +24,15 @@
                 <div class="panel-body">
                     {% include 'fleetpings/ping.html' %}
                 </div>
             </div>
         </div>
 
         <script type="application/javascript">
-            var fleetpingsTranslations = {
+            const fleetpingsTranslations = {
                 ping: {
                     success: '{% blocktrans context "%(platform_used)s is a variable that holds the current used platform. It can be either Slack or Discord. Do not translate it, just use it as it is." %}Success! Your ping has been sent to your {{ platform_used }}.{% endblocktrans %}'
                 },
                 optimer: {
                     created: '{% translate 'Fleet operations timer has been created ...' %}'
                 },
                 srp: {
@@ -47,25 +47,24 @@
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/jquery-datetimepicker-js.html' %}
     {% include 'bundles/clipboard-js.html' %}
 
-    <script type="application/javascript" src="{% static 'fleetpings/js/fleetpings.min.js' %}"></script>
+    <script type="application/javascript" src="{% fleetpings_static 'fleetpings/js/fleetpings.min.js' %}"></script>
+    <script type="application/javascript">
+        $('#formupTime').datetimepicker({
+            lang: '{{ LANGUAGE_CODE }}',
+            maskInput: true,
+            format: 'Y-m-d H:i',
+            dayOfWeekStart: 1,
+            step: 15
+        });
+    </script>
 {% endblock %}
 
 {% block extra_css %}
-    <link rel="stylesheet" type="text/css" href="{% static 'fleetpings/css/fleetpings.min.css' %}">
+    <link rel="stylesheet" type="text/css" href="{% fleetpings_static 'fleetpings/css/fleetpings.min.css' %}">
 
     {% include 'bundles/jquery-datetimepicker-css.html' %}
 {% endblock %}
-
-{% block extra_script %}
-    $('#formupTime').datetimepicker({
-        lang: '{{ LANGUAGE_CODE }}',
-        maskInput: true,
-        format: 'Y-m-d H:i',
-        dayOfWeekStart: 1,
-        step: 15
-    });
-{% endblock extra_script %}
```

#### html2text {}

```diff
@@ -1,13 +1,10 @@
-{% extends 'fleetpings/base.html' %} {% load i18n %} {% load static %} {% block
-details %}
+{% extends 'fleetpings/base.html' %} {% load i18n %} {% load
+fleetpings_versioned_static %} {% block details %}
 {% translate "Fleet Information" %}
 {% include "fleetpings/form.html" %}
 {% translate "Formatted Ping Text" %}
 {% include 'fleetpings/ping.html' %}
 {% endblock %} {% block extra_javascript %} {% include 'bundles/jquery-
 datetimepicker-js.html' %} {% include 'bundles/clipboard-js.html' %}
  {% endblock %} {% block extra_css %}
- {% include 'bundles/jquery-datetimepicker-css.html' %} {% endblock %} {% block
-extra_script %} $('#formupTime').datetimepicker({ lang: '{{ LANGUAGE_CODE }}',
-maskInput: true, format: 'Y-m-d H:i', dayOfWeekStart: 1, step: 15 }); {%
-endblock extra_script %}
+ {% include 'bundles/jquery-datetimepicker-css.html' %} {% endblock %}
```

### Comparing `aa-fleetpings-2.8.0/fleetpings/templates/fleetpings/ping.html` & `aa-fleetpings-2.9.0/fleetpings/templates/fleetpings/ping.html`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/tests/test_access.py` & `aa-fleetpings-2.9.0/fleetpings/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/tests/test_installed_modules.py` & `aa-fleetpings-2.9.0/fleetpings/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/tests/utils.py` & `aa-fleetpings-2.9.0/fleetpings/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/utils.py` & `aa-fleetpings-2.9.0/fleetpings/utils.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/fleetpings/views.py` & `aa-fleetpings-2.9.0/fleetpings/views.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/setup.py` & `aa-fleetpings-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/testauth/celery.py` & `aa-fleetpings-2.9.0/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-fleetpings-2.8.0/testauth/settings.py` & `aa-fleetpings-2.9.0/testauth/settings.py`

 * *Files identical despite different names*

