# Comparing `tmp/aa-inactivity-0.1.0a6.tar.gz` & `tmp/aa-inactivity-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-inactivity-0.1.0a6.tar", last modified: Sun Aug  7 15:47:32 2022, max compression
+gzip compressed data, was "aa-inactivity-0.1.0a7.tar", last modified: Sun May 21 19:45:45 2023, max compression
```

## Comparing `aa-inactivity-0.1.0a6.tar` & `aa-inactivity-0.1.0a7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.844793 aa-inactivity-0.1.0a6/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3160 2022-08-07 15:47:32.844793 aa-inactivity-0.1.0a6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2232 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.831792 aa-inactivity-0.1.0a6/aa_inactivity.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3160 2022-08-07 15:47:32.000000 aa-inactivity-0.1.0a6/aa_inactivity.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1589 2022-08-07 15:47:32.000000 aa-inactivity-0.1.0a6/aa_inactivity.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-07 15:47:32.000000 aa-inactivity-0.1.0a6/aa_inactivity.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      154 2022-08-07 15:47:32.000000 aa-inactivity-0.1.0a6/aa_inactivity.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-08-07 15:47:32.000000 aa-inactivity-0.1.0a6/aa_inactivity.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.835792 aa-inactivity-0.1.0a6/inactivity/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1355 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.837792 aa-inactivity-0.1.0a6/inactivity/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5732 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/migrations/0002_add_manage_leave_perm.py
--rw-rw-rw-   0 root         (0) root         (0)     4251 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/migrations/0003_add_webhooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/migrations/0004_django4_update.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7432 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.825791 aa-inactivity-0.1.0a6/inactivity/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.826791 aa-inactivity-0.1.0a6/inactivity/static/inactivity/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.838792 aa-inactivity-0.1.0a6/inactivity/static/inactivity/css/
--rw-rw-rw-   0 root         (0) root         (0)      291 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/static/inactivity/css/aa-bootstrap-fix.css
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/static/inactivity/css/aa-bootstrap-fix.min.css
--rw-rw-rw-   0 root         (0) root         (0)     2497 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/static/inactivity/css/inactivity.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.838792 aa-inactivity-0.1.0a6/inactivity/static/inactivity/images/
--rw-rw-rw-   0 root         (0) root         (0)    43262 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif
--rw-rw-rw-   0 root         (0) root         (0)    43381 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.839792 aa-inactivity-0.1.0a6/inactivity/static/inactivity/js/
--rw-rw-rw-   0 root         (0) root         (0)     2107 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/static/inactivity/js/loa_request_list.js
--rw-rw-rw-   0 root         (0) root         (0)     2565 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/static/inactivity/js/pending_loa_request_list.js
--rw-rw-rw-   0 root         (0) root         (0)     3265 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.826791 aa-inactivity-0.1.0a6/inactivity/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.841793 aa-inactivity-0.1.0a6/inactivity/templates/inactivity/
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/templates/inactivity/base.html
--rw-rw-rw-   0 root         (0) root         (0)     1916 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/templates/inactivity/create_loa.html
--rw-rw-rw-   0 root         (0) root         (0)     2103 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/templates/inactivity/index.html
--rw-rw-rw-   0 root         (0) root         (0)     2148 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/templates/inactivity/manage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.841793 aa-inactivity-0.1.0a6/inactivity/templates/inactivity/modals/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/templates/inactivity/modals/modal_dialog.html
--rw-rw-rw-   0 root         (0) root         (0)     1275 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/templates/inactivity/modals/view_request_content.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.843793 aa-inactivity-0.1.0a6/inactivity/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3480 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      882 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5109 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/inactivity/views.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2022-08-07 15:47:32.845793 aa-inactivity-0.1.0a6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1717 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 15:47:32.844793 aa-inactivity-0.1.0a6/testauth/
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/testauth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/testauth/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    10000 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/testauth/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/testauth/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2022-08-07 15:47:22.000000 aa-inactivity-0.1.0a6/testauth/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.090696 aa-inactivity-0.1.0a7/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3160 2023-05-21 19:45:45.090696 aa-inactivity-0.1.0a7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2232 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.082696 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3160 2023-05-21 19:45:45.000000 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-21 19:45:45.000000 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 19:45:45.000000 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-21 19:45:45.000000 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-21 19:45:45.000000 aa-inactivity-0.1.0a7/aa_inactivity.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.084696 aa-inactivity-0.1.0a7/inactivity/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.085696 aa-inactivity-0.1.0a7/inactivity/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5731 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/migrations/0002_add_manage_leave_perm.py
+-rw-rw-rw-   0 root         (0) root         (0)     4250 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/migrations/0003_add_webhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/migrations/0004_django4_update.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7431 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.079696 aa-inactivity-0.1.0a7/inactivity/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.080696 aa-inactivity-0.1.0a7/inactivity/static/inactivity/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.086696 aa-inactivity-0.1.0a7/inactivity/static/inactivity/css/
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/css/aa-bootstrap-fix.css
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/css/aa-bootstrap-fix.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     2497 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/css/inactivity.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.086696 aa-inactivity-0.1.0a7/inactivity/static/inactivity/images/
+-rw-rw-rw-   0 root         (0) root         (0)    43262 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif
+-rw-rw-rw-   0 root         (0) root         (0)    43381 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.087696 aa-inactivity-0.1.0a7/inactivity/static/inactivity/js/
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/js/loa_request_list.js
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/static/inactivity/js/pending_loa_request_list.js
+-rw-rw-rw-   0 root         (0) root         (0)     3265 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.080696 aa-inactivity-0.1.0a7/inactivity/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.088696 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     1985 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/create_loa.html
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     2148 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/manage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.088696 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/modals/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/modals/modal_dialog.html
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/templates/inactivity/modals/view_request_content.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.089696 aa-inactivity-0.1.0a7/inactivity/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/tests/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5107 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/inactivity/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-21 19:45:45.090696 aa-inactivity-0.1.0a7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:45:45.090696 aa-inactivity-0.1.0a7/testauth/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/testauth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/testauth/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)    10000 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/testauth/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/testauth/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-05-21 19:45:36.000000 aa-inactivity-0.1.0a7/testauth/wsgi.py
```

### Comparing `aa-inactivity-0.1.0a6/LICENSE` & `aa-inactivity-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/PKG-INFO` & `aa-inactivity-0.1.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-inactivity
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Activity monitoring app for Alliance Auth
 Home-page: https://gitlab.com/eclipse-expeditions/aa-inactivity
 Author: Rebecca Murphy
 Author-email: rebecca@rcmurphy.me
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `aa-inactivity-0.1.0a6/README.md` & `aa-inactivity-0.1.0a7/README.md`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/aa_inactivity.egg-info/PKG-INFO` & `aa-inactivity-0.1.0a7/aa_inactivity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-inactivity
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Activity monitoring app for Alliance Auth
 Home-page: https://gitlab.com/eclipse-expeditions/aa-inactivity
 Author: Rebecca Murphy
 Author-email: rebecca@rcmurphy.me
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `aa-inactivity-0.1.0a6/aa_inactivity.egg-info/SOURCES.txt` & `aa-inactivity-0.1.0a7/aa_inactivity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/admin.py` & `aa-inactivity-0.1.0a7/inactivity/admin.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/auth_hooks.py` & `aa-inactivity-0.1.0a7/inactivity/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/migrations/0001_initial.py` & `aa-inactivity-0.1.0a7/inactivity/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("authentication", "0017_remove_fleetup_permission"),
         ("auth", "0012_alter_user_first_name_max_length"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
```

