# Comparing `tmp/kiwitcms-github-marketplace-2.3.2.tar.gz` & `tmp/kiwitcms-github-marketplace-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwitcms-github-marketplace-2.3.2.tar", last modified: Fri Apr 28 11:19:11 2023, max compression
+gzip compressed data, was "kiwitcms-github-marketplace-2.3.3.tar", last modified: Sun May 21 07:29:57 2023, max compression
```

## Comparing `kiwitcms-github-marketplace-2.3.2.tar` & `kiwitcms-github-marketplace-2.3.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.520529 kiwitcms-github-marketplace-2.3.2/
--rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.3.2/LICENSE
--rw-rw-r--   0 senko     (1001) senko     (1001)      208 2022-02-23 19:15:12.000000 kiwitcms-github-marketplace-2.3.2/MANIFEST.in
--rw-r--r--   0 senko     (1001) senko     (1001)    11146 2023-04-28 11:19:11.520529 kiwitcms-github-marketplace-2.3.2/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)    10377 2023-04-28 11:18:45.000000 kiwitcms-github-marketplace-2.3.2/README.rst
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.516529 kiwitcms-github-marketplace-2.3.2/kiwitcms_github_marketplace.egg-info/
--rw-r--r--   0 senko     (1001) senko     (1001)    11146 2023-04-28 11:19:11.000000 kiwitcms-github-marketplace-2.3.2/kiwitcms_github_marketplace.egg-info/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)     1909 2023-04-28 11:19:11.000000 kiwitcms-github-marketplace-2.3.2/kiwitcms_github_marketplace.egg-info/SOURCES.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-04-28 11:19:11.000000 kiwitcms-github-marketplace-2.3.2/kiwitcms_github_marketplace.egg-info/dependency_links.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       65 2023-04-28 11:19:11.000000 kiwitcms-github-marketplace-2.3.2/kiwitcms_github_marketplace.egg-info/entry_points.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-04-28 11:19:11.000000 kiwitcms-github-marketplace-2.3.2/kiwitcms_github_marketplace.egg-info/not-zip-safe
--rw-r--r--   0 senko     (1001) senko     (1001)       58 2023-04-28 11:19:11.000000 kiwitcms-github-marketplace-2.3.2/kiwitcms_github_marketplace.egg-info/requires.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       42 2023-04-28 11:19:11.000000 kiwitcms-github-marketplace-2.3.2/kiwitcms_github_marketplace.egg-info/top_level.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       58 2023-04-28 10:52:02.000000 kiwitcms-github-marketplace-2.3.2/requirements.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      129 2023-04-28 11:19:11.520529 kiwitcms-github-marketplace-2.3.2/setup.cfg
--rw-r--r--   0 senko     (1001) senko     (1001)     1684 2023-04-28 11:18:45.000000 kiwitcms-github-marketplace-2.3.2/setup.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.517529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     6031 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      321 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/apps.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      553 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/checks.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2613 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/docker.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      879 2022-02-21 15:47:58.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/mailchimp.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      374 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/menu.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.517529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/
--rw-rw-r--   0 senko     (1001) senko     (1001)     1532 2022-06-30 10:13:34.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0001_initial.py
--rw-r--r--   0 senko     (1001) senko     (1001)      965 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0002_update_fields.py
--rw-r--r--   0 senko     (1001) senko     (1001)      415 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0003_sender_email_field.py
--rw-r--r--   0 senko     (1001) senko     (1001)      391 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0004_models_jsonfield.py
--rw-r--r--   0 senko     (1001) senko     (1001)      613 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1039 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0006_add_subscription_field.py
--rw-r--r--   0 senko     (1001) senko     (1001)      694 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0007_manualpurchase.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1712 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/models.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.518529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/quay/
--rw-rw-r--   0 senko     (1001) senko     (1001)       57 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/quay/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2353 2022-02-09 21:44:26.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/quay/quay_api_client.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     4687 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/quay/quay_session.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.513529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/static/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.513529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/static/tcms_github_marketplace/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.518529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/static/tcms_github_marketplace/js/
--rw-rw-r--   0 senko     (1001) senko     (1001)      924 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.514529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.518529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/email/
--rw-r--r--   0 senko     (1001) senko     (1001)     1450 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/email/manual_subscription_notification.txt
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.518529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/tcms_github_marketplace/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.519529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/tcms_github_marketplace/email/
--rw-rw-r--   0 senko     (1001) senko     (1001)      270 2022-08-14 14:51:18.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/tcms_github_marketplace/email/exit_poll.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)    11048 2022-08-04 08:25:18.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.519529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/tcms_tenants/
--rw-rw-r--   0 senko     (1001) senko     (1001)     2562 2021-06-10 13:43:41.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/tcms_tenants/override_new.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.520529 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templatetags/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templatetags/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      373 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templatetags/github_marketplace.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      804 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/urls.py
--rw-r--r--   0 senko     (1001) senko     (1001)     5632 2023-04-28 11:18:45.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/utils.py
--rw-r--r--   0 senko     (1001) senko     (1001)    27800 2023-04-17 14:06:01.000000 kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/views.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-04-28 11:19:11.520529 kiwitcms-github-marketplace-2.3.2/tcms_settings_dir/
--rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.3.2/tcms_settings_dir/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.483153 kiwitcms-github-marketplace-2.3.3/
+-rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.3.3/LICENSE
+-rw-rw-r--   0 senko     (1001) senko     (1001)      208 2022-02-23 19:15:12.000000 kiwitcms-github-marketplace-2.3.3/MANIFEST.in
+-rw-r--r--   0 senko     (1001) senko     (1001)    11337 2023-05-21 07:29:57.483153 kiwitcms-github-marketplace-2.3.3/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)    10568 2023-05-21 07:29:18.000000 kiwitcms-github-marketplace-2.3.3/README.rst
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.480153 kiwitcms-github-marketplace-2.3.3/kiwitcms_github_marketplace.egg-info/
+-rw-r--r--   0 senko     (1001) senko     (1001)    11337 2023-05-21 07:29:57.000000 kiwitcms-github-marketplace-2.3.3/kiwitcms_github_marketplace.egg-info/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)     1909 2023-05-21 07:29:57.000000 kiwitcms-github-marketplace-2.3.3/kiwitcms_github_marketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-05-21 07:29:57.000000 kiwitcms-github-marketplace-2.3.3/kiwitcms_github_marketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       65 2023-05-21 07:29:57.000000 kiwitcms-github-marketplace-2.3.3/kiwitcms_github_marketplace.egg-info/entry_points.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-05-21 07:29:57.000000 kiwitcms-github-marketplace-2.3.3/kiwitcms_github_marketplace.egg-info/not-zip-safe
+-rw-r--r--   0 senko     (1001) senko     (1001)       50 2023-05-21 07:29:57.000000 kiwitcms-github-marketplace-2.3.3/kiwitcms_github_marketplace.egg-info/requires.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       42 2023-05-21 07:29:57.000000 kiwitcms-github-marketplace-2.3.3/kiwitcms_github_marketplace.egg-info/top_level.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       50 2023-05-21 07:29:18.000000 kiwitcms-github-marketplace-2.3.3/requirements.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)      129 2023-05-21 07:29:57.483153 kiwitcms-github-marketplace-2.3.3/setup.cfg
+-rw-r--r--   0 senko     (1001) senko     (1001)     1684 2023-05-21 07:29:18.000000 kiwitcms-github-marketplace-2.3.3/setup.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.481153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     6031 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/admin.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      321 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/apps.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      553 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/checks.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2613 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/docker.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      879 2022-02-21 15:47:58.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/mailchimp.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      374 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/menu.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.482153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/
+-rw-rw-r--   0 senko     (1001) senko     (1001)     1532 2022-06-30 10:13:34.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0001_initial.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      965 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0002_update_fields.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      415 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0003_sender_email_field.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      391 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0004_models_jsonfield.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      613 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1039 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0006_add_subscription_field.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      694 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0007_manualpurchase.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1712 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/models.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.482153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/quay/
+-rw-rw-r--   0 senko     (1001) senko     (1001)       57 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/quay/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2353 2022-02-09 21:44:26.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/quay/quay_api_client.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     4687 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/quay/quay_session.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.477153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/static/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.477153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/static/tcms_github_marketplace/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.482153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/static/tcms_github_marketplace/js/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      924 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.478153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.482153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/email/
+-rw-r--r--   0 senko     (1001) senko     (1001)     1450 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/email/manual_subscription_notification.txt
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.482153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/tcms_github_marketplace/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.482153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/tcms_github_marketplace/email/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      270 2022-08-14 14:51:18.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/tcms_github_marketplace/email/exit_poll.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)    11048 2022-08-04 08:25:18.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.483153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/tcms_tenants/
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2562 2021-06-10 13:43:41.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/tcms_tenants/override_new.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.483153 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templatetags/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templatetags/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      373 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templatetags/github_marketplace.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      804 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/urls.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     5632 2023-04-28 11:18:45.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/utils.py
+-rw-r--r--   0 senko     (1001) senko     (1001)    27901 2023-05-21 07:29:18.000000 kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/views.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-21 07:29:57.483153 kiwitcms-github-marketplace-2.3.3/tcms_settings_dir/
+-rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.3.3/tcms_settings_dir/__init__.py
```

### Comparing `kiwitcms-github-marketplace-2.3.2/LICENSE` & `kiwitcms-github-marketplace-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/PKG-INFO` & `kiwitcms-github-marketplace-2.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-github-marketplace
-Version: 2.3.2
+Version: 2.3.3
 Summary: GitHub Marketplace integration for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/github-marketplace/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Framework :: Django
