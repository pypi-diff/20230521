# Comparing `tmp/wagtailgeowidget-7.0.0.tar.gz` & `tmp/wagtailgeowidget-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailgeowidget-7.0.0.tar", last modified: Sat Dec  3 07:04:45 2022, max compression
+gzip compressed data, was "wagtailgeowidget-8.0.0.tar", last modified: Sun May 21 14:50:23 2023, max compression
```

## Comparing `wagtailgeowidget-7.0.0.tar` & `wagtailgeowidget-8.0.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.973922 wagtailgeowidget-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2022-12-03 07:04:45.973922 wagtailgeowidget-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-03 07:04:45.973922 wagtailgeowidget-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.969922 wagtailgeowidget-7.0.0/wagtailgeowidget/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/geocoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.965921 wagtailgeowidget-7.0.0/wagtailgeowidget/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.965921 wagtailgeowidget-7.0.0/wagtailgeowidget/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.969922 wagtailgeowidget-7.0.0/wagtailgeowidget/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.965921 wagtailgeowidget-7.0.0/wagtailgeowidget/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.969922 wagtailgeowidget-7.0.0/wagtailgeowidget/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.965921 wagtailgeowidget-7.0.0/wagtailgeowidget/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.969922 wagtailgeowidget-7.0.0/wagtailgeowidget/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.969922 wagtailgeowidget-7.0.0/wagtailgeowidget/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.965921 wagtailgeowidget-7.0.0/wagtailgeowidget/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.965921 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.969922 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/css/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/css/google-maps-field.css
--rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/css/leaflet-field.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.969922 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/geocoder-field-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/geocoder-field.js
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/google-maps-field-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/google-maps-field.js
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/leaflet-field-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/leaflet-field.js
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2022-12-03 07:04:30.000000 wagtailgeowidget-7.0.0/wagtailgeowidget/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 07:04:45.969922 wagtailgeowidget-7.0.0/wagtailgeowidget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2022-12-03 07:04:45.000000 wagtailgeowidget-7.0.0/wagtailgeowidget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2022-12-03 07:04:45.000000 wagtailgeowidget-7.0.0/wagtailgeowidget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 07:04:45.000000 wagtailgeowidget-7.0.0/wagtailgeowidget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 07:04:45.000000 wagtailgeowidget-7.0.0/wagtailgeowidget.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-03 07:04:45.000000 wagtailgeowidget-7.0.0/wagtailgeowidget.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-03 07:04:45.000000 wagtailgeowidget-7.0.0/wagtailgeowidget.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.370619 wagtailgeowidget-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-21 14:50:23.370619 wagtailgeowidget-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 14:50:23.370619 wagtailgeowidget-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.366618 wagtailgeowidget-8.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/tests/test_latlng_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.366618 wagtailgeowidget-8.0.0/wagtailgeowidget/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/geocoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.362619 wagtailgeowidget-8.0.0/wagtailgeowidget/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.362619 wagtailgeowidget-8.0.0/wagtailgeowidget/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.366618 wagtailgeowidget-8.0.0/wagtailgeowidget/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.362619 wagtailgeowidget-8.0.0/wagtailgeowidget/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.366618 wagtailgeowidget-8.0.0/wagtailgeowidget/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.362619 wagtailgeowidget-8.0.0/wagtailgeowidget/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.366618 wagtailgeowidget-8.0.0/wagtailgeowidget/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.366618 wagtailgeowidget-8.0.0/wagtailgeowidget/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.362619 wagtailgeowidget-8.0.0/wagtailgeowidget/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.362619 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.366618 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/css/google-maps-field.css
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/css/leaflet-field.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.370619 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/geocoder-field-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/geocoder-field.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/google-maps-field-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/google-maps-field.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/leaflet-field-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/leaflet-field.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14597 2023-05-21 14:50:07.000000 wagtailgeowidget-8.0.0/wagtailgeowidget/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:50:23.366618 wagtailgeowidget-8.0.0/wagtailgeowidget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-21 14:50:23.000000 wagtailgeowidget-8.0.0/wagtailgeowidget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-21 14:50:23.000000 wagtailgeowidget-8.0.0/wagtailgeowidget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:50:23.000000 wagtailgeowidget-8.0.0/wagtailgeowidget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:50:23.000000 wagtailgeowidget-8.0.0/wagtailgeowidget.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-21 14:50:23.000000 wagtailgeowidget-8.0.0/wagtailgeowidget.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-21 14:50:23.000000 wagtailgeowidget-8.0.0/wagtailgeowidget.egg-info/top_level.txt
```

### Comparing `wagtailgeowidget-7.0.0/LICENSE` & `wagtailgeowidget-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/PKG-INFO` & `wagtailgeowidget-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: wagtailgeowidget
-Version: 7.0.0
+Version: 8.0.0
 Summary: Wagtail-Geo-Widget is the complete map solution for your Wagtail site.
 Home-page: https://github.com/frojd/wagtail-geo-widget
 Author: Fröjd
 Author-email: martin@marteinn.se
 License: MIT
 Project-URL: Source, https://github.com/Frojd/wagtail-geo-widget/
 Project-URL: Changelog, https://github.com/Frojd/wagtail-geo-widget/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `wagtailgeowidget-7.0.0/README.md` & `wagtailgeowidget-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/setup.py` & `wagtailgeowidget-8.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,22 +36,21 @@
     include_package_data=True,
     license="MIT",
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Framework :: Wagtail",
-        "Framework :: Wagtail :: 2",
-        "Framework :: Wagtail :: 3",
         "Framework :: Wagtail :: 4",
