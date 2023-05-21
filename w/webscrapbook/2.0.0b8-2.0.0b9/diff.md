# Comparing `tmp/webscrapbook-2.0.0b8.tar.gz` & `tmp/webscrapbook-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscrapbook-2.0.0b8.tar", last modified: Sun May 14 14:29:18 2023, max compression
+gzip compressed data, was "webscrapbook-2.0.0b9.tar", last modified: Sun May 21 17:25:21 2023, max compression
```

## Comparing `webscrapbook-2.0.0b8.tar` & `webscrapbook-2.0.0b9.tar`

### file list

```diff
@@ -1,110 +1,112 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:18.080429 webscrapbook-2.0.0b8/
--rw-rw-rw-   0        0        0     1092 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/LICENSE.txt
--rw-rw-rw-   0        0        0       13 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/MANIFEST.in
--rw-rw-rw-   0        0        0     5611 2023-05-14 14:29:18.080429 webscrapbook-2.0.0b8/PKG-INFO
--rw-rw-rw-   0        0        0     4300 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/README.md
--rw-rw-rw-   0        0        0     2507 2023-05-14 14:29:18.084429 webscrapbook-2.0.0b8/setup.cfg
--rw-rw-rw-   0        0        0       63 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.947815 webscrapbook-2.0.0b8/webscrapbook/
--rw-rw-rw-   0        0        0     7184 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/__init__.py
--rw-rw-rw-   0        0        0      165 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.955816 webscrapbook-2.0.0b8/webscrapbook/_polyfill/
--rw-rw-rw-   0        0        0        0 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/_polyfill/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/_polyfill/argparse.py
--rw-rw-rw-   0        0        0     2084 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/_polyfill/mimetypes.py
--rw-rw-rw-   0        0        0      393 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/_polyfill/zipfile.py
--rw-rw-rw-   0        0        0    55732 2023-05-14 13:47:20.000000 webscrapbook-2.0.0b8/webscrapbook/app.py
--rw-rw-rw-   0        0        0    46417 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/cli.py
--rw-rw-rw-   0        0        0     3131 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/locales.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.963214 webscrapbook-2.0.0b8/webscrapbook/resources/
--rw-rw-rw-   0        0        0      144 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/app.py
--rw-rw-rw-   0        0        0     1040 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/config.ini
--rw-rw-rw-   0        0        0    13234 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/config.md
--rw-rw-rw-   0        0        0     1505 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/mimetypes.md
--rw-rw-rw-   0        0        0      128 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/serve.py
--rw-rw-rw-   0        0        0     1542 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/themes.md
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.971217 webscrapbook-2.0.0b8/webscrapbook/scrapbook/
--rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/__init__.py
--rw-rw-rw-   0        0        0    51823 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/book.py
--rw-rw-rw-   0        0        0    38510 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/cache.py
--rw-rw-rw-   0        0        0    27924 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/check.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.979487 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/
--rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/__init__.py
--rw-rw-rw-   0        0        0    11866 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/file2wsb.py
--rw-rw-rw-   0        0        0    13580 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/items.py
--rw-rw-rw-   0        0        0    41549 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/migrate.py
--rw-rw-rw-   0        0        0    15455 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/sb2wsb.py
--rw-rw-rw-   0        0        0     5934 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/wsb2file.py
--rw-rw-rw-   0        0        0    26003 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/wsb2sb.py
--rw-rw-rw-   0        0        0     8784 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/exporter.py
--rw-rw-rw-   0        0        0    15902 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/host.py
--rw-rw-rw-   0        0        0    18101 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/importer.py
--rw-rw-rw-   0        0        0    38988 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/indexer.py
--rw-rw-rw-   0        0        0    19924 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/search.py
--rw-rw-rw-   0        0        0     7705 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/util.py
--rw-rw-rw-   0        0        0     2356 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/server.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.929467 webscrapbook-2.0.0b8/webscrapbook/themes/
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.933469 webscrapbook-2.0.0b8/webscrapbook/themes/default/
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.933469 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.980188 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/ar/
--rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/ar/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.980188 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/en/
--rw-rw-rw-   0        0        0     7783 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/en/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.980188 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/es/
--rw-rw-rw-   0        0        0     8853 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/es/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.980188 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/fa/
--rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/fa/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.980188 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/he/
--rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/he/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.984191 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh/
--rw-rw-rw-   0        0        0     7912 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.984191 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh_cn/
--rw-rw-rw-   0        0        0     7929 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh_cn/messages.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:18.039025 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/
--rw-rw-rw-   0        0        0      281 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/collapse.png
--rw-rw-rw-   0        0        0      728 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/comment.png
--rw-rw-rw-   0        0        0      877 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/common.css
--rw-rw-rw-   0        0        0     3900 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/common.js
--rw-rw-rw-   0        0        0     1055 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/edit.css
--rw-rw-rw-   0        0        0     1563 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/edit.js
--rw-rw-rw-   0        0        0     2438 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/editx.js
--rw-rw-rw-   0        0        0      279 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/expand.png
--rw-rw-rw-   0        0        0      523 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/external.png
--rw-rw-rw-   0        0        0      752 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/fclose.png
--rw-rw-rw-   0        0        0      449 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/file.png
--rw-rw-rw-   0        0        0      790 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/fopen.png
--rw-rw-rw-   0        0        0     3810 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index-ex.css
--rw-rw-rw-   0        0        0    61757 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index-ex.js
--rw-rw-rw-   0        0        0     2210 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index.css
--rw-rw-rw-   0        0        0     2156 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index.js
--rw-rw-rw-   0        0        0      502 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/item.png
--rw-rw-rw-   0        0        0      387 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/link.png
--rw-rw-rw-   0        0        0      445 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/note.png
--rw-rw-rw-   0        0        0      515 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/postit.png
--rw-rw-rw-   0        0        0      661 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/search.png
--rw-rw-rw-   0        0        0      807 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/toggle.png
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:18.076428 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/
--rw-rw-rw-   0        0        0      482 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/base.html
--rw-rw-rw-   0        0        0      632 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/cli.html
--rw-rw-rw-   0        0        0     1053 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/edit.html
--rw-rw-rw-   0        0        0      965 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/editx.html
--rw-rw-rw-   0        0        0     5632 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/index.html
--rw-rw-rw-   0        0        0      510 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/maff_index.html
--rw-rw-rw-   0        0        0      490 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/markdown.html
--rw-rw-rw-   0        0        0      568 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_frame.html
--rw-rw-rw-   0        0        0     1751 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_index.html
--rw-rw-rw-   0        0        0    12917 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_map.html
--rw-rw-rw-   0        0        0    26766 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_search.html
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:18.080429 webscrapbook-2.0.0b8/webscrapbook/util/
--rw-rw-rw-   0        0        0       72 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/util/__init__.py
--rw-rw-rw-   0        0        0     5867 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/util/css.py
--rw-rw-rw-   0        0        0    44456 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/util/fs.py
--rw-rw-rw-   0        0        0    15308 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/util/html.py
--rw-rw-rw-   0        0        0    36829 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/util/util.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.951818 webscrapbook-2.0.0b8/webscrapbook.egg-info/
--rw-rw-rw-   0        0        0     5611 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3428 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      264 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.335563 webscrapbook-2.0.0b9/
+-rw-rw-rw-   0        0        0     1092 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/LICENSE.txt
+-rw-rw-rw-   0        0        0       13 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5611 2023-05-21 17:25:21.336562 webscrapbook-2.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     4300 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/README.md
+-rw-rw-rw-   0        0        0     2507 2023-05-21 17:25:21.337561 webscrapbook-2.0.0b9/setup.cfg
+-rw-rw-rw-   0        0        0       63 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.268177 webscrapbook-2.0.0b9/webscrapbook/
+-rw-rw-rw-   0        0        0     7184 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.276169 webscrapbook-2.0.0b9/webscrapbook/_polyfill/
+-rw-rw-rw-   0        0        0        0 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/_polyfill/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/_polyfill/argparse.py
+-rw-rw-rw-   0        0        0     2084 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/_polyfill/mimetypes.py
+-rw-rw-rw-   0        0        0      393 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/_polyfill/zipfile.py
+-rw-rw-rw-   0        0        0    58752 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/app.py
+-rw-rw-rw-   0        0        0    46681 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/cli.py
+-rw-rw-rw-   0        0        0     3131 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/locales.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.282163 webscrapbook-2.0.0b9/webscrapbook/resources/
+-rw-rw-rw-   0        0        0      144 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/resources/app.py
+-rw-rw-rw-   0        0        0     1040 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/resources/config.ini
+-rw-rw-rw-   0        0        0    13234 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/resources/config.md
+-rw-rw-rw-   0        0        0     1505 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/resources/mimetypes.md
+-rw-rw-rw-   0        0        0      128 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/resources/serve.py
+-rw-rw-rw-   0        0        0     1542 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/resources/themes.md
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.290155 webscrapbook-2.0.0b9/webscrapbook/scrapbook/
+-rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/__init__.py
+-rw-rw-rw-   0        0        0    51817 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/book.py
+-rw-rw-rw-   0        0        0    38522 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/cache.py
+-rw-rw-rw-   0        0        0    27936 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/check.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.295150 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/
+-rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/__init__.py
+-rw-rw-rw-   0        0        0    11866 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/file2wsb.py
+-rw-rw-rw-   0        0        0    13580 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/items.py
+-rw-rw-rw-   0        0        0    41549 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/migrate.py
+-rw-rw-rw-   0        0        0    15455 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/sb2wsb.py
+-rw-rw-rw-   0        0        0     5934 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/wsb2file.py
+-rw-rw-rw-   0        0        0    26003 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/wsb2sb.py
+-rw-rw-rw-   0        0        0     9025 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/exporter.py
+-rw-rw-rw-   0        0        0     6939 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/exporter1.py
+-rw-rw-rw-   0        0        0    16513 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/host.py
+-rw-rw-rw-   0        0        0    20553 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/importer.py
+-rw-rw-rw-   0        0        0    20146 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/importer1.py
+-rw-rw-rw-   0        0        0    38988 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/indexer.py
+-rw-rw-rw-   0        0        0    19941 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/search.py
+-rw-rw-rw-   0        0        0     7722 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/scrapbook/util.py
+-rw-rw-rw-   0        0        0     2356 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/server.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.254915 webscrapbook-2.0.0b9/webscrapbook/themes/
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.258910 webscrapbook-2.0.0b9/webscrapbook/themes/default/
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.257911 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.296149 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/ar/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/ar/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.298147 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/en/
+-rw-rw-rw-   0        0        0     7783 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/en/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.299146 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/es/
+-rw-rw-rw-   0        0        0     8853 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/es/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.300145 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/fa/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/fa/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.300145 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/he/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/he/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.301144 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh/
+-rw-rw-rw-   0        0        0     7912 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.302142 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh_cn/
+-rw-rw-rw-   0        0        0     7929 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh_cn/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.321219 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/
+-rw-rw-rw-   0        0        0      281 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/collapse.png
+-rw-rw-rw-   0        0        0      728 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/comment.png
+-rw-rw-rw-   0        0        0      877 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/common.css
+-rw-rw-rw-   0        0        0     3900 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/common.js
+-rw-rw-rw-   0        0        0     1055 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/edit.css
+-rw-rw-rw-   0        0        0     1563 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/edit.js
+-rw-rw-rw-   0        0        0     2438 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/editx.js
+-rw-rw-rw-   0        0        0      279 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/expand.png
+-rw-rw-rw-   0        0        0      523 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/external.png
+-rw-rw-rw-   0        0        0      752 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/fclose.png
+-rw-rw-rw-   0        0        0      449 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/file.png
+-rw-rw-rw-   0        0        0      790 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/fopen.png
+-rw-rw-rw-   0        0        0     3810 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index-ex.css
+-rw-rw-rw-   0        0        0    61757 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index-ex.js
+-rw-rw-rw-   0        0        0     2210 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index.css
+-rw-rw-rw-   0        0        0     2156 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index.js
+-rw-rw-rw-   0        0        0      502 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/item.png
+-rw-rw-rw-   0        0        0      387 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/link.png
+-rw-rw-rw-   0        0        0      445 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/note.png
+-rw-rw-rw-   0        0        0      515 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/postit.png
+-rw-rw-rw-   0        0        0      661 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/search.png
+-rw-rw-rw-   0        0        0      807 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/static/toggle.png
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.331568 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/
+-rw-rw-rw-   0        0        0      482 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/base.html
+-rw-rw-rw-   0        0        0      632 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/cli.html
+-rw-rw-rw-   0        0        0     1053 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/edit.html
+-rw-rw-rw-   0        0        0      965 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/editx.html
+-rw-rw-rw-   0        0        0     5632 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/index.html
+-rw-rw-rw-   0        0        0      510 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/maff_index.html
+-rw-rw-rw-   0        0        0      490 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/markdown.html
+-rw-rw-rw-   0        0        0      568 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_frame.html
+-rw-rw-rw-   0        0        0     1751 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_index.html
+-rw-rw-rw-   0        0        0    12917 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_map.html
+-rw-rw-rw-   0        0        0    26766 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_search.html
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.335563 webscrapbook-2.0.0b9/webscrapbook/util/
+-rw-rw-rw-   0        0        0       72 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/util/__init__.py
+-rw-rw-rw-   0        0        0     5867 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/util/css.py
+-rw-rw-rw-   0        0        0    44456 2023-05-21 13:34:24.000000 webscrapbook-2.0.0b9/webscrapbook/util/fs.py
+-rw-rw-rw-   0        0        0    15308 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b9/webscrapbook/util/html.py
+-rw-rw-rw-   0        0        0    36829 2023-05-21 16:56:47.000000 webscrapbook-2.0.0b9/webscrapbook/util/util.py
+drwxrwxrwx   0        0        0        0 2023-05-21 17:25:21.273172 webscrapbook-2.0.0b9/webscrapbook.egg-info/
+-rw-rw-rw-   0        0        0     5611 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3500 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      264 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-21 17:25:21.000000 webscrapbook-2.0.0b9/webscrapbook.egg-info/top_level.txt
```

### Comparing `webscrapbook-2.0.0b8/LICENSE.txt` & `webscrapbook-2.0.0b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/PKG-INFO` & `webscrapbook-2.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapbook
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: A backend toolkit for management of WebScrapBook collection.
 Home-page: https://github.com/danny0838/PyWebScrapBook
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `webscrapbook-2.0.0b8/README.md` & `webscrapbook-2.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/setup.cfg` & `webscrapbook-2.0.0b9/setup.cfg`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/__init__.py` & `webscrapbook-2.0.0b9/webscrapbook/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import re
 from collections import OrderedDict
 from configparser import ConfigParser
 from copy import deepcopy
 
 __all__ = ['WSB_EXTENSION_MIN_VERSION', 'WSB_USER_DIR', 'WSB_USER_CONFIG', 'WSB_DIR', 'WSB_CONFIG', 'config']
 
