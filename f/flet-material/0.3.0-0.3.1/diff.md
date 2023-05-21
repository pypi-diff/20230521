# Comparing `tmp/flet-material-0.3.0.tar.gz` & `tmp/flet-material-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-material-0.3.0.tar", last modified: Mon May  8 17:35:11 2023, max compression
+gzip compressed data, was "flet-material-0.3.1.tar", last modified: Sun May 21 06:57:50 2023, max compression
```

## Comparing `flet-material-0.3.0.tar` & `flet-material-0.3.1.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.532707 flet-material-0.3.0/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.486137 flet-material-0.3.0/.github/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.490906 flet-material-0.3.0/.github/workflows/
--rw-r--r--   0 ahmad      (501) staff       (20)      496 2023-04-23 18:54:25.000000 flet-material-0.3.0/.github/workflows/build.yml
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-04-24 09:59:38.000000 flet-material-0.3.0/.gitignore
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.491398 flet-material-0.3.0/.vscode/
--rw-r--r--   0 ahmad      (501) staff       (20)       64 2023-04-21 12:22:35.000000 flet-material-0.3.0/.vscode/settings.json
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-24 11:04:16.000000 flet-material-0.3.0/CHANGELOG.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-22 18:06:15.000000 flet-material-0.3.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-05-08 17:35:11.532453 flet-material-0.3.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     3798 2023-04-26 17:39:23.000000 flet-material-0.3.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.492080 flet-material-0.3.0/command/
--rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-04-24 15:51:24.000000 flet-material-0.3.0/command/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)      641 2023-04-24 15:57:38.000000 flet-material-0.3.0/command/new_project.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.492723 flet-material-0.3.0/docs/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.493441 flet-material-0.3.0/docs/docs/
--rw-r--r--   0 ahmad      (501) staff       (20)     1819 2023-04-24 12:26:23.000000 flet-material-0.3.0/docs/docs/contribute.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.495972 flet-material-0.3.0/docs/docs/controls/
--rw-r--r--   0 ahmad      (501) staff       (20)     1975 2023-04-24 12:09:58.000000 flet-material-0.3.0/docs/docs/controls/alerts.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1357 2023-04-24 12:10:06.000000 flet-material-0.3.0/docs/docs/controls/annotations.md
--rw-r--r--   0 ahmad      (501) staff       (20)     3198 2023-04-24 11:12:12.000000 flet-material-0.3.0/docs/docs/controls/badges.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1566 2023-04-23 16:04:13.000000 flet-material-0.3.0/docs/docs/controls/buttons.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1605 2023-04-24 12:10:25.000000 flet-material-0.3.0/docs/docs/controls/checkboxes.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1434 2023-04-24 12:10:31.000000 flet-material-0.3.0/docs/docs/controls/chips.md
--rw-r--r--   0 ahmad      (501) staff       (20)     3025 2023-04-24 14:05:53.000000 flet-material-0.3.0/docs/docs/controls/dropdowns.md
--rw-r--r--   0 ahmad      (501) staff       (20)     2811 2023-04-23 14:49:45.000000 flet-material-0.3.0/docs/docs/controls/index.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1296 2023-04-24 12:10:56.000000 flet-material-0.3.0/docs/docs/controls/switches.md
--rw-r--r--   0 ahmad      (501) staff       (20)     3038 2023-04-24 12:28:23.000000 flet-material-0.3.0/docs/docs/index.md
--rw-r--r--   0 ahmad      (501) staff       (20)     3070 2023-04-24 12:35:43.000000 flet-material-0.3.0/docs/mkdocs.yml
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.497536 flet-material-0.3.0/docs/site/
--rw-r--r--   0 ahmad      (501) staff       (20)        8 2023-04-24 12:45:17.000000 flet-material-0.3.0/docs/site/.gitignore
--rw-r--r--   0 ahmad      (501) staff       (20)    28461 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/404.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.487014 flet-material-0.3.0/docs/site/assets/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.497729 flet-material-0.3.0/docs/site/assets/images/
--rw-r--r--   0 ahmad      (501) staff       (20)     1870 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/images/favicon.png
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.498650 flet-material-0.3.0/docs/site/assets/javascripts/
--rw-r--r--   0 ahmad      (501) staff       (20)   113367 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/bundle.51198bba.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)   950772 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/bundle.51198bba.min.js.map
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.502326 flet-material-0.3.0/docs/site/assets/javascripts/lunr/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.511946 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/
--rw-r--r--   0 ahmad      (501) staff       (20)    17074 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     4654 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     6119 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     6208 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    11499 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     9342 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    10669 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     3383 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     9437 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    11232 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     2313 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     7973 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)      817 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     6026 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     4754 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    10171 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    10958 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    10331 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     3647 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     4523 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     2406 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     1031 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    15009 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)      784 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     2062 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    22878 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0 ahmad      (501) staff       (20)   677455 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/wordcut.js
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.512853 flet-material-0.3.0/docs/site/assets/javascripts/workers/
--rw-r--r--   0 ahmad      (501) staff       (20)    38916 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)   209901 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/workers/search.208ed371.min.js.map
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.516201 flet-material-0.3.0/docs/site/assets/stylesheets/
--rw-r--r--   0 ahmad      (501) staff       (20)   113417 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/stylesheets/main.ded33207.min.css
--rw-r--r--   0 ahmad      (501) staff       (20)    38957 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/stylesheets/main.ded33207.min.css.map
--rw-r--r--   0 ahmad      (501) staff       (20)    12355 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css
--rw-r--r--   0 ahmad      (501) staff       (20)     3646 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.516430 flet-material-0.3.0/docs/site/contribute/
--rw-r--r--   0 ahmad      (501) staff       (20)    32427 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/contribute/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.516796 flet-material-0.3.0/docs/site/controls/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.517084 flet-material-0.3.0/docs/site/controls/alerts/
--rw-r--r--   0 ahmad      (501) staff       (20)    38198 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/alerts/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.517369 flet-material-0.3.0/docs/site/controls/annotations/
--rw-r--r--   0 ahmad      (501) staff       (20)    34841 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/annotations/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.517656 flet-material-0.3.0/docs/site/controls/badges/
--rw-r--r--   0 ahmad      (501) staff       (20)    48809 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/badges/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.517990 flet-material-0.3.0/docs/site/controls/buttons/
--rw-r--r--   0 ahmad      (501) staff       (20)    37505 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/buttons/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.518524 flet-material-0.3.0/docs/site/controls/checkboxes/
--rw-r--r--   0 ahmad      (501) staff       (20)    37319 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/checkboxes/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.518941 flet-material-0.3.0/docs/site/controls/chips/
--rw-r--r--   0 ahmad      (501) staff       (20)    36557 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/chips/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.519292 flet-material-0.3.0/docs/site/controls/dropdowns/
--rw-r--r--   0 ahmad      (501) staff       (20)    46453 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/dropdowns/index.html
--rw-r--r--   0 ahmad      (501) staff       (20)    32736 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.519642 flet-material-0.3.0/docs/site/controls/switches/
--rw-r--r--   0 ahmad      (501) staff       (20)    36069 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/switches/index.html
--rw-r--r--   0 ahmad      (501) staff       (20)    38036 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.520087 flet-material-0.3.0/docs/site/search/
--rw-r--r--   0 ahmad      (501) staff       (20)    21580 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/search/search_index.json
--rw-r--r--   0 ahmad      (501) staff       (20)     1484 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/sitemap.xml
--rw-r--r--   0 ahmad      (501) staff       (20)      204 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/sitemap.xml.gz
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.523089 flet-material-0.3.0/flet_material/
--rw-r--r--   0 ahmad      (501) staff       (20)      421 2023-04-23 11:09:44.000000 flet-material-0.3.0/flet_material/__init__.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.527329 flet-material-0.3.0/flet_material/__pycache__/
--rw-r--r--   0 ahmad      (501) staff       (20)      706 2023-04-23 11:09:44.000000 flet-material-0.3.0/flet_material/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     4049 2023-04-24 11:44:19.000000 flet-material-0.3.0/flet_material/__pycache__/admonition.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1892 2023-04-22 18:01:00.000000 flet-material-0.3.0/flet_material/__pycache__/alert.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1697 2023-04-21 17:58:50.000000 flet-material-0.3.0/flet_material/__pycache__/annotation.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1834 2023-04-21 16:25:55.000000 flet-material-0.3.0/flet_material/__pycache__/annotations.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     3211 2023-04-23 15:51:31.000000 flet-material-0.3.0/flet_material/__pycache__/badge.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      738 2023-04-23 14:56:58.000000 flet-material-0.3.0/flet_material/__pycache__/base.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1597 2023-04-23 18:10:10.000000 flet-material-0.3.0/flet_material/__pycache__/button.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1525 2023-04-23 11:36:01.000000 flet-material-0.3.0/flet_material/__pycache__/checkbox.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-24 11:30:35.000000 flet-material-0.3.0/flet_material/__pycache__/chip.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-22 14:16:22.000000 flet-material-0.3.0/flet_material/__pycache__/switch.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     6919 2023-04-24 11:44:19.000000 flet-material-0.3.0/flet_material/admonition.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2689 2023-04-22 18:01:00.000000 flet-material-0.3.0/flet_material/alert.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1503 2023-04-21 17:58:49.000000 flet-material-0.3.0/flet_material/annotation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4731 2023-04-23 15:51:31.000000 flet-material-0.3.0/flet_material/badge.py
--rw-r--r--   0 ahmad      (501) staff       (20)      358 2023-04-23 14:56:57.000000 flet-material-0.3.0/flet_material/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1425 2023-04-23 18:09:54.000000 flet-material-0.3.0/flet_material/button.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1125 2023-05-08 17:33:58.000000 flet-material-0.3.0/flet_material/checkbox.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1528 2023-04-24 11:30:35.000000 flet-material-0.3.0/flet_material/chip.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1399 2023-04-22 14:16:22.000000 flet-material-0.3.0/flet_material/switch.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.524150 flet-material-0.3.0/flet_material.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4509 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       83 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       25 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       21 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       24 2023-04-22 18:53:13.000000 flet-material-0.3.0/requirements.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-08 17:35:11.532749 flet-material-0.3.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)      805 2023-05-08 17:34:47.000000 flet-material-0.3.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.529135 flet-material-0.3.0/styles/
--rw-r--r--   0 ahmad      (501) staff       (20)      271 2023-04-22 17:17:29.000000 flet-material-0.3.0/styles/__init__.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.531184 flet-material-0.3.0/styles/__pycache__/
--rw-r--r--   0 ahmad      (501) staff       (20)      499 2023-04-22 17:17:29.000000 flet-material-0.3.0/styles/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      708 2023-04-23 11:20:49.000000 flet-material-0.3.0/styles/__pycache__/admonition_style.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      493 2023-04-22 17:30:06.000000 flet-material-0.3.0/styles/__pycache__/alert_style.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      494 2023-04-22 17:08:25.000000 flet-material-0.3.0/styles/__pycache__/alert_styles.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      487 2023-04-22 16:10:03.000000 flet-material-0.3.0/styles/__pycache__/badge_style.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      287 2023-04-21 16:08:17.000000 flet-material-0.3.0/styles/__pycache__/fonts.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1040 2023-04-23 14:54:06.000000 flet-material-0.3.0/styles/__pycache__/theme.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-04-23 11:20:48.000000 flet-material-0.3.0/styles/admonition_style.py
--rw-r--r--   0 ahmad      (501) staff       (20)      378 2023-04-22 17:30:06.000000 flet-material-0.3.0/styles/alert_style.py
--rw-r--r--   0 ahmad      (501) staff       (20)      361 2023-04-22 16:10:02.000000 flet-material-0.3.0/styles/badge_style.py
--rw-r--r--   0 ahmad      (501) staff       (20)       90 2023-04-21 16:07:16.000000 flet-material-0.3.0/styles/fonts.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1421 2023-04-23 14:18:26.000000 flet-material-0.3.0/styles/theme.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.532066 flet-material-0.3.0/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)      514 2023-04-23 19:11:47.000000 flet-material-0.3.0/tests/test_admonitions.py
--rw-r--r--   0 ahmad      (501) staff       (20)      392 2023-04-23 17:39:36.000000 flet-material-0.3.0/tests/test_buttons.py
--rw-r--r--   0 ahmad      (501) staff       (20)      662 2023-04-26 17:52:03.000000 flet-material-0.3.0/tests/test_switch.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.732100 flet-material-0.3.1/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.673323 flet-material-0.3.1/.github/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.679886 flet-material-0.3.1/.github/workflows/
+-rw-r--r--   0 ahmad      (501) staff       (20)      496 2023-04-23 18:54:25.000000 flet-material-0.3.1/.github/workflows/build.yml
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-04-24 09:59:38.000000 flet-material-0.3.1/.gitignore
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.680277 flet-material-0.3.1/.vscode/
+-rw-r--r--   0 ahmad      (501) staff       (20)       64 2023-04-21 12:22:35.000000 flet-material-0.3.1/.vscode/settings.json
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-24 11:04:16.000000 flet-material-0.3.1/CHANGELOG.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-22 18:06:15.000000 flet-material-0.3.1/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-05-21 06:57:50.731542 flet-material-0.3.1/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     3798 2023-04-26 17:39:23.000000 flet-material-0.3.1/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.681603 flet-material-0.3.1/command/
+-rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-04-24 15:51:24.000000 flet-material-0.3.1/command/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      641 2023-04-24 15:57:38.000000 flet-material-0.3.1/command/new_project.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.681979 flet-material-0.3.1/docs/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.682876 flet-material-0.3.1/docs/docs/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1819 2023-04-24 12:26:23.000000 flet-material-0.3.1/docs/docs/contribute.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.686361 flet-material-0.3.1/docs/docs/controls/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1975 2023-04-24 12:09:58.000000 flet-material-0.3.1/docs/docs/controls/alerts.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1357 2023-04-24 12:10:06.000000 flet-material-0.3.1/docs/docs/controls/annotations.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3198 2023-04-24 11:12:12.000000 flet-material-0.3.1/docs/docs/controls/badges.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1566 2023-04-23 16:04:13.000000 flet-material-0.3.1/docs/docs/controls/buttons.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1605 2023-04-24 12:10:25.000000 flet-material-0.3.1/docs/docs/controls/checkboxes.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1434 2023-04-24 12:10:31.000000 flet-material-0.3.1/docs/docs/controls/chips.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3025 2023-04-24 14:05:53.000000 flet-material-0.3.1/docs/docs/controls/dropdowns.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     2811 2023-04-23 14:49:45.000000 flet-material-0.3.1/docs/docs/controls/index.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1296 2023-04-24 12:10:56.000000 flet-material-0.3.1/docs/docs/controls/switches.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3038 2023-04-24 12:28:23.000000 flet-material-0.3.1/docs/docs/index.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3070 2023-04-24 12:35:43.000000 flet-material-0.3.1/docs/mkdocs.yml
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.688689 flet-material-0.3.1/docs/site/
+-rw-r--r--   0 ahmad      (501) staff       (20)        8 2023-04-24 12:45:17.000000 flet-material-0.3.1/docs/site/.gitignore
+-rw-r--r--   0 ahmad      (501) staff       (20)    28461 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/404.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.674790 flet-material-0.3.1/docs/site/assets/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.688961 flet-material-0.3.1/docs/site/assets/images/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1870 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/images/favicon.png
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.690703 flet-material-0.3.1/docs/site/assets/javascripts/
+-rw-r--r--   0 ahmad      (501) staff       (20)   113367 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/bundle.51198bba.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)   950772 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/bundle.51198bba.min.js.map
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.694511 flet-material-0.3.1/docs/site/assets/javascripts/lunr/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.707300 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/
+-rw-r--r--   0 ahmad      (501) staff       (20)    17074 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     4654 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     6119 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     6208 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    11499 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     9342 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10669 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     3383 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     9437 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    11232 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     2313 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     7973 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)      817 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     6026 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     4754 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10171 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10958 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10331 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     3647 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     4523 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     2406 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     1031 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    15009 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)      784 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     2062 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    22878 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0 ahmad      (501) staff       (20)   677455 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/lunr/wordcut.js
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.708319 flet-material-0.3.1/docs/site/assets/javascripts/workers/
+-rw-r--r--   0 ahmad      (501) staff       (20)    38916 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)   209901 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/javascripts/workers/search.208ed371.min.js.map
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.711059 flet-material-0.3.1/docs/site/assets/stylesheets/
+-rw-r--r--   0 ahmad      (501) staff       (20)   113417 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/stylesheets/main.ded33207.min.css
+-rw-r--r--   0 ahmad      (501) staff       (20)    38957 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/stylesheets/main.ded33207.min.css.map
+-rw-r--r--   0 ahmad      (501) staff       (20)    12355 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css
+-rw-r--r--   0 ahmad      (501) staff       (20)     3646 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.711326 flet-material-0.3.1/docs/site/contribute/
+-rw-r--r--   0 ahmad      (501) staff       (20)    32427 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/contribute/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.711643 flet-material-0.3.1/docs/site/controls/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.712449 flet-material-0.3.1/docs/site/controls/alerts/
+-rw-r--r--   0 ahmad      (501) staff       (20)    38198 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/controls/alerts/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.712855 flet-material-0.3.1/docs/site/controls/annotations/
+-rw-r--r--   0 ahmad      (501) staff       (20)    34841 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/controls/annotations/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.713242 flet-material-0.3.1/docs/site/controls/badges/
+-rw-r--r--   0 ahmad      (501) staff       (20)    48809 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/controls/badges/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.713629 flet-material-0.3.1/docs/site/controls/buttons/
+-rw-r--r--   0 ahmad      (501) staff       (20)    37505 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/controls/buttons/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.714003 flet-material-0.3.1/docs/site/controls/checkboxes/
+-rw-r--r--   0 ahmad      (501) staff       (20)    37319 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/controls/checkboxes/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.714359 flet-material-0.3.1/docs/site/controls/chips/
+-rw-r--r--   0 ahmad      (501) staff       (20)    36557 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/controls/chips/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.714752 flet-material-0.3.1/docs/site/controls/dropdowns/
+-rw-r--r--   0 ahmad      (501) staff       (20)    46453 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/controls/dropdowns/index.html
+-rw-r--r--   0 ahmad      (501) staff       (20)    32736 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/controls/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.715145 flet-material-0.3.1/docs/site/controls/switches/
+-rw-r--r--   0 ahmad      (501) staff       (20)    36069 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/controls/switches/index.html
+-rw-r--r--   0 ahmad      (501) staff       (20)    38036 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.715788 flet-material-0.3.1/docs/site/search/
+-rw-r--r--   0 ahmad      (501) staff       (20)    21580 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/search/search_index.json
+-rw-r--r--   0 ahmad      (501) staff       (20)     1484 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/sitemap.xml
+-rw-r--r--   0 ahmad      (501) staff       (20)      204 2023-04-24 14:06:21.000000 flet-material-0.3.1/docs/site/sitemap.xml.gz
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.719692 flet-material-0.3.1/flet_material/
+-rw-r--r--   0 ahmad      (501) staff       (20)      421 2023-04-23 11:09:44.000000 flet-material-0.3.1/flet_material/__init__.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.724783 flet-material-0.3.1/flet_material/__pycache__/
+-rw-r--r--   0 ahmad      (501) staff       (20)      706 2023-04-23 11:09:44.000000 flet-material-0.3.1/flet_material/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     4049 2023-04-24 11:44:19.000000 flet-material-0.3.1/flet_material/__pycache__/admonition.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1892 2023-04-22 18:01:00.000000 flet-material-0.3.1/flet_material/__pycache__/alert.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1697 2023-04-21 17:58:50.000000 flet-material-0.3.1/flet_material/__pycache__/annotation.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1834 2023-04-21 16:25:55.000000 flet-material-0.3.1/flet_material/__pycache__/annotations.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     3211 2023-04-23 15:51:31.000000 flet-material-0.3.1/flet_material/__pycache__/badge.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      738 2023-04-23 14:56:58.000000 flet-material-0.3.1/flet_material/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1597 2023-04-23 18:10:10.000000 flet-material-0.3.1/flet_material/__pycache__/button.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1525 2023-04-23 11:36:01.000000 flet-material-0.3.1/flet_material/__pycache__/checkbox.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-24 11:30:35.000000 flet-material-0.3.1/flet_material/__pycache__/chip.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-22 14:16:22.000000 flet-material-0.3.1/flet_material/__pycache__/switch.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     6919 2023-04-24 11:44:19.000000 flet-material-0.3.1/flet_material/admonition.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2689 2023-04-22 18:01:00.000000 flet-material-0.3.1/flet_material/alert.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1503 2023-04-21 17:58:49.000000 flet-material-0.3.1/flet_material/annotation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4731 2023-04-23 15:51:31.000000 flet-material-0.3.1/flet_material/badge.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      358 2023-04-23 14:56:57.000000 flet-material-0.3.1/flet_material/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1425 2023-04-23 18:09:54.000000 flet-material-0.3.1/flet_material/button.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1125 2023-05-08 17:33:58.000000 flet-material-0.3.1/flet_material/checkbox.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1528 2023-04-24 11:30:35.000000 flet-material-0.3.1/flet_material/chip.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1399 2023-04-22 14:16:22.000000 flet-material-0.3.1/flet_material/switch.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.721253 flet-material-0.3.1/flet_material.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-05-21 06:57:50.000000 flet-material-0.3.1/flet_material.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4509 2023-05-21 06:57:50.000000 flet-material-0.3.1/flet_material.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-21 06:57:50.000000 flet-material-0.3.1/flet_material.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       83 2023-05-21 06:57:50.000000 flet-material-0.3.1/flet_material.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       25 2023-05-21 06:57:50.000000 flet-material-0.3.1/flet_material.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       21 2023-05-21 06:57:50.000000 flet-material-0.3.1/flet_material.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       24 2023-04-22 18:53:13.000000 flet-material-0.3.1/requirements.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-21 06:57:50.732186 flet-material-0.3.1/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)      805 2023-05-21 06:55:36.000000 flet-material-0.3.1/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.726984 flet-material-0.3.1/styles/
+-rw-r--r--   0 ahmad      (501) staff       (20)      271 2023-04-22 17:17:29.000000 flet-material-0.3.1/styles/__init__.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.729830 flet-material-0.3.1/styles/__pycache__/
+-rw-r--r--   0 ahmad      (501) staff       (20)      499 2023-04-22 17:17:29.000000 flet-material-0.3.1/styles/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      708 2023-04-23 11:20:49.000000 flet-material-0.3.1/styles/__pycache__/admonition_style.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      493 2023-04-22 17:30:06.000000 flet-material-0.3.1/styles/__pycache__/alert_style.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      494 2023-04-22 17:08:25.000000 flet-material-0.3.1/styles/__pycache__/alert_styles.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      487 2023-04-22 16:10:03.000000 flet-material-0.3.1/styles/__pycache__/badge_style.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      287 2023-04-21 16:08:17.000000 flet-material-0.3.1/styles/__pycache__/fonts.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1040 2023-04-23 14:54:06.000000 flet-material-0.3.1/styles/__pycache__/theme.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-04-23 11:20:48.000000 flet-material-0.3.1/styles/admonition_style.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      378 2023-04-22 17:30:06.000000 flet-material-0.3.1/styles/alert_style.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      361 2023-04-22 16:10:02.000000 flet-material-0.3.1/styles/badge_style.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       90 2023-04-21 16:07:16.000000 flet-material-0.3.1/styles/fonts.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1421 2023-04-23 14:18:26.000000 flet-material-0.3.1/styles/theme.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 06:57:50.731039 flet-material-0.3.1/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)      514 2023-04-23 19:11:47.000000 flet-material-0.3.1/tests/test_admonitions.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      392 2023-04-23 17:39:36.000000 flet-material-0.3.1/tests/test_buttons.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      662 2023-04-26 17:52:03.000000 flet-material-0.3.1/tests/test_switch.py
```

### Comparing `flet-material-0.3.0/LICENSE` & `flet-material-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/README.md` & `flet-material-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/command/new_project.py` & `flet-material-0.3.1/command/new_project.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/contribute.md` & `flet-material-0.3.1/docs/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/controls/alerts.md` & `flet-material-0.3.1/docs/docs/controls/alerts.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/controls/annotations.md` & `flet-material-0.3.1/docs/docs/controls/annotations.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/controls/badges.md` & `flet-material-0.3.1/docs/docs/controls/badges.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/controls/buttons.md` & `flet-material-0.3.1/docs/docs/controls/buttons.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/controls/checkboxes.md` & `flet-material-0.3.1/docs/docs/controls/checkboxes.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/controls/chips.md` & `flet-material-0.3.1/docs/docs/controls/chips.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/controls/dropdowns.md` & `flet-material-0.3.1/docs/docs/controls/dropdowns.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/controls/index.md` & `flet-material-0.3.1/docs/docs/controls/index.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/controls/switches.md` & `flet-material-0.3.1/docs/docs/controls/switches.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/docs/index.md` & `flet-material-0.3.1/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/mkdocs.yml` & `flet-material-0.3.1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/404.html` & `flet-material-0.3.1/docs/site/404.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/images/favicon.png` & `flet-material-0.3.1/docs/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/bundle.51198bba.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/bundle.51198bba.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/bundle.51198bba.min.js.map` & `flet-material-0.3.1/docs/site/assets/javascripts/bundle.51198bba.min.js.map`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.da.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.de.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.du.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.es.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.hi.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.it.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ko.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.no.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ta.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.th.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.zh.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/tinyseg.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/lunr/wordcut.js` & `flet-material-0.3.1/docs/site/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/workers/search.208ed371.min.js` & `flet-material-0.3.1/docs/site/assets/javascripts/workers/search.208ed371.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/javascripts/workers/search.208ed371.min.js.map` & `flet-material-0.3.1/docs/site/assets/javascripts/workers/search.208ed371.min.js.map`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/stylesheets/main.ded33207.min.css` & `flet-material-0.3.1/docs/site/assets/stylesheets/main.ded33207.min.css`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/stylesheets/main.ded33207.min.css.map` & `flet-material-0.3.1/docs/site/assets/stylesheets/main.ded33207.min.css.map`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css` & `flet-material-0.3.1/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css.map` & `flet-material-0.3.1/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css.map`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/contribute/index.html` & `flet-material-0.3.1/docs/site/contribute/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/controls/alerts/index.html` & `flet-material-0.3.1/docs/site/controls/alerts/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/controls/annotations/index.html` & `flet-material-0.3.1/docs/site/controls/annotations/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/controls/badges/index.html` & `flet-material-0.3.1/docs/site/controls/badges/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/controls/buttons/index.html` & `flet-material-0.3.1/docs/site/controls/buttons/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/controls/checkboxes/index.html` & `flet-material-0.3.1/docs/site/controls/checkboxes/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/controls/chips/index.html` & `flet-material-0.3.1/docs/site/controls/chips/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/controls/dropdowns/index.html` & `flet-material-0.3.1/docs/site/controls/dropdowns/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/controls/index.html` & `flet-material-0.3.1/docs/site/controls/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/controls/switches/index.html` & `flet-material-0.3.1/docs/site/controls/switches/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/index.html` & `flet-material-0.3.1/docs/site/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/search/search_index.json` & `flet-material-0.3.1/docs/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/docs/site/sitemap.xml` & `flet-material-0.3.1/docs/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/__init__.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/admonition.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/admonition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/alert.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/alert.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/annotation.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/annotation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/annotations.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/annotations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/badge.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/badge.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/base.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/button.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/checkbox.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/checkbox.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/chip.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/chip.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/__pycache__/switch.cpython-310.pyc` & `flet-material-0.3.1/flet_material/__pycache__/switch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/admonition.py` & `flet-material-0.3.1/flet_material/admonition.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/alert.py` & `flet-material-0.3.1/flet_material/alert.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/annotation.py` & `flet-material-0.3.1/flet_material/annotation.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/badge.py` & `flet-material-0.3.1/flet_material/badge.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/button.py` & `flet-material-0.3.1/flet_material/button.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/checkbox.py` & `flet-material-0.3.1/flet_material/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/chip.py` & `flet-material-0.3.1/flet_material/chip.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material/switch.py` & `flet-material-0.3.1/flet_material/switch.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/flet_material.egg-info/SOURCES.txt` & `flet-material-0.3.1/flet_material.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/setup.py` & `flet-material-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name="flet-material",
-    version="0.3.0",
+    version="0.3.1",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Material UI Library for Flet",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/material_design_flet",
     packages=["flet_material", "styles"],
-    install_requires=["click==8.1.3", "flet==0.5.2"],
+    install_requires=["click==8.1.3", "flet>=0.7.4"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
```

### Comparing `flet-material-0.3.0/styles/__pycache__/admonition_style.cpython-310.pyc` & `flet-material-0.3.1/styles/__pycache__/admonition_style.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/styles/__pycache__/theme.cpython-310.pyc` & `flet-material-0.3.1/styles/__pycache__/theme.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/styles/admonition_style.py` & `flet-material-0.3.1/styles/admonition_style.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/styles/theme.py` & `flet-material-0.3.1/styles/theme.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/tests/test_admonitions.py` & `flet-material-0.3.1/tests/test_admonitions.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.3.0/tests/test_switch.py` & `flet-material-0.3.1/tests/test_switch.py`

 * *Files identical despite different names*