@@ -79,14 +79,22 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.3.3 (21 May 2023)
+~~~~~~~~~~~~~~~~~~~~
+
+- Handle expiration of unpaid requests for add-on services
+- Unpin version for requests library to avoid potential conflicts
+  with other add-ons
+
+
 v2.3.2 (28 Apr 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Update requests from 2.28.2 to 2.29.0
 - Don't fail when trying to delete user after subscription has been cancelled
```

### Comparing `kiwitcms-github-marketplace-2.3.2/README.rst` & `kiwitcms-github-marketplace-2.3.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,22 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.3.3 (21 May 2023)
+~~~~~~~~~~~~~~~~~~~~
+
+- Handle expiration of unpaid requests for add-on services
+- Unpin version for requests library to avoid potential conflicts
+  with other add-ons
+
+
 v2.3.2 (28 Apr 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Update requests from 2.28.2 to 2.29.0
 - Don't fail when trying to delete user after subscription has been cancelled
```

### Comparing `kiwitcms-github-marketplace-2.3.2/kiwitcms_github_marketplace.egg-info/PKG-INFO` & `kiwitcms-github-marketplace-2.3.3/kiwitcms_github_marketplace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-github-marketplace
-Version: 2.3.2
+Version: 2.3.3
 Summary: GitHub Marketplace integration for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/github-marketplace/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Framework :: Django
@@ -79,14 +79,22 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.3.3 (21 May 2023)
+~~~~~~~~~~~~~~~~~~~~
+
+- Handle expiration of unpaid requests for add-on services
+- Unpin version for requests library to avoid potential conflicts
+  with other add-ons
+
+
 v2.3.2 (28 Apr 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Update requests from 2.28.2 to 2.29.0
 - Don't fail when trying to delete user after subscription has been cancelled
```

### Comparing `kiwitcms-github-marketplace-2.3.2/kiwitcms_github_marketplace.egg-info/SOURCES.txt` & `kiwitcms-github-marketplace-2.3.3/kiwitcms_github_marketplace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/setup.py` & `kiwitcms-github-marketplace-2.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 continue
             requires.append(line.strip())
         return requires
 
 
 setup(
     name="kiwitcms-github-marketplace",
-    version="2.3.2",
+    version="2.3.3",
     description="GitHub Marketplace integration for Kiwi TCMS",
     long_description=get_long_description(),
     author="Kiwi TCMS",
     author_email="info@kiwitcms.org",
     url="https://github.com/kiwitcms/github-marketplace/",
     license="GPLv3+",
     install_requires=get_install_requires("requirements.txt"),
```

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/admin.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/admin.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/checks.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/checks.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/docker.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/docker.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/mailchimp.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/mailchimp.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0001_initial.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0002_update_fields.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0002_update_fields.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0006_add_subscription_field.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0006_add_subscription_field.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/migrations/0007_manualpurchase.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/migrations/0007_manualpurchase.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/models.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/models.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/quay/quay_api_client.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/quay/quay_api_client.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/quay/quay_session.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/quay/quay_session.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/email/manual_subscription_notification.txt` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/email/manual_subscription_notification.txt`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/templates/tcms_tenants/override_new.html` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/templates/tcms_tenants/override_new.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/urls.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/urls.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/utils.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/utils.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.3.2/tcms_github_marketplace/views.py` & `kiwitcms-github-marketplace-2.3.3/tcms_github_marketplace/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,14 +414,16 @@
         elif (
             "items" in event["data"]
             and event["data"]["items"]
             and "subscription" in event["data"]["items"][0]
             and "intervalUnit" in event["data"]["items"][0]["subscription"]
         ):
             interval = event["data"]["items"][0]["subscription"]["intervalUnit"]
+        elif "additional-services-for-kiwi-tcms" in json.dumps(event):
+            return "one-time"
         else:
             raise RuntimeError("Cannot find billing cycle information")
 
         if interval == "month":
             return "monthly"
 
         if interval == "year":
```