-__version__ = '2.0.0b8'
+__version__ = '2.0.0b9'
 
-WSB_EXTENSION_MIN_VERSION = '2.0.0b8'
+WSB_EXTENSION_MIN_VERSION = '2.0.0.9'
 WSB_USER_DIR = os.path.join(os.path.expanduser('~'), '.config', 'wsb')  # affected by $HOME
 WSB_USER_CONFIG = os.path.join(os.path.expanduser('~'), '.wsbconfig')  # affected by $HOME
 WSB_DIR = os.environ.get('WSB_DIR') or '.wsb'
 WSB_CONFIG = os.environ.get('WSB_CONFIG') or 'config.ini'
 
 
 class Config():
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/_polyfill/argparse.py` & `webscrapbook-2.0.0b9/webscrapbook/_polyfill/argparse.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/_polyfill/mimetypes.py` & `webscrapbook-2.0.0b9/webscrapbook/_polyfill/mimetypes.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/app.py` & `webscrapbook-2.0.0b9/webscrapbook/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 from werkzeug.middleware.proxy_fix import ProxyFix
 from werkzeug.utils import cached_property
 
 from . import WSB_CONFIG, WSB_DIR, WSB_EXTENSION_MIN_VERSION, __version__, util
 from ._polyfill import mimetypes, zipfile
 from .scrapbook import cache as wsb_cache
 from .scrapbook import check as wsb_check