+        "Framework :: Wagtail :: 5",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
@@ -59,14 +58,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Utilities",
     ],
     extras_require={"test": test_extras},
     install_requires=[
-        "Wagtail>=2.15",
+        "Wagtail>=4.1",
     ],
     project_urls={
         "Source": "https://github.com/Frojd/wagtail-geo-widget/",
         "Changelog": "https://github.com/Frojd/wagtail-geo-widget/blob/main/CHANGELOG.md",
     },
 )
```

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/app_settings.py` & `wagtailgeowidget-8.0.0/wagtailgeowidget/app_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,7 +22,8 @@
 GOOGLE_MAPS_V3_APIKEY = getattr(settings, "GOOGLE_MAPS_V3_APIKEY", None)
 GOOGLE_MAPS_V3_APIKEY_CALLBACK = getattr(
     settings, "GOOGLE_MAPS_V3_APIKEY_CALLBACK", None
 )
 GOOGLE_MAPS_V3_LANGUAGE = getattr(settings, "GOOGLE_MAPS_V3_LANGUAGE", "en")
 
 MAPBOX_ACCESS_TOKEN = getattr(settings, "MAPBOX_ACCESS_TOKEN", None)
+MAPBOX_LANGUAGE = getattr(settings, "MAPBOX_LANGUAGE", "en")
```

#### html2text {}

```diff
@@ -6,8 +6,9 @@
 "GEO_WIDGET_LEAFLET_TILE_LAYER", "https://{s}.tile.openstreetmap.org/{z}/{x}/
 {y}.png", ) GEO_WIDGET_LEAFLET_TILE_LAYER_OPTIONS = getattr( settings,
 "GEO_WIDGET_LEAFLET_TILE_LAYER_OPTIONS", { "attribution": '© OpenStreetMap
 contributors' }, ) GOOGLE_MAPS_V3_APIKEY = getattr(settings,
 "GOOGLE_MAPS_V3_APIKEY", None) GOOGLE_MAPS_V3_APIKEY_CALLBACK = getattr
 ( settings, "GOOGLE_MAPS_V3_APIKEY_CALLBACK", None ) GOOGLE_MAPS_V3_LANGUAGE =
 getattr(settings, "GOOGLE_MAPS_V3_LANGUAGE", "en") MAPBOX_ACCESS_TOKEN =
-getattr(settings, "MAPBOX_ACCESS_TOKEN", None)
+getattr(settings, "MAPBOX_ACCESS_TOKEN", None) MAPBOX_LANGUAGE = getattr
+(settings, "MAPBOX_LANGUAGE", "en")
```

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/blocks.py` & `wagtailgeowidget-8.0.0/wagtailgeowidget/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 from django import forms
 from django.utils.functional import cached_property
-from wagtail import VERSION as WAGTAIL_VERSION
-
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail.blocks import FieldBlock, IntegerBlock
-else:
-    from wagtail.core.blocks import FieldBlock, IntegerBlock
+from wagtail.blocks import FieldBlock, IntegerBlock
 
 from wagtailgeowidget import geocoders
 from wagtailgeowidget.helpers import geosgeometry_str_to_struct
 from wagtailgeowidget.widgets import GeocoderField, GoogleMapsField, LeafletField
 
 
 class GeoAddressBlock(FieldBlock):
```

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/helpers.py` & `wagtailgeowidget-8.0.0/wagtailgeowidget/helpers.py`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/locale/en/LC_MESSAGES/django.po` & `wagtailgeowidget-8.0.0/wagtailgeowidget/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/locale/fr/LC_MESSAGES/django.po` & `wagtailgeowidget-8.0.0/wagtailgeowidget/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/locale/sv/LC_MESSAGES/django.po` & `wagtailgeowidget-8.0.0/wagtailgeowidget/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/panels.py` & `wagtailgeowidget-8.0.0/wagtailgeowidget/panels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-from wagtail import VERSION as WAGTAIL_VERSION
+from wagtail.admin.panels import FieldPanel
 
 from wagtailgeowidget import geocoders
 from wagtailgeowidget.app_settings import GEO_WIDGET_ZOOM
 from wagtailgeowidget.widgets import GeocoderField, GoogleMapsField, LeafletField
 
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail.admin.panels import FieldPanel
-else:
-    from wagtail.admin.edit_handlers import FieldPanel
-
 
 class GoogleMapsPanel(FieldPanel):
     def __init__(self, *args, **kwargs):
         self.classname = kwargs.pop("classname", "")
         self.address_field = kwargs.pop("address_field", "")
         self.zoom_field = kwargs.pop("zoom_field", "")
         self.hide_latlng = kwargs.pop("hide_latlng", False)
