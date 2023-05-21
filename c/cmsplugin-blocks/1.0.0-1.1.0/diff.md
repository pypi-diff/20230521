# Comparing `tmp/cmsplugin-blocks-1.0.0.tar.gz` & `tmp/cmsplugin-blocks-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmsplugin-blocks-1.0.0.tar", last modified: Wed Apr 26 20:11:24 2023, max compression
+gzip compressed data, was "cmsplugin-blocks-1.1.0.tar", last modified: Sun May 21 00:04:46 2023, max compression
```

## Comparing `cmsplugin-blocks-1.0.0.tar` & `cmsplugin-blocks-1.1.0.tar`

### file list

```diff
@@ -1,109 +1,114 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1057 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/LICENCE.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      337 2021-08-10 12:34:03.000000 cmsplugin-blocks-1.0.0/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3302 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1841 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/README.rst
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      179 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1365 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1854 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/slider.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      598 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/apps.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1782 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/choices_helpers.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      839 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/cms_plugins.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/contrib/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/contrib/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2317 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/contrib/django_configuration.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3546 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/defaults.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      756 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/exceptions.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      418 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1752 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1297 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1119 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/container.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1028 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2090 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/slider.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      387 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/user.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      327 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3371 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      950 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      930 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/container.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      874 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1611 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/slider.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1926 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3560 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6408 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0001_initial.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      447 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0002_add_slide_item_order.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      432 2023-04-26 20:09:50.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0003_slideitem_title.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1690 2023-04-26 20:09:50.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    10292 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0005_v1-0-0_changes.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-25 23:04:05.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2925 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/modelfields.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      271 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5838 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3855 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3555 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/container.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3285 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6136 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/slider.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2078 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1776 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1582 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/container.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1369 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1579 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/slider.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1181 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1246 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/container.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1181 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2577 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1557 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/js/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2612 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4081 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       49 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      856 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/test.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       48 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      980 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/test.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       53 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1037 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/test.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       48 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/test.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       50 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1266 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      385 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4372 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/archive.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4859 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/cms_tests.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2558 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/factories.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     7647 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/tests.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4058 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/validators.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3302 2023-04-26 20:11:24.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3371 2023-04-26 20:11:24.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-04-26 20:11:24.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      212 2023-04-26 20:11:24.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       25 2023-04-26 20:11:24.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-04-24 20:19:54.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/zip-safe
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2200 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2021-08-10 12:34:03.000000 cmsplugin-blocks-1.0.0/setup.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1057 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/LICENCE.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      337 2021-08-10 12:34:03.000000 cmsplugin-blocks-1.1.0/MANIFEST.in
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3353 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1853 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/README.rst
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      179 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1365 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1854 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/slider.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      598 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/apps.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1782 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/choices_helpers.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      839 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/cms_plugins.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/contrib/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/contrib/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2317 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/contrib/django_configuration.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3546 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/defaults.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      756 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/exceptions.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      418 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1752 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1297 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1119 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1028 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2090 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/slider.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      387 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/user.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      327 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3554 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1217 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1197 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1141 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2145 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/slider.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3770 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/django.pot
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/en/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3817 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2318 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4533 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6408 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0001_initial.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      447 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0002_add_slide_item_order.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      432 2023-04-26 20:09:50.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0003_slideitem_title.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1690 2023-04-26 20:09:50.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    10292 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0005_v1-0-0_changes.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-25 23:04:05.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2925 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/modelfields.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      271 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5641 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3668 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3358 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3098 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5939 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/slider.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2142 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1840 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1646 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1433 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1643 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/slider.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1181 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1246 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/container.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1181 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2577 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1557 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/js/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2612 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4081 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       49 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      856 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       48 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      980 2023-05-20 20:36:28.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       53 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1037 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       48 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       50 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1266 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      385 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4372 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/archive.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4859 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/cms_tests.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2558 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/factories.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     7647 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/tests.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4058 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/validators.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3353 2023-05-21 00:04:46.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3504 2023-05-21 00:04:46.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/SOURCES.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-05-21 00:04:46.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/dependency_links.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      219 2023-05-21 00:04:46.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/requires.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       25 2023-05-21 00:04:46.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/top_level.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-04-24 20:19:54.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/zip-safe
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2266 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/setup.cfg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2021-08-10 12:34:03.000000 cmsplugin-blocks-1.1.0/setup.py
```

### Comparing `cmsplugin-blocks-1.0.0/LICENCE.txt` & `cmsplugin-blocks-1.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/PKG-INFO` & `cmsplugin-blocks-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsplugin-blocks
-Version: 1.0.0
+Version: 1.1.0
 Summary: A set of DjangoCMS plugins for structured contents in CMS pages
 Home-page: https://github.com/emencia/cmsplugin-blocks
 Author: David Thenon
 Author-email: dthenon@emencia.com
 License: MIT
 Project-URL: Source Code, https://github.com/emencia/cmsplugin-blocks
 Project-URL: Issue Tracker, https://github.com/emencia/cmsplugin-blocks/issues
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: quality
 Provides-Extra: doc
