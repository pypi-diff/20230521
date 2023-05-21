# Comparing `tmp/django-page-blocks-0.3.5.tar.gz` & `tmp/django-page-blocks-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-page-blocks-0.3.5.tar", last modified: Mon Mar 13 19:48:58 2023, max compression
+gzip compressed data, was "django-page-blocks-0.4.0.tar", last modified: Sun May 21 15:17:59 2023, max compression
```

## Comparing `django-page-blocks-0.3.5.tar` & `django-page-blocks-0.4.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.939978 django-page-blocks-0.3.5/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1101 2021-11-10 18:41:53.000000 django-page-blocks-0.3.5/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)      215 2021-11-10 18:53:22.000000 django-page-blocks-0.3.5/MANIFEST.in
--rw-rw-r--   0 mark      (1000) mark      (1000)     5412 2023-03-13 19:48:58.939978 django-page-blocks-0.3.5/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     4405 2023-01-24 18:38:43.000000 django-page-blocks-0.3.5/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.899978 django-page-blocks-0.3.5/django_page_blocks.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     5412 2023-03-13 19:48:58.000000 django-page-blocks-0.3.5/django_page_blocks.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     2063 2023-03-13 19:48:58.000000 django-page-blocks-0.3.5/django_page_blocks.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-03-13 19:48:58.000000 django-page-blocks-0.3.5/django_page_blocks.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       11 2023-03-13 19:48:58.000000 django-page-blocks-0.3.5/django_page_blocks.egg-info/top_level.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.903978 django-page-blocks-0.3.5/pageblocks/
--rw-rw-r--   0 mark      (1000) mark      (1000)      146 2022-05-12 17:17:14.000000 django-page-blocks-0.3.5/pageblocks/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      394 2021-11-09 21:42:48.000000 django-page-blocks-0.3.5/pageblocks/admin.py
--rw-rw-r--   0 mark      (1000) mark      (1000)    11541 2023-03-13 19:44:17.000000 django-page-blocks-0.3.5/pageblocks/blocks.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4257 2021-11-10 19:21:05.000000 django-page-blocks-0.3.5/pageblocks/forms.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.907978 django-page-blocks-0.3.5/pageblocks/migrations/
--rw-r--r--   0 mark      (1000) mark      (1000)     1217 2021-10-12 16:50:46.000000 django-page-blocks-0.3.5/pageblocks/migrations/0001_initial.py
--rw-r--r--   0 mark      (1000) mark      (1000)      483 2021-10-12 16:54:28.000000 django-page-blocks-0.3.5/pageblocks/migrations/0002_auto_20211012_1854.py
--rw-r--r--   0 mark      (1000) mark      (1000)      653 2021-11-07 17:04:20.000000 django-page-blocks-0.3.5/pageblocks/migrations/0003_auto_20211107_1804.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      546 2022-05-12 17:17:14.000000 django-page-blocks-0.3.5/pageblocks/migrations/0004_image.py
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-10-12 16:50:46.000000 django-page-blocks-0.3.5/pageblocks/migrations/__init__.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.927978 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/
--rw-r--r--   0 mark      (1000) mark      (1000)     1125 2023-01-23 12:01:11.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)     1122 2021-10-12 16:50:47.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      615 2023-01-23 12:01:11.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      612 2021-10-12 16:54:30.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      773 2021-11-07 16:51:24.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0003_auto_20211107_1751.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      802 2023-01-23 12:01:11.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      799 2021-11-07 17:04:22.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      685 2023-01-23 12:01:11.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0004_image.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      682 2022-03-16 11:50:13.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0004_image.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      131 2023-01-23 12:01:11.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      130 2021-10-12 16:50:46.000000 django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 mark      (1000) mark      (1000)     2400 2023-01-24 18:42:13.000000 django-page-blocks-0.3.5/pageblocks/models.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.891977 django-page-blocks-0.3.5/pageblocks/static/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.891977 django-page-blocks-0.3.5/pageblocks/static/admin/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.891977 django-page-blocks-0.3.5/pageblocks/static/admin/pageblocks/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.927978 django-page-blocks-0.3.5/pageblocks/static/admin/pageblocks/css/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1915 2022-05-12 17:17:14.000000 django-page-blocks-0.3.5/pageblocks/static/admin/pageblocks/css/change_form.css
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.927978 django-page-blocks-0.3.5/pageblocks/static/admin/pageblocks/js/
--rw-rw-r--   0 mark      (1000) mark      (1000)    13535 2023-01-24 17:39:59.000000 django-page-blocks-0.3.5/pageblocks/static/admin/pageblocks/js/change_form.js
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.895978 django-page-blocks-0.3.5/pageblocks/templates/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.891977 django-page-blocks-0.3.5/pageblocks/templates/admin/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.931978 django-page-blocks-0.3.5/pageblocks/templates/admin/pageblocks/
--rw-rw-r--   0 mark      (1000) mark      (1000)      336 2021-11-08 21:49:59.000000 django-page-blocks-0.3.5/pageblocks/templates/admin/pageblocks/block_editor.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      983 2022-05-12 17:17:14.000000 django-page-blocks-0.3.5/pageblocks/templates/admin/pageblocks/change_form.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      239 2021-08-18 19:18:02.000000 django-page-blocks-0.3.5/pageblocks/templates/admin/pageblocks/multi_language_input.html
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.895978 django-page-blocks-0.3.5/pageblocks/templates/pageblocks/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.931978 django-page-blocks-0.3.5/pageblocks/templates/pageblocks/blocks/
--rw-rw-r--   0 mark      (1000) mark      (1000)       77 2021-11-09 23:08:53.000000 django-page-blocks-0.3.5/pageblocks/templates/pageblocks/blocks/container.html
--rw-rw-r--   0 mark      (1000) mark      (1000)       21 2021-11-09 23:01:34.000000 django-page-blocks-0.3.5/pageblocks/templates/pageblocks/blocks/html.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      139 2022-05-12 17:17:14.000000 django-page-blocks-0.3.5/pageblocks/templates/pageblocks/blocks/image.html
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.935979 django-page-blocks-0.3.5/pageblocks/templatetags/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2021-11-09 22:25:12.000000 django-page-blocks-0.3.5/pageblocks/templatetags/__init__.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-03-13 19:48:58.935979 django-page-blocks-0.3.5/pageblocks/templatetags/__pycache__/
--rw-r--r--   0 mark      (1000) mark      (1000)      133 2023-01-23 12:01:11.000000 django-page-blocks-0.3.5/pageblocks/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      132 2021-11-09 22:26:41.000000 django-page-blocks-0.3.5/pageblocks/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)     1608 2023-03-13 19:39:22.000000 django-page-blocks-0.3.5/pageblocks/templatetags/__pycache__/pageblocks.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)     1671 2022-05-12 17:13:20.000000 django-page-blocks-0.3.5/pageblocks/templatetags/__pycache__/pageblocks.cpython-39.pyc
--rw-rw-r--   0 mark      (1000) mark      (1000)     1196 2023-03-13 19:39:21.000000 django-page-blocks-0.3.5/pageblocks/templatetags/pageblocks.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7393 2021-11-10 19:21:45.000000 django-page-blocks-0.3.5/pageblocks/tests.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      163 2021-08-18 19:49:24.000000 django-page-blocks-0.3.5/pageblocks/utils.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1002 2022-03-15 22:06:20.000000 django-page-blocks-0.3.5/pageblocks/views.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-03-13 19:48:58.939978 django-page-blocks-0.3.5/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)     1342 2023-03-13 19:47:57.000000 django-page-blocks-0.3.5/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.185837 django-page-blocks-0.4.0/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1101 2021-11-10 18:41:53.000000 django-page-blocks-0.4.0/LICENSE
+-rw-rw-r--   0 mark      (1000) mark      (1000)      215 2021-11-10 18:53:22.000000 django-page-blocks-0.4.0/MANIFEST.in
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6035 2023-05-21 15:17:59.185837 django-page-blocks-0.4.0/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5013 2023-05-21 15:17:06.000000 django-page-blocks-0.4.0/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.105835 django-page-blocks-0.4.0/django_page_blocks.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6035 2023-05-21 15:17:59.000000 django-page-blocks-0.4.0/django_page_blocks.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2240 2023-05-21 15:17:59.000000 django-page-blocks-0.4.0/django_page_blocks.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-05-21 15:17:59.000000 django-page-blocks-0.4.0/django_page_blocks.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       11 2023-05-21 15:17:59.000000 django-page-blocks-0.4.0/django_page_blocks.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.109835 django-page-blocks-0.4.0/pageblocks/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      146 2022-05-12 17:17:14.000000 django-page-blocks-0.4.0/pageblocks/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      394 2023-05-20 14:55:38.000000 django-page-blocks-0.4.0/pageblocks/admin.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)    13250 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/blocks.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3648 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/forms.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.109835 django-page-blocks-0.4.0/pageblocks/migrations/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1217 2021-10-12 16:50:46.000000 django-page-blocks-0.4.0/pageblocks/migrations/0001_initial.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      483 2021-10-12 16:54:28.000000 django-page-blocks-0.4.0/pageblocks/migrations/0002_auto_20211012_1854.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      653 2021-11-07 17:04:20.000000 django-page-blocks-0.4.0/pageblocks/migrations/0003_auto_20211107_1804.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      546 2022-05-12 17:17:14.000000 django-page-blocks-0.4.0/pageblocks/migrations/0004_image.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      487 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/migrations/0005_remove_pageblock_language_pageblock_i18n_data.py
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-10-12 16:50:46.000000 django-page-blocks-0.4.0/pageblocks/migrations/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.161837 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1125 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)     1122 2021-10-12 16:50:47.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      615 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      612 2021-10-12 16:54:30.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      773 2021-11-07 16:51:24.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1751.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      802 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      799 2021-11-07 17:04:22.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      685 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0004_image.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      682 2022-03-16 11:50:13.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0004_image.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      647 2023-05-20 15:08:04.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0005_remove_pageblock_language_pageblock_i18n_data.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      131 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      130 2021-10-12 16:50:46.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2449 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/static/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/static/admin/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.161837 django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/css/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2320 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/css/change_form.css
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.165837 django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/js/
+-rw-rw-r--   0 mark      (1000) mark      (1000)    15461 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/js/change_form.js
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/templates/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/templates/admin/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.165837 django-page-blocks-0.4.0/pageblocks/templates/admin/pageblocks/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      382 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/templates/admin/pageblocks/block_editor.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)      983 2022-05-12 17:17:14.000000 django-page-blocks-0.4.0/pageblocks/templates/admin/pageblocks/change_form.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)      239 2021-08-18 19:18:02.000000 django-page-blocks-0.4.0/pageblocks/templates/admin/pageblocks/multi_language_input.html
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/templates/pageblocks/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.165837 django-page-blocks-0.4.0/pageblocks/templates/pageblocks/blocks/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       77 2021-11-09 23:08:53.000000 django-page-blocks-0.4.0/pageblocks/templates/pageblocks/blocks/container.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)       21 2021-11-09 23:01:34.000000 django-page-blocks-0.4.0/pageblocks/templates/pageblocks/blocks/html.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)      139 2022-05-12 17:17:14.000000 django-page-blocks-0.4.0/pageblocks/templates/pageblocks/blocks/image.html
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.169837 django-page-blocks-0.4.0/pageblocks/templatetags/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2021-11-09 22:25:12.000000 django-page-blocks-0.4.0/pageblocks/templatetags/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.185837 django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/
+-rw-r--r--   0 mark      (1000) mark      (1000)      133 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      132 2021-11-09 22:26:41.000000 django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)     1527 2023-05-20 18:04:38.000000 django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/pageblocks.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)     1671 2022-05-12 17:13:20.000000 django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/pageblocks.cpython-39.pyc
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1066 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/templatetags/pageblocks.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7638 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/tests.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      163 2021-08-18 19:49:24.000000 django-page-blocks-0.4.0/pageblocks/utils.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1002 2022-03-15 22:06:20.000000 django-page-blocks-0.4.0/pageblocks/views.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-05-21 15:17:59.185837 django-page-blocks-0.4.0/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1357 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/setup.py
```

### Comparing `django-page-blocks-0.3.5/LICENSE` & `django-page-blocks-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/PKG-INFO` & `django-page-blocks-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-page-blocks
-Version: 0.3.5
-Summary: A simple, Wagtail CMS inspired content block engine for Django.  Intended to give slightly more control than regular flatpages.
+Version: 0.4.0
+Summary: A simple, Wagtail CMS inspired multi language content block engine for Django.  Intended to give slightly more control than regular flatpages.
 Home-page: https://github.com/bravasoftware/django-page-blocks
 Author: Mark Skelton
 Author-email: studio@bravasoftware.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -29,27 +29,31 @@
 
 This documentation is a bit brief at the moment but hopefully the info below can help you get set up.
 
 It was developed and tested on Python 3.9 with Django 3.2.  It will probably work on other recent versions of both as it doesn't do anything particularly special, but your mileage may vary.
 
 The code is still under active development and is very much in an alpha state (hence the lack of documentation.  As always, pull requests and feedback welcome.
 
+**CAUTION** django-page-blocks 0.4 includes an overhaul to the internationalization support in the library, with it moving from a per block to per field option.  It's not a breaking change and won't affect sites already using django-page-blocks < 0.4 if you have only been using one language.  For existing multi-language sites, as the language field is stripped from the existing blocks, they will be merged into the same page so you will need to do some editing.
+
 
 ## Getting Started
 
 Add the app to your INSTALLED_APPS
 
 ```
 INSTALLED_APPS = [
   ...
   'pageblocks'
   ...
 ]
 ```
 
+You will need to also ensure that you have at least one option set in LANGUAGES, and that your LANGUAGE_CODE is set to one of these options.
+
 You can then either use the base model pageblocks.Page or extend it.
 
 ## Extending the Models
 
 There are two options to extend these models depending on your needs, however you'll need to make a decision on it before starting your project or else you may run into problems later.
 
 ### Option 1 - Use pageblocks.Page as a base class
```

### Comparing `django-page-blocks-0.3.5/README.md` & `django-page-blocks-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 
 This documentation is a bit brief at the moment but hopefully the info below can help you get set up.
 
 It was developed and tested on Python 3.9 with Django 3.2.  It will probably work on other recent versions of both as it doesn't do anything particularly special, but your mileage may vary.
 
 The code is still under active development and is very much in an alpha state (hence the lack of documentation.  As always, pull requests and feedback welcome.
 
+**CAUTION** django-page-blocks 0.4 includes an overhaul to the internationalization support in the library, with it moving from a per block to per field option.  It's not a breaking change and won't affect sites already using django-page-blocks < 0.4 if you have only been using one language.  For existing multi-language sites, as the language field is stripped from the existing blocks, they will be merged into the same page so you will need to do some editing.
+
 
 ## Getting Started
 
 Add the app to your INSTALLED_APPS
 
 ```
 INSTALLED_APPS = [
   ...
   'pageblocks'
   ...
 ]
 ```
 
+You will need to also ensure that you have at least one option set in LANGUAGES, and that your LANGUAGE_CODE is set to one of these options.
+
 You can then either use the base model pageblocks.Page or extend it.
 
 ## Extending the Models
 
 There are two options to extend these models depending on your needs, however you'll need to make a decision on it before starting your project or else you may run into problems later.
 
 ### Option 1 - Use pageblocks.Page as a base class
```

### Comparing `django-page-blocks-0.3.5/django_page_blocks.egg-info/PKG-INFO` & `django-page-blocks-0.4.0/django_page_blocks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-page-blocks
-Version: 0.3.5
-Summary: A simple, Wagtail CMS inspired content block engine for Django.  Intended to give slightly more control than regular flatpages.
+Version: 0.4.0
+Summary: A simple, Wagtail CMS inspired multi language content block engine for Django.  Intended to give slightly more control than regular flatpages.
 Home-page: https://github.com/bravasoftware/django-page-blocks
 Author: Mark Skelton
 Author-email: studio@bravasoftware.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -29,27 +29,31 @@
 
 This documentation is a bit brief at the moment but hopefully the info below can help you get set up.
 
 It was developed and tested on Python 3.9 with Django 3.2.  It will probably work on other recent versions of both as it doesn't do anything particularly special, but your mileage may vary.
 
 The code is still under active development and is very much in an alpha state (hence the lack of documentation.  As always, pull requests and feedback welcome.
 
+**CAUTION** django-page-blocks 0.4 includes an overhaul to the internationalization support in the library, with it moving from a per block to per field option.  It's not a breaking change and won't affect sites already using django-page-blocks < 0.4 if you have only been using one language.  For existing multi-language sites, as the language field is stripped from the existing blocks, they will be merged into the same page so you will need to do some editing.
+
 
 ## Getting Started
 
 Add the app to your INSTALLED_APPS
 
 ```
 INSTALLED_APPS = [
   ...
   'pageblocks'
   ...
 ]
 ```
 
+You will need to also ensure that you have at least one option set in LANGUAGES, and that your LANGUAGE_CODE is set to one of these options.
+
 You can then either use the base model pageblocks.Page or extend it.
 
 ## Extending the Models
 
 There are two options to extend these models depending on your needs, however you'll need to make a decision on it before starting your project or else you may run into problems later.
 
 ### Option 1 - Use pageblocks.Page as a base class
```

### Comparing `django-page-blocks-0.3.5/django_page_blocks.egg-info/SOURCES.txt` & `django-page-blocks-0.4.0/django_page_blocks.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 pageblocks/tests.py
 pageblocks/utils.py
 pageblocks/views.py
 pageblocks/migrations/0001_initial.py
 pageblocks/migrations/0002_auto_20211012_1854.py
 pageblocks/migrations/0003_auto_20211107_1804.py
 pageblocks/migrations/0004_image.py
+pageblocks/migrations/0005_remove_pageblock_language_pageblock_i18n_data.py
 pageblocks/migrations/__init__.py
 pageblocks/migrations/__pycache__/0001_initial.cpython-310.pyc
 pageblocks/migrations/__pycache__/0001_initial.cpython-39.pyc
 pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-310.pyc
 pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-39.pyc
 pageblocks/migrations/__pycache__/0003_auto_20211107_1751.cpython-39.pyc
 pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-310.pyc
 pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-39.pyc
 pageblocks/migrations/__pycache__/0004_image.cpython-310.pyc
 pageblocks/migrations/__pycache__/0004_image.cpython-39.pyc
+pageblocks/migrations/__pycache__/0005_remove_pageblock_language_pageblock_i18n_data.cpython-310.pyc
 pageblocks/migrations/__pycache__/__init__.cpython-310.pyc
 pageblocks/migrations/__pycache__/__init__.cpython-39.pyc
 pageblocks/static/admin/pageblocks/css/change_form.css
 pageblocks/static/admin/pageblocks/js/change_form.js
 pageblocks/templates/admin/pageblocks/block_editor.html
 pageblocks/templates/admin/pageblocks/change_form.html
 pageblocks/templates/admin/pageblocks/multi_language_input.html
```

### Comparing `django-page-blocks-0.3.5/pageblocks/blocks.py` & `django-page-blocks-0.4.0/pageblocks/blocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,51 +3,59 @@
 import imghdr
 import re
 import uuid
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.template.loader import render_to_string
-from django.utils.translation import gettext_lazy, gettext
+from django.utils.translation import gettext_lazy, gettext, get_language
 from django.core.files.base import ContentFile
 
 from .utils import class_from_name
 from .models import Image
 
 
 class BaseField(object):
     input_type = 'text'
     input_classes = []
+    multi_lingual = False
 
-    def __init__(self, label=None, required=False, additional_classes=None, *args, **kwargs):
+    def __init__(self, label=None, required=False, additional_classes=None, multi_lingual=None, *args, **kwargs):
         self.label = label
         self.required = required
+        if multi_lingual:
+            self.multi_lingual = multi_lingual
 
         if additional_classes:
             self.input_classes.update(additional_classes)
 
     def serialize_field_definition(self, id):
         return {
             'required': self.required,
             'input_type': self.input_type,
+            'multi_lingual': self.multi_lingual,
             'label': str(self.label) if self.label else self.id,
             'class': ' '.join(self.input_classes)
         }
         
 class CharField(BaseField):
     input_type = 'text'
+    multi_lingual = True
 
 class TextField(BaseField):
     input_type = 'textarea'
+    multi_lingual = True
 
 class HTMLField(TextField):
     input_classes = ['html']
+    multi_lingual = True
 
 class ImageField(BaseField):
     input_type = 'image'
+    multi_lingual = False
 
 class BlockStreamField(BaseField):
     input_type = 'blockstream'
 
     def serialize_field_definition(self, id):
         fd = super().serialize_field_definition(id)
         fd['initial'] = []
@@ -67,58 +75,60 @@
 class BlockProcessor(object):
     def blocks_to_representation(self, blocks, data=None):
         if not data:
             data = []
 
         for page_block in blocks.order_by('index'):
             block_class = class_from_name(page_block.type)
-            block = block_class(data=page_block.data, instance=page_block)
+            block = block_class(data={
+                'data': page_block.data,
+                'i18n_data': page_block.i18n_data,
+                'type': page_block.type
+            }, instance=page_block)
 
             data.append({
                 'id': str(page_block.id),
                 'type': page_block.type,
-                'data': block.data_to_representation()
+                'data': block.data_to_representation(),
+                'i18n_data': block.i18n_data_to_representation(),
             })
         return data
 
-    def clean(self, data, parent_indexes=[], language=''):
+    def clean(self, data, parent_indexes=[]):
         if not data:
             return data
 
-        if not language:
-            raise Exception('No language')
-
         for index, block_data in enumerate(data):
             block_class = class_from_name(block_data['type'])
-            block = block_class(block_data['data'])
+            block = block_class(data=block_data)
             try:
-                block_data['data'] = block.clean(parent_indexes=parent_indexes + [index], language=language)
+                block_data['data'] = block.clean(parent_indexes=parent_indexes + [index])
+                block_data['i18n_data'] = block.clean_i18n(parent_indexes=parent_indexes + [index])
             except BlockValidationError as bve:
-                raise ValidationError(f'B:{language}:{self.format_index(parent_indexes, index)}:{bve.field_id}:' + str(bve))
+                raise ValidationError(f'B:{self.format_index(parent_indexes, index)}:{bve.field_id}:' + str(bve))
 
         return data
 
     def format_index(self, parent_indexes, index):
         indexes = parent_indexes + [index]
         return ','.join([str(i) for i in indexes])
 
-    def save(self, page, data, parent=None, language=None):
+    def save(self, page, data, parent=None):
         processed_blocks = []
         
         for block_index, block_data in enumerate(data):
             block_class = class_from_name(block_data['type'])
-            block = block_class(block_data,
+            block = block_class(data=block_data,
                                 instance=page.blocks.model.objects.get(page=page, id=block_data['id']) if block_data.get('id', None) else None)
 
             processed_blocks += block.save(page=page,
-                                           language=language if not parent else parent.language,
                                            block_index=block_index, parent=parent)
 
         if not parent:
-            cleanup_qs = page.blocks.model.objects.filter(page=page, language=language).exclude(id__in=[str(rec.id) for rec in processed_blocks])
+            cleanup_qs = page.blocks.model.objects.filter(page=page).exclude(id__in=[str(rec.id) for rec in processed_blocks])
             cleanup_qs.delete()
 
         return processed_blocks
 
     def render(self, blocks):
         return ''.join([block.get_block().render() for block in blocks])
     
@@ -156,64 +166,90 @@
         return '\n'.join([ss for ss in set(stylesheets)])
 
 
 class BaseBlock(object):
     template_name = None
     name = None
     description = None
+    block_type = None
     fields = ()
 
     def __init__(self, data=None, instance=None, *args, **kwargs):
-        self.data = data
+        self.data = data.get('data', {}) if data else {}
+        self.block_type = data.get('type', None) if data else None
+        self.i18n_data = data.get('i18n_data', {}) if data else {}
         self.instance = instance
 
     @classmethod
     def serialize_field_definitions(cls):
         return {
             id: field.serialize_field_definition(id) for id, field in cls.fields
         }
 
-    def data_to_representation(self):
-        return self.data
+    def data_to_representation(self, data=None, language=None):
+        if data is None:
+            data = self.data
+        return data
+    
+    def i18n_data_to_representation(self):
+        return {
+            lc: self.data_to_representation(self.i18n_data.get(lc, {}), language=lc) for lc in self.i18n_data.keys()
+        }
 
-    def data_to_internal_value(self, data):
+    def data_to_internal_value(self, data, language=None):
         return data
 
     def clean(self, *args, **kwargs):
         """ Validate the block data """
         for field_id, field in self.fields:
             if field.required and not self.data.get(field_id, None):
                 raise BlockValidationError(gettext('This field is required'), field_id=field_id)
 
         return self.data
 
-    def get_instance_for_saving(self, page, language, block_index, parent, *args, **kwargs):
-        instance = self.instance if self.instance else page.blocks.model(page=page, language=language)
-        instance.language = language
-        instance.type = self.data['type']
-        instance.data = self.data_to_internal_value(self.data['data'])
+    def clean_i18n(self, *args, **kwargs):
+        """ Validate the regional language data """
+        return self.i18n_data
+
+    def get_instance_for_saving(self, page, block_index, parent, *args, **kwargs):
+        instance = self.instance if self.instance else page.blocks.model(page=page)
+        instance.type = self.block_type
+        instance.data = self.data_to_internal_value(self.data)
+        instance.i18n_data = {
+            lc: self.data_to_internal_value(self.i18n_data.get(lc, {}), language=lc) for lc in self.i18n_data.keys()
+        }
         instance.index = block_index
         instance.parent = parent
         return instance
 
-    def save(self, page, language, block_index, parent, *args, **kwargs):
-        self.instance = self.get_instance_for_saving(page, language, block_index, parent, *args, **kwargs)
+    def save(self, page, block_index, parent, *args, **kwargs):
+        self.instance = self.get_instance_for_saving(page, block_index, parent, *args, **kwargs)
         self.instance.save()
         return [self.instance]
 
     def render(self):
         if not self.template_name:
             raise BlockRenderingError(gettext('No template_name defined for') + '.'.join([self.__class__.__module__, self.__class__.__name__]))
-        
+
         return render_to_string(self.template_name, self.get_render_context_data())
 
     def get_render_context_data(self, *args, **kwargs):
+        # Get the current language
+        current_language = get_language()
+        block_data = self.data_to_representation()
+        block_i18n_data = self.i18n_data_to_representation()
+        for lc in block_i18n_data.keys():
+            if lc == current_language:
+                for key in block_i18n_data[lc].keys():
+                    if block_i18n_data[lc][key]:
+                        block_data[key] = block_i18n_data[lc][key]
+
         return {
             'instance': self.instance,
-            'block': self.data_to_representation()
+            'block': block_data
         }
 
     def get_scripts(self, *args, **kwargs):
         """
         Script dependencies to include for this block
         """
         return []
@@ -242,28 +278,35 @@
     description = gettext_lazy('A simple image')
     fields = (
         ('image', ImageField(label=gettext_lazy('Image'), required=True)),
         ('alt', CharField(label=gettext_lazy('Alt text'), required=False)),
         ('class', CharField(label=gettext_lazy('Class'), required=False)),
     )
 
-    def data_to_representation(self):
-        data = self.data
+    def data_to_representation(self, data=None, **kwargs):
+        data = super().data_to_representation(data)
         if data.get('image_id', None):
             try:
                 data['image'] = Image.objects.get(id=data['image_id']).image.url
             except Image.DoesNotExist:
                 pass
         return data
 
-    def data_to_internal_value(self, data):
+    def data_to_internal_value(self, data, language=None):
+        # TODO: Make this multi-language - needs to be able to write to and from i18n_data if language key is set
         image = None
         if self.instance and self.instance.data.get('image_id', None):
             image = Image.objects.filter(id=self.instance.data['image_id']).first()
 
+        if not data.get('image', None):
+            if image:
+                image.image.delete()
+                image.delete()
+            return data
+
         if not re.search('^\/|^(?i)http', data['image']):
             if not image:
                 image = Image()
 
             if image.image:
                 image.image.delete()
 
@@ -304,34 +347,36 @@
     name = gettext_lazy('Container')
     description = gettext_lazy('A container that contains other blocks')
     fields = (
         ('class', CharField(label=gettext_lazy('Class'), required=False)),
         ('blocks', BlockStreamField(label=gettext_lazy('Blocks'), required=True))
     )
 
-    def clean(self, parent_indexes=[], language='', *args, **kwargs):
+    def clean(self, parent_indexes=[], *args, **kwargs):
         data = super().clean(*args, **kwargs)
-        BlockProcessor().clean(data['blocks'], parent_indexes=parent_indexes, language=language)
+        BlockProcessor().clean(data['blocks'], parent_indexes=parent_indexes)
         return data
 
-    def data_to_representation(self):
-        data = super().data_to_representation()
+    def data_to_representation(self, data=None, language=None):
+        if language:
+            return None
+
+        data = super().data_to_representation(data)
         if self.instance:
             data['blocks'] = BlockProcessor().blocks_to_representation(self.instance.children.all())
         return data
 
-    def save(self, page, language, block_index, parent, *args, **kwargs):
+    def save(self, page, block_index, parent, *args, **kwargs):
         if not self.instance:
-            self.instance = page.blocks.model(page=page, language=language)
+            self.instance = page.blocks.model(page=page)
 
-        block_data = copy.deepcopy(self.data['data'])
+        block_data = copy.deepcopy(self.data)
         sub_blocks = BlockProcessor().save(page, block_data.pop('blocks'), parent=self.instance)
 
-        self.instance.language = language
-        self.instance.type = self.data['type']
+        self.instance.type = self.block_type
         self.instance.data = block_data
         self.instance.index = block_index
         self.instance.parent = parent
         self.instance.save()
 
         return [self.instance] + sub_blocks
```

### Comparing `django-page-blocks-0.3.5/pageblocks/forms.py` & `django-page-blocks-0.4.0/pageblocks/forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 class LanguagesInputMixin(object):
     def get_context(self, *args, **kwargs):
         ctx = super().get_context(*args, **kwargs)
         ctx['languages'] = base64.b64encode(json.dumps({
             key: str(value) for key, value in settings.LANGUAGES
         }).encode()).decode()
+        ctx['default_language'] = settings.LANGUAGE_CODE
         return ctx
 
 
 class MultiLanguageInput(LanguagesInputMixin, forms.TextInput):
     template_name = 'admin/pageblocks/multi_language_input.html'
 
 
@@ -44,52 +45,43 @@
             'labelConfirmCopy': gettext('Are you sure you want to do this?  This will overwrite all of the content in this page for this language.'),
             'labelCopyFrom': gettext('Copy from')
         }).encode()).decode()
         return ctx
 
 
 class PageAdminForm(forms.ModelForm):
-    blocks = forms.JSONField(widget=PageBlockEditor, initial=dict({
-        key: [] for key, _ in settings.LANGUAGES
-    }), required=False)
+    blocks = forms.JSONField(widget=PageBlockEditor, initial=list([]), required=False)
     slug = forms.SlugField(required=False)
 
     class Meta:
         model = Page
         fields = ('title', 'slug',)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         if self.instance and self.instance.pk:
             self.init_blocks()
 
     def init_blocks(self):
-        languages = [language for language, _ in settings.LANGUAGES]
-        self.fields['blocks'].initial = {
-            language: BlockProcessor().blocks_to_representation(self.instance.blocks.filter(parent=None, language=language)) for language in languages
-        }
+        self.fields['blocks'].initial = BlockProcessor().blocks_to_representation(self.instance.blocks.filter(parent=None))
 
     def clean(self):
         data = self.cleaned_data
         if not data.get('slug', None) and data.get('title', {}):
             data['slug'] = self.generate_slug(data['title'].get(get_language(), gettext('Untitled')))
         return data
 
     def clean_blocks(self):
         """ Validate the data for each block (and recurse if it's a container block) """
         data = self.cleaned_data['blocks']
         if not data:
             return data
 
-        languages = [language for language, _ in settings.LANGUAGES] + list(data.keys())
-
-        return {
-            language: BlockProcessor().clean(data[language], language=language) for language in set(languages)
-        }
+        return BlockProcessor().clean(data)
 
     def generate_slug(self, val):
         slug = slugify(val)
         offset = 0
         qs = Page.objects.all() if not self.instance and not self.instance.pk else Page.objects.exclude(pk=self.instance.pk)
 
         while qs.filter(slug=slug).count() > 0:
@@ -105,12 +97,8 @@
         return page
 
     def save_blocks(self, page):
         block_data = self.cleaned_data.get('blocks', {})
         if not block_data:
             block_data = {}
 
-        languages = [language for language, _ in settings.LANGUAGES] + list(block_data.keys())
-        processed_blocks = []
-        for language in set(languages):
-            processed_blocks += BlockProcessor().save(page, block_data.get(language, []),
-                                                      language=language)
+        BlockProcessor().save(page, block_data)
```

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/0001_initial.py` & `django-page-blocks-0.4.0/pageblocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/0003_auto_20211107_1804.py` & `django-page-blocks-0.4.0/pageblocks/migrations/0003_auto_20211107_1804.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/0004_image.py` & `django-page-blocks-0.4.0/pageblocks/migrations/0004_image.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-310.pyc` & `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-39.pyc` & `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0003_auto_20211107_1751.cpython-39.pyc` & `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1751.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-310.pyc` & `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-39.pyc` & `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0004_image.cpython-310.pyc` & `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0004_image.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/migrations/__pycache__/0004_image.cpython-39.pyc` & `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0004_image.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/models.py` & `django-page-blocks-0.4.0/pageblocks/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,35 +39,39 @@
 
     @classmethod
     def get_available_blocks(cls):
         return [
             (c, class_from_name(c)) for c in cls.get_available_block_type_classes()
         ]
 
-    def get_blocks_for_language(self, language):
-        return self.blocks.filter(language=language, parent=None).order_by('index')
+    def get_blocks(self):
+        return self.blocks.filter(parent=None).order_by('index')
 
 class Page(AbstractPage):
     pass
 
 class AbstractPageBlock(models.Model):
     id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
-    language = models.CharField(max_length=2, db_index=True)
     index = models.IntegerField(default=-1)
     type = models.TextField()
     data = models.JSONField(default=dict)
+    i18n_data = models.JSONField(default=dict)
     parent = models.ForeignKey('self', on_delete=models.CASCADE, blank=True, null=True,
                                related_name='children')
 
     class Meta:
         abstract = True
         ordering = ['index']
 
     def get_block(self):
-        return class_from_name(self.type)(data=self.data, instance=self)
+        return class_from_name(self.type)(data={
+            'data': self.data,
+            'i18n_data': self.i18n_data,
+            'type': self.type,
+        }, instance=self)
 
 
 class PageBlock(AbstractPageBlock):
     page = models.ForeignKey(Page, on_delete=models.CASCADE, related_name='blocks', db_index=True)
     
 
 class Image(models.Model):
```

### Comparing `django-page-blocks-0.3.5/pageblocks/static/admin/pageblocks/css/change_form.css` & `django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/css/change_form.css`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,29 @@
     cursor: pointer;
 }
 .page-block-editor .image-uploader img {
     width: 240px; height: 240px;
     object-fit: contain;
     cursor: pointer;
 }
