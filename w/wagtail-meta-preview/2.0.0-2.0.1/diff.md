# Comparing `tmp/wagtail-meta-preview-2.0.0.tar.gz` & `tmp/wagtail-meta-preview-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-meta-preview-2.0.0.tar", last modified: Wed May  3 13:10:31 2023, max compression
+gzip compressed data, was "wagtail-meta-preview-2.0.1.tar", last modified: Sun May 21 05:15:53 2023, max compression
```

## Comparing `wagtail-meta-preview-2.0.0.tar` & `wagtail-meta-preview-2.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.371748 wagtail-meta-preview-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-03 13:10:31.371748 wagtail-meta-preview-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:10:31.371748 wagtail-meta-preview-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.359748 wagtail-meta-preview-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/tests/test_panels_facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/tests/test_panels_google.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/tests/test_panels_twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.363747 wagtail-meta-preview-2.0.0/wagtail_meta_preview/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/meta_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.351747 wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.367748 wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/wagtail_meta_preview/
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.351747 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.371748 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_google.html
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-03 13:10:06.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:10:31.367748 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 13:10:31.000000 wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.746583 wagtail-meta-preview-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/tests/test_panels_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/tests/test_panels_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/tests/test_panels_twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.746583 wagtail-meta-preview-2.0.1/wagtail_meta_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/meta_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.746583 wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/wagtail_meta_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.746583 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/_google.html
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/top_level.txt
```

### Comparing `wagtail-meta-preview-2.0.0/LICENSE` & `wagtail-meta-preview-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.0/PKG-INFO` & `wagtail-meta-preview-2.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: wagtail-meta-preview
-Version: 2.0.0
+Version: 2.0.1
 Summary: Add preview panels for meta data to wagtail
-Home-page: https://github.com/rinti/wagtail-meta-preview
+Home-page: https://github.com/Frojd/wagtail-meta-preview
 Author: Andreas Bernacca
 Author-email: ante.bernacca@gmail.com
 License: MIT License
