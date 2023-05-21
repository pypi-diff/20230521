# Comparing `tmp/dj-rest-auth-4.0.0.tar.gz` & `tmp/dj-rest-auth-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-rest-auth-4.0.0.tar", last modified: Sun May  7 05:38:10 2023, max compression
+gzip compressed data, was "dj-rest-auth-4.0.1.tar", last modified: Sun May 21 03:11:15 2023, max compression
```

## Comparing `dj-rest-auth-4.0.0.tar` & `dj-rest-auth-4.0.1.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.092239 dj-rest-auth-4.0.0/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.951946 dj-rest-auth-4.0.0/.circleci/
--rw-r--r--   0 michael    (501) staff       (20)     1057 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/.circleci/config.yml
--rw-r--r--   0 michael    (501) staff       (20)       45 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/.coveralls.yml
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.935868 dj-rest-auth-4.0.0/.github/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.953305 dj-rest-auth-4.0.0/.github/workflows/
--rw-r--r--   0 michael    (501) staff       (20)      352 2020-08-17 05:29:18.000000 dj-rest-auth-4.0.0/.github/workflows/main.yml
--rw-r--r--   0 michael    (501) staff       (20)      923 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/.github/workflows/stale.yml
--rw-r--r--   0 michael    (501) staff       (20)     1330 2020-11-17 22:42:53.000000 dj-rest-auth-4.0.0/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)       52 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/AUTHORS
--rw-r--r--   0 michael    (501) staff       (20)     1102 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)       89 2020-03-01 01:49:31.000000 dj-rest-auth-4.0.0/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     3458 2023-05-07 05:38:10.092425 dj-rest-auth-4.0.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     2815 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.954452 dj-rest-auth-4.0.0/demo/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.956159 dj-rest-auth-4.0.0/demo/demo/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/demo/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     3782 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/demo/settings.py
--rw-r--r--   0 michael    (501) staff       (20)     2313 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/demo/urls.py
--rw-r--r--   0 michael    (501) staff       (20)      385 2020-03-01 05:55:17.000000 dj-rest-auth-4.0.0/demo/demo/wsgi.py
--rwxr-xr-x   0 michael    (501) staff       (20)      247 2021-08-03 03:29:51.000000 dj-rest-auth-4.0.0/demo/manage.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.957790 dj-rest-auth-4.0.0/demo/react-spa/
--rw-r--r--   0 michael    (501) staff       (20)      310 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     2884 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/README.md
--rw-r--r--   0 michael    (501) staff       (20)      745 2020-03-28 16:41:49.000000 dj-rest-auth-4.0.0/demo/react-spa/package.json
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.962974 dj-rest-auth-4.0.0/demo/react-spa/public/
--rw-r--r--   0 michael    (501) staff       (20)     3150 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/favicon.ico
--rw-r--r--   0 michael    (501) staff       (20)     1721 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/index.html
--rw-r--r--   0 michael    (501) staff       (20)     5347 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/logo192.png
--rw-r--r--   0 michael    (501) staff       (20)     9664 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/logo512.png
--rw-r--r--   0 michael    (501) staff       (20)      492 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/manifest.json
--rw-r--r--   0 michael    (501) staff       (20)       67 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/public/robots.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.969612 dj-rest-auth-4.0.0/demo/react-spa/src/
--rw-r--r--   0 michael    (501) staff       (20)      594 2020-03-28 18:49:16.000000 dj-rest-auth-4.0.0/demo/react-spa/src/App.css
--rw-r--r--   0 michael    (501) staff       (20)     1770 2020-03-28 18:50:43.000000 dj-rest-auth-4.0.0/demo/react-spa/src/App.js
--rw-r--r--   0 michael    (501) staff       (20)      280 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/src/App.test.js
--rw-r--r--   0 michael    (501) staff       (20)      821 2020-03-28 18:49:40.000000 dj-rest-auth-4.0.0/demo/react-spa/src/index.css
--rw-r--r--   0 michael    (501) staff       (20)      503 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/src/index.js
--rw-r--r--   0 michael    (501) staff       (20)     2671 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/src/logo.svg
--rw-r--r--   0 michael    (501) staff       (20)     5086 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/src/serviceWorker.js
--rw-r--r--   0 michael    (501) staff       (20)      255 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.0/demo/react-spa/src/setupTests.js
--rw-r--r--   0 michael    (501) staff       (20)      234 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/requirements.pip
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.979474 dj-rest-auth-4.0.0/demo/templates/
--rw-r--r--   0 michael    (501) staff       (20)     4447 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/templates/base.html
--rw-r--r--   0 michael    (501) staff       (20)      188 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/email_verification.html
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.986713 dj-rest-auth-4.0.0/demo/templates/fragments/
--rw-r--r--   0 michael    (501) staff       (20)      652 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/email_verification_form.html
--rw-r--r--   0 michael    (501) staff       (20)      839 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/login_form.html
--rw-r--r--   0 michael    (501) staff       (20)      668 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/logout_form.html
--rw-r--r--   0 michael    (501) staff       (20)      908 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/password_change_form.html
--rw-r--r--   0 michael    (501) staff       (20)     1489 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/password_reset_confirm_form.html
--rw-r--r--   0 michael    (501) staff       (20)      579 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/password_reset_form.html
--rw-r--r--   0 michael    (501) staff       (20)      578 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/templates/fragments/resend_email_verification_form.html
--rw-r--r--   0 michael    (501) staff       (20)     1365 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/signup_form.html
--rw-r--r--   0 michael    (501) staff       (20)     1344 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/fragments/user_details_form.html
--rw-r--r--   0 michael    (501) staff       (20)      253 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/home.html
--rw-r--r--   0 michael    (501) staff       (20)      161 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/login.html
--rw-r--r--   0 michael    (501) staff       (20)      163 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/logout.html
--rw-r--r--   0 michael    (501) staff       (20)     1161 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/password_change.html
--rw-r--r--   0 michael    (501) staff       (20)      179 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/password_reset.html
--rw-r--r--   0 michael    (501) staff       (20)      724 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/password_reset_confirm.html
--rw-r--r--   0 michael    (501) staff       (20)      202 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/demo/templates/resend_email_verification.html
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.987344 dj-rest-auth-4.0.0/demo/templates/rest_framework/
--rw-r--r--   0 michael    (501) staff       (20)     1754 2020-06-20 18:56:14.000000 dj-rest-auth-4.0.0/demo/templates/rest_framework/api.html
--rw-r--r--   0 michael    (501) staff       (20)      163 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/signup.html
--rw-r--r--   0 michael    (501) staff       (20)     1915 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/demo/templates/user_details.html
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.995046 dj-rest-auth-4.0.0/dj_rest_auth/
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.0/dj_rest_auth/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.005155 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/
--rw-r--r--   0 michael    (501) staff       (20)      152 2021-07-11 17:17:01.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      149 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/admin.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1467 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2070 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/forms.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     5531 2023-01-02 22:42:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1044 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    11794 2023-01-02 22:42:47.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2854 2021-07-11 17:17:03.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1012 2021-07-11 17:17:03.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1255 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     9589 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      354 2023-05-07 05:37:31.000000 dj-rest-auth-4.0.0/dj_rest_auth/__version__.py
--rw-r--r--   0 michael    (501) staff       (20)       65 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.0/dj_rest_auth/admin.py
--rw-r--r--   0 michael    (501) staff       (20)     3075 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/app_settings.py
--rw-r--r--   0 michael    (501) staff       (20)     2785 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/forms.py
--rw-r--r--   0 michael    (501) staff       (20)     6282 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/jwt_auth.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.945448 dj-rest-auth-4.0.0/dj_rest_auth/locale/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.938603 dj-rest-auth-4.0.0/dj_rest_auth/locale/ar/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.005908 dj-rest-auth-4.0.0/dj_rest_auth/locale/ar/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3751 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.938960 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.011367 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:52:06.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!63502!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:54:59.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64462!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:55:51.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64600!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:56:43.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!64760!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:05:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65418!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65616!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65791!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!65995!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/.!69818!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2443 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3195 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.939300 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.015526 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65618!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65793!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!65997!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/.!69820!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2230 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2983 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.939643 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.019198 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65620!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65795!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!65999!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/.!69822!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2405 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3151 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.939964 dj-rest-auth-4.0.0/dj_rest_auth/locale/fa/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.019905 dj-rest-auth-4.0.0/dj_rest_auth/locale/fa/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3514 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.940310 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.023426 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!65622!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!65797!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!66001!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/.!69824!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3755 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     5257 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.940653 dj-rest-auth-4.0.0/dj_rest_auth/locale/hr/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.024511 dj-rest-auth-4.0.0/dj_rest_auth/locale/hr/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3091 2021-03-18 00:03:01.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.940983 dj-rest-auth-4.0.0/dj_rest_auth/locale/id/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.025495 dj-rest-auth-4.0.0/dj_rest_auth/locale/id/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     4954 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.941315 dj-rest-auth-4.0.0/dj_rest_auth/locale/it/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.027153 dj-rest-auth-4.0.0/dj_rest_auth/locale/it/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3001 2020-05-09 22:17:42.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3904 2020-05-09 22:17:42.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.941645 dj-rest-auth-4.0.0/dj_rest_auth/locale/ja/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.028117 dj-rest-auth-4.0.0/dj_rest_auth/locale/ja/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     5628 2020-12-04 02:36:07.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.941964 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.032200 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!65624!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!65799!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!66003!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/.!69826!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2562 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3296 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.942627 dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.033849 dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2958 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3524 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.942985 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.039305 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!65626!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!65801!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!66005!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/.!69828!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2265 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2992 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.943328 dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.041155 dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2317 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3090 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.943653 dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.043501 dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2979 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3537 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.943969 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.047702 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!65629!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!65804!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!66008!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/.!69831!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2773 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3508 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.944284 dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.049628 dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2565 2020-12-04 02:36:07.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3774 2020-12-04 02:36:07.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.944595 dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.051876 dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     2222 2020-04-27 03:53:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2920 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.944906 dj-rest-auth-4.0.0/dj_rest_auth/locale/uk/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.052642 dj-rest-auth-4.0.0/dj_rest_auth/locale/uk/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)     3502 2021-03-18 00:03:01.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.945244 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.056466 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65632!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65807!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!66011!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!69834!django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2243 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     3019 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.945581 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.060414 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65634!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65809!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!66013!django.mo
--rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!69836!django.mo
--rw-r--r--   0 michael    (501) staff       (20)      373 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0 michael    (501) staff       (20)     2337 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0 michael    (501) staff       (20)      948 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/models.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.064051 dj-rest-auth-4.0.0/dj_rest_auth/registration/
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.072013 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/
--rw-r--r--   0 michael    (501) staff       (20)      165 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      811 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     8838 2023-01-02 22:42:46.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)      747 2022-07-17 22:38:11.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     8336 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    10813 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/serializers.py
--rw-r--r--   0 michael    (501) staff       (20)     1299 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/urls.py
--rw-r--r--   0 michael    (501) staff       (20)     7732 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/registration/views.py
--rw-r--r--   0 michael    (501) staff       (20)    12700 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/serializers.py
--rw-r--r--   0 michael    (501) staff       (20)     2990 2021-05-17 04:45:09.000000 dj-rest-auth-4.0.0/dj_rest_auth/social_serializers.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.078326 dj-rest-auth-4.0.0/dj_rest_auth/tests/
--rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.084999 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/
--rw-r--r--   0 michael    (501) staff       (20)      158 2021-07-11 17:17:01.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     1793 2022-07-17 22:38:11.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     4196 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2461 2022-07-17 22:38:07.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)    27867 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     7032 2022-07-17 23:28:09.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     9113 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     5299 2022-07-17 22:38:10.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 michael    (501) staff       (20)     2420 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/django_urls.py
--rw-r--r--   0 michael    (501) staff       (20)     4012 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/mixins.py
--rw-r--r--   0 michael    (501) staff       (20)      140 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/requirements.pip
--rw-r--r--   0 michael    (501) staff       (20)     2833 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/settings.py
--rw-r--r--   0 michael    (501) staff       (20)    44032 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/test_api.py
--rw-r--r--   0 michael    (501) staff       (20)     7157 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/test_serializers.py
--rw-r--r--   0 michael    (501) staff       (20)    13998 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/test_social.py
--rw-r--r--   0 michael    (501) staff       (20)      289 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/test_utils.py
--rw-r--r--   0 michael    (501) staff       (20)     4541 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/urls.py
--rw-r--r--   0 michael    (501) staff       (20)     1031 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/tests/utils.py
--rw-r--r--   0 michael    (501) staff       (20)     1198 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/urls.py
--rw-r--r--   0 michael    (501) staff       (20)      541 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/dj_rest_auth/utils.py
--rw-r--r--   0 michael    (501) staff       (20)    10760 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.0/dj_rest_auth/views.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:09.997817 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     3458 2023-05-07 05:38:09.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     8029 2023-05-07 05:38:09.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-07 05:38:09.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2020-03-01 01:18:23.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/not-zip-safe
--rw-r--r--   0 michael    (501) staff       (20)       85 2023-05-07 05:38:09.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       13 2023-05-07 05:38:09.000000 dj-rest-auth-4.0.0/dj_rest_auth.egg-info/top_level.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-07 05:38:10.091574 dj-rest-auth-4.0.0/docs/
--rw-r--r--   0 michael    (501) staff       (20)     6786 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/docs/Makefile
--rw-r--r--   0 michael    (501) staff       (20)     3219 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/docs/api_endpoints.rst
--rw-r--r--   0 michael    (501) staff       (20)     8317 2020-05-09 22:29:21.000000 dj-rest-auth-4.0.0/docs/conf.py
--rw-r--r--   0 michael    (501) staff       (20)     9026 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/docs/configuration.rst
--rw-r--r--   0 michael    (501) staff       (20)      758 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/docs/demo.rst
--rw-r--r--   0 michael    (501) staff       (20)      497 2020-05-30 06:34:32.000000 dj-rest-auth-4.0.0/docs/disclosure.rst
--rw-r--r--   0 michael    (501) staff       (20)     3095 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/docs/faq.rst
--rw-r--r--   0 michael    (501) staff       (20)      754 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.0/docs/index.rst
--rw-r--r--   0 michael    (501) staff       (20)    11426 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/docs/installation.rst
--rw-r--r--   0 michael    (501) staff       (20)     1301 2020-08-10 01:03:45.000000 dj-rest-auth-4.0.0/docs/introduction.rst
--rw-r--r--   0 michael    (501) staff       (20)     6713 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.0/docs/make.bat
--rw-r--r--   0 michael    (501) staff       (20)      657 2021-03-17 23:58:28.000000 dj-rest-auth-4.0.0/runtests.py
--rw-r--r--   0 michael    (501) staff       (20)      474 2023-05-07 05:38:10.093057 dj-rest-auth-4.0.0/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1542 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/setup.py
--rw-r--r--   0 michael    (501) staff       (20)     1135 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.0/tox.ini
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.350633 dj-rest-auth-4.0.1/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.180193 dj-rest-auth-4.0.1/.circleci/
+-rw-r--r--   0 michael    (501) staff       (20)     1057 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/.circleci/config.yml
+-rw-r--r--   0 michael    (501) staff       (20)       45 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.1/.coveralls.yml
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.160278 dj-rest-auth-4.0.1/.github/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.181610 dj-rest-auth-4.0.1/.github/workflows/
+-rw-r--r--   0 michael    (501) staff       (20)      352 2020-08-17 05:29:18.000000 dj-rest-auth-4.0.1/.github/workflows/main.yml
+-rw-r--r--   0 michael    (501) staff       (20)      923 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/.github/workflows/stale.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1330 2020-11-17 22:42:53.000000 dj-rest-auth-4.0.1/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)       52 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.1/AUTHORS
+-rw-r--r--   0 michael    (501) staff       (20)     1102 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)       89 2020-03-01 01:49:31.000000 dj-rest-auth-4.0.1/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     3458 2023-05-21 03:11:15.350910 dj-rest-auth-4.0.1/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     2815 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.182646 dj-rest-auth-4.0.1/demo/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.184457 dj-rest-auth-4.0.1/demo/demo/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/demo/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3782 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/demo/demo/settings.py
+-rw-r--r--   0 michael    (501) staff       (20)     2313 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/demo/demo/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)      385 2020-03-01 05:55:17.000000 dj-rest-auth-4.0.1/demo/demo/wsgi.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      247 2021-08-03 03:29:51.000000 dj-rest-auth-4.0.1/demo/manage.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.185772 dj-rest-auth-4.0.1/demo/react-spa/
+-rw-r--r--   0 michael    (501) staff       (20)      310 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     2884 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/README.md
+-rw-r--r--   0 michael    (501) staff       (20)      745 2020-03-28 16:41:49.000000 dj-rest-auth-4.0.1/demo/react-spa/package.json
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.190796 dj-rest-auth-4.0.1/demo/react-spa/public/
+-rw-r--r--   0 michael    (501) staff       (20)     3150 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/public/favicon.ico
+-rw-r--r--   0 michael    (501) staff       (20)     1721 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/public/index.html
+-rw-r--r--   0 michael    (501) staff       (20)     5347 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/public/logo192.png
+-rw-r--r--   0 michael    (501) staff       (20)     9664 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/public/logo512.png
+-rw-r--r--   0 michael    (501) staff       (20)      492 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/public/manifest.json
+-rw-r--r--   0 michael    (501) staff       (20)       67 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/public/robots.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.196842 dj-rest-auth-4.0.1/demo/react-spa/src/
+-rw-r--r--   0 michael    (501) staff       (20)      594 2020-03-28 18:49:16.000000 dj-rest-auth-4.0.1/demo/react-spa/src/App.css
+-rw-r--r--   0 michael    (501) staff       (20)     1770 2020-03-28 18:50:43.000000 dj-rest-auth-4.0.1/demo/react-spa/src/App.js
+-rw-r--r--   0 michael    (501) staff       (20)      280 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/src/App.test.js
+-rw-r--r--   0 michael    (501) staff       (20)      821 2020-03-28 18:49:40.000000 dj-rest-auth-4.0.1/demo/react-spa/src/index.css
+-rw-r--r--   0 michael    (501) staff       (20)      503 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/src/index.js
+-rw-r--r--   0 michael    (501) staff       (20)     2671 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/src/logo.svg
+-rw-r--r--   0 michael    (501) staff       (20)     5086 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/src/serviceWorker.js
+-rw-r--r--   0 michael    (501) staff       (20)      255 2020-03-28 16:41:44.000000 dj-rest-auth-4.0.1/demo/react-spa/src/setupTests.js
+-rw-r--r--   0 michael    (501) staff       (20)      234 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/demo/requirements.pip
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.205905 dj-rest-auth-4.0.1/demo/templates/
+-rw-r--r--   0 michael    (501) staff       (20)     4447 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/demo/templates/base.html
+-rw-r--r--   0 michael    (501) staff       (20)      188 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/email_verification.html
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.215508 dj-rest-auth-4.0.1/demo/templates/fragments/
+-rw-r--r--   0 michael    (501) staff       (20)      652 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/fragments/email_verification_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      839 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/fragments/login_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      668 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/fragments/logout_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      908 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/fragments/password_change_form.html
+-rw-r--r--   0 michael    (501) staff       (20)     1489 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/fragments/password_reset_confirm_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      579 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/fragments/password_reset_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      578 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/demo/templates/fragments/resend_email_verification_form.html
+-rw-r--r--   0 michael    (501) staff       (20)     1365 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/fragments/signup_form.html
+-rw-r--r--   0 michael    (501) staff       (20)     1344 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/fragments/user_details_form.html
+-rw-r--r--   0 michael    (501) staff       (20)      253 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/home.html
+-rw-r--r--   0 michael    (501) staff       (20)      161 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/login.html
+-rw-r--r--   0 michael    (501) staff       (20)      163 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/logout.html
+-rw-r--r--   0 michael    (501) staff       (20)     1161 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/password_change.html
+-rw-r--r--   0 michael    (501) staff       (20)      179 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/password_reset.html
+-rw-r--r--   0 michael    (501) staff       (20)      724 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/password_reset_confirm.html
+-rw-r--r--   0 michael    (501) staff       (20)      202 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/demo/templates/resend_email_verification.html
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.217175 dj-rest-auth-4.0.1/demo/templates/rest_framework/
+-rw-r--r--   0 michael    (501) staff       (20)     1754 2020-06-20 18:56:14.000000 dj-rest-auth-4.0.1/demo/templates/rest_framework/api.html
+-rw-r--r--   0 michael    (501) staff       (20)      163 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/signup.html
+-rw-r--r--   0 michael    (501) staff       (20)     1915 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/demo/templates/user_details.html
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.225317 dj-rest-auth-4.0.1/dj_rest_auth/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.1/dj_rest_auth/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.241967 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/
+-rw-r--r--   0 michael    (501) staff       (20)      152 2021-07-11 17:17:01.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      149 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/admin.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1467 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2070 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/forms.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     5531 2023-01-02 22:42:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1044 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    11794 2023-01-02 22:42:47.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2854 2021-07-11 17:17:03.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1012 2021-07-11 17:17:03.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1255 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     9589 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      354 2023-05-21 03:10:12.000000 dj-rest-auth-4.0.1/dj_rest_auth/__version__.py
+-rw-r--r--   0 michael    (501) staff       (20)       65 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.1/dj_rest_auth/admin.py
+-rw-r--r--   0 michael    (501) staff       (20)     3075 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/app_settings.py
+-rw-r--r--   0 michael    (501) staff       (20)     2785 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/forms.py
+-rw-r--r--   0 michael    (501) staff       (20)     6282 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.1/dj_rest_auth/jwt_auth.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.172359 dj-rest-auth-4.0.1/dj_rest_auth/locale/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.162783 dj-rest-auth-4.0.1/dj_rest_auth/locale/ar/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.243054 dj-rest-auth-4.0.1/dj_rest_auth/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3751 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.163112 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.250833 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:52:06.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/.!63502!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:54:59.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/.!64462!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:55:51.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/.!64600!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-02-29 23:56:43.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/.!64760!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:05:05.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/.!65418!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/.!65616!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/.!65791!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/.!65995!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/.!69818!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2443 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3195 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.163476 dj-rest-auth-4.0.1/dj_rest_auth/locale/de/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.254518 dj-rest-auth-4.0.1/dj_rest_auth/locale/de/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/de/LC_MESSAGES/.!65618!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/de/LC_MESSAGES/.!65793!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/de/LC_MESSAGES/.!65997!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/de/LC_MESSAGES/.!69820!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2230 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2983 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.163847 dj-rest-auth-4.0.1/dj_rest_auth/locale/es/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.258052 dj-rest-auth-4.0.1/dj_rest_auth/locale/es/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/es/LC_MESSAGES/.!65620!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/es/LC_MESSAGES/.!65795!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/es/LC_MESSAGES/.!65999!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/es/LC_MESSAGES/.!69822!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2405 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3151 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.164278 dj-rest-auth-4.0.1/dj_rest_auth/locale/fa/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.259143 dj-rest-auth-4.0.1/dj_rest_auth/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3514 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.164761 dj-rest-auth-4.0.1/dj_rest_auth/locale/fr/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.262897 dj-rest-auth-4.0.1/dj_rest_auth/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/fr/LC_MESSAGES/.!65622!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/fr/LC_MESSAGES/.!65797!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/fr/LC_MESSAGES/.!66001!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/fr/LC_MESSAGES/.!69824!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3755 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     5257 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.165314 dj-rest-auth-4.0.1/dj_rest_auth/locale/hr/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.278065 dj-rest-auth-4.0.1/dj_rest_auth/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3091 2021-03-18 00:03:01.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.165779 dj-rest-auth-4.0.1/dj_rest_auth/locale/id/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.279107 dj-rest-auth-4.0.1/dj_rest_auth/locale/id/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     4954 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.166222 dj-rest-auth-4.0.1/dj_rest_auth/locale/it/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.280682 dj-rest-auth-4.0.1/dj_rest_auth/locale/it/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3001 2020-05-09 22:17:42.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3904 2020-05-09 22:17:42.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.166746 dj-rest-auth-4.0.1/dj_rest_auth/locale/ja/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.281474 dj-rest-auth-4.0.1/dj_rest_auth/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     5628 2020-12-04 02:36:07.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.167327 dj-rest-auth-4.0.1/dj_rest_auth/locale/ko/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.285101 dj-rest-auth-4.0.1/dj_rest_auth/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ko/LC_MESSAGES/.!65624!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ko/LC_MESSAGES/.!65799!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ko/LC_MESSAGES/.!66003!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ko/LC_MESSAGES/.!69826!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2562 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3296 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.167879 dj-rest-auth-4.0.1/dj_rest_auth/locale/nl/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.286856 dj-rest-auth-4.0.1/dj_rest_auth/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2958 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3524 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.168331 dj-rest-auth-4.0.1/dj_rest_auth/locale/pl/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.294974 dj-rest-auth-4.0.1/dj_rest_auth/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/pl/LC_MESSAGES/.!65626!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/pl/LC_MESSAGES/.!65801!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/pl/LC_MESSAGES/.!66005!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/pl/LC_MESSAGES/.!69828!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2265 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2992 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.168697 dj-rest-auth-4.0.1/dj_rest_auth/locale/pt_BR/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.296590 dj-rest-auth-4.0.1/dj_rest_auth/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2317 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3090 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.169159 dj-rest-auth-4.0.1/dj_rest_auth/locale/ro/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.298196 dj-rest-auth-4.0.1/dj_rest_auth/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2979 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3537 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.169758 dj-rest-auth-4.0.1/dj_rest_auth/locale/ru/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.301627 dj-rest-auth-4.0.1/dj_rest_auth/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ru/LC_MESSAGES/.!65629!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ru/LC_MESSAGES/.!65804!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ru/LC_MESSAGES/.!66008!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ru/LC_MESSAGES/.!69831!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2773 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3508 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.170301 dj-rest-auth-4.0.1/dj_rest_auth/locale/sv/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.303185 dj-rest-auth-4.0.1/dj_rest_auth/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2565 2020-12-04 02:36:07.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3774 2020-12-04 02:36:07.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.170813 dj-rest-auth-4.0.1/dj_rest_auth/locale/tr/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.304948 dj-rest-auth-4.0.1/dj_rest_auth/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     2222 2020-04-27 03:53:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2920 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.171402 dj-rest-auth-4.0.1/dj_rest_auth/locale/uk/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.305662 dj-rest-auth-4.0.1/dj_rest_auth/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)     3502 2021-03-18 00:03:01.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.172020 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hans/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.313483 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65632!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!65807!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!66011!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/.!69834!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2243 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     3019 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.172683 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hant/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.316797 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:06:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65634!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:07:57.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!65809!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 00:08:36.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!66013!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)        0 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/.!69836!django.mo
+-rw-r--r--   0 michael    (501) staff       (20)      373 2021-05-16 17:13:56.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0 michael    (501) staff       (20)     2337 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0 michael    (501) staff       (20)      948 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/models.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.319315 dj-rest-auth-4.0.1/dj_rest_auth/registration/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.1/dj_rest_auth/registration/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.323813 dj-rest-auth-4.0.1/dj_rest_auth/registration/__pycache__/
+-rw-r--r--   0 michael    (501) staff       (20)      165 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/registration/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      811 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     8838 2023-01-02 22:42:46.000000 dj-rest-auth-4.0.1/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)      747 2022-07-17 22:38:11.000000 dj-rest-auth-4.0.1/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     8336 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.1/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    10813 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/registration/serializers.py
+-rw-r--r--   0 michael    (501) staff       (20)     1299 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/registration/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)     7732 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.1/dj_rest_auth/registration/views.py
+-rw-r--r--   0 michael    (501) staff       (20)    12700 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.1/dj_rest_auth/serializers.py
+-rw-r--r--   0 michael    (501) staff       (20)     2990 2021-05-17 04:45:09.000000 dj-rest-auth-4.0.1/dj_rest_auth/social_serializers.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.333070 dj-rest-auth-4.0.1/dj_rest_auth/tests/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2021-05-16 17:38:17.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.340594 dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/
+-rw-r--r--   0 michael    (501) staff       (20)      158 2021-07-11 17:17:01.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     1793 2022-07-17 22:38:11.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     4196 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2461 2022-07-17 22:38:07.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)    27867 2022-07-17 22:38:08.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     7032 2022-07-17 23:28:09.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     9113 2021-07-11 17:17:02.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     5299 2022-07-17 22:38:10.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 michael    (501) staff       (20)     2420 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/django_urls.py
+-rw-r--r--   0 michael    (501) staff       (20)     4012 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/mixins.py
+-rw-r--r--   0 michael    (501) staff       (20)      140 2023-05-21 03:09:30.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/requirements.pip
+-rw-r--r--   0 michael    (501) staff       (20)     2833 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/settings.py
+-rw-r--r--   0 michael    (501) staff       (20)    44032 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/test_api.py
+-rw-r--r--   0 michael    (501) staff       (20)     7157 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/test_serializers.py
+-rw-r--r--   0 michael    (501) staff       (20)    13998 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/test_social.py
+-rw-r--r--   0 michael    (501) staff       (20)      289 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/test_utils.py
+-rw-r--r--   0 michael    (501) staff       (20)     4541 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)     1031 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/tests/utils.py
+-rw-r--r--   0 michael    (501) staff       (20)     1198 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/urls.py
+-rw-r--r--   0 michael    (501) staff       (20)      541 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/dj_rest_auth/utils.py
+-rw-r--r--   0 michael    (501) staff       (20)    10760 2023-05-07 05:35:37.000000 dj-rest-auth-4.0.1/dj_rest_auth/views.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.230002 dj-rest-auth-4.0.1/dj_rest_auth.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3458 2023-05-21 03:11:14.000000 dj-rest-auth-4.0.1/dj_rest_auth.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     8029 2023-05-21 03:11:15.000000 dj-rest-auth-4.0.1/dj_rest_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-21 03:11:14.000000 dj-rest-auth-4.0.1/dj_rest_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2020-03-01 01:18:23.000000 dj-rest-auth-4.0.1/dj_rest_auth.egg-info/not-zip-safe
+-rw-r--r--   0 michael    (501) staff       (20)       85 2023-05-21 03:11:14.000000 dj-rest-auth-4.0.1/dj_rest_auth.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       13 2023-05-21 03:11:14.000000 dj-rest-auth-4.0.1/dj_rest_auth.egg-info/top_level.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-21 03:11:15.349442 dj-rest-auth-4.0.1/docs/
+-rw-r--r--   0 michael    (501) staff       (20)     6786 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/docs/Makefile
+-rw-r--r--   0 michael    (501) staff       (20)     3219 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/docs/api_endpoints.rst
+-rw-r--r--   0 michael    (501) staff       (20)     8317 2020-05-09 22:29:21.000000 dj-rest-auth-4.0.1/docs/conf.py
+-rw-r--r--   0 michael    (501) staff       (20)     9026 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/docs/configuration.rst
+-rw-r--r--   0 michael    (501) staff       (20)      758 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.1/docs/demo.rst
+-rw-r--r--   0 michael    (501) staff       (20)      497 2020-05-30 06:34:32.000000 dj-rest-auth-4.0.1/docs/disclosure.rst
+-rw-r--r--   0 michael    (501) staff       (20)     3095 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/docs/faq.rst
+-rw-r--r--   0 michael    (501) staff       (20)      754 2021-03-20 17:51:05.000000 dj-rest-auth-4.0.1/docs/index.rst
+-rw-r--r--   0 michael    (501) staff       (20)    11426 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/docs/installation.rst
+-rw-r--r--   0 michael    (501) staff       (20)     1301 2020-08-10 01:03:45.000000 dj-rest-auth-4.0.1/docs/introduction.rst
+-rw-r--r--   0 michael    (501) staff       (20)     6713 2020-03-01 01:48:46.000000 dj-rest-auth-4.0.1/docs/make.bat
+-rw-r--r--   0 michael    (501) staff       (20)      657 2021-03-17 23:58:28.000000 dj-rest-auth-4.0.1/runtests.py
+-rw-r--r--   0 michael    (501) staff       (20)      474 2023-05-21 03:11:15.351813 dj-rest-auth-4.0.1/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1542 2023-05-21 03:09:30.000000 dj-rest-auth-4.0.1/setup.py
+-rw-r--r--   0 michael    (501) staff       (20)     1135 2023-03-26 05:23:49.000000 dj-rest-auth-4.0.1/tox.ini
```

### Comparing `dj-rest-auth-4.0.0/.circleci/config.yml` & `dj-rest-auth-4.0.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/.github/workflows/stale.yml` & `dj-rest-auth-4.0.1/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/.gitignore` & `dj-rest-auth-4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/LICENSE` & `dj-rest-auth-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/PKG-INFO` & `dj-rest-auth-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-rest-auth
-Version: 4.0.0
+Version: 4.0.1
 Summary: Authentication and Registration in Django Rest Framework
 Home-page: http://github.com/iMerica/dj-rest-auth
 Author: iMerica
 Author-email: imichael@pm.me
 License: MIT
 Keywords: django rest auth registration rest-framework django-registration api
 Classifier: Framework :: Django
