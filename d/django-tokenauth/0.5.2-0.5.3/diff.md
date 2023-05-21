# Comparing `tmp/django-tokenauth-0.5.2.tar.gz` & `tmp/django-tokenauth-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tokenauth-0.5.2.tar", last modified: Sat Nov 13 01:04:23 2021, max compression
+gzip compressed data, was "django-tokenauth-0.5.3.tar", last modified: Sun May 21 17:19:06 2023, max compression
```

## Comparing `django-tokenauth-0.5.2.tar` & `django-tokenauth-0.5.3.tar`

### file list

```diff
@@ -1,41 +1,35 @@
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2021-11-13 01:04:23.329911 django-tokenauth-0.5.2/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     6123 2018-03-31 01:50:21.000000 django-tokenauth-0.5.2/.gitchangelog.rc
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       81 2018-03-31 01:50:21.000000 django-tokenauth-0.5.2/.gitignore
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      550 2020-01-07 13:12:24.000000 django-tokenauth-0.5.2/.pre-commit-config.yaml
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      340 2020-05-08 21:32:53.000000 django-tokenauth-0.5.2/.travis.yml
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     2578 2021-11-13 01:03:47.000000 django-tokenauth-0.5.2/CHANGELOG.md
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     1481 2018-03-31 01:50:21.000000 django-tokenauth-0.5.2/LICENSE
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       72 2018-03-31 01:50:21.000000 django-tokenauth-0.5.2/MANIFEST.in
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      496 2021-11-13 01:04:23.329911 django-tokenauth-0.5.2/PKG-INFO
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     6197 2021-06-12 13:03:27.000000 django-tokenauth-0.5.2/README.md
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2021-11-13 01:04:23.328910 django-tokenauth-0.5.2/django_tokenauth.egg-info/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      496 2021-11-13 01:04:23.000000 django-tokenauth-0.5.2/django_tokenauth.egg-info/PKG-INFO
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      935 2021-11-13 01:04:23.000000 django-tokenauth-0.5.2/django_tokenauth.egg-info/SOURCES.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2021-11-13 01:04:23.000000 django-tokenauth-0.5.2/django_tokenauth.egg-info/dependency_links.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2021-06-26 13:07:26.000000 django-tokenauth-0.5.2/django_tokenauth.egg-info/not-zip-safe
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       10 2021-11-13 01:04:23.000000 django-tokenauth-0.5.2/django_tokenauth.egg-info/top_level.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      340 2021-11-13 01:04:23.329911 django-tokenauth-0.5.2/setup.cfg
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      825 2019-11-17 18:48:02.000000 django-tokenauth-0.5.2/setup.py
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2021-11-13 01:04:23.328910 django-tokenauth-0.5.2/tokenauth/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       22 2021-11-13 01:04:11.000000 django-tokenauth-0.5.2/tokenauth/__init__.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      385 2021-06-12 12:57:37.000000 django-tokenauth-0.5.2/tokenauth/admin.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       93 2019-11-17 18:46:43.000000 django-tokenauth-0.5.2/tokenauth/apps.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     1559 2020-01-07 13:04:37.000000 django-tokenauth-0.5.2/tokenauth/auth_backends.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     1441 2021-06-12 12:54:58.000000 django-tokenauth-0.5.2/tokenauth/helpers.py
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2021-11-13 01:04:23.329911 django-tokenauth-0.5.2/tokenauth/migrations/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      817 2019-11-17 18:46:43.000000 django-tokenauth-0.5.2/tokenauth/migrations/0001_initial.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      398 2019-11-17 18:46:43.000000 django-tokenauth-0.5.2/tokenauth/migrations/0002_authtoken_next_url.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      568 2019-11-17 19:55:44.000000 django-tokenauth-0.5.2/tokenauth/migrations/0003_authtoken_new_email.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      805 2021-06-12 12:59:07.000000 django-tokenauth-0.5.2/tokenauth/migrations/0004_add_email_log.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)        0 2018-03-31 01:50:21.000000 django-tokenauth-0.5.2/tokenauth/migrations/__init__.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     2077 2021-06-12 12:55:41.000000 django-tokenauth-0.5.2/tokenauth/models.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     1479 2021-06-12 12:58:39.000000 django-tokenauth-0.5.2/tokenauth/settings.py
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2021-11-13 01:04:23.329911 django-tokenauth-0.5.2/tokenauth/templates/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      317 2019-11-17 19:52:27.000000 django-tokenauth-0.5.2/tokenauth/templates/tokenauth_change_body.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       41 2019-11-17 19:50:21.000000 django-tokenauth-0.5.2/tokenauth/templates/tokenauth_change_subject.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      491 2020-03-11 17:13:34.000000 django-tokenauth-0.5.2/tokenauth/templates/tokenauth_login_body.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       15 2020-01-07 13:03:25.000000 django-tokenauth-0.5.2/tokenauth/templates/tokenauth_login_subject.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       68 2019-11-17 18:47:49.000000 django-tokenauth-0.5.2/tokenauth/tests.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      278 2019-11-17 18:46:43.000000 django-tokenauth-0.5.2/tokenauth/urls.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     5163 2021-11-13 01:02:56.000000 django-tokenauth-0.5.2/tokenauth/views.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      241 2020-05-08 21:32:15.000000 django-tokenauth-0.5.2/tox.ini
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2023-05-21 17:19:06.524974 django-tokenauth-0.5.3/
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     1481 2018-03-31 01:50:21.000000 django-tokenauth-0.5.3/LICENSE
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       72 2018-03-31 01:50:21.000000 django-tokenauth-0.5.3/MANIFEST.in
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      477 2023-05-21 17:19:06.524974 django-tokenauth-0.5.3/PKG-INFO
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     6197 2021-06-12 13:03:27.000000 django-tokenauth-0.5.3/README.md
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2023-05-21 17:19:06.520974 django-tokenauth-0.5.3/django_tokenauth.egg-info/
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      477 2023-05-21 17:19:06.000000 django-tokenauth-0.5.3/django_tokenauth.egg-info/PKG-INFO
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      850 2023-05-21 17:19:06.000000 django-tokenauth-0.5.3/django_tokenauth.egg-info/SOURCES.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2023-05-21 17:19:06.000000 django-tokenauth-0.5.3/django_tokenauth.egg-info/dependency_links.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2023-05-21 17:19:06.000000 django-tokenauth-0.5.3/django_tokenauth.egg-info/not-zip-safe
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       10 2023-05-21 17:19:06.000000 django-tokenauth-0.5.3/django_tokenauth.egg-info/top_level.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      340 2023-05-21 17:19:06.524974 django-tokenauth-0.5.3/setup.cfg
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      825 2019-11-17 18:48:02.000000 django-tokenauth-0.5.3/setup.py
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2023-05-21 17:19:06.520974 django-tokenauth-0.5.3/tokenauth/
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       22 2023-05-21 17:18:29.000000 django-tokenauth-0.5.3/tokenauth/__init__.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      385 2021-06-12 12:57:37.000000 django-tokenauth-0.5.3/tokenauth/admin.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       93 2019-11-17 18:46:43.000000 django-tokenauth-0.5.3/tokenauth/apps.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     1559 2020-01-07 13:04:37.000000 django-tokenauth-0.5.3/tokenauth/auth_backends.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     1441 2021-06-12 12:54:58.000000 django-tokenauth-0.5.3/tokenauth/helpers.py
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2023-05-21 17:19:06.520974 django-tokenauth-0.5.3/tokenauth/migrations/
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      817 2019-11-17 18:46:43.000000 django-tokenauth-0.5.3/tokenauth/migrations/0001_initial.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      398 2019-11-17 18:46:43.000000 django-tokenauth-0.5.3/tokenauth/migrations/0002_authtoken_next_url.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      568 2019-11-17 19:55:44.000000 django-tokenauth-0.5.3/tokenauth/migrations/0003_authtoken_new_email.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      805 2021-06-12 12:59:07.000000 django-tokenauth-0.5.3/tokenauth/migrations/0004_add_email_log.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)        0 2018-03-31 01:50:21.000000 django-tokenauth-0.5.3/tokenauth/migrations/__init__.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     2077 2021-06-12 12:55:41.000000 django-tokenauth-0.5.3/tokenauth/models.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     1479 2021-06-12 12:58:39.000000 django-tokenauth-0.5.3/tokenauth/settings.py
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2023-05-21 17:19:06.520974 django-tokenauth-0.5.3/tokenauth/templates/
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      317 2019-11-17 19:52:27.000000 django-tokenauth-0.5.3/tokenauth/templates/tokenauth_change_body.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       41 2019-11-17 19:50:21.000000 django-tokenauth-0.5.3/tokenauth/templates/tokenauth_change_subject.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      562 2023-05-21 17:17:12.000000 django-tokenauth-0.5.3/tokenauth/templates/tokenauth_login_body.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       15 2020-01-07 13:03:25.000000 django-tokenauth-0.5.3/tokenauth/templates/tokenauth_login_subject.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       68 2019-11-17 18:47:49.000000 django-tokenauth-0.5.3/tokenauth/tests.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      278 2019-11-17 18:46:43.000000 django-tokenauth-0.5.3/tokenauth/urls.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     5163 2021-11-13 01:02:56.000000 django-tokenauth-0.5.3/tokenauth/views.py
```

### Comparing `django-tokenauth-0.5.2/LICENSE` & `django-tokenauth-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tokenauth-0.5.2/README.md` & `django-tokenauth-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `django-tokenauth-0.5.2/setup.py` & `django-tokenauth-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-tokenauth-0.5.2/tokenauth/auth_backends.py` & `django-tokenauth-0.5.3/tokenauth/auth_backends.py`

 * *Files identical despite different names*