+.page-block-editor .field-language-picker {
+    float: right;
+    clear: right;
+    display: flex;
+    gap: 4px;
+}
+.page-block-editor .field-language-picker a {
+    border: 2px solid rgba(0,0,0,0);
+}
+.page-block-editor .field-language-picker a.active {
+    border: 2px solid rgba(255, 255, 255, 1.0);
+}
+.page-block-editor .field-language-picker a:hover {
+    border: 2px solid rgba(255, 255, 255, 0.5);
+}
 
 @media (max-width: 767px) {
     .multi-language-row {
         width: 100%;
         margin-left: 0px;
     }
     .multi-language-row input {
```

### Comparing `django-page-blocks-0.3.5/pageblocks/static/admin/pageblocks/js/change_form.js` & `django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/js/change_form.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -108,82 +108,117 @@
             }
         }
     });
 
     Vue.component('page-block-editor-field', {
         template: `
     <div class="field" :class="hasError() ? 'errors' : ''">
-      <label>{{ field.label }}<span class="small" v-if="field.required">*</span></label>
+      <label>
+        {{ field.label }}<span class="small" v-if="field.required">*</span>
+      </label>
       <textarea v-if="field.input_type === 'textarea'" :required="field.required" :class="field.class" v-model="value" v-on:change="onValueChanged()"></textarea>
       <input v-if="field.input_type === 'text'" :type='field.input_type' :required="field.required" :class="field.class" v-model="value" v-on:change="onValueChanged()" />
       <block-editor
         v-if="field.input_type === 'blockstream'"
         v-model="value"
         :available-blocks="availableBlocks"
         v-on:change="onValueChanged()"
         :block-index="blockIndex"
         :input-name="inputName"
-        :input-language="inputLanguage"></block-editor>
+        :languages="languages"
+        :default-language="defaultLanguage"></block-editor>
       <image-uploader
         v-if="field.input_type === 'image'"
         v-model="value"
         v-on:change="onValueChanged()"></image-uploader>
       <div v-if="hasError()" class="error">
         {{ getError() }}
       </div>
     </div>
     `,
-        props: ['value', 'fieldId', 'field', 'availableBlocks', 'blockIndex', 'inputName', 'inputLanguage'],
+        props: ['value', 'fieldId', 'field', 'availableBlocks', 'blockIndex', 'inputName', 'languages', 'defaultLanguage'],
+        data: function() {
+            return {};
+        },
         methods: {
             onValueChanged: function() {
                 this.$emit('input', this.value);
                 this.$emit('change', this.value);
             },
             hasError: function() {
                 return this.getError() !== null;
             },
             getError: function() {
-                if (this.$root.blockEditorErrors && this.inputName && this.inputLanguage && this.$root.blockEditorErrors[this.inputName]) {
+                if (this.$root.blockEditorErrors && this.inputName && this.$root.blockEditorErrors[this.inputName]) {
                     for (const err of this.$root.blockEditorErrors[this.inputName]) {
-                        if (err[1] === this.inputLanguage && err[2] === this.blockIndex.join(',') && err[3] == this.fieldId) {
+                        if (err[1] === this.blockIndex.join(',') && err[2] == this.fieldId) {
                             return err[err.length - 1];
                         }
                     }
                 }
                 return null;
             }
         },
     });
 
     Vue.component('block-editor', {
         template: `
     <div class="block-editor">
       <div class="block" v-for="(block, index) in blocks" :key="'block-' + getBlockIndexKey(index)" v-if="availableBlocks[block.type] !== undefined">
         <div class="header row">
-          <div class="bold">{{ getBlockTypeName(block.type) }} <span :class="'flag-icon flag-icon-'"></span></div>
+          <div class="bold">
+            {{ getBlockTypeName(block.type) }}
+          </div>
           <div class="text-right buttons">
             <a href="javascript:;" :disabled="index <= 0" :class="{'disabled': index <= 0}" v-on:click.prevent="shiftBlock(index, -1)"><i class="fa fas fa-caret-up"></i></a>
             <a href="javascript:;" :disabled="index + 1 >= blocks.length" :class="{'disabled': index + 1 >= blocks.length}" v-on:click.prevent="shiftBlock(index, 1)"><i class="fa fas fa-caret-down"></i></a>
 
             <a v-on:click.prevent="deleteBlock(index)"><i class="fa fas fa-trash"></i></a>
           </div>
         </div>
 
-        <page-block-editor-field 
-          v-for="(field, fieldIndex) in Object.keys(availableBlocks[block.type].fields)" :key="'block-' + getBlockIndexKey(index) + '-' + fieldIndex"
-          :field-id="field"
-          :field="availableBlocks[block.type].fields[field]"
-          v-model="block.data[field]"
-          v-on:change="onBlockChanged()"
-          :available-blocks="availableBlocks"
-          :block-index="getBlockIndex(index)"
-          :input-name="inputName"
-          :input-language="inputLanguage"
-          >
-        </page-block-editor-field>
+        <div v-for="(field, fieldIndex) in Object.keys(availableBlocks[block.type].fields)" :key="'block-' + getBlockIndexKey(index) + '-' + fieldIndex"
+            :class="{'multi-lingual': availableBlocks[block.type].fields[field].multi_lingual}">
+          <ul v-if="availableBlocks[block.type].fields[field].multi_lingual" class="field-language-picker">
+            <li v-for="language in Object.keys(languages)">
+              <a v-on:click.prevent="setActiveLanguageForField(block, field, language)" href="javascript:;" :title="languages[language]" :class="{'active': isActiveLanguageForField(block, field, language)}">
+                <span :class="'flag-icon flag-icon-' + lookupFlag(language)" ></span>
+              </a>
+            </li>
+          </ul>
+
+          <page-block-editor-field 
+            :field-id="field"
+            :field="availableBlocks[block.type].fields[field]"
+            v-model="block.data[field]"
+            v-on:change="onBlockChanged()"
+            :available-blocks="availableBlocks"
+            :block-index="getBlockIndex(index)"
+            :input-name="inputName"
+            :languages="languages"
+            :default-language="defaultLanguage"
+            v-if="isActiveLanguageForField(block, field, defaultLanguage)"
+            >
+          </page-block-editor-field>
+
+          <page-block-editor-field 
+            :field-id="field"
+            :field="availableBlocks[block.type].fields[field]"
+            v-model="block.i18n_data[getActiveLanguageForField(block, field)][field]"
+            v-on:change="onBlockChanged()"
+            :available-blocks="availableBlocks"
+            :block-index="getBlockIndex(index)"
+            :input-name="inputName"
+            :languages="languages"
+            :default-language="defaultLanguage"
+            v-if="!isActiveLanguageForField(block, field, defaultLanguage) && block.i18n_data[getActiveLanguageForField(block, field)]"
+            >
+          </page-block-editor-field>
+
+        </div>
       </div>
 
       <div class="buttons" style="display: flex; clear: both;" v-if="newBlockType">
         <div>
           <select class="form-control" v-model="newBlockType">
             <option v-for="(key, index) of Object.keys(availableBlocks)" :key="'block-' + getBlockIndexKey(index) + '-option'" :value="key">{{ availableBlocks[key].name }}</option>
           </select>
@@ -191,27 +226,55 @@
           <div class="small" v-if="newBlockType && newBlockType.description">
             {{ newBlockType.description }}
           </div>
         </div>
       </div>
     </div>
     `,
-        props: ['value', 'availableBlocks', 'blockIndex', 'inputName', 'inputLanguage'],
-        mixins: [TranslateMixin],
+        props: ['value', 'availableBlocks', 'blockIndex', 'inputName', 'languages', 'defaultLanguage'],
+        mixins: [TranslateMixin, FlagLookupMixin],
         data: function() {
             return {
                 newBlockType: null,
                 blocks: [],
+                activeLanguages: {}
             }
         },
         mounted: function() {
             this.newBlockType = this.availableBlocks ? Object.keys(this.availableBlocks)[0] : null;
             this.parseValue();
         },
         methods: {
+            setActiveLanguageForField: function(block, field, language) {
+                this.activeLanguages[field] = language;
+                if (!block.i18n_data) {
+                    block.i18n_data = {};
+                }
+                if (!block.i18n_data[language] && language !== this.defaultLanguage) {
+                    block.i18n_data[language] = {};
+                }
+                // if (!block.i18n_data[language][field]) {
+                //   block.i18n_data[language][field] = '';
+                // }
+
+                // Force an update
+                this.$forceUpdate();
+            },
+            getActiveLanguageForField: function(block, field) {
+                if (this.activeLanguages[field] === undefined) {
+                    return this.defaultLanguage;
+                }
+                return this.activeLanguages[field];
+            },
+            isActiveLanguageForField: function(block, field, language) {
+                if (this.activeLanguages[field] === undefined) {
+                    return language === this.defaultLanguage;
+                }
+                return this.activeLanguages[field] === language;
+            },
             parseValue: function() {
                 this.blocks = JSON.parse(JSON.stringify(this.value));
             },
             getBlockIndex: function(index) {
                 const parts = JSON.parse(JSON.stringify(this.blockIndex ? this.blockIndex : []));
                 parts.push(index);
                 return parts;
@@ -271,37 +334,25 @@
         }
     });
 
     Vue.component('page-block-editor', {
         template: `
     <div class="page-block-editor">
       <input type="hidden" :name="name" v-model="jsonValue" />
-      
-      <fieldset v-for="language in Object.keys(languages)">
-        <legend><span :class="'flag-icon flag-icon-' + lookupFlag(language)"></span> {{ languages[language] }}</legend>
-
-        <div class="copy-buttons" v-if="Object.keys(languages).length > 1">
-          {{ getText('labelCopyFrom') }}:
-          <button class="button" v-for="(button_language, button_index) in Object.keys(languages)" v-if="language !== button_language"
-              v-on:click.prevent="copyBlocks(button_language, language)">
-            {{ button_language }}
-          </button>
-        </div>
-      
-        <block-editor
-          v-model="blocks[language]"
-          :available-blocks="availableBlocks"
-          v-on:change="onFieldChanged()"
-          :input-name="name"
-          :input-language="language"></block-editor>
 
-      </fieldset>
+      <block-editor
+        v-model="blocks"
+        :available-blocks="availableBlocks"
+        v-on:change="onFieldChanged()"
+        :input-name="name"
+        :languages="languages"
+        :default-language="defaultLanguage"></block-editor>
 
     </div>`,
-        props: ['languages', 'initialValue', 'availableBlocks', 'name'],
+        props: ['languages', 'initialValue', 'availableBlocks', 'name', 'defaultLanguage'],
         mixins: [FlagLookupMixin, TranslateMixin],
         data: function() {
             return {
                 jsonValue: '[]',
                 blocks: {}
             };
         },
```

### Comparing `django-page-blocks-0.3.5/pageblocks/templates/admin/pageblocks/change_form.html` & `django-page-blocks-0.4.0/pageblocks/templates/admin/pageblocks/change_form.html`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/templatetags/__pycache__/pageblocks.cpython-310.pyc` & `django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/pageblocks.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar 13 19:39:21 2023 UTC, .py size: 1196 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e97b 0f64 ac04 0000  o........{.d....
+00000000: 6f0d 0d0a 0000 0000 b50b 6964 2a04 0000  o.........id*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6501 a00a a100  d.l.m.Z...e.....
 00000070: 5a0b 650b 6a0c 6407 6408 8400 8301 5a0d  Z.e.j.d.d.....Z.
@@ -19,83 +19,78 @@
 00000120: 0029 01da 0e42 6c6f 636b 5072 6f63 6573  .)...BlockProces
 00000130: 736f 7263 0100 0000 0000 0000 0000 0000  sorc............
 00000140: 0100 0000 0600 0000 4300 0000 7316 0000  ........C...s...
 00000150: 007c 00a0 0074 0183 007c 00a0 0074 026a  .|...t...|...t.j
 00000160: 03a1 01a1 0253 00a9 014e 2904 da03 6765  .....S...N)...ge
 00000170: 7472 0400 0000 7203 0000 00da 0d4c 414e  tr....r......LAN
 00000180: 4755 4147 455f 434f 4445 2901 da03 7661  GUAGE_CODE)...va
-00000190: 6ca9 0072 0c00 0000 fa2a 2f61 7070 2f70  l..r.....*/app/p
-000001a0: 6167 6562 6c6f 636b 732f 7465 6d70 6c61  ageblocks/templa
-000001b0: 7465 7461 6773 2f70 6167 6562 6c6f 636b  tetags/pageblock
-000001c0: 732e 7079 da09 6d75 6c74 696c 616e 670a  s.py..multilang.
-000001d0: 0000 0073 0200 0000 1602 720e 0000 0063  ...s......r....c
-000001e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000001f0: 0400 0000 4300 0000 f310 0000 0074 0074  ....C........t.t
-00000200: 0183 00a0 027c 00a1 0183 0153 0072 0800  .....|.....S.r..
-00000210: 0000 2903 7205 0000 0072 0700 0000 da06  ..).r....r......
-00000220: 7265 6e64 6572 a901 5a0b 7061 6765 5f62  render..Z.page_b
-00000230: 6c6f 636b 7372 0c00 0000 720c 0000 0072  locksr....r....r
-00000240: 0d00 0000 da06 626c 6f63 6b73 0f00 0000  ......blocks....
-00000250: f302 0000 0010 0272 1200 0000 6301 0000  .......r....c...
-00000260: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000270: 0043 0000 0072 0f00 0000 7208 0000 0029  .C...r....r....)
-00000280: 0372 0500 0000 7207 0000 00da 1272 656e  .r....r......ren
-00000290: 6465 725f 7363 7269 7074 5f74 6167 7372  der_script_tagsr
-000002a0: 1100 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-000002b0: 0000 00da 0d62 6c6f 636b 5f73 6372 6970  .....block_scrip
-000002c0: 7473 1300 0000 7213 0000 0072 1500 0000  ts....r....r....
-000002d0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000002e0: 0004 0000 0043 0000 0072 0f00 0000 7208  .....C...r....r.
-000002f0: 0000 0029 0372 0500 0000 7207 0000 00da  ...).r....r.....
-00000300: 1672 656e 6465 725f 7374 796c 6573 6865  .render_styleshe
-00000310: 6574 5f74 6167 7372 1100 0000 720c 0000  et_tagsr....r...
-00000320: 0072 0c00 0000 720d 0000 00da 1162 6c6f  .r....r......blo
-00000330: 636b 5f73 7479 6c65 7368 6565 7473 1700  ck_stylesheets..
-00000340: 0000 7213 0000 0072 1700 0000 6301 0000  ..r....r....c...
-00000350: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000360: 0043 0000 0073 2800 0000 7c00 a000 7401  .C...s(...|...t.
-00000370: 8300 a101 7d01 7c01 a002 a100 6401 6b02  ....}.|.....d.k.
-00000380: 7212 7c00 a000 7403 6a04 a101 7d01 7c01  r.|...t.j...}.|.
-00000390: 5300 2902 4e72 0100 0000 2905 da17 6765  S.).Nr....)...ge
-000003a0: 745f 626c 6f63 6b73 5f66 6f72 5f6c 616e  t_blocks_for_lan
-000003b0: 6775 6167 6572 0400 0000 da05 636f 756e  guager......coun
-000003c0: 7472 0300 0000 720a 0000 0029 02da 0470  tr....r....)...p
-000003d0: 6167 65da 0271 7372 0c00 0000 720c 0000  age..qsr....r...
-000003e0: 0072 0d00 0000 da13 6765 745f 626c 6f63  .r......get_bloc
-000003f0: 6b73 5f66 6f72 5f70 6167 651c 0000 0073  ks_for_page....s
-00000400: 0800 0000 0c01 0c01 0c01 0401 721c 0000  ............r...
-00000410: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000420: 0000 0300 0000 4300 0000 f30c 0000 0074  ......C........t
-00000430: 0074 017c 0083 0183 0153 0072 0800 0000  .t.|.....S.r....
-00000440: 2902 7212 0000 0072 1c00 0000 a901 721a  ).r....r......r.
-00000450: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000460: 0000 da0a 7061 6765 626c 6f63 6b73 2200  ....pageblocks".
-00000470: 0000 f302 0000 000c 0272 1f00 0000 6301  .........r....c.
-00000480: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000490: 0000 0043 0000 0072 1d00 0000 7208 0000  ...C...r....r...
-000004a0: 0029 0272 1500 0000 721c 0000 0072 1e00  .).r....r....r..
-000004b0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-000004c0: 00da 1270 6167 6562 6c6f 636b 735f 7363  ...pageblocks_sc
-000004d0: 7269 7074 7326 0000 0072 2000 0000 7221  ripts&...r ...r!
-000004e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000004f0: 0100 0000 0300 0000 4300 0000 721d 0000  ........C...r...
-00000500: 0072 0800 0000 2902 7217 0000 0072 1c00  .r....).r....r..
-00000510: 0000 721e 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00000520: 0072 0d00 0000 da16 7061 6765 626c 6f63  .r......pagebloc
-00000530: 6b73 5f73 7479 6c65 7368 6565 7473 2a00  ks_stylesheets*.
-00000540: 0000 7220 0000 0072 2200 0000 4e29 14da  ..r ...r"...N)..
-00000550: 0664 6a61 6e67 6f72 0200 0000 da0b 646a  .djangor......dj
-00000560: 616e 676f 2e63 6f6e 6672 0300 0000 da18  ango.confr......
-00000570: 646a 616e 676f 2e75 7469 6c73 2e74 7261  django.utils.tra
-00000580: 6e73 6c61 7469 6f6e 7204 0000 00da 1764  nslationr......d
-00000590: 6a61 6e67 6f2e 7574 696c 732e 7361 6665  jango.utils.safe
-000005a0: 7374 7269 6e67 7205 0000 0072 1200 0000  stringr....r....
-000005b0: 7207 0000 00da 074c 6962 7261 7279 da08  r......Library..
-000005c0: 7265 6769 7374 6572 da0a 7369 6d70 6c65  register..simple
-000005d0: 5f74 6167 720e 0000 0072 1500 0000 7217  _tagr....r....r.
-000005e0: 0000 0072 1c00 0000 721f 0000 0072 2100  ...r....r....r!.
-000005f0: 0000 7222 0000 0072 0c00 0000 720c 0000  ..r"...r....r...
-00000600: 0072 0c00 0000 720d 0000 00da 083c 6d6f  .r....r......<mo
-00000610: 6475 6c65 3e01 0000 0073 2a00 0000 0c00  dule>....s*.....
-00000620: 0c01 0c01 0c01 0c02 0802 0402 0a01 0404  ................
-00000630: 0a01 0403 0a01 0403 0a01 0804 0406 0a01  ................
-00000640: 0403 0a01 0403 0e01                      ........
+00000190: 6ca9 0072 0c00 0000 fa2b 2f63 6f64 652f  l..r.....+/code/
+000001a0: 7061 6765 626c 6f63 6b73 2f74 656d 706c  pageblocks/templ
+000001b0: 6174 6574 6167 732f 7061 6765 626c 6f63  atetags/pagebloc
+000001c0: 6b73 2e70 79da 096d 756c 7469 6c61 6e67  ks.py..multilang
+000001d0: 0a00 0000 7302 0000 0016 0272 0e00 0000  ....s......r....
+000001e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000001f0: 0004 0000 0043 0000 00f3 1000 0000 7400  .....C........t.
+00000200: 7401 8300 a002 7c00 a101 8301 5300 7208  t.....|.....S.r.
+00000210: 0000 0029 0372 0500 0000 7207 0000 00da  ...).r....r.....
+00000220: 0672 656e 6465 72a9 015a 0b70 6167 655f  .render..Z.page_
+00000230: 626c 6f63 6b73 720c 0000 0072 0c00 0000  blocksr....r....
+00000240: 720d 0000 00da 0662 6c6f 636b 730f 0000  r......blocks...
+00000250: 00f3 0200 0000 1002 7212 0000 0063 0100  ........r....c..
+00000260: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000270: 0000 4300 0000 720f 0000 0072 0800 0000  ..C...r....r....
+00000280: 2903 7205 0000 0072 0700 0000 da12 7265  ).r....r......re
+00000290: 6e64 6572 5f73 6372 6970 745f 7461 6773  nder_script_tags
+000002a0: 7211 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+000002b0: 0d00 0000 da0d 626c 6f63 6b5f 7363 7269  ......block_scri
+000002c0: 7074 7313 0000 0072 1300 0000 7215 0000  pts....r....r...
+000002d0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+000002e0: 0000 0400 0000 4300 0000 720f 0000 0072  ......C...r....r
+000002f0: 0800 0000 2903 7205 0000 0072 0700 0000  ....).r....r....
+00000300: da16 7265 6e64 6572 5f73 7479 6c65 7368  ..render_stylesh
+00000310: 6565 745f 7461 6773 7211 0000 0072 0c00  eet_tagsr....r..
+00000320: 0000 720c 0000 0072 0d00 0000 da11 626c  ..r....r......bl
+00000330: 6f63 6b5f 7374 796c 6573 6865 6574 7317  ock_stylesheets.
+00000340: 0000 0072 1300 0000 7217 0000 0063 0100  ...r....r....c..
+00000350: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000360: 0000 4300 0000 7308 0000 007c 00a0 00a1  ..C...s....|....
+00000370: 0053 0072 0800 0000 2901 da0a 6765 745f  .S.r....)...get_
+00000380: 626c 6f63 6b73 a901 da04 7061 6765 720c  blocks....pager.
+00000390: 0000 0072 0c00 0000 720d 0000 00da 1367  ...r....r......g
+000003a0: 6574 5f62 6c6f 636b 735f 666f 725f 7061  et_blocks_for_pa
+000003b0: 6765 1b00 0000 7302 0000 0008 0172 1b00  ge....s......r..
+000003c0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+000003d0: 0000 0003 0000 0043 0000 00f3 0c00 0000  .......C........
+000003e0: 7400 7401 7c00 8301 8301 5300 7208 0000  t.t.|.....S.r...
+000003f0: 0029 0272 1200 0000 721b 0000 0072 1900  .).r....r....r..
+00000400: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000410: 00da 0a70 6167 6562 6c6f 636b 731e 0000  ...pageblocks...
+00000420: 00f3 0200 0000 0c02 721d 0000 0063 0100  ........r....c..
+00000430: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000440: 0000 4300 0000 721c 0000 0072 0800 0000  ..C...r....r....
+00000450: 2902 7215 0000 0072 1b00 0000 7219 0000  ).r....r....r...
+00000460: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000470: da12 7061 6765 626c 6f63 6b73 5f73 6372  ..pageblocks_scr
+00000480: 6970 7473 2200 0000 721e 0000 0072 1f00  ipts"...r....r..
+00000490: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+000004a0: 0000 0003 0000 0043 0000 0072 1c00 0000  .......C...r....
+000004b0: 7208 0000 0029 0272 1700 0000 721b 0000  r....).r....r...
+000004c0: 0072 1900 0000 720c 0000 0072 0c00 0000  .r....r....r....
+000004d0: 720d 0000 00da 1670 6167 6562 6c6f 636b  r......pageblock
+000004e0: 735f 7374 796c 6573 6865 6574 7326 0000  s_stylesheets&..
+000004f0: 0072 1e00 0000 7220 0000 004e 2914 da06  .r....r ...N)...
+00000500: 646a 616e 676f 7202 0000 00da 0b64 6a61  djangor......dja
+00000510: 6e67 6f2e 636f 6e66 7203 0000 00da 1864  ngo.confr......d
+00000520: 6a61 6e67 6f2e 7574 696c 732e 7472 616e  jango.utils.tran
+00000530: 736c 6174 696f 6e72 0400 0000 da17 646a  slationr......dj
+00000540: 616e 676f 2e75 7469 6c73 2e73 6166 6573  ango.utils.safes
+00000550: 7472 696e 6772 0500 0000 7212 0000 0072  tringr....r....r
+00000560: 0700 0000 da07 4c69 6272 6172 79da 0872  ......Library..r
+00000570: 6567 6973 7465 72da 0a73 696d 706c 655f  egister..simple_
+00000580: 7461 6772 0e00 0000 7215 0000 0072 1700  tagr....r....r..
+00000590: 0000 721b 0000 0072 1d00 0000 721f 0000  ..r....r....r...
+000005a0: 0072 2000 0000 720c 0000 0072 0c00 0000  .r ...r....r....
+000005b0: 720c 0000 0072 0d00 0000 da08 3c6d 6f64  r....r......<mod
+000005c0: 756c 653e 0100 0000 732a 0000 000c 000c  ule>....s*......
+000005d0: 010c 010c 010c 0208 0204 020a 0104 040a  ................
+000005e0: 0104 030a 0104 030a 0108 0304 030a 0104  ................
+000005f0: 030a 0104 030e 01                        .......
```

### Comparing `django-page-blocks-0.3.5/pageblocks/templatetags/__pycache__/pageblocks.cpython-39.pyc` & `django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/pageblocks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/pageblocks/templatetags/pageblocks.py` & `django-page-blocks-0.4.0/pageblocks/templatetags/pageblocks.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,20 +20,16 @@
 def block_scripts(page_blocks):
     return mark_safe(BlockProcessor().render_script_tags(page_blocks))
 
 @register.simple_tag
 def block_stylesheets(page_blocks):
     return mark_safe(BlockProcessor().render_stylesheet_tags(page_blocks))
 
-
 def get_blocks_for_page(page):
-    qs = page.get_blocks_for_language(get_language())
-    if qs.count() == 0:
-        qs = page.get_blocks_for_language(settings.LANGUAGE_CODE)
-    return qs
+    return page.get_blocks()
 
 @register.simple_tag
 def pageblocks(page):
     return blocks(get_blocks_for_page(page))
 
 @register.simple_tag
 def pageblocks_scripts(page):
```

### Comparing `django-page-blocks-0.3.5/pageblocks/tests.py` & `django-page-blocks-0.4.0/pageblocks/tests.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 from . import PAGEBLOCKS_DEFAULT_AVAILABLE
 
 class AvailableBlockTestCase(TestCase):
     """
     Test logic to get available block types, with and without overridden settings
     """
 
-    def test_without_settings_override(self):
-        self.assertEqual(Page.get_available_block_type_classes(), PAGEBLOCKS_DEFAULT_AVAILABLE)
-
     @override_settings(PAGEBLOCKS_AVAILABLE_BLOCKS=[
         'pageblocks.blocks.RawHTMLBlock'
     ])
     def test_with_settings_override(self):
         self.assertEqual(Page.get_available_block_type_classes(), [
             'pageblocks.blocks.RawHTMLBlock'
         ])
@@ -42,129 +39,166 @@
         self.assertEqual(page.title['es'], 'prueba')
         self.assertTrue(page.slug is not None)
         self.assertEqual(page.slug, 'test')
 
     def test_create_basic_page(self):
         form = PageAdminForm(data={
             'slug': 'basic_page',
-            'title': {"es":"prueba", "en":"test"},
-            'blocks': {"es":[{"type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>Es una prueba</b>"}},{"type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>Es una prueba otra vez</b>"}}],"en":[{"type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>This is a test</b>"}}]}
+            'title': {"es": "prueba", "en": "test"},
+            'blocks': [
+                {
+                    'type': 'pageblocks.blocks.HTMLBlock',
+                    'data': {
+                        'html': '<b>This is a test</b>'
+                    },
+                    'i18n_data': {}
+                },
+                {
+                    'type': 'pageblocks.blocks.HTMLBlock',
+                    'data': {
+                        'html': '<b>Second block</b>'
+                    },
+                    'i18n_data': {
+                        'es': {
+                            'html': '<b>Segundo bloque</b>'
+                        }
+                    }
+                },
+            ]
         })
         self.assertTrue(form.is_valid(), form.errors)
         with translation_override('en'):
             page = form.save()
 
         self.assertEqual(page.slug, 'basic_page')
 
-        self.assertEqual(page.blocks.filter(language='en').count(), 1)
-        self.assertEqual(page.blocks.filter(language='es').count(), 2)
+        self.assertEqual(page.blocks.filter().count(), 2)
 
-        self.assertEqual(page.blocks.filter(language='en')[0].data['html'], '<b>This is a test</b>')
-        self.assertEqual(page.blocks.filter(language='en')[0].index, 0)
+        self.assertEqual(page.blocks.filter()[0].data['html'], '<b>This is a test</b>')
+        self.assertEqual(page.blocks.filter()[0].index, 0)
 
-        self.assertEqual(page.blocks.filter(language='es')[0].data['html'], '<b>Es una prueba</b>')
-        self.assertEqual(page.blocks.filter(language='es')[0].index, 0)
-        self.assertEqual(page.blocks.filter(language='es')[1].data['html'], '<b>Es una prueba otra vez</b>')
-        self.assertEqual(page.blocks.filter(language='es')[1].index, 1)
+        self.assertEqual(page.blocks.filter()[1].data['html'], '<b>Second block</b>')
+        self.assertEqual(page.blocks.filter()[1].i18n_data['es']['html'], '<b>Segundo bloque</b>')
+        self.assertEqual(page.blocks.filter()[1].index, 1)
 
     # TODO: Test editing a page .. does it load the blocks properly
     def test_editing_basic_page(self):
         PageBlock.objects.all().delete()
 
         form = PageAdminForm(data={
             'slug': 'basic_page',
             'title': {"es":"prueba", "en":"test"},
-            'blocks': {"es":[{"type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>Es una prueba</b>"}},{"type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>Es una prueba otra vez</b>"}}],"en":[{"type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>This is a test</b>"}}]}
+            'blocks': [
+                {
+                    'type': 'pageblocks.blocks.HTMLBlock',
+                    'data': {
+                        'html': '<b>This is a test</b>'
+                    },
+                    'i18n_data': {}
+                },
+                {
+                    'type': 'pageblocks.blocks.HTMLBlock',
+                    'data': {
+                        'html': '<b>Second block</b>'
+                    },
+                    'i18n_data': {
+                        'es': {
+                            'html': '<b>Segundo bloque</b>'
+                        }
+                    }
+                },
+            ]
         })
         self.assertTrue(form.is_valid(), form.errors)
         with translation_override('en'):
             page = form.save()
 