```

### Comparing `dj-rest-auth-4.0.0/README.md` & `dj-rest-auth-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/demo/settings.py` & `dj-rest-auth-4.0.1/demo/demo/settings.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/demo/urls.py` & `dj-rest-auth-4.0.1/demo/demo/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/README.md` & `dj-rest-auth-4.0.1/demo/react-spa/README.md`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/package.json` & `dj-rest-auth-4.0.1/demo/react-spa/package.json`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/public/favicon.ico` & `dj-rest-auth-4.0.1/demo/react-spa/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/public/index.html` & `dj-rest-auth-4.0.1/demo/react-spa/public/index.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/public/logo192.png` & `dj-rest-auth-4.0.1/demo/react-spa/public/logo192.png`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/public/logo512.png` & `dj-rest-auth-4.0.1/demo/react-spa/public/logo512.png`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/src/App.css` & `dj-rest-auth-4.0.1/demo/react-spa/src/App.css`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/src/App.js` & `dj-rest-auth-4.0.1/demo/react-spa/src/App.js`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/src/index.css` & `dj-rest-auth-4.0.1/demo/react-spa/src/index.css`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/src/logo.svg` & `dj-rest-auth-4.0.1/demo/react-spa/src/logo.svg`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/react-spa/src/serviceWorker.js` & `dj-rest-auth-4.0.1/demo/react-spa/src/serviceWorker.js`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/base.html` & `dj-rest-auth-4.0.1/demo/templates/base.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/fragments/email_verification_form.html` & `dj-rest-auth-4.0.1/demo/templates/fragments/email_verification_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/fragments/login_form.html` & `dj-rest-auth-4.0.1/demo/templates/fragments/login_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/fragments/logout_form.html` & `dj-rest-auth-4.0.1/demo/templates/fragments/logout_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/fragments/password_change_form.html` & `dj-rest-auth-4.0.1/demo/templates/fragments/password_change_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/fragments/password_reset_confirm_form.html` & `dj-rest-auth-4.0.1/demo/templates/fragments/password_reset_confirm_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/fragments/password_reset_form.html` & `dj-rest-auth-4.0.1/demo/templates/fragments/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/fragments/resend_email_verification_form.html` & `dj-rest-auth-4.0.1/demo/templates/fragments/resend_email_verification_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/fragments/signup_form.html` & `dj-rest-auth-4.0.1/demo/templates/fragments/signup_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/fragments/user_details_form.html` & `dj-rest-auth-4.0.1/demo/templates/fragments/user_details_form.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/password_change.html` & `dj-rest-auth-4.0.1/demo/templates/password_change.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/password_reset_confirm.html` & `dj-rest-auth-4.0.1/demo/templates/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/rest_framework/api.html` & `dj-rest-auth-4.0.1/demo/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/demo/templates/user_details.html` & `dj-rest-auth-4.0.1/demo/templates/user_details.html`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/app_settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/forms.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/forms.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/jwt_auth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/models.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/serializers.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/social_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/urls.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/utils.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/__pycache__/views.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/app_settings.py` & `dj-rest-auth-4.0.1/dj_rest_auth/app_settings.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/forms.py` & `dj-rest-auth-4.0.1/dj_rest_auth/forms.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/jwt_auth.py` & `dj-rest-auth-4.0.1/dj_rest_auth/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/ar/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/cs/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/de/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/es/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/fa/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/fr/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/hr/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/id/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/it/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/ja/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/ko/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/nl/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/pl/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/ro/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/ru/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/sv/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/tr/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/uk/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po` & `dj-rest-auth-4.0.1/dj_rest_auth/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/models.py` & `dj-rest-auth-4.0.1/dj_rest_auth/models.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/registration/__pycache__/app_settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/registration/__pycache__/serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/registration/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/registration/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/registration/serializers.py` & `dj-rest-auth-4.0.1/dj_rest_auth/registration/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/registration/urls.py` & `dj-rest-auth-4.0.1/dj_rest_auth/registration/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/registration/views.py` & `dj-rest-auth-4.0.1/dj_rest_auth/registration/views.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/serializers.py` & `dj-rest-auth-4.0.1/dj_rest_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/social_serializers.py` & `dj-rest-auth-4.0.1/dj_rest_auth/social_serializers.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/django_urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/mixins.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/test_api.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/test_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/test_social.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/django_urls.py` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/django_urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/mixins.py` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/settings.py` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/settings.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/test_api.py` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/test_serializers.py` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/test_social.py` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/test_social.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/urls.py` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/tests/utils.py` & `dj-rest-auth-4.0.1/dj_rest_auth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/urls.py` & `dj-rest-auth-4.0.1/dj_rest_auth/urls.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/utils.py` & `dj-rest-auth-4.0.1/dj_rest_auth/utils.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth/views.py` & `dj-rest-auth-4.0.1/dj_rest_auth/views.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth.egg-info/PKG-INFO` & `dj-rest-auth-4.0.1/dj_rest_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-rest-auth
-Version: 4.0.0
+Version: 4.0.1
 Summary: Authentication and Registration in Django Rest Framework
 Home-page: http://github.com/iMerica/dj-rest-auth
 Author: iMerica
 Author-email: imichael@pm.me
 License: MIT
 Keywords: django rest auth registration rest-framework django-registration api
 Classifier: Framework :: Django
```