@@ -77,17 +78,17 @@
 
 
 Dependancies
 ************
 
 * Python>=3.8;
 * Django>=3.2;
-* `DjangoCMS`_ >= 3.11.0;
-* `djangocms-text-ckeditor`_;
-* `django-smart-media`_;
+* `DjangoCMS`_>=3.11.0;
+* `djangocms-text-ckeditor`_>=5.0.1;
+* `django-smart-media`_>=0.3.0;
 
 
 Links
 *****
 
 * Read the documentation on `Read the docs <https://cmspluginblocks.readthedocs.io/>`_;
 * Download its `PyPi package <https://pypi.python.org/pypi/cmsplugin-blocks>`_;
```

### Comparing `cmsplugin-blocks-1.0.0/README.rst` & `cmsplugin-blocks-1.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 
 
 Dependancies
 ************
 
 * Python>=3.8;
 * Django>=3.2;
-* `DjangoCMS`_ >= 3.11.0;
-* `djangocms-text-ckeditor`_;
-* `django-smart-media`_;
+* `DjangoCMS`_>=3.11.0;
+* `djangocms-text-ckeditor`_>=5.0.1;
+* `django-smart-media`_>=0.3.0;
 
 
 Links
 *****
 
 * Read the documentation on `Read the docs <https://cmspluginblocks.readthedocs.io/>`_;
 * Download its `PyPi package <https://pypi.python.org/pypi/cmsplugin-blocks>`_;
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/album.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/album.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/slider.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/slider.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/apps.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/apps.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/choices_helpers.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/choices_helpers.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/cms_plugins.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/contrib/django_configuration.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/contrib/django_configuration.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/defaults.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/defaults.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/exceptions.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/exceptions.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/album.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/album.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/card.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/card.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/container.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/container.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/hero.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/hero.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/slider.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/slider.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/album.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/album.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,19 +38,43 @@
         label=_("Add items from a ZIP"),
         max_length=100,
         required=False,
         help_text=_("Select a '*.zip' file of images to upload as new items."),
         widget=FileInputButtonBase,
     )
 
+    class Meta:
+        model = Album
+        exclude = []
+        fields = [
+            "title",
+            "template",
+            "features",
+            "mass_upload",
+        ]
+        widgets = {
+            "features": forms.SelectMultiple,
+            "order": NumberInput(attrs={"style": "width: 80px !important;"}),
+        }
+
+    class Media:
+        css = {
+            "all": ("cmsplugin_blocks/css/admin/album.css",),
+        }
+
     def __init__(self, *args, **kwargs):
         self.uploaded_zip = None
 
         super().__init__(*args, **kwargs)
 
+        # Get back original model field name onto the field
+        self.fields["features"].label = (
+            self._meta.model._meta.get_field("features").verbose_name
+        )
+
     def clean_mass_upload(self):
         """
         Validate uploaded ZIP archive file and temporary store it to
         "uploaded_zip" form object attribute if valid.
         """
         data = self.cleaned_data["mass_upload"]
 
@@ -71,33 +95,14 @@
             "album",
             "image",
             label_attrname="title"
         )
 
         return album
 