-        self.assertEqual(PageBlock.objects.all().count(), 3)
+        self.assertEqual(PageBlock.objects.all().count(), 2)
 
         form = PageAdminForm(instance=page)
-        block_edit_data = {"es":[
-            {"id": str(page.blocks.filter(language="es")[0].id), "type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>Es una prueba</b>"}},
-            {"id": str(page.blocks.filter(language="es")[1].id), "type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>Es una prueba otra vez</b>"}}
-        ],"en":
-        [
-            {"id": str(page.blocks.filter(language="en")[0].id), "type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>This is a test</b>"}}
-        ]}
-        self.assertDictEqual(form.fields['blocks'].initial, block_edit_data)
+        block_edit_data = [
+            {"id": str(page.blocks.filter()[0].id), 'type': 'pageblocks.blocks.HTMLBlock', 'data': {'html': '<b>This is a test</b>'}, 'i18n_data': {}},
+            {"id": str(page.blocks.filter()[1].id), "type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>Second block</b>"},"i18n_data":{"es":{"html":"<b>Segundo bloque</b>"}}}
+        ]
+        self.assertDictEqual(form.fields['blocks'].initial[0], block_edit_data[0])
+        self.assertDictEqual(form.fields['blocks'].initial[1], block_edit_data[1])
 