+from .scrapbook import exporter as wsb_exporter
 from .scrapbook import host as wsb_host
+from .scrapbook import importer as wsb_importer
 from .scrapbook import search as wsb_search
 from .scrapbook import util as wsb_util
 from .util.fs import (
     ZIP_SUBPATH_DIR,
     ZIP_SUBPATH_DIR_IMPLICIT,
     ZIP_SUBPATH_DIR_ROOT,
     ZIP_SUBPATH_FILE,
@@ -265,15 +267,15 @@
     if perm == 'all':
         return True
 
     if perm == 'read':
         return action not in {
             'token', 'lock', 'unlock',
             'mkdir', 'mkzip', 'save', 'delete', 'move', 'copy',
-            'backup', 'unbackup', 'cache', 'check', 'query',
+            'backup', 'unbackup', 'cache', 'check', 'export', 'import', 'query',
         }
 
     if perm == 'view':
         return action in {'view', 'info', 'source', 'download', 'static', 'unknown'}
 
     return False
 
@@ -1228,26 +1230,25 @@
 
     book_ids = request.values.getlist('book')
     item_ids = request.values.getlist('item')
     book_items = {}
     for i, book_id in enumerate(book_ids):
         book_items[book_id] = request.values.getlist(f'item[{i}]') + item_ids
 
-    kwargs = {
-        'book_items': book_items,
-        'lock': not request.values.get('no_lock', default=False, type=bool),
-        'backup': not request.values.get('no_backup', default=False, type=bool),
-        'fulltext': request.values.get('fulltext', default=False, type=bool),
-        'recreate': request.values.get('recreate', default=False, type=bool),
-        'static_site': request.values.get('static_site', default=False, type=bool),
-        'static_index': request.values.get('static_index', default=None, type=bool),
-        'rss': request.values.get('rss', default=None, type=bool),
-    }
-
-    gen = wsb_cache.generate((host.root, host.config), **kwargs)
+    gen = wsb_cache.generate(
+        (host.root, host.config),
+        book_items=book_items,
+        lock=request.values.get('lock', default=True),
+        backup=request.values.get('backup', default=True, type=bool),
+        fulltext=request.values.get('fulltext', default=False, type=bool),
+        recreate=request.values.get('recreate', default=False, type=bool),
+        static_site=request.values.get('static_site', default=False, type=bool),
+        static_index=request.values.get('static_index', default=None, type=bool),
+        rss=request.values.get('rss', default=None, type=bool),
+    )
 
     if format == 'sse':
         def wrapper():
             for info in gen:
                 yield json.dumps({
                     'type': info.type,
                     'msg': info.msg,
@@ -1272,32 +1273,31 @@
 
 @handle_action_advanced
 @handle_action_token
 def action_check():
     """Invoke the checker."""
     format = request.format
 
-    kwargs = {
-        'book_ids': request.values.getlist('book'),
-        'lock': not request.values.get('no_lock', default=False, type=bool),
-        'backup': not request.values.get('no_backup', default=False, type=bool),
-        'resolve_invalid_id': request.values.get('resolve_invalid_id', default=False, type=bool),
-        'resolve_missing_index': request.values.get('resolve_missing_index', default=False, type=bool),
-        'resolve_missing_index_file': request.values.get('resolve_missing_index_file', default=False, type=bool),
-        'resolve_missing_date': request.values.get('resolve_missing_date', default=False, type=bool),
-        'resolve_older_mtime': request.values.get('resolve_older_mtime', default=False, type=bool),
-        'resolve_toc_unreachable': request.values.get('resolve_toc_unreachable', default=False, type=bool),
-        'resolve_toc_invalid': request.values.get('resolve_toc_invalid', default=False, type=bool),
-        'resolve_toc_empty_subtree': request.values.get('resolve_toc_empty_subtree', default=False, type=bool),
-        'resolve_unindexed_files': request.values.get('resolve_unindexed_files', default=False, type=bool),
-        'resolve_absolute_icon': request.values.get('resolve_absolute_icon', default=False, type=bool),
-        'resolve_unused_icon': request.values.get('resolve_unused_icon', default=False, type=bool),
-    }
-
-    gen = wsb_check.run((host.root, host.config), **kwargs)
+    gen = wsb_check.run(
+        (host.root, host.config),
+        book_ids=request.values.getlist('book'),
+        lock=request.values.get('lock', default=True),
+        backup=request.values.get('backup', default=True, type=bool),
+        resolve_invalid_id=request.values.get('resolve_invalid_id', default=False, type=bool),
+        resolve_missing_index=request.values.get('resolve_missing_index', default=False, type=bool),
+        resolve_missing_index_file=request.values.get('resolve_missing_index_file', default=False, type=bool),
+        resolve_missing_date=request.values.get('resolve_missing_date', default=False, type=bool),
+        resolve_older_mtime=request.values.get('resolve_older_mtime', default=False, type=bool),
+        resolve_toc_unreachable=request.values.get('resolve_toc_unreachable', default=False, type=bool),
+        resolve_toc_invalid=request.values.get('resolve_toc_invalid', default=False, type=bool),
+        resolve_toc_empty_subtree=request.values.get('resolve_toc_empty_subtree', default=False, type=bool),
+        resolve_unindexed_files=request.values.get('resolve_unindexed_files', default=False, type=bool),
+        resolve_absolute_icon=request.values.get('resolve_absolute_icon', default=False, type=bool),
+        resolve_unused_icon=request.values.get('resolve_unused_icon', default=False, type=bool),
+    )
 
     if format == 'sse':
         def wrapper():
             for info in gen:
                 yield json.dumps({
                     'type': info.type,
                     'msg': info.msg,
@@ -1318,20 +1318,114 @@
                              )
 
     return Response(stream)
 
 
 @handle_action_advanced
 @handle_action_token
+def action_export():
+    """Invoke the exporter."""
+    format = request.format
+
+    if format:
+        abort(400, 'Action not supported.')
+
+    book_id = request.values.get('book', default='')
+    export_dir = os.path.join(host.books[book_id].tree_dir, 'exports')
+    if os.path.lexists(export_dir):
+        util.fs.delete(export_dir)
+    gen = wsb_exporter.run(
+        (host.root, host.config), export_dir,
+        book_id=book_id,
+        items=request.values.get('items', type=json.loads),
+        scheme=wsb_exporter.SCHEME_ROOT_INDEXES,
+        recursive=request.values.get('recursive', default=False, type=bool),
+        singleton=request.values.get('singleton', default=False, type=bool),
+        lock=request.values.get('lock', default=True),
+    )
+
+    def wrapper():
+        for info in gen:
+            if info.type == 'critical':
+                abort(500, info.msg)
+        yield from util.fs.zip_compress(None, export_dir, '')
+        if os.path.lexists(export_dir):
+            util.fs.delete(export_dir)
+
+    filename = 'exports.zip'
+    mimetype, _ = mimetypes.guess_type(filename)
+    filename = quote_path(filename)
+    response = Response(wrapper(), mimetype=mimetype)
+    response.headers.set('Content-Disposition',
+                         f'''attachment; filename*=UTF-8''{filename}; filename="{filename}"''')
+    return response
+
+
+@handle_action_advanced
+@handle_action_token
+def action_import():
+    """Invoke the importer."""
+    format = request.format
+
+    book_id = request.values.get('book', default='')
+    target_id = request.values.get('target')
+    target_index = request.values.get('index', type=int)
+    rebuild_folders = request.values.get('rebuild', default=False, type=bool)
+    resolve_id_used = request.values.get('resolve', default='new')
+    lock = request.values.get('lock', default=True)
+
+    export_dir = os.path.join(host.books[book_id].tree_dir, 'exports')
+    os.makedirs(export_dir, exist_ok=True)
+    _gen = wsb_importer.run(
+        (host.root, host.config), [export_dir],
+        book_id=book_id,
+        target_id=target_id,
+        target_index=target_index,
+        rebuild_folders=rebuild_folders,
+        resolve_id_used=resolve_id_used,
+        lock=lock,
+    )
+
+    def gen():
+        yield from _gen
+        util.fs.delete(export_dir)
+
+    if format == 'sse':
+        def wrapper():
+            for info in gen():
+                yield json.dumps({
+                    'type': info.type,
+                    'msg': info.msg,
+                }, ensure_ascii=False)
+
+        return http_response(wrapper(), format=format)
+
+    elif format:
+        for info in gen():
+            if info.type == 'critical':
+                abort(500, info.msg)
+        return None
+
+    stream = stream_template('cli.html',
+                             title='Importing...',
+                             messages=gen(),
+                             debug=False,
+                             )
+
+    return Response(stream)
+
+
+@handle_action_advanced
+@handle_action_token
 def action_query():
     """Perform queries on the scrapbook(s)."""
     query = request.values.getlist('q', type=json.loads)
     auto_cache = request.values.get('auto_cache', type=json.loads)
     details = request.values.get('details', default=False, type=bool)
-    lock = not request.values.get('no_lock', default=False, type=bool)
+    lock = request.values.get('lock', default=True)
 
     try:
         rv = wsb_util.HostQuery((host.root, host.config),
                                 query, auto_cache, lock=lock).run()
     except Exception as exc:
         traceback.print_exc()
         abort(500, str(exc))
@@ -1344,29 +1438,30 @@
 def action_search():
     """Search in scrapbooks."""
     format = request.format
 
     if format != 'json':
         abort(400, 'Action not supported.')
 
-    kwargs = {
-        'query': request.values.get('q', default=''),
-        'context': {
+    gen = wsb_search.search(
+        (host.root, host.config),
+        query=request.values.get('q', default=''),
+        context={
             'title': -1,
             'file': -1,
             'comment': request.values.get('comment', default=None, type=int),
             'source': request.values.get('source', default=None, type=int),
             'fulltext': request.values.get('fulltext', default=None, type=int),
         },
-        'lock': not request.values.get('no_lock', default=False, type=bool),
-    }
+        lock=request.values.get('lock', default=True),
+    )
 
     data = {}
     try:
-        for item in wsb_search.search((host.root, host.config), **kwargs):
+        for item in gen:
             data.setdefault(item.book_id, []).append({
                 'id': item.id,
                 'file': item.file,
                 'context': item.context,
             })
     except wsb_search.QueryError as exc:
         abort(400, str(exc))
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/cli.py` & `webscrapbook-2.0.0b9/webscrapbook/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -744,17 +744,20 @@
     parser_import.add_argument(
         '--target-index', metavar='INDEX',
         type=int, action='store',
         help="""the index number (starting from 0) the imported items will be
 inserted at (default: last)""")
     parser_import.add_argument(
         '--rebuild-folders', default=False, action='store_true',
-        help="""insert imported items under the original parent, and
-auto-generate parent folders if not found (ignores --target and
---target-index)""")
+        help="""rebuild the original scrapbook tree and auto-genereate missing
+ancestor folders. When `--target` is not specified, imported items are inserted
+under the original parent whenever possible (with `--target-index` ignored).
+When `--target` is specified, imported items are inserted under it (at the
+position specified by `--target-index`), and descendant items are inserted
+under them accordingly.""")
     parser_import.add_argument(
         '--resolve-id-used', metavar='MODE',
         default='skip', action='store',
         choices={'skip', 'replace', 'new'},
         help="""what to do if an importing item ID already exists (default: "%(default)s")""")
     parser_import.add_argument(
         '--filename', dest='target_filename', metavar='PATTERN',
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/locales.py` & `webscrapbook-2.0.0b9/webscrapbook/locales.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/resources/config.ini` & `webscrapbook-2.0.0b9/webscrapbook/resources/config.ini`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/resources/config.md` & `webscrapbook-2.0.0b9/webscrapbook/resources/config.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/resources/mimetypes.md` & `webscrapbook-2.0.0b9/webscrapbook/resources/mimetypes.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/resources/themes.md` & `webscrapbook-2.0.0b9/webscrapbook/resources/themes.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/book.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/book.py`

 * *Files 0% similar despite different names*

```diff
@@ -786,15 +786,15 @@
         if tasks:
             try:
                 it = reversed(tasks)
             except TypeError:
                 # Python 3.7 does not support dict reverse
                 it = reversed(tuple(tasks))
 
-            for item_id, current_parent_id, current_index in it:
+            for _, current_parent_id, current_index in it:
                 # remove from parent TOC
                 del self.toc[current_parent_id][current_index]
                 if not self.toc[current_parent_id]:
                     del self.toc[current_parent_id]
 
                 # fix when moving within the same parent
                 if current_parent_id == target_parent_id and current_index < target_index:
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/cache.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -940,15 +940,15 @@
                 continue
 
             if book.no_tree:
                 yield Info('info', f'Skipped book {book_id!r} ({book.name!r}) (no_tree).')
                 continue
 
             yield Info('info', f'Caching book {book_id!r} ({book.name!r}).')
-            lh = book.get_tree_lock().acquire() if lock else nullcontext()
+            lh = book.get_tree_lock(persist=lock).acquire() if lock else nullcontext()
             with lh:
                 if fulltext:
                     generator = FulltextCacheGenerator(
                         book,
                         recreate=recreate,
                     )
                     yield from generator.run(item_ids)
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/check.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -678,15 +678,15 @@
             yield Info('debug', f'Loading book {book_id!r}...')
 
             if book.no_tree:
                 yield Info('info', f'Skipped book {book_id!r} ({book.name}) (no_tree).')
                 continue
 
             yield Info('info', f'Checking book {book_id!r} ({book.name}).')
-            lh = book.get_tree_lock().acquire() if lock else nullcontext()
+            lh = book.get_tree_lock(persist=lock).acquire() if lock else nullcontext()
             with lh:
                 generator = BookChecker(book, **kwargs)
                 yield from generator.run()
 
             yield Info('info', 'Done.')
     except Exception as exc:
         traceback.print_exc()
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/file2wsb.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/file2wsb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/items.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/items.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/migrate.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/migrate.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/sb2wsb.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/sb2wsb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/wsb2file.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/wsb2file.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/wsb2sb.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/convert/wsb2sb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/exporter.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 import traceback
 from collections import OrderedDict
 from contextlib import nullcontext
 from datetime import datetime, timedelta
 
 from .. import util
-from .._polyfill import zipfile
+from .._polyfill import mimetypes, zipfile
 from ..util import Info
 from .book import _id_now
 from .host import Host
 
 EXPORTER_VERSION = 2
 
 SCHEME_ITEM_IDS = 0
@@ -174,16 +174,20 @@
             'id': eid,
             'timestamp': ets,
             'timezone': int(datetime.now().astimezone().utcoffset().total_seconds()),
             'path': parents,
             'index': pos,
         }
         with zipfile.ZipFile(dst, 'w') as zh:
-            zh.writestr('meta.json', json.dumps(meta_data, ensure_ascii=False, indent=2))
-            zh.writestr('export.json', json.dumps(export_data, ensure_ascii=False, indent=2))
+            fn = 'meta.json'
+            zh.writestr(fn, json.dumps(meta_data, ensure_ascii=False, indent=2),
+                        **util.fs.zip_compression_params(mimetypes.guess_type(fn)[0]))
+            fn = 'export.json'
+            zh.writestr(fn, json.dumps(export_data, ensure_ascii=False, indent=2),
+                        **util.fs.zip_compression_params(mimetypes.guess_type(fn)[0]))
 
             # include data file(s)
             if index:
                 zh.writestr('data/', '')
                 src = os.path.join(self.book.data_dir, os.path.dirname(index) if index.endswith('/index.html') else index)
                 yield Info('debug', f'Saving data files for {id!r}: {self.book.get_subpath(src)!r}')
                 util.fs.zip_compress(zh, src, f'data/{os.path.basename(src)}')
@@ -223,15 +227,15 @@
         book = host.books[book_id]
 
         if book.no_tree:
             yield Info('error', f'Unable to export book {book_id!r} ({book.name!r}) (no_tree).')
             return
 
         yield Info('info', f'Exporting from book {book_id!r} ({book.name!r}).')
-        lh = book.get_tree_lock().acquire() if lock else nullcontext()
+        lh = book.get_tree_lock(persist=lock).acquire() if lock else nullcontext()
         with lh:
             generator = Exporter(output, book, scheme=scheme, singleton=singleton)
             yield from generator.run(items, recursive)
 
     except Exception as exc:
         traceback.print_exc()
         yield Info('critical', str(exc), exc=exc)
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/host.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/host.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,26 +86,26 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         if self.lock.locked:
             self.lock.release()
 
 
 class FileLock:
-    """Controller of file lock.
+    """Controller of a file lock.
     """
     def __init__(self, host, name, *,
                  timeout=5, stale=60, persist=False):
         self.host = host
         self.name = name
         self.timeout = timeout
         self.stale = stale
         self.file = os.path.join(host.locks, f'{util.encrypt(name, method="md5")}.lock')
         self._keeper = None
 
-        if persist:
+        if isinstance(persist, str) and persist:
             try:
                 with open(self.file, encoding='UTF-8') as fh:
                     assert fh.read() == persist
             except OSError as exc:
                 raise LockPersistOSError(
                     f'unable to access lock file for {name!r}',
                     name=self.name, file=self.file, id=persist
@@ -140,14 +140,17 @@
 
             lock.acquire()
             try:
                 '''do something'''
             finally:
                 lock.release()
 
+        In the former case an automatic keeper will be set to keep the lock
+        from getting expired during the context.
+
         Args:
             timeout: float timeout to wait for a lock. < 0 to block until the
                 lock can be acquired. None to use default timeout.
             poll_interval: float interval of seconds to check whether the lock
                 is available.
 
         Raises:
@@ -203,15 +206,15 @@
 
                 t = time.time()
 
                 if t >= timeout_time:
                     raise LockTimeoutError(
                         f'timeout when acquiring lock {self.name!r}',
                         name=self.name, file=self.file
-                    )
+                    ) from None
 
                 stale_time = st.st_mtime + self.stale
 
                 if t >= stale_time:
                     # Current lock file is stale. Rewrite with current ID.
                     try:
                         with open(self.file, 'w', encoding='UTF-8') as fh:
@@ -233,14 +236,19 @@
                 break
 
         self._lock = True
         return _FileLockAcquireProxy(self)
 
     def extend(self):
         """Extend duration of the lock.
+
+        Raises:
+            LockExtendError: if the lock cannot be extended
+            LockExtendNotAcquiredError: if the lock hasn't been acquired
+            LockExtendNotFoundError: if the lock file not exist
         """
         if not self._lock:
             raise LockExtendNotAcquiredError(
                 f'lock {self.name!r} has not been acquired',
                 name=self.name, file=self.file
             )
 
@@ -255,14 +263,19 @@
             raise LockExtendError(
                 f'unable to extend lock {self.name!r}',
                 name=self.name, file=self.file
             ) from exc
 
     def release(self):
         """Release the lock.
+
+        Raises:
+            LockReleaseError: if the lock cannot be released
+            LockReleaseNotAcquiredError: if the lock hasn't been acquired
+            LockReleaseNotFoundError: if the lock file not exist
         """
         if not self._lock:
             raise LockReleaseNotAcquiredError(
                 f'lock {self.name!r} has not been acquired',
                 name=self.name, file=self.file
             )
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/importer.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/importer1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Legacy module for importing version 1 *.wsba"""
 import copy
 import json
 import os
 import re
 import shutil
 import time
 import traceback
@@ -14,25 +15,49 @@
 from ..util import Info
 from .host import Host
 
 REGEX_TARGET_FILENAME_FORMATTER = re.compile(r'%([^%]*)%')
 
 
 class Importer():
-    """Main class for importing."""
+    """Main class for importing.
+
+    For a scrapbook tree:
+
+        item0
+            item1
+                item1-1
+                item1-1
+                item1-2
+        item1
+            item1-1
+            item1-1
+            item1-2
+
+    Due to a technical limitation, items with same ID won't be inserted to the
+    same parent, and thus the reconstructed scrapbook tree will be:
+
+        item0
+            item1
+                item1-1
+                item1-2
+        item1
+            item1-1
+            item1-2
+    """
     def __init__(self, book, *,
                  target_id=None,
                  target_index=None,
                  target_filename=None,
                  rebuild_folders=False,
                  prune=False,
                  resolve_id_used='skip',  # skip, replace, new
                  ):
         self.book = book
-        self.target_id = target_id or book.ROOT_ITEM_ID
+        self.target_id = target_id
         self.target_index = target_index if (isinstance(target_index, int) and target_index >= 0) else None
         self.target_filename = target_filename or '%ID%'
         self.rebuild_folders = rebuild_folders
         self.prune = prune
         self.resolve_id_used = resolve_id_used
 
     def run(self, files=None):
@@ -43,15 +68,17 @@
         self.map_id_to_new_id = {}
 
         book_meta_orig = copy.deepcopy(self.book.meta)
         book_toc_orig = copy.deepcopy(self.book.toc)
 
         # fix target_id
         if not self.rebuild_folders:
-            if not (self.target_id in self.book.meta or self.target_id in self.book.SPECIAL_ITEM_ID):
+            if self.target_id is None:
+                self.target_id = self.book.ROOT_ITEM_ID
+            elif not (self.target_id in self.book.meta or self.target_id in self.book.SPECIAL_ITEM_ID):
                 yield Info('warn', f'Target ID {self.target_id!r} is invalid. Use {self.book.ROOT_ITEM_ID!r} instead.')
                 self.target_id = self.book.ROOT_ITEM_ID
 
         for file in files:
             if os.path.isdir(file):
                 with os.scandir(file) as entries:
                     srcs = sorted(f.path for f in entries if util.is_wsba(f.path))
@@ -200,25 +227,15 @@
         with zipfile.ZipFile(file) as zh:
             with zh.open('meta.json') as fh:
                 meta = json.load(fh)
 
             with zh.open('export.json') as fh:
                 export_info = json.load(fh)
 
-            if export_info['version'] == 2:
-                try:
-                    assert isinstance(export_info['id'], str)
-                    assert isinstance(export_info['timestamp'], str)
-                    assert isinstance(export_info['timezone'], int)
-                    assert isinstance(export_info['path'], list)
-                    assert isinstance(export_info['index'], int)
-                except (AssertionError, KeyError):
-                    raise RuntimeError('Malformed archive')
-
-            elif export_info['version'] == 1:
+            if export_info['version'] == 1:
                 try:
                     assert isinstance(export_info['id'], str)
                     assert isinstance(export_info['timestamp'], str)
                     assert isinstance(export_info['timezone'], float)
                     assert isinstance(export_info['path'], list)
                 except (AssertionError, KeyError):
                     raise RuntimeError('Malformed archive')
@@ -260,14 +277,15 @@
             _, ext = os.path.splitext(src)
             filename = self.generate_imported_filename(id, meta, export_info) + ext
             dst = os.path.normpath(os.path.join(self.book.data_dir, filename))
             meta['index'] = filename + ('/index.html' if index.endswith('/index.html') else '')
 
         # handle resolve cases if id exists
         # may overwrite id, dst, and meta['index']
+        new_id = id
         if id in self.book.meta:
             if self.resolve_id_used == 'skip':
                 raise RuntimeError(f'ID {id!r} already exists')
 
             elif self.resolve_id_used == 'replace':
                 index_old = self.book.meta[id].get('index', '')
 
@@ -299,26 +317,50 @@
                             pass
 
                 self.map_eid_to_info.setdefault(export_info['id'], {}).setdefault('replaced', True)
 
             elif self.resolve_id_used == 'new':
                 new_id = self.book.get_unique_id()
                 yield Info('info', f'Importing duplicated {id!r} as {new_id!r}...')
-                self.map_id_to_new_id[id] = new_id
-                id = new_id
 
                 if index:
                     # overwrite dst and index
-                    filename = self.generate_imported_filename(id, meta, export_info) + ext
+                    filename = self.generate_imported_filename(new_id, meta, export_info) + ext
                     dst = os.path.normpath(os.path.join(self.book.data_dir, filename))
                     meta['index'] = filename + ('/index.html' if index.endswith('/index.html') else '')
 
             else:
                 raise RuntimeError(f'unknown resolve mode: {self.resolve_id_used!r}')
 
+        # if a new folder for id has been generated, replace it with new_id
+        # (e.g. when X/Y has been imported before Z/X, there will be an X' when
+        # importing X under Z)
+        try:
+            folder_id = self.map_id_to_new_id[id]
+        except KeyError:
+            pass
+        else:
+            yield Info('info', f'Replacing {folder_id!r} with {new_id!r}')
+            try:
+                self.book.toc[new_id] = self.book.toc.pop(folder_id)
+            except KeyError:
+                # folder_id not in toc
+                pass
+
+            # @TODO: better algorithm for the global replacement
+            for toc in self.book.toc.values():
+                for i, v in enumerate(toc):
+                    if v == folder_id:
+                        toc[i] = new_id
+
+            del self.book.meta[folder_id]
+
+        # mark id as generated
+        self.map_id_to_new_id[id] = new_id
+
         # import data files
         if index:
             if os.path.lexists(dst):
                 raise RuntimeError(f'file {dst!r} already exists')
 
             yield Info('debug', f'Extracting data files to {self.book.get_subpath(dst)!r}')
             os.makedirs(os.path.dirname(dst), exist_ok=True)
@@ -336,46 +378,40 @@
                 except FileExistsError:
                     yield Info('debug', f'Skipped existing favicon cache {basename!r}')
                 else:
                     yield Info('info', f'Added favicon cache {basename!r}')
 
                 # rewrite icon property to be consistent with the importing book
                 try:
-                    base = os.path.dirname(dst)
+                    base = dst if index.endswith('/index.html') else os.path.dirname(dst)
                 except UnboundLocalError:
                     base = self.book.data_dir
                 meta['icon'] = pathname2url(os.path.relpath(iconfile, base))
 
                 break
 
-        self.book.meta[id] = meta
-        return id
+        self.book.meta[new_id] = meta
+        return new_id
 
     def _insert_to_toc(self, id, export_info):
         """Insert the importing item to TOC
 
         Returns:
             string: ID of the parent the item is inserted under
         """
         if self.map_eid_to_info.setdefault(export_info['id'], {}).get('replaced'):
             yield Info('debug', f'Skipped inserting replaced {id!r}')
             return None
 
         # deduplicate by checking the ref_key
         if self.rebuild_folders:
             export_path = export_info['path']
-            if export_info['version'] == 2:
-                ref_key = (export_path[-1]['id'], export_info['index'])
-            elif export_info['version'] == 1:
-                ref_key = export_path[-1]['id']
+            ref_key = export_path[-1]['id']
         else:
-            if export_info['version'] == 2:
-                ref_key = (self.target_id, None)
-            elif export_info['version'] == 1:
-                ref_key = self.target_id
+            ref_key = self.target_id
 
         if ref_key in self.map_eid_to_info[export_info['id']].setdefault('refs', set()):
             yield Info('debug', f'Skipped inserting multi-referenced {id!r}')
             return None
 
         self.map_eid_to_info[export_info['id']]['refs'].add(ref_key)
 
@@ -383,39 +419,65 @@
         if not self.rebuild_folders:
             parent_id = self.target_id
             self._insert_to_id(id, parent_id)
             return parent_id
 
         for i in reversed(range(len(export_path))):
             parent_id = export_path[i]['id']
+            if parent_id in self.book.SPECIAL_ITEM_ID:
+                break
+
             parent_id = self.map_id_to_new_id.get(parent_id, parent_id)
-            if parent_id in self.book.meta or parent_id in self.book.SPECIAL_ITEM_ID:
+
+            # Assume that an item in meta also exists somewhere in toc, except
+            # for id, which is the one being imported and is not in toc (yet).
+            if parent_id == id:
+                continue
+
+            if parent_id in self.book.meta:
                 break
         else:
             # for a bad path data not starting from 'root'
             i = -1
             parent_id = self.book.ROOT_ITEM_ID
 
         for j in range(i + 1, len(export_path)):
             folder_id = export_path[j]['id']
             folder_title = export_path[j]['title']
-            try:
-                new_id = self.map_id_to_new_id[folder_id]
-            except KeyError:
-                new_items = self.book.add_item({
-                    'title': folder_title,
-                    'type': 'folder',
-                }, parent_id)
-                new_id = next(iter(new_items))
-                self.map_id_to_new_id[folder_id] = new_id
-                yield Info('info', f'Generated folder {new_id!r} for missing {folder_id!r} under {parent_id!r}')
-            else:
-                if new_id not in self.book.toc.get(parent_id, ()):
+
+            # special handling for id
+            if folder_id == id:
+                new_id = folder_id
+                if parent_id == self.map_id_to_new_id.get(export_path[-1]['id'], export_path[-1]['id']):
+                    # this ancestor is identical to the direct parent,
+                    # and folder_id will eventually be inserted under it
+                    yield Info('debug', f'Skipped inserting {new_id!r} under {parent_id!r} (same as parent)')
+                elif new_id not in self.book.toc.get(parent_id, ()):
                     self._insert_to_id(new_id, parent_id, allow_insert=False)
-                    yield Info('info', f'Inserted folder {new_id!r} for missing {folder_id!r} under {parent_id!r}')
+                    yield Info('info', f'Inserted {new_id!r} under {parent_id!r}')
+                else:
+                    yield Info('debug', f'Skipped inserting {new_id!r} under {parent_id!r} (already in)')
+            else:
+                try:
+                    new_id = self.map_id_to_new_id[folder_id]
+                except KeyError:
+                    new_items = self.book.add_item({
+                        'title': folder_title,
+                        'type': 'folder',
+                    }, parent_id)
+                    new_id = next(iter(new_items))
+                    self.map_id_to_new_id[folder_id] = new_id
+                    yield Info('info', f'Generated folder {new_id!r} for missing {folder_id!r} under {parent_id!r}')
+                else:
+                    if new_id not in self.book.toc.get(parent_id, ()):
+                        self._insert_to_id(new_id, parent_id, allow_insert=False)
+                        yield Info('info', f'Inserted folder {new_id!r} under {parent_id!r}')
+                    else:
+                        yield Info('debug', f'Skipped inserting {new_id!r} under {parent_id!r} (already in)')
+
             parent_id = new_id
 
         self._insert_to_id(id, parent_id, allow_insert=False)
         return parent_id
 
     def _insert_to_id(self, id, parent_id, allow_insert=True):
         parent = self.book.toc.setdefault(parent_id, [])
@@ -450,15 +512,15 @@
         book = host.books[book_id]
 
         if book.no_tree:
             yield Info('error', f'Unable to import to book {book_id!r} ({book.name!r}) (no_tree).')
             return
 
         yield Info('info', f'Impoting to book {book_id!r} ({book.name!r}).')
-        lh = book.get_tree_lock().acquire() if lock else nullcontext()
+        lh = book.get_tree_lock(persist=lock).acquire() if lock else nullcontext()
         with lh:
             generator = Importer(book, **kwargs)
             yield from generator.run(files)
 
     except Exception as exc:
         traceback.print_exc()
         yield Info('critical', str(exc), exc=exc)
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/indexer.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/indexer.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/search.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -470,15 +470,15 @@
         else:
             book_ids = self.host.books
 
         for book_id in book_ids:
             if book_id in self.query.books.setdefault('exclude', []):
                 continue
 
-            lh = self.host.books[book_id].get_tree_lock().acquire() if self.lock else nullcontext()
+            lh = self.host.books[book_id].get_tree_lock(persist=self.lock).acquire() if self.lock else nullcontext()
             with lh:
                 for item in self.search_book_sorted(book_id):
                     yield item
 
     def search_book_sorted(self, book_id):
         results = self.search_book(book_id)
         for sort in self.query.sorts:
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/scrapbook/util.py` & `webscrapbook-2.0.0b9/webscrapbook/scrapbook/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             book_id = None
 
         if book_id is None:
             self._run_tasks()
             return
 
         book = self.host.books[book_id]
-        lh = book.get_tree_lock().acquire() if self.lock else nullcontext()
+        lh = book.get_tree_lock(persist=self.lock).acquire() if self.lock else nullcontext()
         with lh:
             if 'meta' in self.loads[book_id]:
                 book.load_meta_files()
 
             if 'toc' in self.loads[book_id]:
                 book.load_toc_files()
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook/server.py` & `webscrapbook-2.0.0b9/webscrapbook/server.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/en/messages.py` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/en/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/es/messages.py` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/es/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh/messages.py` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh_cn/messages.py` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/locales/zh_cn/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/comment.png` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/comment.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/common.css` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/common.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/common.js` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/common.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/edit.css` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/edit.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/edit.js` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/edit.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/editx.js` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/editx.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/external.png` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/external.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/fclose.png` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/fclose.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/fopen.png` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/fopen.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index-ex.css` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index-ex.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index-ex.js` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index-ex.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index.css` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index.js` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/index.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/postit.png` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/postit.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/search.png` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/search.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/toggle.png` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/static/toggle.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/cli.html` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/cli.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/edit.html` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/edit.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/editx.html` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/editx.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/index.html` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/index.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_frame.html` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_frame.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_index.html` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_index.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_map.html` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_map.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_search.html` & `webscrapbook-2.0.0b9/webscrapbook/themes/default/templates/static_search.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/util/css.py` & `webscrapbook-2.0.0b9/webscrapbook/util/css.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/util/fs.py` & `webscrapbook-2.0.0b9/webscrapbook/util/fs.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/util/html.py` & `webscrapbook-2.0.0b9/webscrapbook/util/html.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook/util/util.py` & `webscrapbook-2.0.0b9/webscrapbook/util/util.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.0.0b8/webscrapbook.egg-info/PKG-INFO` & `webscrapbook-2.0.0b9/webscrapbook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapbook
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: A backend toolkit for management of WebScrapBook collection.
 Home-page: https://github.com/danny0838/PyWebScrapBook
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `webscrapbook-2.0.0b8/webscrapbook.egg-info/SOURCES.txt` & `webscrapbook-2.0.0b9/webscrapbook.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,18 @@
 webscrapbook/resources/serve.py
 webscrapbook/resources/themes.md
 webscrapbook/scrapbook/__init__.py
 webscrapbook/scrapbook/book.py
 webscrapbook/scrapbook/cache.py
 webscrapbook/scrapbook/check.py
 webscrapbook/scrapbook/exporter.py
+webscrapbook/scrapbook/exporter1.py
 webscrapbook/scrapbook/host.py
 webscrapbook/scrapbook/importer.py
+webscrapbook/scrapbook/importer1.py
 webscrapbook/scrapbook/indexer.py
 webscrapbook/scrapbook/search.py
 webscrapbook/scrapbook/util.py
 webscrapbook/scrapbook/convert/__init__.py
 webscrapbook/scrapbook/convert/file2wsb.py
 webscrapbook/scrapbook/convert/items.py
 webscrapbook/scrapbook/convert/migrate.py
```