-    class Meta:
-        model = Album
-        exclude = []
-        fields = [
-            "title",
-            "template",
-            "features",
-            "mass_upload",
-        ]
-        widgets = {
-            "features": forms.SelectMultiple,
-            "order": NumberInput(attrs={"style": "width: 80px !important;"}),
-        }
-
-    class Media:
-        css = {
-            "all": ("cmsplugin_blocks/css/admin/album.css",),
-        }
-
 
 class AlbumItemForm(forms.ModelForm):
     # Enforce the right field since ModelAdmin ignore the formfield defined in custom
     # modelfield. Option have to fit to the modelfield ones.
     features = forms.MultipleChoiceField(
         choices=get_albumitem_feature_choices(),
         required=False,
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/container.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/container.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,7 +29,15 @@
             "features": forms.SelectMultiple,
         }
 
     class Media:
         css = {
             "all": ("cmsplugin_blocks/css/admin/container.css",),
         }
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Get back original model field name onto the field
+        self.fields["features"].label = (
+            self._meta.model._meta.get_field("features").verbose_name
+        )
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/hero.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/card.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 from django import forms
 
 from djangocms_text_ckeditor.widgets import TextEditorWidget
 
-from ..choices_helpers import get_hero_feature_choices
-from ..models.hero import Hero
+from ..choices_helpers import get_card_feature_choices
+from ..models.card import Card
 
 
-class HeroForm(forms.ModelForm):
+class CardForm(forms.ModelForm):
     # Enforce the right field since ModelAdmin ignore the formfield defined in custom
     # modelfield. Option have to fit to the modelfield ones.
     features = forms.MultipleChoiceField(
-        choices=get_hero_feature_choices(),
+        choices=get_card_feature_choices(),
         required=False,
     )
 
     class Meta:
-        model = Hero
+        model = Card
         exclude = []
         fields = [
+            "title",
             "template",
             "features",
             "image",
             "content",
+            "link_url",
+            "link_open_blank",
         ]
         widgets = {
             "content": TextEditorWidget,
             "features": forms.SelectMultiple,
         }
 
     class Media:
         css = {
-            "all": ("cmsplugin_blocks/css/admin/hero.css",),
+            "all": ("cmsplugin_blocks/css/admin/card.css",),
         }
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Get back original model field name onto the field
+        self.fields["features"].label = (
+            self._meta.model._meta.get_field("features").verbose_name
+        )
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -4,148 +4,183 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-03-08 16:14+0100\n"
+"POT-Creation-Date: 2023-05-20 01:57+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: cms_plugins.py:73 cms_plugins.py:112 cms_plugins.py:141 cms_plugins.py:198
-msgid "Blocks"
-msgstr "Blocs"
-
-#: cms_plugins.py:74 models/album.py:52
-msgid "Album"
-msgstr ""
-
-#: cms_plugins.py:113 models/card.py:63
-msgid "Card"
-msgstr ""
-
-#: cms_plugins.py:142 models/hero.py:51
-msgid "Hero"
-msgstr ""
-
-#: cms_plugins.py:199 models/slider.py:52
-msgid "Slider"
+#: admin/album.py:18 models/album.py:160 models/card.py:68
+#: models/container.py:57 models/hero.py:57 models/slider.py:142
+msgid "Image"
 msgstr ""
 
-#: forms/album.py:32
-msgid "Add items from a ZIP file"
-msgstr "Import depuis un fichier ZIP"
+#: admin/slider.py:18
+msgid "Slide"
+msgstr "Slider"
+
+#: forms/album.py:38
+msgid "Add items from a ZIP"
+msgstr "Importer depuis un fichier ZIP"
 
-#: forms/album.py:35
+#: forms/album.py:41
 msgid "Select a '*.zip' file of images to upload as new items."
 msgstr "Fichier '*.zip' contenant des images à ajouter."
 
-#: models/album.py:19 models/album.py:66 models/slider.py:19
+#: models/album.py:46 models/album.py:129 models/card.py:33
+#: models/container.py:34 models/slider.py:37 models/slider.py:120
 msgid "Title"
 msgstr "Titre"
 