-        block_edit_data['es'][0]['data']['html'] = '<b>He cambiado!</b>'
-        del block_edit_data['es'][1]
+        block_edit_data[0]['i18n_data']['es'] = {'html': '<b>He cambiado!</b>'}
+        del block_edit_data[1]
 
-        block_edit_data['en'].append(
-            {"type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>This is a new block</b>"}}
+        block_edit_data.append(
+            {"type": "pageblocks.blocks.HTMLBlock", "data": {"html": "<b>This is a new block</b>"}}
         )
 
         form = PageAdminForm(instance=page, data={
             'slug': 'basic_page',
-            'title': {"es":"prueba", "en":"test"},
+            'title': {"es": "prueba", "en": "test"},
             'blocks': block_edit_data
         })
         self.assertTrue(form.is_valid(), form.errors)
 
         page = form.save()
 
-        self.assertEqual(page.blocks.filter(language='en').count(), 2)
-        self.assertEqual(page.blocks.filter(language='es').count(), 1)
-
-        self.assertEqual(page.blocks.filter(language='en')[0].data['html'], '<b>This is a test</b>')
-        self.assertEqual(page.blocks.filter(language='en')[0].index, 0)
-        self.assertEqual(page.blocks.filter(language='en')[1].data['html'], '<b>This is a new block</b>')
-        self.assertEqual(page.blocks.filter(language='en')[1].index, 1)
+        self.assertEqual(page.blocks.filter().count(), 2)
 