+Project-URL: Source, https://github.com/Frojd/wagtail-meta-preview/
+Project-URL: Changelog, https://github.com/Frojd/wagtail-meta-preview/blob/main/CHANGELOG.md
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 ![wagtail-meta-preview](https://github.com/rinti/wagtail-meta-preview/workflows/wagtail-meta-preview/badge.svg)
 [![PyPI version](https://badge.fury.io/py/wagtail-meta-preview.svg)](https://badge.fury.io/py/wagtail-meta-preview)
```

### Comparing `wagtail-meta-preview-2.0.0/README.md` & `wagtail-meta-preview-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.0/setup.py` & `wagtail-meta-preview-2.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     name="wagtail-meta-preview",
     version=version,
     description="Add preview panels for meta data to wagtail",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Andreas Bernacca",
     author_email="ante.bernacca@gmail.com",
-    url="https://github.com/rinti/wagtail-meta-preview",
-    install_requires=["wagtail>=3.0.0"],
+    url="https://github.com/Frojd/wagtail-meta-preview",
+    install_requires=["wagtail>=3.0"],
     extras_require={
         "testing": testing_extras,
     },
     setup_requires=["wheel"],
     zip_safe=False,
     license="MIT License",
     packages=find_packages(exclude=["tests*"]),
@@ -32,14 +32,21 @@
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Django",
         "Framework :: Wagtail",
         "Framework :: Wagtail :: 3",
         "Framework :: Wagtail :: 4",
+        "Framework :: Wagtail :: 5",
         "License :: OSI Approved :: MIT License",
     ],
+    project_urls={
+        "Source": "https://github.com/Frojd/wagtail-meta-preview/",
+        "Changelog": "https://github.com/Frojd/wagtail-meta-preview/blob/main/CHANGELOG.md",
+    },
 )
```

### Comparing `wagtail-meta-preview-2.0.0/tests/test_admin.py` & `wagtail-meta-preview-2.0.1/tests/test_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.test import TestCase, override_settings
 from django.urls import reverse
-
-from wagtail.test.utils import WagtailTestUtils
 from wagtail.models import Page
+from wagtail.test.utils import WagtailTestUtils
 
-from tests.app.models import TwitterPage, FacebookPage
+from tests.app.models import FacebookPage, TwitterPage
 
 
 @override_settings(ALLOWED_HOSTS=["*"])
 class TestMetaPreviewAdminView(TestCase, WagtailTestUtils):
     def setUp(self):
         self.root_page = Page.objects.first()
```

### Comparing `wagtail-meta-preview-2.0.0/tests/test_panels_facebook.py` & `wagtail-meta-preview-2.0.1/tests/test_panels_facebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django.test import TestCase
-
-from wagtail.test.utils import WagtailTestUtils
 from wagtail.models import Page
+from wagtail.test.utils import WagtailTestUtils
 
 from tests.app.models import FacebookPage
-from wagtail_meta_preview.utils import FacebookSettings
 from wagtail_meta_preview import meta_settings
+from wagtail_meta_preview.utils import FacebookSettings
 
 
 class TestMetaPreviewFacebookAdminView(TestCase, WagtailTestUtils):
     def setUp(self):
         self.root_page = Page.objects.first()
 
         self.facebook_page = self.root_page.add_child(
```

### Comparing `wagtail-meta-preview-2.0.0/tests/test_panels_google.py` & `wagtail-meta-preview-2.0.1/tests/test_panels_google.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django.test import TestCase
-
-from wagtail.test.utils import WagtailTestUtils
 from wagtail.models import Page
+from wagtail.test.utils import WagtailTestUtils
 
 from tests.app.models import MetaPage
-from wagtail_meta_preview.utils import GoogleSettings
 from wagtail_meta_preview import meta_settings
+from wagtail_meta_preview.utils import GoogleSettings
 
 
 class TestMetaPreviewGoogleAdminView(TestCase, WagtailTestUtils):
     def setUp(self):
         self.root_page = Page.objects.first()
 
         self.google_page = self.root_page.add_child(
```

### Comparing `wagtail-meta-preview-2.0.0/tests/test_panels_twitter.py` & `wagtail-meta-preview-2.0.1/tests/test_panels_twitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django.test import TestCase
-
-from wagtail.test.utils import WagtailTestUtils
 from wagtail.models import Page
+from wagtail.test.utils import WagtailTestUtils
 
 from tests.app.models import TwitterPage
-from wagtail_meta_preview.utils import TwitterSettings
 from wagtail_meta_preview import meta_settings
+from wagtail_meta_preview.utils import TwitterSettings
 
 
 class TestMetaPreviewTwitterAdminView(TestCase, WagtailTestUtils):
     def setUp(self):
         self.root_page = Page.objects.first()
 
         self.twitter_page = self.root_page.add_child(
```

### Comparing `wagtail-meta-preview-2.0.0/tests/test_utils.py` & `wagtail-meta-preview-2.0.1/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from io import BytesIO
 
 import PIL.Image
-from django.test import TestCase
 from django.core.files.images import ImageFile
-from wagtail.test.utils import WagtailTestUtils
+from django.test import TestCase
 from wagtail.images.models import Image
+from wagtail.test.utils import WagtailTestUtils
 
 from wagtail_meta_preview.utils import get_focal
 
 
 # Taken from wagtail.images.test.utils
 def get_test_image_file(filename="test.png", colour="white", size=(640, 480)):
     f = BytesIO()
```

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview/meta_settings.py` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview/meta_settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview/panels.py` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview/panels.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 .meta-preview-box-container {
     position: relative;
     padding: 12px 12px 8px 54px;
     text-align: left;
     border: 1px solid #dbdbdb;
     border-radius: 5px;
+    background-color: #FFF;
 }
 
 /* Twitter */
 
 .meta-twitter-author {
 	position: relative;
     margin-right: 75px;
```

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview/utils.py` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview/views.py` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from django.http import JsonResponse, HttpResponseForbidden
 from django.contrib.auth.decorators import login_required
-from wagtail_meta_preview.meta_settings import META_PREVIEW_IMAGE_DEFAULT_SIZE
+from django.http import HttpResponseForbidden, JsonResponse
 from wagtail.images import get_image_model
+
+from wagtail_meta_preview.meta_settings import META_PREVIEW_IMAGE_DEFAULT_SIZE
 from wagtail_meta_preview.utils import get_focal
 
 
 @login_required
 def get_image_rendition(request, pk):
     img = get_image_model().objects.get(pk=pk)
     if not img.is_editable_by_user(request.user):
```

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview/wagtail_hooks.py` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview/wagtail_hooks.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.urls import path
 from django.utils.html import format_html
-from wagtail.admin.staticfiles import versioned_static
 from wagtail import hooks
+from wagtail.admin.staticfiles import versioned_static
 
 from .views import get_image_rendition
 
 
 @hooks.register("insert_global_admin_css", order=100)
 def global_admin_css():
     """Add /static/css/custom.css to the admin."""
```

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/PKG-INFO` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: wagtail-meta-preview
-Version: 2.0.0
+Version: 2.0.1
 Summary: Add preview panels for meta data to wagtail
-Home-page: https://github.com/rinti/wagtail-meta-preview
+Home-page: https://github.com/Frojd/wagtail-meta-preview
 Author: Andreas Bernacca
 Author-email: ante.bernacca@gmail.com
 License: MIT License
+Project-URL: Source, https://github.com/Frojd/wagtail-meta-preview/
+Project-URL: Changelog, https://github.com/Frojd/wagtail-meta-preview/blob/main/CHANGELOG.md
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 ![wagtail-meta-preview](https://github.com/rinti/wagtail-meta-preview/workflows/wagtail-meta-preview/badge.svg)
 [![PyPI version](https://badge.fury.io/py/wagtail-meta-preview.svg)](https://badge.fury.io/py/wagtail-meta-preview)
```

### Comparing `wagtail-meta-preview-2.0.0/wagtail_meta_preview.egg-info/SOURCES.txt` & `wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