-#: models/album.py:25 models/card.py:31 models/hero.py:19 models/slider.py:25
+#: models/album.py:56 models/card.py:43 models/container.py:44
+#: models/hero.py:32 models/slider.py:47
 msgid "Template"
 msgstr "Gabarits"
 
-#: models/album.py:30
+#: models/album.py:61
 msgid "Used template for content formatting."
 msgstr "Gabarit HTML spécifique pour la mise en forme."
 
-#: models/album.py:53
+#: models/album.py:69 models/album.py:148 models/card.py:56
+#: models/container.py:79 models/hero.py:45 models/slider.py:60
+#: models/slider.py:130
+msgid "Layout features"
+msgstr "Fonctionnalités d'apparence"
+
+#: models/album.py:114 plugins/album.py:23
+msgid "Album"
+msgstr ""
+
+#: models/album.py:115
 msgid "Albums"
 msgstr ""
 
-#: models/album.py:72
+#: models/album.py:139 models/slider.py:164
 msgid "Order"
 msgstr "Ordre"
 
-#: models/album.py:77 models/card.py:39 models/hero.py:27 models/slider.py:67
-msgid "Image"
-msgstr ""
-
-#: models/album.py:89
+#: models/album.py:194
 msgid "Album item"
 msgstr "Élément d'album"
 
-#: models/album.py:90
+#: models/album.py:195
 msgid "Album items"
 msgstr "Éléments de l'album"
 
-#: models/card.py:19
-msgid "Content to the left, image to the right"
-msgstr "Contenu à gauche, image à droite"
-
-#: models/card.py:20
-msgid "Image to the left, content to the reft"
-msgstr "Image à gauche, contenu à droite"
-
-#: models/card.py:24
-msgid "Alignment"
-msgstr "Alignement"
-
-#: models/card.py:36 models/hero.py:24 models/slider.py:30
+#: models/card.py:48 models/container.py:49 models/hero.py:37
+#: models/slider.py:52
 msgid "Used template for content look."
 msgstr "Gabarit HTML spécifique pour la mise en forme."
 
-#: models/card.py:47 models/hero.py:35 models/slider.py:75
+#: models/card.py:81 models/container.py:70 models/hero.py:70
+#: models/slider.py:155
 msgid "Content"
 msgstr "Contenu"
 
-#: models/card.py:64
+#: models/card.py:90
+msgid "Link url"
+msgstr "URL du lien"
+
+#: models/card.py:99
+msgid "Open in new window"
+msgstr "Ouvrir dans une nouvelle fenêtre"
+
+#: models/card.py:101
+msgid "If checked the link will be opened in a new window"
+msgstr "Si coché, le lien sera ouvert dans une nouvelle fenêtre"
+
+#: models/card.py:133 plugins/card.py:17
+msgid "Card"
+msgstr ""
+
+#: models/card.py:134
 msgid "Cards"
 msgstr ""
 
-#: models/hero.py:52
+#: models/container.py:116 plugins/container.py:17
+msgid "Container"
+msgstr "Conteneur"
+
+#: models/container.py:117
+msgid "Containers"
+msgstr "Conteneurs"
+
+#: models/hero.py:104 plugins/hero.py:17
+msgid "Hero"
+msgstr ""
+
+#: models/hero.py:105
 msgid "Heros"
 msgstr ""
 
-#: models/slider.py:53
+#: models/slider.py:105 plugins/slider.py:21
+msgid "Slider"
+msgstr ""
+
+#: models/slider.py:106
 msgid "Sliders"
 msgstr ""
 
-#: models/slider.py:80
+#: models/slider.py:173
 msgid "link name"
 msgstr "Label du lien"
 
-#: models/slider.py:85
+#: models/slider.py:182
 msgid "link url"
 msgstr "URL du lien"
 
-#: models/slider.py:90
+#: models/slider.py:191
 msgid "open new window"
 msgstr "Nouvelle fenêtre ?"
 