### Comparing `aa-inactivity-0.1.0a6/inactivity/migrations/0002_add_manage_leave_perm.py` & `aa-inactivity-0.1.0a7/inactivity/migrations/0002_add_manage_leave_perm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.1.2 on 2021-01-18 01:50
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("inactivity", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="general",
```

### Comparing `aa-inactivity-0.1.0a6/inactivity/migrations/0003_add_webhooks.py` & `aa-inactivity-0.1.0a7/inactivity/migrations/0003_add_webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import multiselectfield.db.fields
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("auth", "0012_alter_user_first_name_max_length"),
         ("authentication", "0017_remove_fleetup_permission"),
         ("inactivity", "0002_add_manage_leave_perm"),
     ]
 
     operations = [
```

### Comparing `aa-inactivity-0.1.0a6/inactivity/migrations/0004_django4_update.py` & `aa-inactivity-0.1.0a7/inactivity/migrations/0004_django4_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.0.3 on 2022-03-03 13:09
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("auth", "0012_alter_user_first_name_max_length"),
         ("authentication", "0017_remove_fleetup_permission"),
         ("inactivity", "0003_add_webhooks"),
     ]
 
     operations = [
```

### Comparing `aa-inactivity-0.1.0a6/inactivity/models.py` & `aa-inactivity-0.1.0a7/inactivity/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,14 @@
         for config in InactivityPingConfig.objects.all():
             if config.is_applicable_to(self.user):
                 configs.append(config)
         webhooks = Webhook.objects.filter(
             Q(ping_configs__in=configs) | Q(ping_configs=None), Q(is_active=True)
         )
         if self._state.adding:
-
             for webhook in webhooks:
                 if str(Webhook.NOTIFICATION_TYPE_LOA_NEW) in webhook.notification_types:
                     if webhook.webhook_type == Webhook.WEBHOOK_TYPE_DISCORD:
                         hook = dhooks_lite.Webhook(webhook.url)
                         hook.execute(
                             "**%(user_name)s** has submitted a new leave of absence from **%(start)s** to **%(end)s**"
                             % {
```

### Comparing `aa-inactivity-0.1.0a6/inactivity/static/inactivity/css/inactivity.css` & `aa-inactivity-0.1.0a7/inactivity/static/inactivity/css/inactivity.css`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif` & `aa-inactivity-0.1.0a7/inactivity/static/inactivity/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif` & `aa-inactivity-0.1.0a7/inactivity/static/inactivity/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/static/inactivity/js/loa_request_list.js` & `aa-inactivity-0.1.0a7/inactivity/static/inactivity/js/loa_request_list.js`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/static/inactivity/js/pending_loa_request_list.js` & `aa-inactivity-0.1.0a7/inactivity/static/inactivity/js/pending_loa_request_list.js`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/tasks.py` & `aa-inactivity-0.1.0a7/inactivity/tasks.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/templates/inactivity/create_loa.html` & `aa-inactivity-0.1.0a7/inactivity/templates/inactivity/create_loa.html`

 * *Files 16% similar despite different names*

```diff
@@ -37,16 +37,19 @@
 
 </script>
 <script type="application/javascript" src="{% static 'inactivity/js/loa_request_list.js' %}" ></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/jqueryui/1.12.1/jquery-ui.min.js" integrity="sha512-uto9mlQzrs59VwILcLiRYeLKPPbS/bT71da/OEBYEwcdNUk8jYIy+D176RYoop1Da+f9mvkYrmj5MCLZWEtQuA==" crossorigin="anonymous"></script>
 
   <script>
   $( function() {
-    $( "#id_start" ).datepicker();
-    $( "#id_end" ).datepicker();
+    let params = {
+        dateFormat: "yy-mm-dd"
+    };
+    $( "#id_start" ).datepicker(params);
+    $( "#id_end" ).datepicker(params);
   } );
   </script>
 {% endblock %}
 
 {% block extra_css %}
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/jqueryui/1.12.1/jquery-ui.min.css"  type="text/css">
 {% endblock %}
```

### Comparing `aa-inactivity-0.1.0a6/inactivity/templates/inactivity/index.html` & `aa-inactivity-0.1.0a7/inactivity/templates/inactivity/index.html`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/templates/inactivity/manage.html` & `aa-inactivity-0.1.0a7/inactivity/templates/inactivity/manage.html`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/templates/inactivity/modals/modal_dialog.html` & `aa-inactivity-0.1.0a7/inactivity/templates/inactivity/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/templates/inactivity/modals/view_request_content.html` & `aa-inactivity-0.1.0a7/inactivity/templates/inactivity/modals/view_request_content.html`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/tests/factories.py` & `aa-inactivity-0.1.0a7/inactivity/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/tests/test_models.py` & `aa-inactivity-0.1.0a7/inactivity/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/tests/test_tasks.py` & `aa-inactivity-0.1.0a7/inactivity/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/urls.py` & `aa-inactivity-0.1.0a7/inactivity/urls.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/inactivity/views.py` & `aa-inactivity-0.1.0a7/inactivity/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,21 @@
 from .forms import CreateRequestForm
 from .models import LeaveOfAbsence
 
 
 @login_required
 @permission_required("inactivity.basic_access")
 def index(request):
-
     context = {}
     return render(request, "inactivity/index.html", context)
 
 
 @login_required
 @permission_required("inactivity.manage_leave")
 def manage(request):
-
     context = {}
     return render(request, "inactivity/manage.html", context)
 
 
 def convert_loa(loa: LeaveOfAbsence) -> dict:
     return {
         "user": loa.user.profile.main_character.character_name,
```

### Comparing `aa-inactivity-0.1.0a6/setup.py` & `aa-inactivity-0.1.0a7/setup.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/testauth/celery.py` & `aa-inactivity-0.1.0a7/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-inactivity-0.1.0a6/testauth/settings.py` & `aa-inactivity-0.1.0a7/testauth/settings.py`

 * *Files identical despite different names*