```

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/geocoder-field-telepath.js` & `wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/geocoder-field-telepath.js`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/geocoder-field.js` & `wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/geocoder-field.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -217,14 +217,15 @@
 // Mapbox
 function MapboxGeocoderField(options) {
     GeocoderField.call(this, options);
 
     var params = options.params || {};
 
     this.accessToken = params.accessToken;
+    this.language = params.language;
 }
 
 MapboxGeocoderField.prototype = Object.create(GeocoderField.prototype);
 MapboxGeocoderField.prototype.constructor = GeocoderField;
 
 MapboxGeocoderField.prototype.geocodeSearch = function(query) {
     var self = this;
@@ -232,14 +233,15 @@
     var url =
         "https://api.mapbox.com/geocoding/v5/mapbox.places/" +
         query +
         ".json?" +
         new URLSearchParams({
             limit: 1,
             access_token: this.accessToken,
+            language: this.language,
         });
 
     fetch(url)
         .then((response) => response.json())
         .then((data) => {
             if (!data.features.length) {
                 self.displayWarning(
```

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/google-maps-field-telepath.js` & `wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/google-maps-field-telepath.js`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/google-maps-field.js` & `wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/google-maps-field.js`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/leaflet-field-telepath.js` & `wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/leaflet-field-telepath.js`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/static/wagtailgeowidget/js/leaflet-field.js` & `wagtailgeowidget-8.0.0/wagtailgeowidget/static/wagtailgeowidget/js/leaflet-field.js`

 * *Files identical despite different names*

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget/widgets.py` & `wagtailgeowidget-8.0.0/wagtailgeowidget/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,17 @@
 
 from django import forms
 from django.forms import widgets
 from django.utils.functional import cached_property
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext as _
-from wagtail import VERSION as WAGTAIL_VERSION
-
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail.telepath import register
-    from wagtail.widget_adapters import WidgetAdapter
-else:
-    from wagtail.core.telepath import register
-    from wagtail.core.widget_adapters import WidgetAdapter
+from wagtail.telepath import register
 from wagtail.utils.widgets import WidgetWithScript
+from wagtail.widget_adapters import WidgetAdapter
 
 try:
     from django.contrib.gis.geos.point import Point
 except:  # NOQA
     Point = None
 
 from wagtailgeowidget import geocoders
@@ -268,17 +262,21 @@
             "google_maps": "GoogleMapsGeocoderField",
             "mapbox": "MapboxGeocoderField",
         }
 
         options = {"id": id_, "translations": translations}
         params = {}
         if self.geocoder == geocoders.MAPBOX:
-            from wagtailgeowidget.app_settings import MAPBOX_ACCESS_TOKEN
+            from wagtailgeowidget.app_settings import (
+                MAPBOX_ACCESS_TOKEN,
+                MAPBOX_LANGUAGE,
+            )
 
             params["accessToken"] = MAPBOX_ACCESS_TOKEN
+            params["language"] = MAPBOX_LANGUAGE
 
         options["params"] = params
 
         return "new {0}({1});".format(
             field_by_geocoder[self.geocoder],
             json.dumps(options),
         )
```

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget.egg-info/PKG-INFO` & `wagtailgeowidget-8.0.0/wagtailgeowidget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: wagtailgeowidget
-Version: 7.0.0
+Version: 8.0.0
 Summary: Wagtail-Geo-Widget is the complete map solution for your Wagtail site.
 Home-page: https://github.com/frojd/wagtail-geo-widget
 Author: Fröjd
 Author-email: martin@marteinn.se
 License: MIT
 Project-URL: Source, https://github.com/Frojd/wagtail-geo-widget/
 Project-URL: Changelog, https://github.com/Frojd/wagtail-geo-widget/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `wagtailgeowidget-7.0.0/wagtailgeowidget.egg-info/SOURCES.txt` & `wagtailgeowidget-8.0.0/wagtailgeowidget.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+tests/test_latlng_parse.py
+tests/test_widgets.py
 wagtailgeowidget/__init__.py
 wagtailgeowidget/app_settings.py
 wagtailgeowidget/apps.py
 wagtailgeowidget/blocks.py
 wagtailgeowidget/geocoders.py
 wagtailgeowidget/helpers.py
 wagtailgeowidget/panels.py
```