-#: models/slider.py:92
+#: models/slider.py:193
 msgid "If checked the link will be open in a new window"
 msgstr "Si coché, le lien sera ouvert dans une nouvelle fenêtre"
 
-#: models/slider.py:103
+#: models/slider.py:221
 msgid "Slide item"
 msgstr "Élément d'un slider"
 
-#: models/slider.py:104
+#: models/slider.py:222
 msgid "Slide items"
 msgstr "Éléments de sliders"
 
+#: plugins/album.py:22 plugins/card.py:16 plugins/container.py:16
+#: plugins/hero.py:16 plugins/slider.py:20
+msgid "Blocks"
+msgstr "Blocs"
+
 #: templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html:20
 msgid "Delete?"
 msgstr "Supprimer?"
 
 #: templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html:34
 msgid "Change"
-msgstr ""
+msgstr "Changer"
 
 #: templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html:36
 msgid "View on site"
-msgstr ""
+msgstr "Voir sur le site"
+
+#: templates/cmsplugin_blocks/slider/test.html:18
+msgid "Read more"
+msgstr "Lire la suite"
 
-#: utils.py:51
+#: utils/validators.py:42
 msgid "Please keep filesize under {}. Current filesize {}"
-msgstr "Veuillez limiter la taille du fichier à {}. La taille de votre fichier envoyé est {}"
+msgstr ""
+"Veuillez limiter la taille du fichier à {}. La taille de votre fichier "
+"envoyé est {}"
+
+#: utils/validators.py:121
+#, python-format
+msgid "'%(value)s' is not a valid CSS class name"
+msgstr "'%(value)s' n'est pas une classe CSS valide"
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0001_initial.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0005_v1-0-0_changes.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0005_v1-0-0_changes.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/modelfields.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/modelfields.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/album.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/album.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 setting ``BLOCKS_ALLOWED_IMAGE_EXTENSIONS``. Each image will create a new Album
 item where the name will be filled with the full relative image file path. Images
 in archive can be structured in multiple subdirectory. Created Album item from
 an archive don't have any order.
 """
 from django.conf import settings
 from django.db import models
-from django.db.models.signals import post_delete, pre_save
+from django.db.models.signals import pre_save
 from django.utils.html import strip_tags
 from django.utils.text import Truncator
 from django.utils.translation import gettext_lazy as _
 
 from cms.models.pluginmodel import CMSPlugin
 
 from smart_media.mixins import SmartFormatMixin
 from smart_media.modelfields import SmartMediaField
-from smart_media.signals import auto_purge_files_on_change, auto_purge_files_on_delete
+from smart_media.signals import auto_purge_files_on_change
 
 from ..choices_helpers import (
     get_album_feature_choices,
     get_albumitem_feature_choices,
     get_album_template_choices,
     get_album_template_default,
 )
@@ -191,19 +191,13 @@
         return self.media_format(self.image)
 
     class Meta:
         verbose_name = _("Album item")
         verbose_name_plural = _("Album items")
 
 
-post_delete.connect(
-    auto_purge_files_on_delete(["image"]),
-    dispatch_uid="block_albumitem_files_on_delete",
-    sender=AlbumItem,
-    weak=False,
-)
 pre_save.connect(
     auto_purge_files_on_change(["image"]),
     dispatch_uid="block_albumitem_files_on_change",
     sender=AlbumItem,
     weak=False,
 )
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/card.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/card.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 A card component with a title, image, features and content.
 """
 from django.conf import settings
 from django.db import models
-from django.db.models.signals import post_delete, pre_save
+from django.db.models.signals import pre_save
 from django.utils.encoding import force_str
 from django.utils.html import strip_tags
 from django.utils.text import Truncator
 from django.utils.translation import gettext_lazy as _
 
 from cms.models.pluginmodel import CMSPlugin
 
 from smart_media.mixins import SmartFormatMixin
 from smart_media.modelfields import SmartMediaField
-from smart_media.signals import auto_purge_files_on_change, auto_purge_files_on_delete
+from smart_media.signals import auto_purge_files_on_change
 
 from ..choices_helpers import (
     get_card_feature_choices,
     get_card_template_choices,
     get_card_template_default,
 )
 from ..modelfields import CommaSeparatedStringsField