### Comparing `dj-rest-auth-4.0.0/dj_rest_auth.egg-info/SOURCES.txt` & `dj-rest-auth-4.0.1/dj_rest_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/docs/Makefile` & `dj-rest-auth-4.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/docs/api_endpoints.rst` & `dj-rest-auth-4.0.1/docs/api_endpoints.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/docs/conf.py` & `dj-rest-auth-4.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/docs/configuration.rst` & `dj-rest-auth-4.0.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/docs/demo.rst` & `dj-rest-auth-4.0.1/docs/demo.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/docs/faq.rst` & `dj-rest-auth-4.0.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/docs/index.rst` & `dj-rest-auth-4.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/docs/installation.rst` & `dj-rest-auth-4.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/docs/introduction.rst` & `dj-rest-auth-4.0.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/docs/make.bat` & `dj-rest-auth-4.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/runtests.py` & `dj-rest-auth-4.0.1/runtests.py`

 * *Files identical despite different names*

### Comparing `dj-rest-auth-4.0.0/setup.py` & `dj-rest-auth-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,19 @@
     keywords='django rest auth registration rest-framework django-registration api',
     zip_safe=False,
     install_requires=[
         'Django>=2.0',
         'djangorestframework>=3.7.0',
     ],
     extras_require={
-        'with_social': ['django-allauth>=0.40.0,<0.53.0'],
+        'with_social': ['django-allauth>=0.40.0,<0.55.0'],
     },
     tests_require=[
         'coveralls>=1.11.1',
-        'django-allauth==0.52.0',
+        'django-allauth==0.54.0',
         'djangorestframework-simplejwt==4.6.0',
         'responses==0.12.1',
         'unittest-xml-reporting==3.0.4',
     ],
     test_suite='runtests.runtests',
     include_package_data=True,
     python_requires='>=3.5',
```

### Comparing `dj-rest-auth-4.0.0/tox.ini` & `dj-rest-auth-4.0.1/tox.ini`

 * *Files identical despite different names*