-        self.assertEqual(page.blocks.filter(language='es')[0].data['html'], '<b>He cambiado!</b>')
-        self.assertEqual(page.blocks.filter(language='es')[0].index, 0)
+        self.assertEqual(page.blocks.filter()[0].data['html'], '<b>This is a test</b>')
+        self.assertEqual(page.blocks.filter()[0].i18n_data['es']['html'], '<b>He cambiado!</b>')
+        self.assertEqual(page.blocks.filter()[0].index, 0)
+        self.assertEqual(page.blocks.filter()[1].data['html'], '<b>This is a new block</b>')
+        self.assertEqual(page.blocks.filter()[1].index, 1)
 
     def test_create_page_missing_required_field(self):
         form = PageAdminForm(data={
             'slug': 'basic_page',
             'title': {"es":"prueba", "en":"test"},
-            'blocks': {"es":[],"en":[
-                {"type":"pageblocks.blocks.HTMLBlock","data":{}}
-            ]}
+            'blocks': [
+                {
+                    'type': 'pageblocks.blocks.HTMLBlock',
+                    'data': {
+                    }
+                }
+            ]
         })
         with translation_override('en'):
             self.assertFalse(form.is_valid(), 'Form validated when it shouldn\'t have')
-            self.assertEqual(form.errors['blocks'].as_text(), '* B:en:0:html:This field is required')
+            self.assertEqual(form.errors['blocks'].as_text(), '* B:0:html:This field is required')
 
     def test_create_page_with_nested_blocks(self):
         """ ContainerBlocks are special block types which allow other blocks to be embedded within them """
 