@@ -130,19 +130,13 @@
         )
 
     class Meta:
         verbose_name = _("Card")
         verbose_name_plural = _("Cards")
 
 
-post_delete.connect(
-    auto_purge_files_on_delete(["image"]),
-    dispatch_uid="block_card_files_on_delete",
-    sender=Card,
-    weak=False,
-)
 pre_save.connect(
     auto_purge_files_on_change(["image"]),
     dispatch_uid="block_card_files_on_change",
     sender=Card,
     weak=False,
 )
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/container.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/container.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 A container component with a title, image, features, content and able to include other
 plugins.
 """
 from django.conf import settings
 from django.db import models
-from django.db.models.signals import post_delete, pre_save
+from django.db.models.signals import pre_save
 from django.utils.encoding import force_str
 from django.utils.html import strip_tags
 from django.utils.text import Truncator
 from django.utils.translation import gettext_lazy as _
 
 from cms.models.pluginmodel import CMSPlugin
 
 from smart_media.mixins import SmartFormatMixin
 from smart_media.modelfields import SmartMediaField
-from smart_media.signals import auto_purge_files_on_change, auto_purge_files_on_delete
+from smart_media.signals import auto_purge_files_on_change
 
 from ..choices_helpers import (
     get_container_feature_choices,
     get_container_template_choices,
     get_container_template_default,
 )
 from ..modelfields import CommaSeparatedStringsField
@@ -113,19 +113,13 @@
         )
 
     class Meta:
         verbose_name = _("Container")
         verbose_name_plural = _("Containers")
 
 
-post_delete.connect(
-    auto_purge_files_on_delete(["image"]),
-    dispatch_uid="block_container_files_on_delete",
-    sender=Container,
-    weak=False,
-)
 pre_save.connect(
     auto_purge_files_on_change(["image"]),
     dispatch_uid="block_container_files_on_change",
     sender=Container,
     weak=False,
 )
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/hero.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/hero.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 A hero component with an image (commonly for background) and a content.
 """
 from django.conf import settings
 from django.db import models
-from django.db.models.signals import post_delete, pre_save
+from django.db.models.signals import pre_save
 from django.utils.encoding import force_str
 from django.utils.html import strip_tags
 from django.utils.text import Truncator
 from django.utils.translation import gettext_lazy as _
 
 from cms.models.pluginmodel import CMSPlugin
 
 from smart_media.mixins import SmartFormatMixin
 from smart_media.modelfields import SmartMediaField
-from smart_media.signals import auto_purge_files_on_change, auto_purge_files_on_delete
+from smart_media.signals import auto_purge_files_on_change
 
 from ..choices_helpers import (
     get_hero_feature_choices,
     get_hero_template_choices,
     get_hero_template_default,
 )
 from ..modelfields import CommaSeparatedStringsField
@@ -101,19 +101,13 @@
         return self.media_format(self.image)
 
     class Meta:
         verbose_name = _("Hero")
         verbose_name_plural = _("Heros")
 
 