### Comparing `django-tokenauth-0.5.2/tokenauth/helpers.py` & `django-tokenauth-0.5.3/tokenauth/helpers.py`

 * *Files identical despite different names*

### Comparing `django-tokenauth-0.5.2/tokenauth/migrations/0001_initial.py` & `django-tokenauth-0.5.3/tokenauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tokenauth-0.5.2/tokenauth/migrations/0003_authtoken_new_email.py` & `django-tokenauth-0.5.3/tokenauth/migrations/0003_authtoken_new_email.py`

 * *Files identical despite different names*

### Comparing `django-tokenauth-0.5.2/tokenauth/migrations/0004_add_email_log.py` & `django-tokenauth-0.5.3/tokenauth/migrations/0004_add_email_log.py`

 * *Files identical despite different names*

### Comparing `django-tokenauth-0.5.2/tokenauth/models.py` & `django-tokenauth-0.5.3/tokenauth/models.py`

 * *Files identical despite different names*

### Comparing `django-tokenauth-0.5.2/tokenauth/settings.py` & `django-tokenauth-0.5.3/tokenauth/settings.py`

 * *Files identical despite different names*

### Comparing `django-tokenauth-0.5.2/tokenauth/views.py` & `django-tokenauth-0.5.3/tokenauth/views.py`

 * *Files identical despite different names*