-        block_edit_data = {"es":[],"en":[
+        block_edit_data = [
             {
                 "type": "pageblocks.blocks.ContainerBlock",
                 "data": {
                     "class": "col-12",
                     "blocks": [
                         {
-                            "type":"pageblocks.blocks.HTMLBlock","data":{"html":"<b>This is a sub block</b>"}
+                            "type": "pageblocks.blocks.HTMLBlock", "data": {"html": "<b>This is a sub block</b>"},
+                            "i18n_data": {
+                                "es": {
+                                    "html": "<b>Este es un sub bloque</b>"
+                                }
+                            }
                         }
                     ]
                 }
             }
-        ]}
+        ]
+
         form = PageAdminForm(data={
             'slug': 'basic_page',
-            'title': {"es":"prueba", "en":"test"},
+            'title': {"es": "prueba", "en": "test"},
             'blocks': block_edit_data
         })
         self.assertTrue(form.is_valid(), form.errors)
         with translation_override('en'):
             page = form.save()
 
         self.assertEqual(page.slug, 'basic_page')
 
-        self.assertEqual(page.blocks.filter(language='en').count(), 2)
-        self.assertEqual(page.blocks.filter(language='en', parent=None).count(), 1)
-
-        block_edit_data['en'][0]['id'] = str(page.blocks.filter(language='en', parent=None).first().id)
-        block_edit_data['en'][0]['data']['blocks'][0]['id'] = str(page.blocks.filter(language='en').exclude(parent=None).first().id)
-
-        form = PageAdminForm(instance=page)
-        self.assertDictEqual(form.fields['blocks'].initial, block_edit_data)
+        self.assertEqual(page.blocks.filter().count(), 2)
+        self.assertEqual(page.blocks.filter(parent=None).count(), 1)
 
+        self.assertEqual(page.blocks.exclude(parent=None)[0].data['html'], '<b>This is a sub block</b>')
+        self.assertEqual(page.blocks.exclude(parent=None)[0].i18n_data['es']['html'], '<b>Este es un sub bloque</b>')
 
     # TODO: Test creating a page with a required block field (or type) missing
```

### Comparing `django-page-blocks-0.3.5/pageblocks/views.py` & `django-page-blocks-0.4.0/pageblocks/views.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.3.5/setup.py` & `django-page-blocks-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-page-blocks',
-    version='0.3.5',
+    version='0.4.0',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
-    description='A simple, Wagtail CMS inspired content block engine for Django.  Intended to give slightly more control than regular flatpages.',
+    description='A simple, Wagtail CMS inspired multi language content block engine for Django.  Intended to give slightly more control than regular flatpages.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/bravasoftware/django-page-blocks',
     author='Mark Skelton',
     author_email='studio@bravasoftware.com',
     classifiers=[
         'Environment :: Web Environment',
```