-post_delete.connect(
-    auto_purge_files_on_delete(["image"]),
-    dispatch_uid="block_hero_files_on_delete",
-    sender=Hero,
-    weak=False,
-)
 pre_save.connect(
     auto_purge_files_on_change(["image"]),
     dispatch_uid="block_hero_files_on_change",
     sender=Hero,
     weak=False,
 )
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/slider.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/slider.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 Slide items are ordered from their ``order`` field value. Items with a zero
 value for their order will be ordered in an almost arbitrary order (mostly
 depending from item object id).
 """
 from django.conf import settings
 from django.db import models
-from django.db.models.signals import post_delete, pre_save
+from django.db.models.signals import pre_save
 from django.utils.html import strip_tags
 from django.utils.text import Truncator
 from django.utils.translation import gettext_lazy as _
 
 from cms.models.pluginmodel import CMSPlugin
 
 from smart_media.mixins import SmartFormatMixin
 from smart_media.modelfields import SmartMediaField
-from smart_media.signals import auto_purge_files_on_change, auto_purge_files_on_delete
+from smart_media.signals import auto_purge_files_on_change
 
 from ..choices_helpers import (
     get_slider_feature_choices,
     get_slideritem_feature_choices,
     get_slider_template_choices,
     get_slider_template_default,
 )
@@ -218,19 +218,13 @@
         return self.media_format(self.image)
 
     class Meta:
         verbose_name = _("Slide item")
         verbose_name_plural = _("Slide items")
 
 
-post_delete.connect(
-    auto_purge_files_on_delete(["image"]),
-    dispatch_uid="block_slideitem_files_on_delete",
-    sender=SlideItem,
-    weak=False,
-)
 pre_save.connect(
     auto_purge_files_on_change(["image"]),
     dispatch_uid="block_slideitem_files_on_change",
     sender=SlideItem,
     weak=False,
 )
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/album.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/album.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from django.utils.translation import gettext_lazy as _
 
 from cms.plugin_base import CMSPluginBase
 
+from smart_media.admin import SmartAdminMixin
+
 from ..admin.album import AlbumItemAdmin
 from ..choices_helpers import (
     get_album_feature_choices,
     get_album_template_default,
 )
 from ..forms.album import AlbumForm
 from ..models.album import Album
 
 
-class AlbumPlugin(CMSPluginBase):
+class AlbumPlugin(SmartAdminMixin, CMSPluginBase):
     """
     Album interface is able to add/edit/remove items within inline forms.
 
     Also used template is dynamically retrieved from "template" value.
     """
     module = _("Blocks")
     name = _("Album")
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/card.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/card.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from django.utils.translation import gettext_lazy as _
 
 from cms.plugin_base import CMSPluginBase
 
+from smart_media.admin import SmartAdminMixin
+
 from ..choices_helpers import (
     get_card_feature_choices,
     get_card_template_default,
 )
 from ..forms.card import CardForm
 from ..models.card import Card
 
 
-class CardPlugin(CMSPluginBase):
+class CardPlugin(SmartAdminMixin, CMSPluginBase):
     module = _("Blocks")
     name = _("Card")
     model = Card
     form = CardForm
     render_template = get_card_template_default()
     cache = True
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/container.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/container.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from django.utils.translation import gettext_lazy as _
 
 from cms.plugin_base import CMSPluginBase
 
+from smart_media.admin import SmartAdminMixin
+
 from ..choices_helpers import (
     get_container_feature_choices,
     get_container_template_default,
 )
 from ..forms.container import ContainerForm
 from ..models.container import Container
 
 
-class ContainerPlugin(CMSPluginBase):
+class ContainerPlugin(SmartAdminMixin, CMSPluginBase):
     module = _("Blocks")
     name = _("Container")
     model = Container
     form = ContainerForm
     allow_children = True
     render_template = get_container_template_default()
     cache = True
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/hero.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/hero.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from django.utils.translation import gettext_lazy as _
 
 from cms.plugin_base import CMSPluginBase
 
+from smart_media.admin import SmartAdminMixin
+
 from ..choices_helpers import (
     get_hero_feature_choices,
     get_hero_template_default,
 )
 from ..forms.hero import HeroForm
 from ..models.hero import Hero
 
 
-class HeroPlugin(CMSPluginBase):
+class HeroPlugin(SmartAdminMixin, CMSPluginBase):
     module = _("Blocks")
     name = _("Hero")
     model = Hero
     form = HeroForm
     render_template = get_hero_template_default()
     cache = True
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/slider.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/slider.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from django.utils.translation import gettext_lazy as _
 
 from cms.plugin_base import CMSPluginBase
 
+from smart_media.admin import SmartAdminMixin
+
 from ..admin.slider import SlideItemAdmin
 from ..choices_helpers import (
     get_slider_feature_choices,
     get_slider_template_default,
 )
 from ..forms.slider import SliderForm
 from ..models.slider import Slider
 
 
-class SliderPlugin(CMSPluginBase):
+class SliderPlugin(SmartAdminMixin, CMSPluginBase):
     """
     Slider interface is able to add/edit/remove slide items as inline forms.
     """
     module = _("Blocks")
     name = _("Slider")
     model = Slider
     form = SliderForm
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/container.css` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/container.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/test.html` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/test.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/test.html` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/test.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/test.html` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/test.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/archive.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/archive.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/cms_tests.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/cms_tests.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/factories.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/factories.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/tests.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/tests.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/validators.py` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/PKG-INFO` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsplugin-blocks
-Version: 1.0.0
+Version: 1.1.0
 Summary: A set of DjangoCMS plugins for structured contents in CMS pages
 Home-page: https://github.com/emencia/cmsplugin-blocks
 Author: David Thenon
 Author-email: dthenon@emencia.com
 License: MIT
 Project-URL: Source Code, https://github.com/emencia/cmsplugin-blocks
 Project-URL: Issue Tracker, https://github.com/emencia/cmsplugin-blocks/issues
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: quality
 Provides-Extra: doc
@@ -77,17 +78,17 @@
 
 
 Dependancies
 ************
 
 * Python>=3.8;
 * Django>=3.2;
-* `DjangoCMS`_ >= 3.11.0;
-* `djangocms-text-ckeditor`_;
-* `django-smart-media`_;
+* `DjangoCMS`_>=3.11.0;
+* `djangocms-text-ckeditor`_>=5.0.1;
+* `django-smart-media`_>=0.3.0;
 
 
 Links
 *****
 
 * Read the documentation on `Read the docs <https://cmspluginblocks.readthedocs.io/>`_;
 * Download its `PyPi package <https://pypi.python.org/pypi/cmsplugin-blocks>`_;
```

### Comparing `cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/SOURCES.txt` & `cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 cmsplugin_blocks/factories/user.py
 cmsplugin_blocks/forms/__init__.py
 cmsplugin_blocks/forms/album.py
 cmsplugin_blocks/forms/card.py
 cmsplugin_blocks/forms/container.py
 cmsplugin_blocks/forms/hero.py
 cmsplugin_blocks/forms/slider.py
+cmsplugin_blocks/locale/django.pot
+cmsplugin_blocks/locale/en/LC_MESSAGES/django.mo
+cmsplugin_blocks/locale/en/LC_MESSAGES/django.po
 cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo
 cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po
 cmsplugin_blocks/migrations/0001_initial.py
 cmsplugin_blocks/migrations/0002_add_slide_item_order.py
 cmsplugin_blocks/migrations/0003_slideitem_title.py
 cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py
 cmsplugin_blocks/migrations/0005_v1-0-0_changes.py
```

### Comparing `cmsplugin-blocks-1.0.0/setup.cfg` & `cmsplugin-blocks-1.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cmsplugin-blocks
-version = 1.0.0
+version = 1.1.0
 description = A set of DjangoCMS plugins for structured contents in CMS pages
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = David Thenon
 author_email = dthenon@emencia.com
 url = https://github.com/emencia/cmsplugin-blocks
 project_urls = 
@@ -23,24 +23,25 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 include_package_data = True
 install_requires = 
 	django-cms>=3.11.0
 	djangocms-text-ckeditor>=5.0.1
-	django-smart-media
+	django-smart-media>=0.3.0
 packages = find:
 zip_safe = True
 
 [options.extras_require]
 dev = 
 	pytest
 	pytest-django
@@ -82,21 +83,22 @@
 python_files = 
 	*.py
 testpaths = 
 	tests
 
 [tox:tox]
 minversion = 3.4.0
-envlist = py{38,310}-django{32,40,41}-cms{311}
+envlist = py{38,310}-django{32,40,41,42}-cms{311}
 
 [testenv]
 deps = 
 	django32: Django>=3.2,<4.0
 	django40: Django>=4.0,<4.1
 	django41: Django>=4.1,<4.2
+	django42: Django>=4.2,<5.0
 	cms311: django-cms>=3.11.0,<4.0
 	py38-django32: backports.zoneinfo
 commands = 
 	pip install -e .[dev]
 	pytest -vv tests
 
 [egg_info]
```

